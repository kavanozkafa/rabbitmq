# rabbitmq
RabbitMQ is lightweight and easy to deploy on premises and in the cloud. It supports multiple messaging protocols. RabbitMQ can be deployed in distributed and federated configurations to meet high-scale, high-availability requirements. 

![core](/img/core%20(1).png)

![core](/img/core%20(2).png)

![core](/img/core%20(3).png)




### Authentication

Authentication --> Who are you ?
Authorization --> What are you allowed to do ?

RabbitMQ Authentication
* Username/Password
* x.509 certs

Authentication Back Ends
* RabbitMQ
* LDAP
* HTTP

Default user / password : guest / guest 

![user](/img/user.JPG)

Authorization
* Configure
* Write
* Read
* Requires reconnecting
  
[Access Control](https://www.rabbitmq.com/access-control.html)

![user](/img/access.JPG)



### Dead Letter Exchanges

Your messages's last resting place


Conditions fro Dead Letters
* Rejection or negative ack without requeue
* Message expiration due to TTL ,time to live.
* Queue length limit exceeded


Dead Letter Messages ;
* Sent to specified dead letter exchange
* Extra headers added for investigation

x-death
* queue
* reason
* time
* exchange
* routing-keys

Original Dead Letter Event Details
* x-first-death-reason
* x-first-death-queue
* x-first-death-exchange
  * investigate issues
  * trigger alerts
  * corrective actions



## Exchange Types

* Direct
* Fanout
* Topic
* Headers

![direct](/img/direct.png)

![fanout](/img/fanout.png)

![headers](/img/headers.png)

![topic](/img/topic.png)

![topic2](/img/topic2.png)

---

![exchange](/img/exchange%20(1).png)

![exchange](/img/exchange%20(2).png)

![exchange](/img/exchange%20(3).png)

![exchange](/img/exchange%20(4).png)

![exchange](/img/exchange%20(5).png)

![exchange](/img/exchange%20(6).png)

![exchange](/img/exchange%20(7).png)

![exchange](/img/exchange%20(8).png)

![exchange](/img/exchange%20(9).png)

![exchange](/img/exchange%20(10).png)

![exchange](/img/exchange%20(11).png)

![exchange](/img/exchange%20(12).png)



## Tracing Messages

![trace](/img/trace%20(1).png)

![trace](/img/trace%20(2).png)

![trace](/img/trace%20(3).png)

![trace](/img/trace%20(4).png)

![trace](/img/trace%20(5).png)


## Protocols

![protocols](/img/protocols.png)

![amqp](/img/amqp%20(1).png)

![amqp](/img/amqp%20(2).png)



# Le protocole AMQP : 
Le protocole AMQP (Advanced Message Queuing Protocol) est un protocole de message ouvert qui peut envoyer des messages transactionnels entre les serveurs. Les avantages d'AMQP sont la communication fiable (les données sont reçues de manière fiable exactement une fois à l'extrémité de réception) et l'interopérabilité. AMQP utilise un broker pour recevoir les données d'un client.

# RABBITMQ (Producer, Exchane (binding routing), Queue, et conssumer)
est un message broker open source qui implemente le protocole AMQP, dévelopé en earlang. son rôle est de transporter et router les messages depuis les publishers vers les consumers. <br>

Application web (Producer) send request to generate PDF, le msg est envoyé par le producer a rabbitmq (Exchange) et l'exchange redirige le msg vers la queue en se basant sur le binding et le rtouting key et apres consummer execute le message qui existe dans la queue. <br>

# Type d'exchange : 
- Direct.
- Fanout.
- Topic.
- Headers.

https://www.cloudamqp.com/blog/part1-rabbitmq-for-beginners-what-is-rabbitmq.html <br>

# Messanger : 

est un composant qui permet d'envoyer des messages et de les executer. <br>
on passe Message object au handler (une classe qui implemente l'interface MessageHandlerInterface et apres dispatch (Method dans BusMessageInterface) le handler. <br>.




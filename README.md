# SystemIntegration_assignment_EIP

Enterprise Integration pattern

Message router

• pattern name: Message router

• visual representation (diagram)

• short definition: Forwarding multiple messages to other message channel on specific filtered condition. 
The router only sends the message to destination without any modification of message content. 

• problem it can solve: If one needs to send multiple messages to some consumer who has specific needs, a 
message router could solve the problem by filtering the conditions and forward the messages to those that match the 
condition 

• solution it provides: The consumer receives your message. 

• what is it good for: when you want to broadcast messages to multiple consumers. It is basically usefull in almost
any situation when you pass messages to multiple receivers.

• what is it not so good for: There is no use for message router if the application only demands one to one connection.

• one example of implementation

Implementation example
Start docker container

docker run -d --rm -p 5672:5672 -p 15672:15672 --name localrabbit rabbitmq:3-management

Open browser http://localhost:15672 and login with username:guest and password:guest

In terminal: consumer.py integration
In another terminal: producer.py integration "write something here"

If you omit to write integration the consumer will not receive the message.
So the word integration is the binding route which will be received by consumer.

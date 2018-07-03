# JMSMessaging

Code to send and receive messages to and from an Apache Active MQ message broker.

System Requirements
===================
JDK 1.8
Maven
Apache Active MQ
Eclipse IDE

To use the application
======================

1. Fetch from Git to a local folder (project folder)
2. Run mvn package in the project folder.
3. Run the following command in the activemq installation folder to start activemq:
	"bin\activemq start"
4. Send a message by running the following command in the project folder: java -cp target\emtalent-jms-0.1.0.jar com.emtalent.jms.MessageSender "Hello World Again"
5. Navigate to http://localhost:8161 and browse queue "QUEUE1" to view the message.

6. To fetch messages from the queue : java -cp target\emtalent-jms-0.1.0.jar com.emtalent.jms.MessageReceiver

To change or extend the code in eclipse.
========================================
1. Create a new project in eclipse using the source code fetched from git.
2. Add all dependencies in the {project folder}/target/lib folder (created by maven) to the class path.
3. You are now ready to modify the source code in eclipse.




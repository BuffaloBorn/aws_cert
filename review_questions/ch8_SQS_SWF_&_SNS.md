1.Which of the following is not a supported Amazon Simple Notification Service (Amazon SNS) protocol?

- A. HTTPS
- B. AWS Lambda
- C. Email-JSON
- **D. Amazon DynamoDB**

Answer: D

2.When you create a new Amazon Simple Notification Service (Amazon SNS) topic, which
of the following is created automatically?

- **A. An Amazon Resource Name (ARN)**
- B. A subscriber
- C. An Amazon Simple Queue Service (Amazon SQS) queue to deliver your Amazon SNS topic
- D. A message

Answer: A

3.Which of the following are features of Amazon Simple Notification Service (Amazon SNS)? (Choose 3 answers)

- **A. Publishers**
- B. Readers
- **C. Subscribers**
- **D. Topic**

Answer: A, C, D

4.What is the default time for an Amazon Simple Queue Service (Amazon SQS) visibility
timeout?

- **A. 30 seconds**
- B. 60 seconds
- C. 1 hour
- D. 12 hours

Answer: A

5.What is the longest time available for an Amazon Simple Queue Service (Amazon SQS) visibility timeout?

- A. 30 seconds
- B. 60 seconds
- C. 1 hour
- **D. 12 hours**

Answer: D

6.Which of the following options are valid properties of an Amazon Simple Queue Service
(Amazon SQS) message? (Choose 2 answers)

- A. Destination
- **B. Message ID**
- C. Type
- **D. Body**

Answer: B, D

7.You are a solutions architect who is working for a mobile application company that
wants to use Amazon Simple Workflow Service (Amazon SWF) for their new takeout
ordering application. They will have multiple workflows that will need to interact. What
should you advise them to do in structuring the design of their Amazon SWF
environment?

- A. Use multiple domains, each containing a single workflow, and design the workflows to interact across the different domains.
- **B. Use a single domain containing multiple workflows. In this manner, the workflows will be able to interact.**
- C. Use a single domain with a single workflow and collapse all activities to within this single workflow.
- D. Workflows cannot interact with each other; they would be better off using Amazon Simple Queue Service (Amazon SQS) and Amazon Simple Notification Service (Amazon SNS) for their application.

Answer: B 

8.In Amazon Simple Workflow Service (Amazon SWF), which of the following are actors?
(Choose 3 answers)

- **A. Activity workers**
- B. Workflow starters
- **C. Deciders**
- **D. Activity tasks**

Answer: A, C, D

9.You are designing a new application, and you need to ensure that the components of
your application are not tightly coupled. You are trying to decide between the different
AWS Cloud services to use to achieve this goal. Your requirements are that messages
between your application components may not be delivered more than once, tasks must
be completed in either a synchronous or asynchronous fashion, and there must be some
form of application logic that decides what do when tasks have been completed. What
application service should you use?

- A. Amazon Simple Queue Service (Amazon SQS)
- **B. Amazon Simple Workflow Service (Amazon SWF)**
- C. Amazon Simple Storage Service (Amazon S3)
- D. Amazon Simple Email Service (Amazon SES)

Answer: B

10.How does Amazon Simple Queue Service (Amazon SQS) deliver messages?

- A. Last In, First Out (LIFO)
- B. First In, First Out (FIFO)
- C. Sequentially
- **D. Amazon SQS doesn’t guarantee delivery of your messages in any particular order.**

Answer: D

11.Of the following options, what is an efficient way to fanout a single Amazon Simple
Notification Service (Amazon SNS) message to multiple Amazon Simple Queue Service
(Amazon SQS) queues?

- **A. Create an Amazon SNS topic using Amazon SNS. Then create and subscribe multiple Amazon SQS queues sent to the Amazon SNS topic.**
- B. Create one Amazon SQS queue that subscribes to multiple Amazon SNS topics.
- C. Amazon SNS allows exactly one subscriber to each topic, so fanout is not possible.
- D. Create an Amazon SNS topic using Amazon SNS. Create an application that subscribes to that topic and duplicates the message. Send copies to multiple Amazon SQS queues.

Answer: A

12.Your application polls an Amazon Simple Queue Service (Amazon SQS) queue frequently
and returns immediately, often with empty ReceiveMessageResponses. What is one
thing that can be done to reduce Amazon SQS costs?

- A. Pricing on Amazon SQS does not include a cost for service requests; therefore, there is no concern.
- B. Increase the timeout value for short polling to wait for messages longer before returning a response.
- C. Change the message visibility value to a higher number.
- **D. Use long polling by supplying a WaitTimeSeconds of greater than 0 seconds when calling ReceiveMessage.**

Answer: D

13.What is the longest time available for an Amazon Simple Queue Service (Amazon SQS) long polling timeout?

- A. 10 seconds
- **B. 20 seconds**
- C. 30 seconds
- D. 1 hour

Answer: B

14.What is the longest configurable message retention period for Amazon Simple Queue Service (Amazon SQS)?

- A. 30 minutes
- B. 4 days
- C. 30 seconds
- **D. 14 days**

Answer: D

15.What is the default message retention period for Amazon Simple Queue Service (Amazon SQS)?

- A. 30 minutes
- B. 4 days
- **C. 30 seconds**
- D. 14 days

Answer: C

16.Amazon Simple Notification Service (Amazon SNS) is a push notification service that lets you send individual or multiple messages to large numbers of recipients. What types of
clients are supported?

- A. Java and JavaScript clients that support publisher and subscriber types
- B. Producers and consumers supported by C and C++ clients
- C. Mobile and AMQP support for publisher and subscriber client types
- **D. Publisher and subscriber client types**

Answer: D

17.In Amazon Simple Workflow Service (Amazon SWF), a decider is responsible for what?

- A. Executing each step of the work
- **B. Defining work coordination logic by specifying work sequencing, timing, and failure conditions**
- C. Executing your workflow
- D. Registering activities and workflow with Amazon SWF

Answer: B

18.Can an Amazon Simple Notification Service (Amazon SNS) topic be recreated with a
previously used topic name?

- A. Yes. The topic name should typically be available after 24 hours after the previous topic with the same name has been deleted.
- B. Yes. The topic name should typically be available after 1–3 hours after the previous topic with the same name has been deleted.
- **C. Yes. The topic name should typically be available after 30–60 seconds after the previous topic with the same name has been deleted.**
- D. At this time, this feature is not supported.

Answer: C

19.What should you do in order to grant a different AWS account permission to your Amazon Simple Queue Service (Amazon SQS) queue?

- A. Share credentials to your AWS account and have the other account’s applications use your account’s credentials to access the Amazon SQS queue.
- B. Create a user for that account in AWS Identity and Access Management (IAM) and establish an IAM policy that grants access to the queue.
- **C. Create an Amazon SQS policy that grants the other account access.**
- D. Amazon Virtual Private Cloud (Amazon VPC) peering must be used to achieve this.

Answer: C

20.Can an Amazon Simple Notification Service (Amazon SNS) message be deleted after being published to a topic?

- A. Only if a subscriber(s) has/have not read the message yet
- B. Only if the Amazon SNS recall message parameter has been set
- **C. No. After a message has been successfully published to a topic, it cannot be recalled.**
- D. Yes. However it can be deleted only if the subscribers are Amazon SQS queues.

Answer: C
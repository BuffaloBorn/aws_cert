1.When designing a loosely coupled system, which AWS services provide an intermediate
durable storage layer between components? (Choose 2 answers)

- A. Amazon CloudFront
- B. Amazon Kinesis
- C. Amazon Route 53
- D. AWS CloudFormation
- **E. Amazon Simple Queue Service (Amazon SQS)**

Answer: E

2.Which of the following options will help increase the availability of a web server farm?
(Choose 2 answers)

- A. Use Amazon CloudFront to deliver content to the end users with low latency and high data transfer speeds.
- B. Launch the web server instances across multiple Availability Zones.
- C. Leverage Auto Scaling to recover from failed instances.
- D. Deploy the instances in an Amazon Virtual Private Cloud (Amazon VPC).
- E. Add more CPU and RAM to each instance.

3.Which of the following AWS Cloud services are designed according to the Multi-AZ
principle? (Choose 2 answers)

- A. Amazon DynamoDB
- B. Amazon ElastiCache
- C. Elastic Load Balancing
- D. Amazon Virtual Private Cloud (Amazon VPC)
- E. Amazon Simple Storage Service (Amazon S3)

4.Your e-commerce site was designed to be stateless and currently runs on a fleet of
Amazon Elastic Compute Cloud (Amazon EC2) instances. In an effort to control cost and
increase availability, you have a requirement to scale the fleet based on CPU and network
utilization to match the demand curve for your site. What services do you need to meet
this requirement? (Choose 2 answers)

- A. Amazon CloudWatch
- B. Amazon DynamoDB
- C. Elastic Load Balancing
- D. Auto Scaling
- E. Amazon Simple Storage Service (Amazon S3)

5.Your compliance department has mandated a new requirement that all data on Amazon
Elastic Block Storage (Amazon EBS) volumes must be encrypted. Which of the following
steps would you follow for your existing Amazon EBS volumes to comply with the new
requirement? (Choose 3 answers)

- A. Move the existing Amazon EBS volume into an Amazon Virtual Private Cloud
(Amazon VPC).
- B. Create a new Amazon EBS volume with encryption enabled.
- C. Modify the existing Amazon EBS volume properties to enable encryption.
- D. Attach an Amazon EBS volume with encryption enabled to the instance that hosts
the data, then migrate the data to the encryption-enabled Amazon EBS volume.
- E. Copy the data from the unencrypted Amazon EBS volume to the Amazon EBS
volume with encryption enabled.

6.When building a Distributed Denial of Service (DDoS)-resilient architecture, how does
Amazon Virtual Private Cloud (Amazon VPC) help minimize the attack surface area?
(Choose 3 answers)

- A. Reduces the number of necessary Internet entry points
- B. Combines end user traffic with management traffic
- C. Obfuscates necessary Internet entry points to the level that untrusted end users
cannot access them
- D. Adds non-critical Internet entry points to the architecture
- E. Scales the network to absorb DDoS attacks

7.Your e-commerce application provides daily and ad hoc reporting to various business
units on customer purchases. This is resulting in an extremely high level of read traffic
to your MySQL Amazon Relational Database Service (Amazon RDS) instance. What can
you do to scale up read traffic without impacting your database’s performance?

- A. Increase the allocated storage for the Amazon RDS instance.
- B. Modify the Amazon RDS instance to be a Multi-AZ deployment.
- C. Create a read replica for an Amazon RDS instance.
- D. Change the Amazon RDS instance DB engine version.

8.Your website is hosted on a fleet of web servers that are load balanced across multiple
Availability Zones using an Elastic Load Balancer (ELB). What type of record set in
Amazon Route 53 can be used to point myawesomeapp.com to your website?

- A. Type A Alias resource record set
- B. MX record set
- C. TXT record set
- D. CNAME record set

9.You need a secure way to distribute your AWS credentials to an application running on
Amazon Elastic Compute Cloud (Amazon EC2) instances in order to access
supplementary AWS Cloud services. What approach provides your application access to
use short-term credentials for signing requests while protecting those credentials from
other users?
- A. Add your credentials to the UserData parameter of each Amazon EC2 instance.
- B. Use a configuration file to store your access and secret keys on the Amazon EC2
instances.
- C. Specify your access and secret keys directly in your application.
- D. Provision the Amazon EC2 instances with an instance profile that has the
appropriate privileges.

10.You are running a suite of microservices on AWS Lambda that provide the business logic
and access to data stored in Amazon DynamoDB for your task management system. You
need to create well-defined RESTful Application Program Interfaces (APIs) for these
microservices that will scale with traffic to support a new mobile application. What AWS
Cloud service can you use to create the necessary RESTful APIs?

- A. Amazon Kinesis
- B. Amazon API Gateway
- C. Amazon Cognito
- D. Amazon Elastic Compute Cloud (Amazon EC2) Container Registry

11.Your WordPress website is hosted on a fleet of Amazon Elastic Compute Cloud (Amazon
EC2) instances that leverage Auto Scaling to provide high availability. To ensure that the
content of the WordPress site is sustained through scale up and scale down events, you
need a common file system that is shared between more than one Amazon EC2 instance.
Which AWS Cloud service can meet this requirement?

- A. Amazon CloudFront
- B. Amazon ElastiCache
- C. Amazon Elastic File System (Amazon EFS)
- D. Amazon Elastic Beanstalk

12.You are changing your application to move session state information off the individual
Amazon Elastic Compute Cloud (Amazon EC2) instances to take advantage of the
elasticity and cost benefits provided by Auto Scaling. Which of the following AWS Cloud
services is best suited as an alternative for storing session state information?

- A. Amazon DynamoDB
- B. Amazon Redshift
- C. Amazon Storage Gateway
- D. Amazon Kinesis

13.A media sharing application is producing a very high volume of data in a very short
period of time. Your back-end services are unable to manage the large volume of
transactions. What option provides a way to manage the flow of transactions to your
back-end services?

- A. Store the inbound transactions in an Amazon Relational Database Service (Amazon
RDS) instance so that your back-end services can retrieve them as time permits.
- B.  Use an Amazon Simple Queue Service (Amazon SQS) queue to buffer the inbound
transactions.
- C. Use an Amazon Simple Notification Service (Amazon SNS) topic to buffer the
inbound transactions.
- D. Store the inbound transactions in an Amazon Elastic MapReduce (Amazon EMR)
cluster so that your back-end services can retrieve them as time permits.

14.Which of the following are best practices for managing AWS Identity and Access
Management (IAM) user access keys? (Choose 3 answers)
- A. Embed access keys directly into application code.
- B. Use different access keys for different applications.
- C. Rotate access keys periodically.
- D. Keep unused access keys for an indefinite period of time.
- E. Configure Multi-Factor Authentication (MFA) for your most sensitive operations.

15.You need to implement a service to scan Application Program Interface (API) calls and
related events’ history to your AWS account. This service will detect things like unused
permissions, overuse of privileged accounts, and anomalous logins. Which of the
following AWS Cloud services can be leveraged to implement this service? (Choose 3
answers)

- A. AWS CloudTrail
- B. Amazon Simple Storage Service (Amazon S3)
- C. Amazon Route 53
- D. Auto Scaling
- E. AWS Lambda

16.Government regulations require that your company maintain all correspondence for a
period of seven years for compliance reasons. What is the best storage mechanism to
keep this data secure in a cost-effective manner?

- A. Amazon S3
- B. Amazon Glacier
- C. Amazon EBS
- D. Amazon EFS

17.Your company provides media content via the Internet to customers through a paid
subscription model. You leverage Amazon CloudFront to distribute content to your
customers with low latency. What approach can you use to serve this private content
securely to your paid subscribers?

- A. Provide signed Amazon CloudFront URLs to authenticated users to access the paid
content.
- B. Use HTTPS requests to ensure that your objects are encrypted when Amazon
CloudFront serves them to viewers.
- C. Configure Amazon CloudFront to compress the media files automatically for paid
subscribers.
- D. Use the Amazon CloudFront geo restriction feature to restrict access to all of the
paid subscription media at the country level.

18.Your company provides transcoding services for amateur producers to format their short
films to a variety of video formats. Which service provides the best option for storing the
videos?
- A. Amazon Glacier
- B. Amazon Simple Storage Service (Amazon S3)
- C. Amazon Relational Database Service (Amazon RDS)
- D. AWS Storage Gateway

19.A week before Cyber Monday last year, your corporate data center experienced a failed
air conditioning unit that caused flooding into the server racks. The resulting outage cost
your company significant revenue. Your CIO mandated a move to the cloud, but he is
still concerned about catastrophic failures in a data center. What can you do to alleviate
his concerns?

- A. Distribute the architecture across multiple Availability Zones.
- B. Use an Amazon Virtual Private Cloud (Amazon VPC) with subnets.
- C. Launch the compute for the processing services in a placement group.
- D. Purchase Reserved Instances for the processing services instances.

20.Your Amazon Virtual Private Cloud (Amazon VPC) includes multiple private subnets.
The instances in these private subnets must access third-party payment Application
Program Interfaces (APIs) over the Internet. Which option will provide highly available
Internet access to the instances in the private subnets?

- A. Create an AWS Storage Gateway in each Availability Zone and configure your
routing to ensure that resources use the AWS Storage Gateway in the same
Availability Zone.
- B. Create a customer gateway in each Availability Zone and configure your routing to
ensure that resources use the customer gateway in the same Availability Zone.
- C. Create a Network Address Translation (NAT) gateway in each Availability Zone and
configure your routing to ensure that resources use the NAT gateway in the same
Availability Zone.
- D. Create a NAT gateway in one Availability Zone and configure your routing to ensure
that resources use that NAT gateway in all the Availability Zones.
1.What origin servers are supported by Amazon CloudFront? (Choose 3 answers)

- A.  An Amazon Route 53 Hosted Zone
- **B.  An Amazon Simple Storage Service (Amazon S3) bucket**
- **C.  An HTTP server running on Amazon Elastic Compute Cloud (Amazon EC2)**
- **D.  An Amazon EC2 Auto Scaling Group**
- E.  An HTTP server running on-premises

Answer: B, C, D

2.Which of the following are good use cases for Amazon CloudFront? (Choose 2 answers)

- **A.  A popular software download site that supports users around the world, with
dynamic content that changes rapidly**
- B.  A corporate website that serves training videos to employees. Most employees are
located in two corporate campuses in the same city.
- C.  **A heavily used video and music streaming service that requires content to be
delivered only to paid subscribers**
- D.  A corporate HR website that supports a global workforce. Because the site contains
sensitive data, all users must connect through a corporate Virtual Private Network
(VPN).

Answer: A, C 

3.You have a web application that contains both static content in an Amazon Simple
Storage Service (Amazon S3) bucket—primarily images and CSS files—and also dynamic
content currently served by a PHP web app running on Amazon Elastic Compute Cloud
(Amazon EC2). What features of Amazon CloudFront can be used to support this
application with a single Amazon CloudFront distribution?

4. (Choose 2 answers)

- A.  Multiple Origin Access Identifiers
- B.  Multiple signed URLs
- **C.  Multiple origins**
- D.  Multiple edge locations
- **E.  Multiple cache behaviors**

Answer: C, E 

5.You are building a media-sharing web application that serves video files to end users on
both PCs and mobile devices. The media files are stored as objects in an Amazon Simple
Storage Service (Amazon S3) bucket, but are to be delivered through Amazon
CloudFront. What is the simplest way to ensure that only Amazon CloudFront has access
to the objects in the Amazon S3 bucket?

- A.  Create Signed URLs for each Amazon S3 object.
- **B.  Use an Amazon CloudFront Origin Access Identifier (OAI).**
- C.  Use public and private keys with signed cookies.
- D.  Use an AWS Identity and Access Management (IAM) bucket policy.

Answer: B

6.Your company data center is completely full, but the sales group has determined a need
to store 200TB of product video. The videos were created over the last several years, with
the most recent being accessed by sales the most often. The data must be accessed
locally, but there is no space in the data center to install local storage devices to store this
data. What AWS cloud service will meet sales’ requirements?

- A.  AWS Storage Gateway Gateway-Stored volumes
- B.  Amazon Elastic Compute Cloud (Amazon EC2) instances with attached Amazon EBS Volumes
- **C.  AWS Storage Gateway Gateway-Cached volumes**
- D.  AWS Import/Export Disk

Answer: C

7.Your company wants to extend their existing Microsoft Active Directory capability into
an Amazon Virtual Private Cloud (Amazon VPC) without establishing a trust relationship
with the existing on-premises Active Directory. Which of the following is the best
approach to achieve this goal?

- **A.  Create and connect an AWS Directory Service AD Connector.**
- B.  Create and connect an AWS Directory Service Simple A- D. 
- C.  Create and connect an AWS Directory Service for Microsoft Active Directory (Enterprise Edition).
- D.  None of the above

Answer: A

8.Which of the following are AWS Key Management Service (AWS KMS) keys that will
never exit AWS unencrypted?

- A.  AWS KMS data keys
- B.  Envelope encryption keys
- C.  AWS KMS Customer Master Keys (CMKs)
- **D.  A and C**

Answer: D

9.Which cryptographic method is used by AWS Key Management Service (AWS KMS) to
encrypt data?

- A.  Password-based encryption
- **B.  Asymmetric**
- C.  Shared secret
- D.  Envelope encryption

Answer: B

10.Which AWS service records Application Program Interface (API) calls made on your
account and delivers log files to your Amazon Simple Storage Service (Amazon S3) bucket?

- **A.  AWS CloudTrail**
- B.  Amazon CloudWatch
- C.  Amazon Kinesis
- D.  AWS Data Pipeline

Answer: A

11.You are trying to decrypt ciphertext with AWS KMS and the decryption operation is
failing. Which of the following are possible causes? (Choose 2 answers)

- A.  The private key does not match the public key in the ciphertext.
- **B.  The plaintext was encrypted along with an encryption context, and you are not
      providing the identical encryption context when calling the Decrypt API.**
- **C.  The ciphertext you are trying to decrypt is not valid.**
- D.  You are not providing the correct symmetric key to the Decrypt API.

Answer: B, C

12.Your company has 30 years of financial records that take up 15TB of on-premises
storage. It is regulated that you maintain these records, but in the year you have worked
for the company no one has ever requested any of this data. Given that the company data
center is already filling the bandwidth of its Internet connection, what is an alternative
way to store the data on the most appropriate cloud storage?

- A.  AWS Import/Export to Amazon Simple Storage Service (Amazon S3)
- **B.  AWS Import/Export to Amazon Glacier**
- C.  Amazon Kinesis
- D.  Amazon Elastic MapReduce (AWS EMR)

Answer: B

13.Your company collects information from the point of sale registers at all of its franchise
locations. Each month these processes collect 200TB of information stored in Amazon
Simple Storage Service (Amazon S3). Analytics jobs taking 24 hours are performed to
gather knowledge from this data. Which of the following will allow you to perform these
analytics in a cost-effective way?

- A.  Copy the data to a persistent Amazon Elastic MapReduce (Amazon EMR) cluster,
and run the MapReduce jobs.
- B.  Create an application that reads the information of the Amazon S3 bucket and runs
it through an Amazon Kinesis stream.
- **C.  Run a transient Amazon EMR cluster, and run the MapReduce jobs against the data
directly in Amazon S3.**
- D.  Launch a d2.8xlarge (32 vCPU, 244GB RAM) Amazon Elastic Compute Cloud
(Amazon EC2) instance, and run an application to read and process each object
sequentially.

Answer: C

14.Which service allows you to process nearly limitless streams of data in flight?

- A.  Amazon Kinesis Firehose
- B.  Amazon Elastic MapReduce (Amazon EMR)
- C.  Amazon Redshift
- **D.  Amazon Kinesis Streams**

Answer: D

15.What combination of services enable you to copy daily 50TB of data to Amazon storage,
process the data in Hadoop, and store the results in a large data warehouse?

- A.  Amazon Kinesis, Amazon Data Pipeline, Amazon Elastic MapReduce (Amazon
EMR), and Amazon Elastic Compute Cloud (Amazon EC2)
- B.  Amazon Elastic Block Store (Amazon EBS), Amazon Data Pipeline, Amazon EMR,
and Amazon Redshift
- **C.  Amazon Simple Storage Service (Amazon S3), Amazon Data Pipeline, Amazon EMR,
and Amazon Redshift**
- D.  Amazon S3, Amazon Simple Workflow, Amazon EMR, and Amazon DynamoDB

Answer: C

16.Your company has 50,000 weather stations around the country that send updates every 2
seconds. What service will enable you to ingest this stream of data and store it to
Amazon Simple Storage Service (Amazon S3) for future processing?

- A.  Amazon Simple Queue Service (Amazon SQS)
- **B.  Amazon Kinesis Firehose**
- C.  Amazon Elastic Compute Cloud (Amazon EC2)
- D.  Amazon Data Pipeline

Answer: B

17.Your organization uses Chef heavily for its deployment automation. What AWS cloud
service provides integration with Chef recipes to start new application server instances,
configure application server software, and deploy applications?

- A.  AWS Elastic Beanstalk
- B.  Amazon Kinesis
- **C.  AWS OpsWorks**
- D.  AWS CloudFormation

Answer: C

18.A firm is moving its testing platform to AWS to provide developers with instant access to
clean test and development environments. The primary requirement for the firm is to
make environments easily reproducible and fungible. What service will help the firm
meet their requirements?

- **A.  AWS CloudFormation**
- B.  AWS Config
- C.  Amazon Redshift
- D.  AWS Trusted Advisor

Answer: A

19.Your company’s IT management team is looking for an online tool to provide
recommendations to save money, improve system availability and performance, and to
help close security gaps. What can help the management team?

- A.  Cloud-init
- **B.  AWS Trusted Advisor**
- C.  AWS Config
- D.  Configuration Recorder

Answer: B

20.Your company works with data that requires frequent audits of your AWS environment
to ensure compliance with internal policies and best practices. In order to perform these
audits, you need access to historical configurations of your resources to evaluate relevant
configuration changes. Which service will provide the necessary information for your
audits?

- **A.  AWS Config**
- B.  AWS Key Management Service (AWS KMS)
- C.  AWS CloudTrail
- D.  AWS OpsWorks

Answer: A 

21.All of the website deployments are currently done by your company’s development team.
With a surge in website popularity, the company is looking for ways to be more agile
with deployments. What AWS cloud service can help the developers focus more on
writing code instead of spending time managing and configuring servers, databases, load
balancers, firewalls, and networks?

- A.  AWS Config
- B.  AWS Trusted Advisor
- C.  Amazon Kinesis
- **D.  AWS Elastic Beanstalk**

Answer: D

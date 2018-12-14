1.Which is an operational process performed by AWS for data security?

- A. Advanced Encryption Standard (AES)-256 encryption of data stored on any shared storage device
- B. Decommissioning of storage devices using industry-standard practices
- C. Background virus scans of Amazon Elastic Block Store (Amazon EBS) volumes and Amazon EBS snapshots
- D. Replication of data across multiple AWS regions
- **E. Secure wiping of Amazon EBS data when an Amazon EBS volume is unmounted**

Answer: E

2.You have launched a Windows Amazon Elastic Compute Cloud (Amazon EC2) instance
and specified an Amazon EC2 key pair for the instance at launch. Which of the following
accurately describes how to log in to the instance?

- A. Use the Amazon EC2 key pair to securely connect to the instance via Secure Shell (SSH).
- B. Use your AWS Identity and Access Management (IAM) user X.509 certificate to log in to the instance.
- **C. Use the Amazon EC2 key pair to decrypt the administrator password and then securely connect to the instance via Remote Desktop Protocol (RDP) as the administrator.**
- D. A key pair is not needed. Securely connect to the instance via RDP.

Answer: C

3.A Database security group controls network access to a database instance that is inside a
Virtual Private Cloud (VPC) and by default allows access from?

- **A. Access from any IP address for the standard ports that the database uses is provided
by default.**
- B. Access from any IP address for any port is provided by default in the DB security
group.
- C. No access is provided by default, and any access must be explicitly added with a rule
to the DB security group.
- D. Access for the database connection string is provided by default in the DB security
group.

Answer: A

4.Which encryption algorithm is used by Amazon Simple Storage Service (Amazon S3) to
encrypt data at rest with Service-Side Encryption (SSE)?

- **A. Advanced Encryption Standard (AES)-256**
- B. RSA 1024
- C. RSA 2048
- D. AES-128

Answer: A

5.How many access keys may an AWS Identity and Access Management (IAM) user have active at one time?

- A. 0
- B. 1
- **C. 2**
- D. 3

Answer: C

6.Which of the following is the name of the security model employed by AWS with its
customers?

- A. The shared secret model
- **B. The shared responsibility model**
- C. The shared secret key model
- D. The secret key responsibility model

Answer: B

7.Which of the following describes the scheme used by an Amazon Redshift cluster
leveraging AWS Key Management Service (AWS KMS) to encrypt data-at-rest?

- A. Amazon Redshift uses a one-tier, key-based architecture for encryption.
- B. Amazon Redshift uses a two-tier, key-based architecture for encryption.
- C. Amazon Redshift uses a three-tier, key-based architecture for encryption.
- **D. Amazon Redshift uses a four-tier, key-based architecture for encryption.**

Answer: D

8.Which of the following Elastic Load Balancing options ensure that the load balancer
determines which cipher is used for a Secure Sockets Layer (SSL) connection?

- A. Client Server Cipher Suite
- B. Server Cipher Only
- C. First Server Cipher
- D. Server Order Preference

9.Which technology does Amazon WorkSpaces use to provide data security?

- A. Secure Sockets Layer (SSL)/Transport Layer Security (TLS)
- B. Advanced Encryption Standard (AES)-256
- C. PC-over-IP (PCoIP)
- D. AES-128

10.As a Solutions Architect, how should you architect systems on AWS?

- A. You should architect for least cost.
- B. You should architect your AWS usage to take advantage of Amazon Simple Storage Service’s (Amazon S3) durability.
- C. You should architect your AWS usage to take advantage of multiple regions and Availability Zones.
- D. You should architect with Amazon Elastic Compute Cloud (Amazon EC2) Auto Scaling to ensure capacity is available when needed.

11.Which security scheme is used by the AWS Multi-Factor Authentication (AWS MFA) token?

- A. Time-Based One-Time Password (TOTP)
- B. Perfect Forward Secrecy (PFC)
- C. Ephemeral Diffie Hellman (EDH)
- D. Split-Key Encryption (SKE)

12.DynamoDB tables may contain sensitive data that needs to be protected. Which of the
following is a way for you to protect DynamoDB table content? (Choose 2 answers)

- A. DynamoDB encrypts all data server-side by default so nothing is required.
- B. DynamoDB can store data encrypted with a client-side encryption library solution
before storing the data in DynamoD- B.  
- C. DynamoDB obfuscates all data stored so encryption is not required.
- D. DynamoDB can be used with the AWS Key Management Service to encrypt the data
before storing the data in DynamoD- B.  
- E.  DynamoDB should not be used to store sensitive information requiring protection.

13.You have launched an Amazon Linux Elastic Compute Cloud (Amazon EC2) instance
into EC2-Classic, and the instance has successfully passed the System Status Check and
Instance Status Check. You attempt to securely connect to the instance via Secure Shell
(SSH) and receive the response, “WARNING: UNPROTECTED PRIVATE KEY FILE,”
after which the login fails. Which of the following is the cause of the failed login?

- A. You are using the wrong private key.
- B. The permissions for the private key are too insecure for the key to be trusted.
- C. A security group rule is blocking the connection.
- D. A security group rule has not been associated with the private key.

14.Which of the following public identity providers are supported by Amazon Cognito
Identity?

- A. Amazon
- B. Google
- C. Facebook
- D. All of the above

15.Which feature of AWS is designed to permit calls to the platform from an Amazon Elastic
Compute Cloud (Amazon EC2) instance without needing access keys placed on the
instance?

- A. AWS Identity and Access Management (IAM) instance profile
- B. IAM groups
- C. IAM roles
- D. Amazon EC2 key pairs

16.Which of the following Amazon Virtual Private Cloud (Amazon VPC) elements acts as a
stateless firewall?

- A. Security group
- B. Network Access Control List (ACL)
- C. Network Address Translation (NAT) instance
- D. An Amazon VPC endpoint

17.Which of the following is the most recent version of the AWS digital signature
calculation process?

- A. Signature Version 1
- B. Signature Version 2
- C. Signature Version 3
- D. Signature Version 4

18.Which of the following is the name of the feature within Amazon Virtual Private Cloud
(Amazon VPC) that allows you to launch Amazon Elastic Compute Cloud (Amazon EC2)
instances on hardware dedicated to a single customer?

- A. Amazon VPC-based tenancy
- B. Dedicated tenancy
- C. Default tenancy
- D. Host-based tenancy

19.Which of the following describes how Amazon Elastic MapReduce (Amazon EMR)
protects access to the cluster?

- A. The master node and the slave nodes are launched into an Amazon Virtual Private Cloud (Amazon VPC).
- B. The master node supports a Virtual Private Network (VPN) connection from the key specified at cluster launch.
- C. The master node is launched into a security group that allows Secure Shell (SSH)
and service access, while the slave nodes are launched into a separate security group
that only permits communication with the master node.
- D. The master node and slave nodes are launched into a security group that allows SSH and service access.

Answer: 

20.To help prevent data loss due to the failure of any single hardware component, Amazon
Elastic Block Storage (Amazon EBS) automatically replicates EBS volume data to which
of the following?

- **A. Amazon EBS replicates EBS volume data within the same Availability Zone in a region.**
- B. Amazon EBS replicates EBS volume data across other Availability Zones within the same region.
- C. Amazon EBS replicates EBS volume data across Availability Zones in the same region and in Availability Zones in one other region.
- D. Amazon EBS replicates EBS volume data across Availability Zones in the same region and in Availability Zones in every other region.

Answer: A
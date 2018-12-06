1.Which of the following objects are good candidates to store in a cache? (Choose 3 answers)

- **A. Session state**
- **B. Shopping cart**
- **C. Product catalog**
- D. Bank account balance

Answer: A, B, C 

2.Which of the following cache engines are supported by Amazon ElastiCache? (Choose 2 answers)

- A. MySQL
- **B. Memcached**
- **C. Redis**
- D. Couchbase

Answer: B, C

3.How many nodes can you add to an Amazon ElastiCache cluster running Memcached?

- A. 1
- B. 5
- **C. 20**
- D. 100

Answer: C

4.How many nodes can you add to an Amazon ElastiCache cluster running Redis?

- **A. 1**
- B. 5
- C. 20
- D. 100

Answer: 

5.An application currently uses Memcached to cache frequently used database queries.
Which steps are required to migrate the application to use Amazon ElastiCache with
minimal changes? (Choose 2 answers)

- A. Recompile the application to use the Amazon ElastiCache libraries.
- **B. Update the configuration file with the endpoint for the Amazon ElastiCache cluster.**
- **C. Configure a security group to allow access from the application servers.**
- D. Connect to the Amazon ElastiCache nodes using Secure Shell (SSH) and install the latest version of Memcached.

Answer: B, C

6.How can you back up data stored in Amazon ElastiCache running Redis? (Choose 2 answers)

- A. Create an image of the Amazon Elastic Compute Cloud (Amazon EC2) instance.
- **B. Configure automatic snapshots to back up the cache environment every night.**
- **C. Create a snapshot manually.**
- D. Redis clusters cannot be backed up.

Answer: B, C

7.How can you secure an Amazon ElastiCache cluster? (Choose 3 answers)

- A. Change the Memcached root password.
- **B. Restrict Application Programming Interface (API) actions using AWS Identity and Access Management (IAM) policies.**
- C. Restrict network access using security groups.
- D. Restrict network access using a network Access Control List (ACL).

Answer: B

8.You are working on a mobile gaming application and are building the leaderboard feature
to track the top scores across millions of users. Which AWS services are best suited for
this use case?

- A. Amazon Redshift
- B. Amazon ElastiCache using Memcached
- **C. Amazon ElastiCache using Redis**
- D. Amazon Simple Storage Service (S3)

Answer: C

9.You have built a large web application that uses Amazon ElastiCache using Memcached
to store frequent query results. You plan to expand both the web fleet and the cache fleet
multiple times over the next year to accommodate increased user traffic. How do you
minimize the amount of changes required when a scaling event occurs? **_Guess_**

- **A. Configure AutoDiscovery on the client side**
- B. Configure AutoDiscovery on the server side
- C. Update the configuration file each time a new cluster
- D. Use an Elastic Load Balancer to proxy the requests

Answer: A

10. Which cache engines does Amazon ElastiCache support? (Choose 2 answers)

- **A. Memcached**
- **B. Redis**
- C. Membase
- D. Couchbase

Answer: A, B
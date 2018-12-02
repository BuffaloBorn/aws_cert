Which of the following are required elements of an Auto Scaling group? (Choose 2 answers)

- **A. Minimum size**
- B. Health checks
- C. Desired capacity
- **D. Launch configuration**

Answer: A, D

You have created an Elastic Load Balancing load balancer listening on port 80, and you
registered it with a single Amazon Elastic Compute Cloud (Amazon EC2) instance also
listening on port 80. A client makes a request to the load balancer with the correct
protocol and port for the load balancer. In this scenario, how many connections does the
balancer maintain?

- A. 1
- **B. 2**
- C. 3
- D. 4

Answer: B

How long does Amazon CloudWatch keep metric data?

- A. 1 day
- B. 2 days
- C. 1 week
- **D. 2 weeks**

Answer: D

Which of the following are the minimum required elements to create an Auto Scaling launch configuration?

- **A. Launch configuration name, Amazon Machine Image (AMI), and instance type**
- B. Launch configuration name, AMI, instance type, and key pair
- C. Launch configuration name, AMI, instance type, key pair, and security group
- D. Launch configuration name, AMI, instance type, key pair, security group, and block device mapping

Answer: A

You are responsible for the application logging solution for your company’s existing
applications running on multiple Amazon EC2 instances. Which of the following is the
best approach for aggregating the application logs within AWS?

- A. Amazon CloudWatch custom metrics
- **B. Amazon CloudWatch Logs Agent**
- C. An Elastic Load Balancing listener
- D. An internal Elastic Load Balancing load balancer

Answer: B

Which of the following must be configured on an Elastic Load Balancing load balancer to accept incoming traffic?

- A. A port
- B. A network interface
- **C. A listener**
- D. An instance

Answer: C

You create an Auto Scaling group in a new region that is configured with a minimum size
value of 10, a maximum size value of 100, and a desired capacity value of 50. However,
you notice that 30 of the Amazon Elastic Compute Cloud (Amazon EC2) instances within
the Auto Scaling group fail to launch. Which of the following is the cause of this
behavior?

- A. You cannot define an Auto Scaling group larger than 20.
- B. The Auto Scaling group maximum value cannot be more than 20.
- C. You did not attach an Elastic Load Balancing load balancer to the Auto Scaling group.
- **D. You have not raised your default Amazon EC2 capacity (20) for the new region.**

Answer: D

You want to host multiple Hypertext Transfer Protocol Secure (HTTPS) websites on a
fleet of Amazon EC2 instances behind an Elastic Load Balancing load balancer with a
single X.509 certificate. How must you configure the Secure Sockets Layer (SSL)
certificate so that clients connecting to the load balancer are not presented with a
warning when they connect?

- **A. Create one SSL certificate with a Subject Alternative Name (SAN) value for each website name.**
- B. Create one SSL certificate with the Server Name Indication (SNI) value checked.
- C. Create multiple SSL certificates with a SAN value for each website name.
- D. Create SSL certificates for each Availability Zone with a SAN value for each website name.

Answer: A

Your web application front end consists of multiple Amazon Compute Cloud (Amazon
EC2) instances behind an Elastic Load Balancing load balancer. You have configured the
load balancer to perform health checks on these Amazon EC2 instances. If an instance
fails to pass health checks, which statement will be true?

- A. The instance is replaced automatically by the load balancer.
- B. The instance is terminated automatically by the load balancer.
- **C. The load balancer stops sending traffic to the instance that failed its health check.**
- D. The instance is quarantined by the load balancer for root cause analysis.

Answer: C

In the basic monitoring package for Amazon Elastic Compute Cloud (Amazon EC2), what
Amazon CloudWatch metrics are available?

- A. Web server visible metrics such as number of failed transaction requests
- B. Operating system visible metrics such as memory utilization
- C. Database visible metrics such as number of connections
- **D. Hypervisor visible metrics such as CPU utilization**

Answer: D

A cell phone company is running dynamic-content television commercials for a contest.
They want their website to handle traffic spikes that come after a commercial airs. The
website is interactive, offering personalized content to each visitor based on location,
purchase history, and the current commercial airing. Which architecture will configure
Auto Scaling to scale out to respond to spikes of demand, while minimizing costs during
quiet periods?

- A. Set the minimum size of the Auto Scaling group so that it can handle high traffic volumes without needing to scale out.
- B. Create an Auto Scaling group large enough to handle peak traffic loads, and then stop some instances. Configure Auto Scaling to scale out when traffic increases using the stopped instances, so new capacity will come online quickly.
- C. Configure Auto Scaling to scale out as traffic increases. Configure the launch configuration to start new instances from a preconfigured Amazon Machine Image (AMI).
- **D. Use Amazon CloudFront and Amazon Simple Storage Service (Amazon S3) to cache changing content, with the Auto Scaling group set as the origin. Configure Auto Scaling to have sufficient instances necessary to initially populate CloudFront and Amazon ElastiCache, and then scale in after the cache is fully populated.**

Answer: D

For an application running in the ap-northeast-1 region with three Availability Zones (apnortheast-
1a, ap-northeast-1b, and ap-northeast-1c), which instance deployment provides
high availability for the application that normally requires nine running Amazon Elastic
Compute Cloud (Amazon EC2) instances but can run on a minimum of 65 percent
capacity while Auto Scaling launches replacement instances in the remaining Availability
Zones?

- A. Deploy the application on four servers in ap-northeast-1a and five servers in apnortheast-1b, and keep five stopped instances in ap-northeast-1a as reserve.
- **B. Deploy the application on three servers in ap-northeast-1a, three servers in apnortheast-1b, and three servers in ap-northeast-1c.**
- C. Deploy the application on six servers in ap-northeast-1b and three servers in apnortheast-1c.
- D. Deploy the application on nine servers in ap-northeast-1b, and keep nine stopped instances in ap-northeast-1a as reserve.

Answer: B

Which of the following are characteristics of the Auto Scaling service on AWS? (Choose 3
answers)

- **A. Sends traffic to healthy instances**
- **B. Responds to changing conditions by adding or terminating Amazon Elastic Compute Cloud (Amazon EC2) instances**
- C. Collects and tracks metrics and sets alarms
- D. Delivers push notifications
- E. Launches instances from a specified Amazon Machine Image (AMI)
- **F. Enforces a minimum number of running Amazon EC2 instances**

Answer: A, B, F

Why is the launch configuration referenced by the Auto Scaling group instead of being
part of the Auto Scaling group?

- A. It allows you to change the Amazon Elastic Compute Cloud (Amazon EC2) instance type and Amazon Machine Image (AMI) without disrupting the Auto Scaling group.
- B. It facilitates rolling out a patch to an existing set of instances managed by an Auto Scaling group.
- C. It allows you to change security groups associated with the instances launched without having to make changes to the Auto Scaling group.
- **D. All of the above**
- E. None of the above

Answer: D

An Auto Scaling group may use: (Choose 2 answers)

- **A. On-Demand Instances**
- B. Stopped instances
- **C. Spot Instances**
- D. On-premises instances
- E. Already running instances if they use the same Amazon Machine Image (AMI) as the Auto Scaling group’s launch configuration and are not already part of another Auto Scaling group

Answer: A, C

Amazon CloudWatch supports which types of monitoring plans? (Choose 2 answers)

- **A. Basic monitoring, which is free**
- B. Basic monitoring, which has an additional cost
- C. Ad hoc monitoring, which is free
- D. Ad hoc monitoring, which has an additional cost
- E. Detailed monitoring, which is free
- **F. Detailed monitoring, which has an additional cost**

Answer: A, F

Elastic Load Balancing health checks may be: (Choose 3 answers)

- **A. A ping**
- B. A key pair verification
- **C. A connection attempt**
- **D. A page request**
- E. An Amazon Elastic Compute Cloud (Amazon EC2) instance status check

Answer: A, C, D

When an Amazon Elastic Compute Cloud (Amazon EC2) instance registered with an
Elastic Load Balancing load balancer using connection draining is deregistered or
unhealthy, which of the following will happen? (Choose 2 answers)

- A. Immediately close all existing connections to that instance.**
- **B. Keep the connections open to that instance, and attempt to complete in-flight requests.**
- C. Redirect the requests to a user-defined error page like “Oops this is embarrassing” or “Under Construction.”
- **D. Forcibly close all connections to that instance after a timeout period.**
- E. Leave the connections open as long as the load balancer is running.

Answer: B, D

Elastic Load Balancing supports which of the following types of load balancers? (Choose
3 answers)

- **A. Cross-region**
- **B. Internet-facing**
- C. Interim
- D. Itinerant
- **E. Internal**
- F. Hypertext Transfer Protocol Secure (HTTPS) using Secure Sockets Layer (SSL)

Answer: A, B, E

Auto Scaling supports which of the following plans for Auto Scaling groups? (Choose 3
answers)

- A. Predictive
- **B. Manual**
- C. Preemptive
- **D. Scheduled**
- **E. Dynamic**
- F. End-user request driven
- G. Optimistic

Answer: B, D, E
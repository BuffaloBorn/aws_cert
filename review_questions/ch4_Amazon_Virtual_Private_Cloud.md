What is the minimum size subnet that you can have in an Amazon VPC?
- A. /24
- B. /26
- __C. /28__
- D. /30
Answer: C

You are a solutions architect working for a large travel company that is migrating its
   existing server estate to AWS. 
   
   You have recommended that they use a custom Amazon VPC, and they have agreed to proceed. 
  
   They will need a public subnet for their web servers and a private subnet in which to place 
   their databases. They also require that the web servers and database servers be highly 
   available and that there be a minimum of two web servers and two database servers each. 
   
   How many subnets should you have to maintain high availability?
   
- A. 2
- B. 3
- __C. 4__
- D. 1

Answer: C

Which of the following is an optional security control that can be applied at the subnet
layer of a VPC?

- A. Network ACL
- __B. Security Group__
- C. Firewall
- D. Web application firewall

Answer: B

What is the maximum size IP address range that you can have in an Amazon VPC?

- __A. /16__
- B. /24
- C. /28
- D. /30

Answer: A

You create a new subnet and then add a route to your route table that routes traffic out
from that subnet to the Internet using an IGW. What type of subnet have you created?

- A. An internal subnet
- B. A private subnet
- C. An external subnet
- __D. A public subnet__

Answer: D

What happens when you create a new Amazon VPC? **_Guess_**

- __A. A main route table is created by default.__
- B. Three subnets are created by default—one for each Availability Zone.
- C. Three subnets are created by default in one Availability Zone.
- D. An IGW is created by default.

Answer: A

You create a new VPC in US-East-1 and provision three subnets inside this Amazon VPC.

Which of the following statements is true?

- __A. By default, these subnets will not be able to communicate with each other; you will
     need to create routes.__
- B. All subnets are public by default.
- C. All subnets will be able to communicate with each other by default.
- D. Each subnet will have identical CIDR blocks.

Answer: A

How many IGWs can you attach to an Amazon VPC at any one time?

- __A. 1__
- B. 2
- C. 3
- D. 4

Answer: A

What aspect of an Amazon VPC is stateful?

- A. Network ACLs
- __B. Security groups__
- C. Amazon DynamoDB
- D. Amazon S3

Answer: B

You have created a custom Amazon VPC with both private and public subnets. You have
created a NAT instance and deployed this instance to a public subnet. You have attached
an EIP address and added your NAT to the route table. Unfortunately, instances in your
private subnet still cannot access the Internet.    **_Guess_** 

What may be the cause of this?

- A. Your NAT is in a public subnet, but it needs to be in a private subnet.
- B. Your NAT should be behind an Elastic Load Balancer.
- __C. You should disable source/destination checks on the NAT.__
- D. Your NAT has been deployed on a Windows instance, but your other instances are
     Linux. You should redeploy the NAT onto a Linux instance.
 
Answer: A 

Which of the following will occur when an Amazon Elastic Block Store (Amazon EBS)-
backed Amazon EC2 instance in an Amazon VPC with an associated EIP is stopped and
started? (Choose 2 answers)

- __A. The EIP will be dissociated from the instance.__
- B. All data on instance-store devices will be lost.
- C. All data on Amazon EBS devices will be lost.
- __D. The ENI is detached.__
- E. The underlying host for the instance is changed.

Answer: A, D

How many VPC Peering connections are required for four VPCs located within the same
AWS region to be able to send traffic to each of the others?

- __A. 3__
- B. 4
- C. 5
- D. 6  

Answer: A

Which of the following AWS resources would you use in order for an EC2-VPC instance
to resolve DNS names outside of AWS?  **_Guess_** 

- A. A VPC peering connection
- B. A DHCP option set
- C. A routing rule
- __D. An IGW__

Answer: D

                                                                               
Which of the following is the Amazon side of an Amazon VPN connection?   **_Look this in Summary; need more reseach_** 

- A. An EIP
- B. A CGW
- C. An IGW
- __D. A VPG__

Answer: D

What is the default limit for the number of Amazon VPCs that a customer may have in a
region?

- A. 5
- B. 6
- C. 7
- __D. There is no default maximum number of VPCs within a region.__

Answer: D

You are responsible for your company’s AWS resources, and you notice a significant
amount of traffic from an IP address in a foreign country in which your company does
not have customers. Further investigation of the traffic indicates the source of the traffic
is scanning for open ports on your EC2-VPC instances. Which one of the following
resources can deny the traffic from reaching the instances?

- A. Security group
- __B. Network ACL__
- C. NAT instance
- D. An Amazon VPC endpoint

Answer: B

Which of the following is the security protocol supported by Amazon VPC?

- A. SSH
- __B. Advanced Encryption Standard (AES)__
- C. Point-to-Point Tunneling Protocol (PPTP)
- D. IPsec

Answer: B

Which of the following Amazon VPC resources would you use in order for EC2-VPC
instances to send traffic directly to Amazon S3?

- A. Amazon S3 gateway
- B. IGW
- C. CGW
- __D. VPC endpoint__

Answer: D

What properties of an Amazon VPC must be specified at the time of creation? **_Guess_**
(Choose 2 answers)

- __A. The CIDR block representing the IP address range__
- B. One or more subnets for the Amazon VPC
- __C. The region for the Amazon VPC__
- D. Amazon VPC Peering relationships

Answer: A, C

Which Amazon VPC feature allows you to create a dual-homed instance?  **_Look this in Summary; need more reseach_**

- A. EIP address
- __B. ENI__
- C. Security groups
- D. CGW

Answer: B
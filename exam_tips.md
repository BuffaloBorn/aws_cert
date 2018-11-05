### IAM - Identity Access Management 

* IAM consists of the following:
    - Users 
    - Groups ( A way to group our users and apply polices to them collectively ) 
    - Roles 
    - Policy Documents.
        - are made up of javascript object notation. 
* IAM is universal. It does not apply to regions at this time. 
    - region that you perform IAM actions in does not matter.
* The "root account" is simply the account created when first setup your AWS account. 
    - It has complete Admin access by default.
* New Users have NO permissions when first created. 
* New Users are assigned Access Key ID & Secret Access Keys when first created.
* These are not the same as a password, and you cannot use Access Key ID & Secret Access Key to login in to console. You can use this to access AWS via the APIs ans Command Line however.
* You only get to view these once. If you lose them, you have to regenerate them. So save them in secure location. 
* Always setup Multifactor Authentication on your root account.
* You can create and customize your own password rotation policies.
   
### S3 (Simple Storage Service) - Exam Tips For S3 101

* Remember that S3 is Object-based: ie allows you to upload files
* Files can be from 0 bytes to 5 TB.
* There unlimited storage
* Files are stored in buckets.
* S3 is universal namespace. That is, names must be unique globally, 
* Example of bucket name: https://s3-eu-west-1.amazonaws.com/acloudguru
* Read after Write consistency for PUTS of new Objects
    - so if you create a new object in S3 or you put a new object in two and three you’ll be able to read that information immediately after you've written to S3 to be able to read a text
* Eventual consistency for overwrite PUTS and DELETES (can take some time to propagate)
* S3 Storage Classes/Tiers
    - S3 (durable, immediately available, frequently accessed)
    - S3-IA (durable, immediately available, infrequently accessed)
    - S3 One Zone - IA (even cheaper than IA, but only in one availability zone.)
    - Glacier - Archived data, where you can wait 3 - 5 hours before accessing.
* Remember the core fundamentals of an S3 object:
    - Key (name)
    - Value (data)
    - Version ID
    - Metadata
    - Sub-resources
        - ACL
        - Torrent
* Object-based storage only (for files.)
* Not suitable to install an operating system on.
* Successful updates will generate a HTTP 200 status code.
* Read the S3 FAQs before taking the exam. It comes up LOT!!	 
 
### Creates an S3 Bucket - Exam Tips

* Buckets are universal name space
* Upload an object to S3 receive
* S3
    - availability - 99.99%
    - durability - 99.9999999999% 
* S3-IA
    - availability - 99.99%
    - durability - 
* S3 Reduced Redundancy Storage
    - availability - 99.99%
    - durability - 99.99%
* Encryption  
    - Client Side Encryption
    - Server Side Encryption
        - Server Side Encryption with Amazon S3 Managed Keys (SSE-S3)
        - Server Side Encryption with KMS (SSE-KMS)
        - Server Side Encryption with Customer Provided Keys (SSE-C)
 * Control access to buckets using either a bucket ACL or using Bucket Polices
 * BT DEFAULT ARE PRIVATE AND ALL OBJECTS STORED INSIDE THEM ARE PRIVATE
        
 ### S3 - Versioning - Exam Tips
  
* Stores all versions of an object (including all writes and even if you delete an object )
* Great backup tool
* Once enabled, versioning cannot be disabled, only suspended.
* Integrates with Lifecycle rules
* Versioning's MFA Delete capability, which uses multi-factor authentication, can be used to provide an additional layer of security. 

##### S3 - Cross Region Replication 

* Versioning must be enabled on both the source and destination buckets. 
* Regions must be unique. 
* Files in an existing bucket are not replicated automatically. All subsequent updated files will be replicated automatically. 
* You cannot replicate to multiple buckets or use daisy chaining (at this time.)
* Delete marker are replicated. 
* Deleting individual versions or delete markers will not be replicated. 
* Understand what Cross Region Replication is high level. 

#### S3 - Lifecycle Management 

* Can be used in conjuction wiht versioning
* Can be applied to current versions and previous versions.
* Following actions can now be down:
    - Transition to the standard - Infrequent Access Storage Class
    (30 days after the creation date.) 
   - Archive to the Glacier Storage Class (30 days after IA, if relevant)
* Permanently Delete

##### S3 - CloudFront - Exam Tips

* Edge Location - This is the location where content will be cached. This separate to AWS Region/AZ
* Origin - This is the origin of all the files that the CDN will distribute. This can be either an S3 Bucket, an EC2 instance, an Elastic Load Balancer or Route53.
* Distribution - This is the name given the CDN which consists of a collection of Edge Locations.
    - Web Distribution - Typically used for websites.
    - RTMP - Used for media streaming
* Edge locations are not just READ only, you can write to them too. (ie. put an object on them)
* Objects are cached for the life of the TTL (Time To Live)
* You can clear cached objects, but you will be charged. 
     
     
 ##### S3 - Storage Gateway
 
 * File Gateway - For flat files, stored directly on S3
 * Volume Gateway: 
    - Stored Volumes - Entire Dataset is stored on site and is asynchronously backed up to S3.
    - Cached Volumes - Entire Dataset is stored on S3 and the most frequently accessed data is cached on site. 
 * Gateway Virtual Tape Library (VTL)
    - Used for backup ans uses popular backup applications like NetBackup, Backup Exec, Veeam etc.
    
##### S3 - Snowball

* Understand what snowball is
* Understand what Import Export is
    - from historical perceptive 
* Snowball can do 
    - import to S3
    - export from S3  
   
 ### EC2 (Elastic Cloud Compute)
 * Know the difference between pricing models:
    - On-demand
        - You buy the second or by the hour
    - Spot 
        - You set a bid price 
        - If that spot price equals that bid price your instances will be provisioned 
        - As soon as the spot price goes over your bid price instances will terminate.
        - Remember that if that happens in and out 1 hour period or let's say 20 minutes you won't be charged
          for that hour.
    - Reserved
        - Where we can reserve capacity
        - The contracts run from 12 months to 36 months.
        - The more you pay up front the bigger discount that you get.
    - Dedicated 
        - Are typically around licensing 
        - Could have issues where your regulator does not want you to use shared or multi-tenant to the hardware.
 * Remember with Spot instances: 
    - If you terminate the instance you pay for the hour.
    - if AWS terminates the spot instances then you get the hour that it was terminated in for free.
 * Instance Types
 
 |Family|Speciality|Use Case|
 |------|-----------|-------|
 |F1|Field Programmable Gate Array| Genomics research, financial analytics, real-time video processing, big data etc|
 |I3|High Speed Storage|NoSQL DBs, Datawarehousing|
 |G3|Graphics Intensive |Video Encoding / 3D Application Streaming|
 |H1|High Disk Thoughhout|MapReduce-based workloads, distributed file systems such as HDFS and MapR-FS|
 |T2|Lowest Cost General Purpose|Web Servers / Small DBs|
 |D2|Dense Storage|Fileservers / Data Warehousing / Hadoop|
 |R4|Memory Optimized |Memory Intensive Apps/DBs|
 |M5|General Purpose|Application Servers|
 |C3| Compute Optimized|CPU Intensive Apps / DBs|
 |P3|Graphics/General Purpose GPU|Machine Learning, Bit Coin Mining etc|
 |X1| Memory Optimized|SAP HANA / Apache Spark|  
 
 * How do I remember them now:
    - F for FPGA
    - I for IOPS
    - G for Graphics
    - H for High Disk Throughput
    - T for cheap general purpose(think T2 Mirco)
    - D for Density
    - R for RAM
    - M - main choice for general purpose apps
    - C for compute
    - P - Graphic (think PICS)
    - X - Extreme Memory
    
    FIGHT DR MC PIX 
 
 ### EBS (Elastic Block Storage)
 * Performance for EBS is primarily measured in input/output operations per second (IOPS)
 
 * EBS Consists of:
    - SSD, General Purpose 
        - GP2 - (Up to 10,000 IOPS)
    - SSD, Provisioned IOPS - 
        - IO1 - (More than 10,000 IOPS)
    - HDD, Throughput Optimized 
        - ST1 - frequently accessed workloads 
    - HDD, Cold 
        - SC1 - less frequently accessed data
        - things like you know file servers
    - HDD, Magnetic 
        - Standard 
        - cheap, infrequently accessed storage
  * You can not mount 1 EBS volume to multiple EC2 instance
    - instead use EFS if you do need to share data between instances 
      or access via S3 bucket.    
  * Termination Protection is turned off by default, you must turn it on
  * On an EBS-backed instance, the default action is for the root EBS volume to be deleted when the instance is terminated
  * EBS backed root volumes can now be encrypted using AWS API or console or you can use a third party tool to encrypt the root volume
    - Bitlocker, etc 
    
### Volumes vs Snapshots
  
  * Volumes exist on EBS
    - basically a Virtual Hard Disk in the cloud
  * Snapshots exit on S3
  * You can take a snapshot of a volume, this will store that volume on S3
  * Snapshots are point in time copies of Volumes
  * Snapshots are incremental. 
    - This means that only the blocks that have changed since your last snapshot are moved to S3.
    - a way of saving storage
  * If this is your first snapshot, it may take some time to create.
  * Snapshots of encrypted volumes are encrtyed automatically
  * Volumes restored from encrypted snapshots are encrypted automatically. 
  * You can share snapshots, but only if they unencrypted.
    - that's why when you go into provision an E2C instance using the Amazon AMI. You can actually encrypt it right from the get go. 
    - You basically have to have an unencrypted root device volume when you provision it. 
    - And then you basically deploy that snapshot and you can then encrypt the root device volume's 
    - And then finally these snapshots can be shared with other AWOS accounts all made public but only if they are unencrypted.  
        - These snapshot can be shared with other other AWS accounts or made public.
  
 ### Snapshots of Root Device Volumes
 
 * To create a snapshot for Amazon EBS volumes that serve as root devices, you should stop the instance before taking the snapshot. 
 
 ### EBS (Elastic Block Storage)vs Instance Store
 
 * Instance storage volumes are sometimes called Ephemeral Storage
 * Instance storage cannot be stopped. If the underlying host fails, you will lose your data. 
 * EBS backed volumes can be stopped. You will not lose the data on this instance if it is stopped. 
 * You can reboot both, you will not lose your data.
 * By default, both ROOT volumes will be deleted on termination. 
    - Root volume is where you install your Operating System
    - However, with EBS volumes, you can tell  AWS to keep the root device volume. 
##### How can I take a snapshot of RAID Array?

 * Problem - Take a snapshot, the snapshot excludes data help in the cache bt applications and ths OS. This tends not to matter on a single volume. However, using multiple volumes in a RAID array, this can be to interdependenies  of the array.
 * Soulution - Take an application consistent snapshot
 * Stop the application from writing to disk.
 * Flush all caches to the disk
 * How can we do this?
    - Freeze the file system
    - Unmount the RAID Array
    - Shutting down the associated EC2 instance
    
### AMI - Amazon Machine Images

 * AMI are regional. You can only launch an AMI from the region in which it is stored. However you can copy AMIs to other regions using the console, command line, or the Amazon EC2 API.   
 
 ### Monitoring 
 
 * By default, the standard monitoring is set every 5 minutes
 * If you want more refined monitoring, we have detailed monitoring 
    - will be every 1 minute; that will cost you a little bit extra 
 * CloudWatch is used for performance monitoring so things like CPQ utilization, network throughput, disk utilization and etc..
 * CloudTrails is for auditing. 
     - By turning on cloudTrail ```on```; it basically audits any API call or anything that you do inside the AWS console will be recorded in CloudTrail.
 * The Exam will try to trick you between CloudWatch and CloudTrail. 
     - CloudWatch is for performance monitoring and CloudTrail is for auditing. 
 ##### What can I do with CloudWatch?
 
 1. Dashboards - CloudWatch creates awesome dashboards to see what is happening with youe environment.
 2. Alarms - Allows you to set Alarms that notify you when particular threshold are hit.
    - So when we go and do the Wordpress lab we're going to look at CPU utilization of over 80 percent that would trigger an alarm which would then trigger some auto scaling groups. 
 3. Events - CloudWatch Events helps you to respond to state changes in AWS resources. 
    - We do actually look at that in a lot more detail in the security specialty course which is where we basically use cloud watch events to trigger automated security responses.
 4. Logs - CloudWatch Logs helps you to aggregate, monitor, and store logs. 
    - The cool thing about CloudWatch logs is you can actually send data from outside your AWS environment to cloud watch logs as well. 
 
 ##### Roles 
 
 * Roles are more secure then storing your access key and secret access key on individual EC2 instance. 
    - Because if that instances is compromised obviously people have got access to your secret access and they would be able to access your AWS resources from anywhere in the world. 
    - It's much easier to just give an EC2 instance a role which allows it to access other services such as S3.
 * Roles are easier to manage
    - Roles are also much easier to manage because if you are storing your access key ID and secret access key on a thousand two instances and a key does get compromised and you suddenly revoke the key and re-issue a new one.
    - Then you have to go into each thousand instance and update the access key ID and secret access key.
 * Roles can be assigned  to an EC2 instance AFTER it has been provisioned using both the command line and AWS console. 
    - On the exam, it was only able to apply roles when you provision your EC2 instance.
    - this is no longer the case
    - Now you can definitely assign and change 0 to an easy to instance after it's been commissioned.
    - Roles are universal so you can use them in any region.
    - Basically almost everything inside identity access management such as users groups etc. is universal so it's not region specific.

##### Instance Meta

* Used to get information about an instance (such as public ip)
* Using the following command: 
    - curl http://169.254.169.254/latest/metadata/
        - getting data about the instance
            - private IP
            - public IP
            - DNS
            - etc
    - curl http://169.254.169.254/latest/usr-data/
    
 ##### EFS (Elastic File System) - Features
 
 * Supports the Network File File System version 4(NFSv4) protocol
 * You only pay for the storage you use (no pre-provisioning required)
 * Can scale up to the petabytes
    - And it can scale all the way up to petabytes so it is a really resilient service.
 * Can support thousands of concurrent NFC connections
 * Data is stored across multiple AZs within a region
 * Read After Write Consistency 
    - So it is very resilient and the consistency model for FS is read after so as soon as you've written the data you would then be able to go in and read that data.
    
 ##### What is Lamba?
  * AWS Lamba is a compute service where you can upload you code and create a Lamba function. AWS Lamba takes care of provisioning and managing the servers that you use to run the code. You don't have to worry about operating systems, patching, scaling, etc. You can use Lamba in the following ways:
    * As an event-driven compute service where AWS Lamba runs your code in response to events. There events could  be changes to data in an Amazon S3   bucket or Amazon DynamDB table.
    * As a compute service to run your code in response to HTTP requests using Amazon API Gateway or API calls  made using AWS SDKs. This is what we use A Cloud Guru.    
    
 ##### What is Placement Group?
  * Two Types of Place Groups: 
    - Clustered Placement Group 
        * Essentially mean that it's always going to be in one availability zone and it's use for big data.
        * It's used for things like low latency and high network throughput.
    - Spread Placement Group 
        - You've got like really important EC2 instances and you want them on individual pieces of hardware.
        - You don't want the your critical EC2 instances to be on the same hardware.
        - You essentially are guaranteeing that they are in separate pieces of hardware.
         
  * If you see the term, placement group on the Exam and it does not say clustered or spread; assume that it clustered  
  
### Exam tip breakdown

##### Certainly with EC2 and S3, you're probably actually 75 percent on the way to passing your exam.

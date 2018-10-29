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
   
### S3 - Exam Tips For S3 101

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
    - Subresources
        - ACL
        - Torrent
* Object-based storage only (for files.)
* Not suitable to install an operating system on.
* Successful updates will generate a HTTP 200 status code.
* Read the S3 FAQs before taking the exam. It comes up LOT!!	 
 
### Creates an S3 Bucket - Exam Tips

* Buckets are universal name space
* Upload an object to S3 receive
* S3, S3-IA, S3 Reduced Redundancy Storage
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
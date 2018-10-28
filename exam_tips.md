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
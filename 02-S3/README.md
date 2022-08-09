## What is S3?

S3 provides developers and IT teams with secure, durable, highly scalable object storage. Amazon
S3 is easy to use, with a simple web services interfaces.

- Perfect for files that don't change.
- Object Based Storage.
- S3 Safe place to store your files.
- Data is spread across multiple datacenters.
- Unlimited storage.
- Storage buckets is like a folder in the cloud.
- S3 is a universal namespace. Unique name globally.


https://s3-eu-west-1.amazonaws.com/acloudguru

When you upload a file to S3, you will receive a 200 response.

Objects consist of:
- Key - File Name
- Value - data that makes up an object
- Version ID -
- Metadata -
- Subresources:
	- Access Control Lists
	- Torrent

How does data consistency work for S3?
- If you write a new file and read it immediately afterwards, you will be able to view that data.
- If you update an existing file, or delete a file and read it immediately, you may get the older version, or you may not. Basically changes to objects can take a little bit of time to propagate globally.
* Read after Write consistency for PUTS of new Objects
* Eventual Consistency for overwrites PUTS and DELETES

#Guarantees
* Built for 99.99% availability for the S3 platform.
* Amazon guarantees 99.99999999% durability  11 9's.

- Tiered Storage Available
- Lifecycle Management
- Versioning
- Encryption
- Secure your data using Access Control Lists (file level) and Bucket Policies (bucket level)

* S3 Standard 11 9's durability
* S3 IA - Infrequently Accessed - Data that is access less frequently, but requires rapid access when needed. Lower fee than S3, but you are charged a retrieval fee. Access once ever 2-3 Months
* S3 Once Zone - IA - Do not require multiple Availability Zone data resilience
* S3 Intelligent Tiering - Designed to optimize costs by automatically moving data to the most cost-effective access tier, without performance impact or overhead performance.

* S3 Glacier Flexible Retrieval - is a secure, durable, and low-cost storage class for data archiving. Files that are accessed 1-2 times a year. You can reliably store any amount of data at costs, that are competitive with or cheaper than on-premises solutions. Retrieval times configurable from minutes to hours.
* S3 Glacier Instant Retrieval - Fastest access to S3 Archival data.
* S3 Glacier Deep Archive - is Amazons S3 lowest-cost where retrieval time of 12 hours is acceptable. Lowest cost storage class designed for long-term retention of data that will be retained for 7-10 years

## S3 Transfer Acceleration
Utilizes Amazon's Cloud Front global distributed edge locations. As the data arrives at a an edge location, data is routed to Amazon S3 over an optimized network path. It's own backbone network.

Cross-Region - allows disaster recovery.

Exam Tips:
 * S3 is Object based
 * Files can be from 0 Bytes to 5 TB.
 * There is unlimited storage
 * Files are stored in Buckets
 * S3 is universal namespace
 * Not suitable for an operating system
 * Successful uploads will generate a HTTP 200 status code

```
joel@joels-desktop:~/Desktop$ aws s3 cp image.jpeg s3://joels-personal-bucket/ --acl public-read --profile personal
upload: ./image.jpeg to s3://joels-personal-bucket/image.jpeg
```

'https://joels-personal-bucket.s3.amazonaws.com/image.jpeg'


Static website can be served up from S3 specifically

```
joel@joels-desktop:~/Desktop$ aws s3 cp ~/Documents/Stelligent/certified-aws-cloud-practioner/02-S3/website-index-sample.html s3://joels-personal-bucket/ --acl public-read --profile personal
upload: ../Documents/Stelligent/certified-aws-cloud-practioner/02-S3/website-index-sample.html to s3://joels-personal-bucket/website-index-sample.html
```

```
https://joels-personal-bucket.s3.amazonaws.com/website-index-sample.html
```

## S3 Versioning

* Stores all versions of an object
* Great backup tool
* Versioning cannot be disabled
* Integrates with lifecycle rules
* Versioning's MFA Delete capacity


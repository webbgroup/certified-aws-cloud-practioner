# STorage Types

## S3

* Provides developers and IT Teams with secure, durable, highly scalable object storage
* Easy to use. for Files.
* Can't install for database, or OS's on
* Flat files.

## Elastic Block Storage (EBS)
* Used for Volumes
* Used for OS's or Databases store.
* Not as redundant as S3. Storing OS.
* Automatically replicated and protention from component failure

## Elastic File Storage (EFS)
* Doesn't come as a set size,
* So if you have 10 gigs, and it will grow to accompany it.
* Multiple EC2 Instances can access the EFS store.


### Differences between EFS and EBS
* It automatically adjusts



- S3 is used to storing flat files.
- EBS is a virtual disk that can be attached to an EC2 instances, Size of disk can be changed but not automatic.
- EFS is a virtual disk that can be attached to EC2 and is scaled up/down depending on usage. Multiple EC2 instances.





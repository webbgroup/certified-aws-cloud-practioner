# Compliance


# Shared Responsibility

In the Cloud is responsibility of the Customer
Nobody can run into the Datacenter

If you don't patch your own EC2 instances, and you get hacked, that's your fault.

Customer Responsibilities - Security IN the cloud
* Customer Data
* Platform Applications
* OS'es in the EC2
* Client Side Encryption/Server Side Encryption/Networking Traffic

AWS - Security OF the Cloud
* Software
* Hardware AWS Global Infrastructure
* Regions/ Availability Zones
* Edge Locations

RDS, S3 - Amazons Responsibility
EC2 - YOU are responsible

Can you, yourself do this in the AWS console or in EC2?
If yes, you are likely responsible. Security Groups, IAM Users, Patching EC2 Operating Systems, patching databases running on EC2 etc.
If not, AWS are likely responsible. Management of DataCenters, security cameras, cabling, patching RDS Operating System. etc.
Encryption is a shared responsibility.

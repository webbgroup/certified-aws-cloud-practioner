# Cloud Concepts

- Trade Capital Expense For Variable Expense
- Benefit from massive economies at scale
- Stop guessing about capacity
- Increase speed and agility
- Stop spending money running and maintaining data centers
- Go global in minutes


Types of Cloud Computing
* Infrastructure as a Service
* Platform as a Service
* Software as a Service

3 Types of Cloud Computing Deployments
* Public Cloud - AWS, Azure,GCP
* Hybrid - Mixture of publick and Private
* Private Cloud - using Openstack or VMWare


AZ's EdgeLocations and Rgions.

* A Region is a physical location in the world that consists of two or more Availability Zones.
Edge Locations > AZ > Region.

* An AZ is one or more discrete Data centers, each with redundant power networking, and connectivity, housed in seperate facilities

* Edge Location are endpoints for AWS which are used for caching content. Typically consists of Cloud Front, Amazons Content Delivery Network (CDN)


Choosing the right AWS Region
- Data Sovereignty Laws
	Is there a regulation that governs.
- Latency to end users
- AWS Services - us-east-1

Support Basic.
- Basic
- Developer 29/month
- Business 100/month
- Enterprise 15k/month and a Technical Account Manager (TAM)

Billing Alarms - will set one up if it goes over a certain value.


IAM stands for Identity Access Management, this is global
* Via the Console
* Programatically
* SDK's

Root has everything... and accounts should always have multi-factor authentication. A Group will always a place to store users. and assign policies to group.
Policies are JSON.

S3 is Object-based 0 Bytes to 5 TB's
Unlimited storage
Files are stored in Buckets
S3 is  universal namespace. one name that is used globally.
https://s3-eu-west-1.amazonaws.com/acloudguru

Not suitable for OS's
Key - Name of the Object
Value - Data in sequence of bytes

Read after Write constancy for PUTS on new Objects
Eventual Consistency for overwrites PUTS and GETS, can take time to propagate

Can have bucket in Regions

Can replicate the buckets and have a backup bucket to US can copy to Sydney. They can copy through edge locations.

S3 Standard
99.99% availabliltiy
11 9's of durability

S3-IA infrequently accessed
S3-One Zone - IA
S3-Intelligent Tiering
S3 Glacier
S3 Glacier Deep Archive - 12 hours of retrieval is acceptable.


Static websites can reside on website automatically. Like a Movie preview.

Edge Locations will cache. where content will be cached.

Origin this is the origin of all of the files that the CDN will disrbute


Distribution
Web Distribution
RTMP

Edge Locations are no just read only, you can write to them as well, put an object onto them. Objects are cached with a TTL.

EC2 -
On Demand - Pay as you go
Reserved - capacity reservation. Pay up front and get a discount 1-3 years terms
Spot - allows you to bid for what price you want to pay.
Dedicated Hosts - Physical EC2 services. regularity or server bound licensee.


F - FPGA
I - Iops
G - Graphical
H - High Disk Throughput
T - Cheap General Purpose T2 Micro
D - Density
R - RAM
M - Main choice
C - Compute
P - Picture Graphics
X - Xtream Memory
Y - Extream Memory and CPU
A - ARM Based
U - Utility Bare Metal


SSD -
	- General Purpose SSD (GP2) - Balances price and performance for a wide variety of workloads
	- Provisioned IOPS (IO1) - Highest Performance SSD volume for mission-critical low-latency or high-throughput workloads

Magnetic
  - ST1 - Low cost HDD volume designed for frequently accessed, throughput-intensive workloads
  - SC1 - Lowest cost HDD volume designed for less frequently access workloads (File Servers)
  - Magnetic - Previous Generation

Linux SSH Port 22
Windows 3389
HTTP 80
HTTPS 443

Everything in on 0.0.0.0/0
Individual IP address 1.2.3.4/32

Security Groups using ports
Each EC2 instance in each availability zone.

# Summary of Cloud Concepts Part 2

Interact with AWS 3 ways
* Console
* Command Line Interface
* SDK

Apply to EC2 Roles to instances at any time. When you do this the change takes place immediately.

Roles are universal, you do not need to specify what region they are on.

Load Balancers,

Application Load Balancers - Layer 7 Make Intelligent Decisions
Network load Balancers - Extream Performance/ Static IP Addresses
Classic Load Blanacers - Test & Dev, Keep Costs Low   Test and Dev

RDS -
 SQL
 MySQL
 PostGreSQL
 Auroroa
 MariaDB
 Oracle

DynamoDB (NoSQL)
RedShift (OLAP)

Elastic Cache
- Memcached
- Redis

Redshift for Business Data Warehousing.

Graph Databases - Neptune
* Scalability
* High Availability

RDS as 2 key Features
* Multi-AZ for Disaster Recovery
* Read Replicas - For Performance

Autoscaling allows you to provision multiple EXC2 instances behind a load balancer automatically depending on your demand.

DNS and Route 53 - works like a phone book. Amazons DNS is Route 53 (Port 53)

Elastic Beanstalk - quickly deploy and manage preconfgured CloudFormation

CloudFormation, use it all the time and set up all of these Resources.
Json or Yaml

Both Elastic Beanstalk and Cloud Formation are free, but resources are not free.


# Global Services
IAM
Route53
CloudFront
SES
SMS

# On Premise
Snowball - Data storage
Snowball Edge - Data Storage and Compute
Storage Gateway -
CodeDeploy
Opsworks
IoT Greengrass

#Cloud Watch
used for monitoring performance
installed on AWS as well as other applications
monitored for 5 minutes every 5 minutes by default.
You can have 1 minute intervals by turning on detailed monitoring
You can create Cloud watch alarms as it i

AWS Systems Manager
- Agent, on-premise or for fleet management.














































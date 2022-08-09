## Amazons Compute Platform

Historically, you would use Rackspace, they would aquire the servers, rack and stack.
And sign a contract for 3-5 years and renting.
Deployment would be like 2 weeks to 6 months.

Amazon and EC2, and say "Hey I want a VM", and get one in seconds.

Changed industry overnight.

1. On Demand - Allows you to pay a fixed rate by the hour (or by the second) with no commitment.

2. Reserved - Provides you with a capacity reservation, and offer a significant discount on the hourly charge for an instance.
Contract Terms are 1 Year or 3 Year Terms. The more you pay up front the better the term. Pay larger up front, greater the discount.

3. Spot - Enables you to bid whatever price you want for instance capacity, providing for even greater savings if your applications have flexible start and end times.

4. Dedicated Hosts - Physical EC2 server dedicated for your use. Dedicated Hosts can help you reduce costs by allowing you to use your existing server-bound software licenses. Fewer and fewer people use this.

### Pricing

On Demand pricing is useful for

- Users want the low cost and flexibility with no up front payment
- Applications with short term, spiky or unpredictable workloads that cannot be interrupted.
- Applications being developed for tested on Amazon EC2 for the first time.

Reserved Pricing
- Applications with steady state or predictable usage
- Applications that require reserved capacity
- Users able to make upfront payments to reduce their total computing costs even further.

Standard Reserve Instances - 75% off on Demand. More you pay up front, the greater the discount.
Convertible Reserved Instances - Offer up to 54% off on demand capability to change the attributes, as long as the exchange results are equal and greater values.
Scheduled Reserve Instances - Are available to launch within the time windows you reserve. Allows you to match your capacity reservation to a predictable recurring schedule that only requires a fraction of a day,week, or month.

Spot Pricing
- Applications that have flexible start and end times
- Applications that are only feasible at very low compute prices
- Users with urgent computing needs for a large amounts of additional capacity

Dedicated Hosts Pricing
- Useful for regulatory requirements that may not support multi-tenant virtualization
	- Government or Banking
- Great for licensing which does not support multi-tenancy or cloud deployments
- Can be purchased On-Demand.
- Can be purchased as a Reservation up to 70% on-demand price

EC2 Instance Types

F1 - Field Programmable Gate Array ++ Genomics research, financial analytics, real-time video processing, big data
I3 - High Speed Storage ++ NoSQL DB's, Data Warehousing, etc.
G4 - Graphics Intensive ++ Video Encoding/3D Application Streaming
H1 - High Disk Throughput ++ MapReduse-based workloads, distributed file systems such as HDFS and MapR-FS
T4g - Lowest Cost, General Purpose ++ Web Servers/Small DB's
D2 - Dense Storage ++ FileServers/Data Warehousing/Hadoop
R6g - Memory Optimized * RAM ++ Memory Intensive Apps/ DB's
M6g - General Purpose ++ Application Servers
C6g - Compute Optimized ++ CPU Intensive Apps/DB's
P3 - Processing Graphics General Purpose GPU ++ Machine Learning, Bit Coin Mining, etc
X1e - Memory Optimized ++ SAP HANA/Apache Spark, etc
Z1D - High compute capacity and a high memory foot print ++ Ideal for electronic design automation EDA and certain relational database workloads with high per-core licensing costs.
A1 - Arm-based workloads ++ Scale out workloads such as web servers
U-12TB1 - Bare Metal * UTILITY ++ Bare metal capabilities that eliminate virtualization overhead.


Fight Dr McPXZ in Australia!

F - FPGA
I - IOPS
G - Graphics
H - High Disk Throughput
T - Cheap general purpose (think T2 Micro)
D - For Density
R - For RAM
M - Main choice for general purpose apps
C - Compute
P - Picture Graphics (think Pics)
X - Extreme Memory
Z - Extreme Memory and CPU
A - Arm-based workloads
U - Utility Bare Metal

Amazon Elastic Block Storage (EBS) allows you to create storage volumes and attach them to Amazon EC2 instances. Once attached you can create a file system

### SSD
- General Purpose SSD (GP2) - balances price and performance
- Provisioned IOPS SSD (IO1) - Highest performance SSD volume Perfect for Databases

### Magnetic
- Throughput Optimized (ST1) - Low cost HDD volume designed for frequently access, throughput-intensive workloads
- Cold HDD (SC1) - Lowest cost HDD volume designed for less frequently access workloads (File Servers)
- Magnetic - Previous Generation

Amazon EC2 Computes in the Cloud.
On Demand - Pay a fixed rate, Pay by the HOUR or by the second
Reserved - pay up front for the compute
Spot - flex pricing, make use of low demand. Price moves around
Dedicated Hosts - Government or Licensing Requirements.

if a Spot Instance is terminated by Amazon EC2, you will not be charged for a partial hour of usage. However if you termninate the instance yourself, you will be charged the instance hour.




















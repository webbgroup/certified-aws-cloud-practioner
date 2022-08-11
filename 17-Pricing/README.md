# How AWS Pricing Works

AWS Pricing

While number and services have increased dramatically.

Pay less when you reserve capacity.


Capex - Capital Expenditure
 - Buying a Server up front or a Server up front
 - It is a fixed sunk costs

Opex - Operational Expenditure
	- Pay for what you used. Think utility billing
	- Think of water, gas, electricity

* Pay as you go
* Pay less when you reserve
* Pay even less per unit by using more
* Pay even less as AWS grows
* Custom Pricing

## While pricing models vary across services, it's worthwhile to review key principles and best practices that are broadly available.

- Understand the Fundamentals of Pricing
- Start early with cost optimization.

3 Fundamental drivers of cost with AWS
- Compute
- Storage
- Data Outbound

Adopting cloud services is not just a technical evolution. It also requires changes to how organizations operate.
Start early with cost optimization before the environment grows complex.
Managing cost-effectively is needed at start.

AWS Services are priced independently and transparently. Reduce to paying as you need it. and not procurement.

Don't pay for them, when they are not running. instead of paying for them 24/7


AWS Services provide several pricing models depending on product

- On Demand
- Dedicated Instances
- Spot Instances
- Reservation

# Free Usage Tier. Free M2 micro.. What services are free

- Amazon VPC
- Elastic Beanstalk - CloudFormation and Resources are not
- CloudFormation - Resources you pay for
- Identity Access Management IAM
- Auto Scaling -
- Opsworks - DevOps product
- Consolidated Billing

# EC2 Pricing
* Clock Hours of Server Time
* Instance Type
* Pricing Model
* Number of Instances
* Load Balancing
* Detailed Monitoring 1 minute
* Auto Scaling
* Elastic IP Addresses
* Operating Systems and Software Packages (Windows is more expensive)

## Pricing

On-Demand
Reserved, capacity reservation discount up front
Spot, Pay when their capacity comes down. Bid for instance capacity. Flexible start and end time.
Dedicated Host - Dedicated for ServerBound licenses, or Compliancy.

More you pay up front the greater the savings.

## Lambda
What are the prices for Lambda. and build Alexa, it is Lambda.
* Request Pricing
	* Free Tier: 1 million requests per month
	* $.20 per 1 million request thereafter
* Duration Pricing
	* $400,000 GB-seconds per month free, up to 3.2 million seconds of compute time
	* $0.00001667 for every GB-second used thereafter

What determines price
* Additional charges
	* my incur additional charges for connectivity to S3

## EBS
* Volumes (Per GB)
* Snapshots (Per GB)
* Data Transfer

## S3
* Storage Class
* Storage
* Request - get puts or copies
* Data Transfer

## Glacier

* Storage
* Data Retrieval Times

## Snowball
* PetaByte-scale data transport solution that uses secure appliances to transfer large amounts of data
* Service fee per job
	* Snowball 50TB - $200
	* Snowball 80TB - $250
* Daily Charge
	* First 10 days are free, after that it is $15 a day
* Data Transfer
	* Data Transfer in to S3 is free. Data transfer out is not

## RDS
* Clock Hours of Server Time
* Data Characteristics
* Database Purchase Type
* Number of Database Instances
* Provisioned Storage
* Additional Storage
* Request
* Deployment Type
* Data Transfer

## DynamoDB
* One write capacity unit provides up to one write per second, enough for 2.5 million writes per month. .47
* One read capacity unit RCU provides up to two reads per second, enough for 5.2 million reads per month
* Indexed data storage, DynamoDB charges an hourly rate per GB of disk space. .25

## CloudFront
* Traffic Distribution
* Requests
* Data Transfer Out






















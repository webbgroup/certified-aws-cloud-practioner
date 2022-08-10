# Traditional Computing vs Cloud Computing

* IT Assets as Provisioned Resources
* Traditional would Purchase Order, Rack and Stack, and Time to Market.
* Global, Available and Scalable Capacity
	You can deploy in Dublin, Tokyo
* Higher Level Managed Services
* Built-in Security
* Architecture For Cost
* Operations on AWS


## Scalability

* Scale Up - Vertical Scaling - Add more Memory
* Scale Out
	* Stateless Applications - Like Alexa - runs on Lambda
	* Distribute Load to Multiple Nodes
	* Stateless Components - Account Details, Store it in Cookies
	* Stateful Components - What's in the Shopping Cart? Stored in the DB.
	* Implement Session Affinity - Sticky session stuck to an EC2 instance.
	* Distributed Processing - Multiple EC2 instances
	* Implement Distributed Processing -

## Instantiate Compute Resources

* Bootstrapping
* Golden Images - Set up Golden Images; WordPress already installed
* Containers -
* Hybrid -

## Infrastructure as Code
* CloudFormation

## Serverless Management and Deployment
* AWS Elastic Beanstalk
* Amazon EC2 auto Recovery
* AWS Systems Manager
* Auto Scaling

## Alarms and Events
* Amazon CloudWatch Alarms
* Amazon CloudWatch Events - File upload, triggering a Lambda Function
* AWS Lambda scheduled Events
* AwS WAF security automations

## Loose Coupling
Well Defined Interfaces
* Amazon API Gateway

Service Discovery
* Implement Service Discovery - Using RDS, will switch over to the other availability zone

SQS, put messages in this queue. Watermarks images, multiple EC2's polling to digest jobs.

## Distributed Systems Best Practices
* Graceful Failure in Practice

## Services Not Servers
* Managed Services Lambda, S3, Not relying on physical servers
* Serverless Architectures

"No server is easier to manage than no servers" Wener Vogels

### Part 2

## Relational Databases (Aurora)
* Scalability 6 copies or more
* High Availability - Multi AZ
* Anti-Patterns - no need for joins or complex transactions, use No-SQL

## Non-Relational Database (DynamoDB)
* Scalability
* High Availability - Multi-AZ
* Anti-Patterns - requires joins or complex transactions, should use RDMS instead.

## Data Warehouse (RedShift)
* Scalability
* High Availability - Multi-AZ
* Anti-Patterns - not meant for OnLine Transaction Processing. more for analysis

## Search
* Scalability
* Highly Available

## Graph Databases
* Scalability Neptune
* High Availability

###
Data Lake, an architectural approach that allows you to store massive amounts of data in a central
location so that it is readily available to be categorized, processed, analysed, and consumed by a diverse
groups within your organization.

* Introducing Redundancy
* Detect Failure
* Durable Data Storage
* Automated Multi-Data Center
* Fault Isolation and Traditional Horizontal Scaling
* Sharding

## Optimize for Cost
* Right Size
* Elasticity - Should be available for Black Friday Sales
* Take Advantage of the Variety of Purchasing Options
	* Reserved Capacity
	* Spot Instances

## Caching
* Application Caching
* Cloud Front

## Security
* Use AWS Features for Defense in Depth
* Share Security Responsibility with AWS
* Reduce Privileged Access
* Security as Code - Hardened EC2 with Security, and allow Golden Images
* Real-Time Auditing









































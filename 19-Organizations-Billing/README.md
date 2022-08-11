# AWS Organizations

- Available in two feature sets:
- Consolidated Billing
- All Features



 Root
 OU - Policy - Might want Developers to be serverless. No EC2 instances
 		- AWS Account
 		- AWS Account

 OU - AWS Account
 		- AWS Account

You can just use it for Consolidated Billing

Paying Account 	- Test/Dev
								- Production
							  - Back Office

Paying Account is independent. Cannot access resources of other accounts

	20 Linked Account
	S3 Tiered Pricing
	Consolidated Billing will get volume discount

Practical Example

Test/Dev is using 600DB, Production uses 900 GB, and Back Office users 500GB.

* Without Consolidated Billing, we would pay
	- 600x.03 = $18
	- 900x.03 = $27
	- 500x.03 = $15
	- Total Bill = $60.00 for 2TB of storage
* 1TBx.03 = $30
* Next 1TB x.$002 $29.50
* Total Bill of $59.50


Test/Dev = Uses 6 on Demand Instances
Production = Has 5 Reserved Instances, Uses 3
Back Office =

Best Practices
* Always enable multi-factor authentication on root account
* Always use a strong and complex password on root account
* Paying account should be used for billing purposes only. Do not deploy resources into the paying account.

# Cloud Trail

Cloud Watch - Personal Trainer Monitors Performance EC2, used for AutoScaling. Historical Performance
Cloud Trail - Monitors API calls within the AWS platform. Auditing and Monitors API

Per AWS account and is enabled per region
Can consolidate logs using an S3 bucket
	1. Turn on CloudTrail in paying account.
	2. Create a bucket policy that allows cross-account access
	3. Turn on CloudTrail in the other accounts and use the bucket in the paying account. Log forwarding to Paying account.

Consolidated Billing allows you to get volume discounts on all your accounts.

Organizations is very handy for large organizations, because it allows an org to define polices based on departments as well as provides consolidated billing.













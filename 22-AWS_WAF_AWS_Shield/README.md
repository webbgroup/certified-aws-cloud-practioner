# AWS WAF and AWS Shield

What is a AWS WAF?
* Web Application Firewall

OSI Layers
Hardware..... Application Layer 7

Hardware Firewalls work at Layer 4.

Attacker => scripts WordPress vulnerability => SQL injection. Deleting all of the tables.
Attacker => Load Balancer

Attacker => WAF => Load Balancer = Prevents SQL injection.



AWS Shield is a managed DDoS protection service that safeguards web applications running on AWS.

Shield is turned on automatically.

- Standard
- Advanced

AWS Inspector vs AWS Trusted Advisor vs Cloud Trail


Amazon Inspector - looks for compliancy, provides finding by severity, or detailed. Agent installed on EC2 Instance, left this port open. or patch this
Amazon Trusted Advisor - allows to look at real time guidance for Performance, Security and Fault Tolerance
	- Core Checks and Recommendations
Cloud Watch - monitors performance
Cloud Trail - captures API calls and logs them


Amazon Inspector - Agent Service for vulnerabilities

Amazon Trusted Advisor - like a CCTV what things are doing. Cost optimization

CloudTrail increases visibility into your user and resource activity by recording AWS Management and Console API calls.

# CloudWatch vs AWS Config

CloudWatch - monitoring performance and historical applications. Personal Trainer Monitors Performance

Host Level Metrics Consist of
* CPU
* Network
* Disk
* Status Check
* Memory

AWS Config provides a detailed view of the configuration of AWS resources in your AWS account. This includes the resources in your AWS account.
Monitors the configuration of the resource. Show you what the configuration change.

Remember;
Cloudwatch is used for monitoring performance.
AWS Config is used to monitor configurations of your AWS Resources


# Load Balancers

3 Types
*	Application Load Balancers
		Choose an Application Load Balancer when you need a flexible feature set for your applications with HTTP and HTTPS traffic. Operating at the request level, Application Load Balancers provide advanced routing and visibility features targeted at application architectures, including microservices and containers.
* Network Load Balancers
    Choose a Network Load Balancer when you need ultra-high performance, TLS offloading at scale, centralized certificate deployment, support for UDP, and static IP addresses for your applications. Operating at the connection level, Network Load Balancers are capable of handling millions of requests per second securely while maintaining ultra-low latencies.
* Gateway Load Balancers
    Choose a Gateway Load Balancer when you need to deploy and manage a fleet of third-party virtual appliances that support GENEVE. These appliances enable you to improve security, compliance, and policy controls.

1. Need to create the Load Balancer
2. Need to assign the Target Group

Have EC2 instances in multiple availability zones.


Application Load Balancers - Layer 7 ( Make Intelligent Decisions)
Network Load Balancers - Extreme Performance/Static IP Addresses.
Classic Load Balancers - Test & Dev, Keep Costs Low.

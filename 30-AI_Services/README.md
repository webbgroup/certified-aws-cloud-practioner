# Lex

Lex service is what powers Alexa. A service that allows you to build conversational chatbots.
These can be powered either via voice or text.

When you hear Lex, think chatbot

# Polly
Service Converts text to voice. You can use different languages, etc.

# Transcribe
Converts speech into text. Use this to generate subtitles. A Cloud Guru uses it to transcribe voices for subtitles

# Rekognition
Converts Images into tags or text. Allows software to see, and allows what it thinks the image is with a certain degree of confidence

Can be used with a lot of apps. With a plant snapshot,

# EC2 Pricing Models.

1 - On Demand - Pay as you go
2 - Reserved - Pay up front for future usage. 1 or 3. best contracted rate.
3 - Spot - Variable costs, and servers run when it is within your price range
4 - Dedicated - Compliancy, or Server License - SQL Server, MS Server, SUSE Licensing


# Different Compute Services

EC2 - Virtual Machine in the Cloud
LightSail - Preconfigured Simple Cloud Servers; Connect with S3, Type of Virtual Machine
Lambda - Serverless Computing within the cloud
Batch - Compute service for batch computing
Elastic Beanstalk - Platform as a Service compute service, web servers
Serverless Application Repository - Allows you to deploy pre-provisioned serverless applications, Alexa skills)
AWS Outpost - Way of extending compute to your own data centers
EC2 Image Builder - Helps you build your own custom EC2 images for Linux and Windows

# AWS VPC
Default VPC in that Region.

Virtual Private Cloud - where you can launch EC2 within your region
Logically isolated place where you can launch your own instances, subnets, public or private.

Virtual Data Center in the cloud

Customize the network, public or private, and database in a private network that has no Internet Access

AWS cloud as an extension of your corporate data center

# Connecting On Premise to You
VPN Connection between corporate data centers.

AWS Direct Connect


# Lambda

Traditional

Serverless Architecture
Only when Lambda executes.

Cloud Guru - ran for free for the first 2 years. and allows you to get charged ONLY when it is done.

* Node.js
* Java
* C#
* Python
* Go
* Powershell

## Priced

1. Number of requests - Million requests are free.
.20 cents for next Million.

2. Duration - calculated from the time your code begins until it returns or otherwise terminates. Rounded up to the nearest millisecond

Version control can be used.

YOU are responsible for your own code. Amazon is responsible for everything else.

### Why do we love Lambda

* Scales Great!
* No Servers!
* Super Cheap!

Every time you talk to Alexa, you're using Lambda


# Lambda Exam Tips

1. Lambda scales out
2. Lambda functions are independent. 1 event = 1 function
3. Lambda is serverless
4. Know how it is priced, per invocation and duration
5. Can have multiple versions of your code within Lambda
6. Understand the shared responsibility model.
















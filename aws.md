Notes on learning AWS
---------------------

### Before Cloud Computing
 
 - Buy stack of servers
 - keeping peak traffic in mind, buy more servers
 - monitoring and maintainance of servers

#### Disadvantages

- Troubleshooting is tedious
- Really very expensive
- Traffic varying; servers ideal most of the time.

So, with cloud computing

- Rent servers
- No infra management (done by cloud provider)
- Scalability (vary according to traffic)


### Cloud Computing

Use of remote servers on internet to store, manage and process data rather than a local server or personal computer

------------------------------------------------------

# Amazon Web Services

## Amazon Compute Services

### (EC2)
Bare server; host applications or do anything.

### Lambda
Cannot host application; just carry out background tasks.

### Elastic Beanstalk
Deploy application without worrying about underlying hardware. (Automated form of EC2). No env config like EC2.

### Elastic Load Balancer
Distribute load on a number of deployed instances.

### Auto Scaling
Scale up and down automatically.

## AWS Storage System

### Simple Storage Service
Bucket is the root of file system. You upload objects to folders in buckets that have then a specific path alotted.

### Cloudfront
CDN for caching resources.

### Elastic Block Storage
Block level storage; provide high IOPS

### Glacier
Data archiving service

### Snowball
Physical transfer of data to AWS Infrastructure

### Storage Gateway
Provides seamless integration between your on premise servers and AWS Infra

Or may be EC2 and RDS. It would take snapshots, and triggers recovery through snapshot in case of any failiures.

## AWS Database Services

### RDS
Services that can be used to manage various databases like MySQL, Postgres etc.

### Aurora
Amazon's SQL; Use MySQL at core but Amazon claims that it is 5x faster performance wise.

### DynamoDB
Manage non-relational databases.

### ElastiCache
Setup, manage & scale distributed cache-in environment in cloud.

### RedShift
Data Warehouse services to manage peta-byte sclae of data. Can take data from RDS/DynamoDB and then used for analytics purpose.

## AWS Networking Services

### VPC

Virtual Network where in you launch your AWS instances

### Direct Connect

Direct leased line to AWS infra. Used if the internet bandwidth is a constraint.

### Route 53

A Domain Name System. Point URL to Compute.

## AWS Management Services

### CloudWatch

Cloud monitoring tool (Trigger an alarm to send notification if CPU usage goes above 70% at any time)

### CloudFormation

Templatize your AWS instance.Takes snapshot of infrastructure and use in different environment from templating it.

### CloudTrail

Logging service from AWS. It generates logs from AWS services and then can send them to S3 for storage.

### AWS CLI
Replacement for the AWS GUI to carry any task though command-line.

### OpsWorks
A configuration management tool

Consists of Stack and Layers

Layers are different AWS services. You combine these services to form a Stack. So, change a config value in Stack to get reflected in all the layers.

### Trusted Advisor

Personal Assistant to you in the AWS Infrastructure

## AWS Security Services

### IAM (Identification and Authentication Management tool)

Give granular access to users.

### KMS (Key Management System)

Create and manage encryption keys to encrypt data.

## AWS Application Services

### SES (Simple Emailing Service)

Send bulk emails to your users.

### SQS (Simple Queue Service)

Queuing service which acts as a buffer.

### SNS (Simple Notification Service)

Send notifications of events (may be to SQS) to trigger some tasks.

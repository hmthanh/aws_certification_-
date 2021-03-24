# AWS Certified Developer Associate - DVA-C01

## Exam 1

### Question 1:
The development team at a retail organization wants to allow a Lambda function in its AWS Account A to access a DynamoDB table in another AWS Account B.
* Add a resource policy to the DynamoDB table in AWS Account B to give access to the Lambda function in Account A
* Create an IAM role in Account B with access to DynamoDB. Modify the trust policy of the execution role in Account A to allow the execution role of Lambda to assume the IAM role in Account B. Update the Lambda function code to add the AssumeRole API call
* Create a clone of the Lambda function in AWS Account B so that it can access the DynamoDB table in the same account
* Create an IAM role in Account B with access to DynamoDB. Modify the trust policy of the role in Account B to allow the execution role of Lambda to assume this role. Update the Lambda function code to add the AssumeRole API call

### Question 2:
A development team lead is responsible for managing access for her IAM principals. At the start of the cycle, she has granted excess privileges to users to keep them motivated for trying new things. She now wants to ensure that the team has only the minimum permissions required to finish their work.
* Access Advisor feature on IAM console
* Amazon Inspector
* IAM Access Analyzer
* AWS Trusted Advisor

### Question 3:
A company is looking at optimizing their Amazon EC2 instance costs. Few instances are sure to run for a few years, but the instance type might change based on business requirements.
* Convertible Reserved instances
* Scheduled Reserved instances
* Standard Reserved instances
* Elastic Reserved instances

### Question 4:
A Developer has been entrusted with the job of securing certain S3 buckets that are shared by a large team of users. Last time, a bucket policy was changed, the bucket was erroneously available for everyone, outside the organization too.
* S3 Analytics
* IAM Access Analyzer
* Access Advisor feature on IAM console
* S3 Object Lock

### Question 5:
You're a developer doing contract work for the media sector. Since you work alone, you opt for technologies that require little maintenance, which allows you to focus more on your coding. You have chosen AWS Elastic Beanstalk to assist with the deployment of your applications. While reading online documentation you find that Elastic Beanstalk relies on another AWS service to provision your resources.
* CloudFormation
* CodeDeploy
* CodeCommit
* Systems Manager

### Question 6:
An IT company is configuring Auto Scaling for its Amazon EC2 instances spread across different AZs and Regions.
* Auto Scaling groups that span across multiple Regions need to be enabled for all the Regions specified
* An Auto Scaling group can contain EC2 instances in only one Availability Zone of a Region
* An Auto Scaling group can contain EC2 instances in one or more Availability Zones within the same Region
* For Auto Scaling groups in a VPC, the EC2 instances are launched in subnets
* Amazon EC2 Auto Scaling attempts to distribute instances evenly between the Availability Zones that are enabled for your Auto Scaling group

### Question 7:
A company has hired you as an AWS Certified Developer Associate to help with redesigning a real-time data processor. The company wants to build custom applications that process and analyze the streaming data for its specialized needs.
* Use Kinesis Data Streams to process the data streams as well as decouple the producers and consumers for the real-time data processor
* Use SNS to process the data streams as well as decouple the producers and consumers for the real-time data processor
* Use Kinesis Data Firehose to process the data streams as well as decouple the producers and consumers for the real-time data processor
* Use SQS to process the data streams as well as decouple the producers and consumers for the real-time data processor

### Question 8:
An organization has hosted its EC2 instances in two AZs. AZ1 has two instances and AZ2 has 8 instances. The Elastic Load Balancer managing the instances in the two AZs has cross-zone load balancing enabled in its configuration.
* 10
* 15
* 25
* 20

### Question 9:
The development team at a company creates serverless solutions using AWS Lambda. Functions are invoked by clients via AWS API Gateway which anyone can access. The team lead would like to control access using a 3rd party authorization mechanism.
* Cognito User Pools
* Lambda Authorizer
* API Gateway User Pools
* IAM permissions with sigv4

### Question 10:
You have created an Elastic Load Balancer that has marked all the EC2 instances in the target group as unhealthy. Surprisingly, when you enter the IP address of the EC2 instances in your web browser, you can access your website.
* Your web-app has a runtime that is not supported by the Application Load Balancer
* The EBS volumes have been improperly mounted
* You need to attach Elastic IP to the EC2 instances
* The security group of the EC2 instance does not allow for traffic from the security group of the Application Load Balancer
* The route for the health check is misconfigured

### Question 11:
You are creating a Cloud Formation template to deploy your CMS application running on an EC2 instance within your AWS account. Since the application will be deployed across multiple regions, you need to create a map of all the possible values for the base AMI.
* !FindInMap [ MapName, TopLevelKey ]
* !FindInMap [ MapName, TopLevelKey, SecondLevelKey ]
* !FindInMap [ MapName, TopLevelKey, SecondLevelKey, ThirdLevelKey ]
* !FindInMap [ MapName ]

### Question 12:
A SaaS company runs a HealthCare web application that is used worldwide by users. There have been requests by mobile developers to expose public APIs for the application-specific functionality. You decide to make the APIs available to mobile developers as product offerings.
* Use CloudFront Usage Plans
* Use AWS Lambda Custom Authorizers
* Use AWS Billing Usage Plans
* Use API Gateway Usage Plans

### Question 13:
Your global organization has an IT infrastructure that is deployed using CloudFormation on AWS Cloud. One employee, in us-east-1 Region, has created a stack 'Application1' and made an exported output with the name 'ELBDNSName'. Another employee has created a stack for a different application 'Application2' in us-east-2 Region and also exported an output with the name 'ELBDNSName'. The first employee wanted to deploy the CloudFormation stack 'Application1' in us-east-2, but it got an error. What is the cause of the error?
* Exported Output Values in CloudFormation must have unique names across all Regions
* Output Values in CloudFormation must have unique names within a single Region
* Exported Output Values in CloudFormation must have unique names within a single Region
* Output Values in CloudFormation must have unique names across all Regions

### Question 14:
You have chosen AWS Elastic Beanstalk to upload your application code and allow it to handle details such as provisioning resources and monitoring.
* .ebextensions_<mysettings>.config
* .config/<mysettings>.ebextensions
* .config_<mysettings>.ebextensions
* .ebextensions/<mysettings>.config

### Question 15:
A video encoding application running on an EC2 instance takes about 20 seconds on average to process each raw footage file. The application picks the new job messages from an SQS queue. The development team needs to account for the use-case when the video encoding process takes longer than usual so that the same raw footage is not processed by multiple consumers.
* Use WaitTimeSeconds action to long poll and extend a message's visibility timeout
* Use DelaySeconds action to delay a message's visibility timeout
* Use ChangeMessageVisibility action to extend a message's visibility timeout
* Use WaitTimeSeconds action to short poll and extend a message's visibility timeout

### Question 16:
A media company has created a video streaming application and it would like their Brazilian users to be served by the company's Brazilian servers. Other users around the globe should not be able to access the servers through DNS queries.
* Geolocation
* Latency
* Failover
* Weighted

### Question 17:
An IT company has a HealthCare application with data security requirements such that the encryption key must be stored in a custom application running on-premises. The company wants to offload the data storage as well as the encryption process to Amazon S3 but continue to use the existing encryption keys.
* Server-Side Encryption with Customer Master Keys (CMKs) Stored in AWS Key Management Service (SSE-KMS)
* Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3)
* Server-Side Encryption with Customer-Provided Keys (SSE-C)
* Client-Side Encryption with data encryption is done on the client-side before sending it to Amazon S3

### Question 18:
A startup with newly created AWS account is testing different EC2 instances. They have used Burstable performance instance - T2.micro - for 35 seconds and stopped the instance.
* 60 seconds
* 30 seconds
* 35 seconds
* 0 seconds

### Question 19:
A developer has just completed configuring the Application Load Balancer for the EC2 instances. Just as he started testing his configuration, he realized that he has missed assigning target groups to his ALB.
* HTTP 500
* HTTP 403
* HTTP 503
* HTTP 504

### Question 20:
A developer in your company has configured a build using AWS CodeBuild. The build fails and the developer needs to quickly troubleshoot the issue to see which commands or settings located in the BuildSpec file are causing an issue.
* Freeze the CodeBuild during its next execution
* Enable detailed monitoring
* SSH into the CodeBuild Docker container
* Run AWS CodeBuild locally using CodeBuild Agent

### Question 21:
A Developer at a company is working on a CloudFormation template to set up resources. Resources will be defined using code and provisioned based on certain conditions.
* Conditions
* Resources
* Parameters
* Outputs

### Question 22:
An e-commerce company has a fleet of EC2 based web servers running into very high CPU utilization issues. The development team has determined that serving secure traffic via HTTPS is a major contributor to the high CPU load.
* Create an HTTPS listener on the Application Load Balancer with SSL termination
* Create an HTTPS listener on the Application Load Balancer with SSL pass-through
* Configure an SSL/TLS certificate on an Application Load Balancer via AWS Certificate Manager (ACM)
* Create an HTTP listener on the Application Load Balancer with SSL pass-through
* Create an HTTP listener on the Application Load Balancer with SSL termination

### Question 23:
A firm runs its technology operations on a fleet of Amazon EC2 instances. The firm needs a certain software to be available on the instances to support their daily workflows. The developer team has been told to use the user data feature of EC2 instances.
* By default, scripts entered as user data do not have root user privileges for executing
* By default, user data runs only during the boot cycle when you first launch an instance
* By default, scripts entered as user data are executed with root user privileges
* By default, user data is executed every time an EC2 instance is re-started
* When an instance is running, you can update user data by using root user credentials

### Question 24:
A data analytics company wants to use clickstream data for Machine Learning tasks, develop algorithms, and create visualizations and dashboards to support the business stakeholders. Each of these business units works independently and would need real-time access to this clickstream data for their applications.
* AWS Kinesis Data Streams
* AWS Kinesis Data Analytics
* Amazon SQS
* AWS Kinesis Data Firehose

### Question 25:
The development team at an IT company wants to make changes to a current application written in Node.js and deployed on a Linux server. The team lead would like to decouple the application into microservices, package the application to a Docker container which is then run on the AWS infrastructure.
* Step Functions
* ECR
* Lambda
* ECS

### Question 26:
Which of the following best describes how KMS Encryption works?
* KMS receives CMK from the client at every Encrypt call, and encrypts the data with that
* KMS sends the CMK to the client, which performs the encryption and then deletes the CMK
* KMS generates a new CMK for each Encrypt call and encrypts the data with it
* KMS stores the CMK, and receives data from the clients, which it encrypts and sends back

### Question 27:
A developer at a company is trying to create a digital signature for SSH'ing into the Amazon EC2 instances.
* Root user credentials
* Multi-Factor Authentication (MFA)
* Access keys
* Key pairs

### Question 28:
An application is hosted by a 3rd party and exposed at yourapp.3rdparty.com. You would like to have your users access your application using www.mydomain.com, which you own and manage under Route 53.
* Create a CNAME record
* Create an A record
* Create an Alias Record
* Create a PTR record

### Question 29:
Which of the following security credentials can only be created by the AWS Account root user?
* CloudFront Key Pairs
* IAM User Access Keys
* EC2 Instance Key Pairs
* IAM User passwords

### Question 30:
A developer has been asked to create an application that can be deployed across a fleet of EC2 instances. The configuration must allow for full control over the deployment steps using the blue-green deployment.
* CodePipeline
* CodeBuild
* Elastic Beanstalk
* CodeDeploy

### Question 31:
The Technical Lead of your team has reviewed a CloudFormation YAML template written by a new recruit and specified that an invalid section has been added to the template.
* 'Conditions' section of the template
* 'Dependencies' section of the template
* 'Resources' section of the template
* 'Parameters' section of the template

### Question 32:
A financial services company is undergoing a compliance audit by the regulator. The company has hundreds of IAM users that make API calls but specifically it needs to be determined who is making KMS API calls.
* Config
* CloudTrail
* X-Ray
* CloudWatch Metrics

### Question 33:
The development team has just configured and attached the IAM policy needed to access AWS Billing and Cost Management for all users under the Finance department. But, the users are unable to see AWS Billing and Cost Management service in the AWS console.
* Only root user has access to AWS Billing and Cost Management console
* You need to activate IAM user access to the Billing and Cost Management console for all the users who need access
* The users might have another policy that restricts them from accessing the Billing information
* IAM user should be created under AWS Billing and Cost Management and not under AWS account to have access to Billing console

### Question 34:
You have deployed a Java application to an EC2 instance where it uses the X-Ray SDK. When testing from your personal computer, the application sends data to X-Ray but when the application runs from within EC2, the application fails to send data to X-Ray.
* X-Ray sampling
* EC2 Instance Role
* EC2 X-Ray Daemon
* CloudTrail

### Question 35:
You are running workloads on AWS and have embedded RDS database connection strings within each web server hosting your applications. After failing a security audit, you are looking at a different approach to store your secrets securely and automatically rotate the database credentials.
* SSM Parameter Store
* KMS
* Systems Manager
* Secrets Manager

### Question 36:
A development team at a social media company uses AWS Lambda for its serverless stack on AWS Cloud. For a new deployment, the Team Lead wants to send only a certain portion of the traffic to the new Lambda version. In case the deployment goes wrong, the solution should also support the ability to roll back to a previous version of the Lambda function, with MIMINUM downtime for the application.
* Set up the application to have multiple alias of the Lambda function. Deploy the new version of the code. Configure a new alias that points to the current alias of the Lambda function for handling 10% of the traffic. If the deployment goes wrong, reset the new alias to point all traffic to the most recent working alias of the Lambda function
* Set up the application to directly deploy the new Lambda version. If the deployment goes wrong, reset the application back to the current version using the version number in the ARN
* Set up the application to use an alias that points to the current version. Deploy the new version of the code and configure alias to send all users to this new version. If the deployment goes wrong, reset the alias to point to the current version
* Set up the application to use an alias that points to the current version. Deploy the new version of the code and configure the alias to send 10% of the users to this new version. If the deployment goes wrong, reset the alias to point all traffic to the current version

### Question 37:
You're a developer working on a large scale order processing application. After developing the features, you commit your code to AWS CodeCommit and begin building the project with AWS CodeBuild before it gets deployed to the server. The build is taking too long and the error points to an issue resolving dependencies from a third-party. You would like to prevent a build running this long in the future for similar underlying reasons.
* Use AWS CloudWatch Events
* Use VPC Flow Logs
* Use AWS Lambda
* Enable CodeBuild timeouts

### Question 38:
The development team at an IT company would like to provision their own Docker images that can be used as input sources for CodeBuild. These images will contain cached dependencies as well as special tooling for builds that are proprietary to the company.
* ECR
* EBS
* S3
* ECS

### Question 39:
The manager at an IT company wants to set up member access to user-specific folders in an Amazon S3 bucket - bucket-a. So, user x can only access files in his folder - bucket-a/user/user-x/ and user y can only access files in her folder - bucket-a/user/user-y/ and so on.
* IAM policy variables
* IAM policy resource
* IAM policy principal
* IAM policy condition

### Question 40:
As an AWS Certified Developer Associate, you are given a document written in YAML that represents the architecture of a serverless application. The first line of the document contains Transform: 'AWS::Serverless-2016-10-31'.
* It represents an intrinsic function
* It represents a Lambda function definition
* Presence of Transform section indicates it is a Serverless Application Model (SAM) template
* Presence of Transform section indicates it is a CloudFormation Parameter

### Question 41:
A multi-national company has multiple business units with each unit having its own AWS account. The development team at the company would like to debug and trace data across accounts and visualize it in a centralized account.
* X-Ray
* VPC Flow Logs
* CloudTrail
* CloudWatch Events

### Question 42:
An E-commerce business, has its applications built on a fleet of Amazon EC2 instances, spread across various Regions and AZs. The technical team has suggested using Elastic Load Balancer for better architectural design.
* Improve vertical scalability of the system
* Separate public traffic from private traffic
* Build a highly available system
* Deploy EC2 instances across multiple AWS Regions
* The Load Balancer communicates with the underlying EC2 instances using their public IPs

### Question 43:
As an AWS Certified Developer Associate, you been asked to create an AWS Elastic Beanstalk environment to handle deployment for an application that has high traffic and high availability needs. You need to deploy the new version using Beanstalk while making sure that performance and availability are not affected.
* Deploy using 'Rolling' deployment policy
* Deploy using 'Immutable' deployment policy
* Deploy using 'All at once' deployment policy
* Deploy using 'Rolling with additional batch' deployment policy

### Question 44:
A retail company manages its IT infrastructure on AWS Cloud via Elastic Beanstalk. The development team at the company is planning to deploy the next version with MINIMUM application downtime and the ability to rollback quickly in case deployment goes wrong.
* Deploy the new application version using 'Rolling' deployment policy
* Deploy the new application version using 'Rolling with additional batch' deployment policy
* Deploy the new application version using 'All at once' deployment policy
* Deploy the new version to a separate environment via Blue/Green Deployment, and then swap Route 53 records of the two environments to redirect traffic to the new version

### Question 45:
A multi-national company has just moved to AWS Cloud and it has configured forecast-based AWS Budgets alerts for cost management. However, no alerts have been received even though the account and the budgets have been created almost three weeks ago.
* Budget forecast has been created from an account that does not have enough privileges
* AWS requires approximately 5 weeks of usage data to generate budget forecasts
* Amazon CloudWatch could be down and hence alerts are not being sent
* Account has to be part of AWS Organizations to receive AWS Budgets alerts

### Question 46:
Your company has stored all application secrets in SSM Parameter Store. The audit team has requested to get a report to better understand when and who has issued API calls against SSM Parameter Store.
* Use SSM Parameter Store List feature to get a record of actions taken by a user
* Use SSM Parameter Store Access Logs in S3 to get a record of actions taken by a user
* Use AWS CloudTrail to get a record of actions taken by a user
* Use SSM Parameter Store Access Logs in CloudWatch Logs to get a record of actions taken by a user

### Question 47:
A photo-sharing application manages its EC2 server fleet running behind an Application Load Balancer and the traffic is fronted by a CloudFront distribution. The development team wants to decouple the user authentication process for the application so that the application servers can just focus on the business logic.
* Use Cognito Authentication via Cognito User Pools for your Application Load Balancer
* Use Cognito Authentication via Cognito Identity Pools for your Application Load Balancer
* Use Cognito Authentication via Cognito Identity Pools for your CloudFront distribution
* Use Cognito Authentication via Cognito User Pools for your CloudFront distribution

### Question 48:
You have created a Java application that uses RDS for its main data storage and ElastiCache for user session storage. The application needs to be deployed using Elastic Beanstalk and every new deployment should allow the application servers to reuse the RDS database. On the other hand, user session data stored in ElastiCache can be re-created for every deployment.
* RDS database defined externally and referenced through environment variables
* RDS database defined in .ebextensions/
* ElastiCache defined in .ebextensions/
* ElastiCache database defined externally and referenced through environment variables
* ElastiCache bundled with the application source code

### Question 49:
A cybersecurity firm wants to run their applications on single-tenant hardware to meet security guidelines.
* On-Demand Instances
* Spot Instances
* Dedicated Hosts
* Dedicated Instances

### Question 50:
As part of his development work, an AWS Certified Developer Associate is creating policies and attaching them to IAM identities. After creating necessary Identity-based policies, he is now creating Resource-based policies.
* Permissions boundary
* Access control list (ACL)
* Trust policy
* AWS Organizations Service Control Policies (SCP)

### Question 51:
A company uses Elastic Beanstalk to manage its IT infrastructure on AWS Cloud and it would like to deploy the new application version to the EC2 instances. When the deployment is executed, some instances should serve requests with the old application version, while other instances should serve requests using the new application version until the deployment is completed.
* Rolling
* All at once
* Immutable
* Rolling with additional batches

### Question 52:
As an AWS Certified Developer Associate, you have configured the AWS CLI on your workstation. Your default region is us-east-1 and your IAM user has permissions to operate commands on services such as EC2, S3 and RDS in any region. You would like to execute a command to stop an EC2 instance in the us-east-2 region.
* You need to override the default region by using aws configure
* You should create a new IAM user just for that other region
* Use boto3 dependency injection
* Use the --region parameter

### Question 53:
The development team at an IT company uses CloudFormation to manage its AWS infrastructure. The team has created a network stack containing a VPC with subnets and a web application stack with EC2 instances and an RDS instance. The team wants to reference the VPC created in the network stack into its web application stack.
* Create a cross-stack reference and use the Export output field to flag the value of VPC from the network stack. Then use Fn::ImportValue intrinsic function to import the value of VPC into the web application stack
* Create a cross-stack reference and use the Outputs output field to flag the value of VPC from the network stack. Then use Ref intrinsic function to reference the value of VPC into the web application stack
* Create a cross-stack reference and use the Export output field to flag the value of VPC from the network stack. Then use Ref intrinsic function to reference the value of VPC into the web application stack
* Create a cross-stack reference and use the Outputs output field to flag the value of VPC from the network stack. Then use Fn::ImportValue intrinsic function to import the value of VPC into the web application stack

### Question 54:
You are a developer for a web application written in .NET which uses the AWS SDK. You need to implement an authentication mechanism that returns a JWT (JSON Web Token).
* Cognito Identity Pools
* Cognito Sync
* API Gateway
* Cognito User Pools

### Question 55:
CodeCommit is a managed version control service that hosts private Git repositories in the AWS cloud.
* AWS Access Keys
* IAM username and password
* SSH Keys
* Git credentials

### Question 56:
An organization has offices across multiple locations and the technology team has configured an Application Load Balancer across targets in multiple Availability Zones. The team wants to analyze the incoming requests for latencies and the client's IP address patterns.
* CloudTrail logs
* ALB access logs
* ALB request tracing
* CloudWatch metrics

### Question 57:
Your company has configured AWS Organizations to manage multiple AWS accounts. Within each AWS account, there are many CloudFormation scripts running. Your manager has requested that each script output the account number of the account the script was executed in.
* AWS::StackName
* AWS::NoValue
* AWS::Region
* AWS::AccountId

### Question 58:
A development team lead is configuring policies for his team at an IT company.
* Identity-based policy
* AWS Organizations Service Control Policy (SCP)
* Access control list (ACL)
* Permissions boundary
* Resource-based policy

### Question 59:
The development team at an e-commerce company wants to run a serverless data store service on two docker containers using shared memory.
* Put the two containers into two separate task definitions using an EC2 Launch Type
* Put the two containers into two separate task definitions using a Fargate Launch Type
* Put the two containers into a single task definition using a Fargate Launch Type
* Put the two containers into a single task definition using an EC2 Launch Type

### Question 60:
You are a developer working on AWS Lambda functions that are invoked via REST API's using Amazon API Gateway. Currently, when a GET request is invoked by the consumer, the entire data-set returned by the Lambda function is visible. Your team lead asked you to format the data response.
* Use a Lambda custom interceptor
* Use an API Gateway stage variable
* Deploy an interceptor shell script
* Use API Gateway Mapping Templates

### Question 61:
To enable HTTPS connections for his web application deployed on the AWS Cloud, a developer is in the process of creating server certificate.
* AWS Secrets Manager
* IAM
* AWS Systems Manager
* AWS CloudFormation
* AWS Certificate Manager

### Question 62:
A developer has been asked to create a web application to be deployed on EC2 instances. The developer just wants to focus on writing application code without worrying about server provisioning, configuration and deployment.
* CodeDeploy
* CloudFormation
* Elastic Beanstalk
* Serverless Application Model

### Question 63:
You are a developer in a manufacturing company that has several servers on-site. The company decides to move new development to the cloud using serverless technology. You decide to use the AWS Serverless Application Model (AWS SAM) and work with an AWS SAM template file to represent your serverless architecture.
* AWS::Serverless::Api
* AWS::Serverless::Function
* AWS::Serverless::SimpleTable
* AWS::Serverless::UserPool

### Question 64:
The development team at an IT company has configured an Application Load Balancer (ALB) with a Lambda function A as the target but the Lambda function A is not able to process any request from the ALB. Upon investigation, the team finds that there is another Lambda function B in the AWS account that is exceeding the concurrency limits.
* Set up reserved concurrency for the Lambda function B so that it throttles if it goes above a certain concurrency limit
* Use an API Gateway instead of an Application Load Balancer (ALB) for Lambda function A
* Use a Cloudfront Distribution instead of an Application Load Balancer (ALB) for Lambda function A
* Set up provisioned concurrency for the Lambda function B so that it throttles if it goes above a certain concurrency limit

### Question 65:
In addition to regular sign-in credentials, AWS supports Multi-Factor Authentication (MFA) for accounts with privileged access.
* Virtual MFA devices
* U2F security key
* SMS text message-based MFA
* Hardware MFA device

# Exam 2

### Question 1:
A business has purchased one m4.xlarge Reserved Instance but it has used three m4.xlarge instances concurrently for an hour.
* One instance is charged at one hour of On-Demand usage and the other two instances are charged at two hours of Reserved Instance usage
* One instance is charged at one hour of Reserved Instance usage and the other two instances are charged at two hours of On-Demand usage
* All instances are charged at one hour of On-Demand Instance usage
* All instances are charged at one hour of Reserved Instance usage

### Question 2:
An Accounting firm extensively uses Amazon EBS volumes for persistent storage of application data of Amazon EC2 instances. The volumes are encrypted to protect the critical data of the clients. As part of managing the security credentials, the project manager has come across a policy snippet that looks like the following:
* The second statement in this policy provides the security group (mentioned in first statement of the policy), the ability to create, list, and revoke grants for Amazon EC2
* The first statement provides a specified IAM principal the ability to generate a data key and decrypt that data key from the CMK when necessary
* The first statement provides the security group the ability to generate a data key and decrypt that data key from the CMK when necessary
* The second statement in the policy mentions that all the resources stated in the first statement can take the specified role which will provide the ability to create, list, and revoke grants for Amazon EC2

### Question 3:
The development team at a retail company is gearing up for the upcoming Thanksgiving sale and wants to make sure that the application's serverless backend running via Lambda functions does not hit latency bottlenecks as a result of the traffic spike.
* Configure Application Auto Scaling to manage Lambda reserved concurrency on a schedule
* Configure Application Auto Scaling to manage Lambda provisioned concurrency on a schedule
* Add an Application Load Balancer in front of the Lambda functions
* No need to make any special provisions as Lambda is automatically scalable because of its serverless nature

### Question 4:
You are a developer working on a web application written in Java and would like to use AWS Elastic Beanstalk for deployment because it would handle deployment, capacity provisioning, load balancing, auto-scaling, and application health monitoring. In the past, you connected to your provisioned instances through SSH to issue configuration commands. Now, you would like a configuration mechanism that automatically applies settings for you.
* Include config files in .ebextensions/ at the root of your source code
* Use an AWS Lambda hook
* Deploy a CloudFormation wrapper
* Use SSM parameter store as an input to your Elastic Beanstalk Configurations

### Question 5:
A company that specializes in cloud communications platform as a service allows software developers to programmatically use their services to send and receive text messages. The initial platform did not have a scalable architecture as all components were hosted on one server and should be redesigned for high availability and scalability.
* ALB + ECS
* EBS + RDS
* SES + S3
* API Gateway + Lambda
* CloudWatch + CloudFront

### Question 6:
A development team has configured their Amazon EC2 instances for Auto Scaling. A Developer during routine checks has realized that only basic monitoring is active, as opposed to detailed monitoring.
* AWS CLI was used to create the launch configuration
* SDK was used to create the launch configuration
* The default configuration was Auto Scaling was not set
* AWS Management Console might have been used to create the launch configuration

### Question 7:
A developer with access to the AWS Management Console terminated an instance in the us-east-1a availability zone. The attached EBS volume remained and is now available for attachment to other instances. Your colleague launches a new Linux EC2 instance in the us-east-1e availability zone and is attempting to attach the EBS volume. Your colleague informs you that it is not possible and need your help.
* EBS volumes are region locked
* The EBS volume is encrypted
* The required IAM permissions are missing
* EBS volumes are AZ locked

### Question 8:
A data analytics company is processing real-time Internet-of-Things (IoT) data via Kinesis Producer Library (KPL) and sending the data to a Kinesis Data Streams driven application. The application has halted data processing because of a ProvisionedThroughputExceeded exception.
* Use Amazon Kinesis Agent instead of Kinesis Producer Library (KPL) for sending data to Kinesis Data Streams
* Configure the data producer to retry with an exponential backoff
* Use Kinesis enhanced fan-out for Kinesis Data Streams
* Increase the number of shards within your data streams to provide enough capacity
* Use Amazon SQS instead of Kinesis Data Streams

### Question 9:
The development team at a multi-national retail company wants to support trusted third-party authenticated users from the supplier organizations to create and update records in specific DynamoDB tables in the company's AWS account.
* Use Cognito Identity pools to enable trusted third-party authenticated users to access DynamoDB
* Use Cognito User pools to enable trusted third-party authenticated users to access DynamoDB
* Create a new IAM user in the company's AWS account for each of the third-party authenticated users from the supplier organizations. The users can then use the IAM user credentials to access DynamoDB
* Create a new IAM group in the company's AWS account for each of the third-party authenticated users from the supplier organizations. The users can then use the IAM group credentials to access DynamoDB

### Question 10:
While troubleshooting, a developer realized that the Amazon EC2 instance is unable to connect to the Internet using the Internet Gateway.
* The network ACLs associated with the subnet must have rules to allow inbound and outbound traffic
* The subnet has been configured to be Public and has no access to the internet
* The instance's subnet is not associated with any route table
* The instance's subnet is associated with multiple route tables with conflicting configurations
* The route table in the instance’s subnet should have a route to an Internet Gateway

### Question 11:
Your team lead has asked you to learn AWS CloudFormation to create a collection of related AWS resources and provision them in an orderly fashion. You decide to provide AWS-specific parameter types to catch invalid values.
* CommaDelimitedList
* AWS::EC2::KeyPair::KeyName
* DependentParameter
* String

### Question 12:
As an AWS certified developer associate, you are working on an AWS CloudFormation template that will create resources for a company's cloud infrastructure. Your template is composed of three stacks which are Stack-A, Stack-B, and Stack-C. Stack-A will provision a VPC, a security group, and subnets for public web applications that will be referenced in Stack-B and Stack-C.
* Stack A, Stack C then Stack B
* Stack B, then Stack C, then Stack A
* Stack C then Stack A then Stack B
* Stack A, then Stack B, then Stack C

### Question 13:
An Auto Scaling group has a maximum capacity of 3, a current capacity of 2, and a scaling policy that adds 3 instances.
* Amazon EC2 Auto Scaling adds 3 instances to the group
* Amazon EC2 Auto Scaling adds only 1 instance to the group
* Amazon EC2 Auto Scaling does not add any instances to the group, but suggests changing the scaling policy to add one instance
* Amazon EC2 Auto Scaling adds 3 instances to the group and scales down 2 of those instances eventually

### Question 14:
A team lead has asked you to create an AWS CloudFormation template that creates EC2 instances and RDS databases. The template should be reusable by allowing the user to input a parameter value for an Amazon EC2 AMI ID.
* !Join
* !GetAtt
* !Ref
* !Param

### Question 15:
A university has created a student portal that is accessible through a smartphone app and web application. The smartphone app is available in both Android and IOS and the web application works on most major browsers. Students will be able to do group study online and create forum questions. All changes made via smartphone devices should be available even when offline and should synchronize with other devices.
* BeanStalk
* Cognito Identity Pools
* Cognito User Pools
* Cognito Sync

### Question 16:
A developer needs to automate software package deployment to both Amazon EC2 instances and virtual servers running on-premises, as part of continuous integration and delivery that the business has adopted.
* AWS CodePipeline
* AWS CodeDeploy
* AWS Elastic Beanstalk
* AWS CodeBuild

### Question 17:
A pharmaceutical company runs their database workloads on Provisioned IOPS SSD (io1) volumes.
* 200 GiB size volume with 2000 IOPS
* 200 GiB size volume with 10000 IOPS
* 200 GiB size volume with 15000 IOPS
* 200 GiB size volume with 5000 IOPS

### Question 18:
As a Senior Developer, you are tasked with creating several API Gateway powered APIs along with your team of developers. The developers are working on the API in the development environment, but they find the changes made to the APIs are not reflected when the API is called.
* Developers need IAM permissions on API execution component of API Gateway
* Enable Lambda authorizer to access API
* Use Stage Variables for development state of API
* Redeploy the API to an existing stage or to a new stage

### Question 19:
The app development team at a social gaming mobile app wants to simplify the user sign up process for the app. The team is looking for a fully managed scalable solution for user management in anticipation of the rapid growth that the app foresees.
* Create a custom solution using EC2 and DynamoDB to facilitate sign up and user management for the mobile app
* Create a custom solution using Lambda and DynamoDB to facilitate sign up and user management for the mobile app
* Use Cognito Identity pools to facilitate sign up and user management for the mobile app
* Use Cognito User pools to facilitate sign up and user management for the mobile app

### Question 20:
A company has created an Amazon S3 bucket that holds customer data. The team lead has just enabled access logging to this bucket. The bucket size has grown substantially after starting access logging. Since no new files have been added to the bucket, the perplexed team lead is looking for an answer.
* S3 access logging is pointing to the same bucket and is responsible for the substantial growth of bucket size
* Object Encryption has been enabled and each object is stored twice as part of this configuration
* Erroneous Bucket policies for batch uploads can sometimes be responsible for the exponential growth of S3 Bucket size
* A DDoS attack on your S3 bucket can potentially blow up the size of data in the bucket if the bucket security is compromised during the attack

### Question 21:
A social gaming application supports the transfer of gift vouchers between users. When a user hits a certain milestone on the leaderboard, they earn a gift voucher that can be redeemed or transferred to another user. The development team wants to ensure that this transfer is captured in the database such that the records for both users are either written successfully with the new gift vouchers or the status quo is maintained.
* Complete both operations on RDS MySQL in a single transaction block
* Use the Amazon Athena transactional read and write APIs on the table items as a single, all-or-nothing operation
* Complete both operations on Amazon RedShift in a single transaction block
* Perform DynamoDB read and write operations with ConsistentRead parameter set to true
* Use the DynamoDB transactional read and write APIs on the table items as a single, all-or-nothing operation

### Question 22:
A company runs its flagship application on a fleet of Amazon EC2 instances. After misplacing a couple of private keys from the SSH key pairs, they have decided to re-use their SSH key pairs for the different instances across AWS Regions.
* Store the public and private SSH key pair in AWS Trusted Advisor and access it across AWS Regions
* It is not possible to reuse SSH key pairs across AWS Regions
* Encrypt the private SSH key and store it in the S3 bucket to be accessed from any AWS Region
* Generate a public SSH key from a private SSH key. Then, import the key into each of your AWS Regions

### Question 23:
You are a developer handling a deployment service that automates application deployments to Amazon EC2 instances. Most of the deployments consist of code, but sometimes web and configuration files. One of your deployments failed and was rolled back by AWS CodeDeploy to the last known good application revision.
* To the new instances
* To the failed instances
* You cannot rollback a CodeDeploy deployment
* To the non-failed instances

### Question 24:
The development team at a HealthCare company has deployed EC2 instances in AWS Account A. These instances need to access patient data with Personally Identifiable Information (PII) on multiple S3 buckets in another AWS Account B.
* Add a bucket policy to all the Amazon S3 buckets in Account B to allow access from EC2 instances in Account A
* Create an IAM role with S3 access in Account B and set Account A as a trusted entity. Create another role (instance profile) in Account A and attach it to the EC2 instances in Account A and add an inline policy to this role to assume the role from Account B
* Create an IAM role (instance profile) in Account A and set Account B as a trusted entity. Attach this role to the EC2 instances in Account A and add an inline policy to this role to access S3 data from Account B
* Copy the underlying AMI for the EC2 instances from Account A into Account B. Launch EC2 instances in Account B using this AMI and then access the PII data on Amazon S3 in Account B

### Question 25:
As an AWS Certified Developer Associate, you are writing a CloudFormation template in YAML. The template consists of an EC2 instance creation and one RDS resource. Once your resources are created you would like to output the connection endpoint for the RDS database.
* !FindInMap
* !Sub
* !GetAtt
* !Ref

### Question 26:
The Development team at a media company is working on securing their databases.
* RDS Maria DB
* RDS Sequel Server
* RDS PostGreSQL
* RDS MySQL
* RDS Oracle

### Question 27:
As an AWS Certified Developer Associate, you have been hired to work with the development team at a company to create a REST API using the serverless architecture.
* Fargate with Lambda at the front
* API Gateway exposing Lambda Functionality
* Route 53 with EC2 as backend
* Public-facing Application Load Balancer with ECS on Amazon EC2

### Question 28:
A cyber forensics application, running behind an ALB, wants to analyze patterns for the client IPs.
* X-Forwarded-IP
* X-Forwarded-Proto
* X-Forwarded-For
* X-Forwarded-Port

### Question 29:
As a Team Lead, you are expected to generate a report of the code builds for every week to report internally and to the client. This report consists of the number of code builds performed for a week, the percentage success and failure, and overall time spent on these builds by the team members. You also need to retrieve the CodeBuild logs for failed builds and analyze them in Athena.
* Enable S3 and CloudWatch Logs integration
* Use AWS Lambda integration
* Use CloudWatch Events
* Use AWS CloudTrail and deliver logs to S3

### Question 30:
You have launched several AWS Lambda functions written in Java. A new requirement was given that over 1MB of data should be passed to the functions and should be encrypted and decrypted at runtime.
* Use Envelope Encryption and store as environment variable
* Use KMS Encryption and store as environment variable
* Use Envelope Encryption and reference the data as file within the code
* Use KMS direct encryption and store as file

### Question 31:
The development team at an analytics company is using SQS queues for decoupling the various components of application architecture. As the consumers need additional time to process SQS messages, the development team wants to postpone the delivery of new messages to the queue for a few seconds.
* Use FIFO queues to postpone the delivery of new messages to the queue for a few seconds
* Use visibility timeout to postpone the delivery of new messages to the queue for a few seconds
* Use delay queues to postpone the delivery of new messages to the queue for a few seconds
* Use dead-letter queues to postpone the delivery of new messages to the queue for a few seconds

### Question 32:
You are a development team lead setting permissions for other IAM users with limited permissions. On the AWS Management Console, you created a dev group where new developers will be added, and on your workstation, you configured a developer profile. You would like to test that this user cannot terminate instances.
* Using the CLI, create a dummy EC2 and delete it using another CLI call
* Use the AWS CLI --dry-run option
* Retrieve the policy using the EC2 metadata service and use the IAM policy simulator
* Use the AWS CLI --test option

### Question 33:
A media publishing company is using Amazon EC2 instances for running their business-critical applications. Their IT team is looking at reserving capacity apart from savings plans for the critical instances.
* Neither Regional Reserved Instances nor Zonal Reserved Instances
* Regional Reserved Instances
* Zonal Reserved Instances
* Both Regional Reserved Instances and Zonal Reserved Instances

### Question 34:
A company uses AWS CodeDeploy to deploy applications from GitHub to EC2 instances running Amazon Linux. The deployment process uses a file called appspec.yml for specifying deployment hooks. A final lifecycle event should be specified to verify the deployment success.
* AfterInstall
* ValidateService
* ApplicationStart
* AllowTraffic

### Question 35:
A diagnostic lab stores its data on DynamoDB. The lab wants to backup a particular DynamoDB table data on Amazon S3, so it can download the S3 backup locally for some operational use.
* Use Hive with Amazon EMR to export your data to an S3 bucket and download locally
* Use AWS Data Pipeline to export your table to an S3 bucket in the account of your choice and download locally
* Use the DynamoDB on-demand backup capability to write to Amazon S3 and download locally
* Use AWS Glue to copy your table to Amazon S3 and download locally

### Question 36:
After a code review, a developer has been asked to make his publicly accessible S3 buckets private, and enable access to objects with a time-bound constraint.
* Use Bucket policy to block the unintended access
* Share pre-signed URLs with resources that need access
* Use Routing policies to re-route unintended access
* It is not possible to implement time constraints on Amazon S3 Bucket access

### Question 37:
A new recruit is trying to understand the nuances of EC2 Auto Scaling. As an AWS Certified Developer Associate, you have been asked to mentor the new recruit.
* Amazon EC2 Auto Scaling works with both Application Load Balancers and Network Load Balancers
* EC2 Auto Scaling groups are regional constructs. They span across Availability Zones and AWS regions
* You cannot use Amazon EC2 Auto Scaling for health checks (to replace unhealthy instances) if you are not using Elastic Load Balancing (ELB)
* Amazon EC2 Auto Scaling cannot add a volume to an existing instance if the existing volume is approaching capacity
* Every time you create an Auto Scaling group from an existing instance, it creates a new AMI (Amazon Machine Image)

### Question 38:
A developer while working on Amazon EC2 instances, realized that an instance was not needed and had shut it down. But another instance of the same type automatically got launched in the account.
* The instance could have been a part of Application Load Balancer and hence was automatically started
* The instance could have been a part of Network Load Balancer and hence was automatically started
* The user did not have the right permissions to shutdown the instance. User needs root permissions to terminate an instance
* Instance might be part of Auto Scaling Group and hence re-launched similar instance

### Question 39:
A startup has been experimenting with DynamoDB in its new test environment. The development team has discovered that some of the write operations have been overwriting existing items that have the specified primary key. This has messed up their data, leading to data discrepancies.
* Conditional writes
* Batch writes
* Use Scan operation
* Atomic Counters

### Question 40:
As a Developer, you are given a document written in YAML that represents the architecture of a serverless application. The first line of the document contains Transform: 'AWS::Serverless-2016-10-31'.
* It represents an intrinsic function
* Presence of Transform section indicates it is a Serverless Application Model (SAM) template
* Presence of Transform section indicates it is a CloudFormation Parameter
* It represents a Lambda function definition

### Question 41:
An application running on EC2 instances processes messages from an SQS queue. However, sometimes the messages are not processed and they end up in errors. These messages need to be isolated for further processing and troubleshooting.
* Implement a Dead-Letter Queue
* Reduce the VisibilityTimeout
* Increase the VisibilityTimeout
* Use DeleteMessage

### Question 42:
You are an administrator for a video-on-demand web application where content creators upload videos directly into S3. Recent support requests from customers state that uploading video files near 500GB size causes the website to break. After doing some investigation you find the following error: 'Your proposed upload exceeds the maximum allowed size'.
* You need to place a service limit request increase with AWS
* You need to use multi-part upload for large files
* Your IAM permissions are incorrect
* The maximum file size is 5 GB

### Question 43:
A developer is looking at establishing access control for an API that connects to a Lambda function downstream.
* AWS Security Token Service (STS)
* Cognito User Pools
* Standard AWS IAM roles and policies
* Lambda Authorizer

### Question 44:
Recently in your organization, the AWS X-Ray SDK was bundled into each Lambda function to record outgoing calls for tracing purposes. When your team leader goes to the X-Ray service in the AWS Management Console to get an overview of the information collected, they discover that no data is available.
* X-Ray only works with AWS Lambda aliases
* Enable X-Ray sampling
* Fix the IAM Role
* Change the security group rules

### Question 45:
A company needs a version control system for their fast development lifecycle with incremental changes, version control, and support to existing Git tools.
* AWS CodeCommit
* Amazon Versioned S3 Bucket
* AWS CodeBuild
* AWS CodePipeline

### Question 46:
A new recruit is trying to configure what an Amazon EC2 should do when it interrupts a Spot Instance.
* Stop the Spot Instance
* Reboot the Spot Instance
* Terminate the Spot Instance
* Hibernate the Spot Instance

### Question 47:
As an AWS Certified Developer Associate, you have been hired to consult with a company that uses the NoSQL database for mobile applications. The developers are using DynamoDB to perform operations such as GetItem but are limited in knowledge. They would like to be more efficient with retrieving some attributes rather than all.
* Use the --query parameter
* Use a Scan
* Use a FilterExpression
* Specify a ProjectionExpression

### Question 48:
You create an Auto Scaling group to work with an Application Load Balancer. The scaling group is configured with a minimum size value of 5, a maximum value of 20, and the desired capacity value of 10. One of the 10 EC2 instances has been reported as unhealthy.
* The ASG will format the root EBS drive on the EC2 instance and run the User Data again
* The ASG will keep the instance running and re-start the application
* The ASG will detach the EC2 instance from the group, and leave it running
* The ASG will terminate the EC2 Instance

### Question 49:
A developer at a university is encrypting a large XML payload transferred over the network using AWS KMS and wants to test the application before going to production.
* 16KB
* 4KB
* 10MB
* 1MB

### Question 50:
You're a developer for 'Movie Gallery', a company that just migrated to the cloud. A database must be created using NoSQL technology to hold movies that are listed for public viewing. You are taking an important step in designing the database with DynamoDB and need to choose the appropriate partition key.
* movie_language
* producer_name
* lead_actor_name
* movie_id

### Question 51:
The technology team at an investment bank uses DynamoDB to facilitate high-frequency trading where multiple trades can try and update an item at the same time.
* Use ConsistentRead = false while doing PutItem operation for any item
* Use ConsistentRead = true while doing PutItem operation for any item
* Use ConsistentRead = true while doing GetItem operation for any item
* Use ConsistentRead = true while doing UpdateItem operation for any item

### Question 52:
A company wants to automate the creation of ECS clusters using CloudFormation. The process has worked for a while, but after creating task definitions and assigning roles, the development team discovers that the tasks for containers are not using the permissions assigned to them.
* ECS_ENGINE_AUTH_DATA
* ECS_ENABLE_TASK_IAM_ROLE
* ECS_CLUSTER
* ECS_AVAILABLE_LOGGING_DRIVERS

### Question 53:
A company has AWS Lambda functions where each is invoked by other AWS services such as Amazon Kinesis Data Firehose, Amazon API Gateway, Amazon Simple Storage Service, or Amazon CloudWatch Events. What these Lambda functions have in common is that they process heavy workloads such as big data analysis, large file processing, and statistical computations.
* Change the instance type for your Lambda function
* Change your Lambda function runtime to use Golang
* Increase the RAM assigned to your Lambda function
* Increase the Lambda function timeout

### Question 54:
A developer in your company was just promoted to Team Lead and will be in charge of code deployment on EC2 instances via AWS CodeCommit and AWS CodeDeploy. Per the new requirements, the deployment process should be able to change permissions for deployed files as well as verify the deployment success.
* Define an appspec.yml file in the codebuild/ directory
* Define a buildspec.yml file in the codebuild/ directory
* Define an appspec.yml file in the root directory
* Define a buildspec.yml file in the root directory

### Question 55:
You are a developer working at a cloud company that embraces serverless. You have performed your initial deployment and would like to work towards adding API Gateway stages and associate them with existing deployments. Your stages will include prod, test, and dev and will need to match a Lambda function variant that can be updated over time.
* Stage Variables
* Mapping Templates
* Lambda Versions
* Lambda Aliases
* Lambda X-Ray integration

### Question 56:
Other than the Resources section, which of the following sections in a Serverless Application Model (SAM) Template is mandatory?
* Mappings
* Transform
* Globals
* Parameters

### Question 57:
A developer working with EC2 Windows instance has installed Kinesis Agent for Windows to stream JSON-formatted log files to Amazon Simple Storage Service (S3) via Amazon Kinesis Data Firehose. The developer wants to understand the sink type capabilities of Kinesis Firehose.
* Amazon Redshift with Amazon S3
* Amazon ElastiCache with Amazon S3 as backup
* Amazon Elasticsearch Service (Amazon ES) with optionally backing up data to Amazon S3
* Amazon Simple Storage Service (Amazon S3) as a direct Firehose destination

### Question 58:
A Developer is configuring Amazon EC2 Auto Scaling group to scale dynamically.
* ASGAverageCPUUtilization
* ASGAverageNetworkOut
* ApproximateNumberOfMessagesVisible
* ALBRequestCountPerTarget

### Question 59:
Your company has embraced cloud-native microservices architectures. New applications must be dockerized and stored in a registry service offered by AWS. The architecture should support dynamic port mapping and support multiple tasks from a single service on the same container instance. All services should run on the same EC2 instance.
* Application Load Balancer + Beanstalk
* Application Load Balancer + ECS
* Classic Load Balancer + Beanstalk
* Classic Load Balancer + ECS

### Question 60:
As a senior architect, you are responsible for the development, support, maintenance, and implementation of all database applications written using NoSQL technology. A new project demands a throughput requirement of 10 strongly consistent reads per second of 6KB in size each.
* 20
* 60
* 10
* 30

### Question 61:
A business has their test environment built on Amazon EC2 configured on General purpose SSD volume.
* 16 TiB
* 2.7 TiB
* 10.6 TiB
* 5.3 TiB

### Question 62:
The development team at an e-commerce company completed the last deployment for their application at a reduced capacity because of the deployment policy. The application took a performance hit because of the traffic spike due to an on-going sale.
* Deploy the new application version using 'All at once' deployment policy
* Deploy the new application version using 'Rolling with additional batch' deployment policy
* Deploy the new application version using 'Rolling' deployment policy
* Deploy the new application version using 'Immutable' deployment policy

### Question 63:
A company has a cloud system in AWS with components that send and receive messages using SQS queues. While reviewing the system you see that it processes a lot of information and would like to be aware of any limits of the system.
* 10000
* no limit
* 100000
* 10000000

### Question 64:
You have created a continuous delivery service model with automated steps using AWS CodePipeline. Your pipeline uses your code, maintained in a CodeCommit repository, AWS CodeBuild, and AWS Elastic Beanstalk to automatically deploy your code every time there is a code change. However, the deployment part to Elastic Beanstalk is taking a very long time due to resolving dependencies on all of your 100 target EC2 instances.
* Create a custom platform for Elastic Beanstalk
* Bundle the dependencies in the source code in CodeCommit
* Bundle the dependencies in the source code during the last stage of CodeBuild
* Store the dependencies in S3

### Question 65:
As a Developer Associate, you are responsible for the data management of the AWS Kinesis streams at your company. The security team has mandated stricter security requirements by leveraging mechanisms available with the Kinesis Data Streams service that won't require code changes on your end.
* SSE-C encryption
* KMS encryption for data at rest
* Encryption in flight with HTTPS endpoint
* Envelope Encryption
* Client-Side Encryption

# Exam 3

### Question 1:
A Company uses a large set of EBS volumes for their fleet of Amazon EC2 instances. As an AWS Certified Developer Associate, your help has been requested to understand the security features of the EBS volumes. The company does not want to build or maintain their own encryption key management infrastructure.
* A snapshot of an encrypted volume can be encrypted or unencrypted
* Encryption by default is an AZ specific setting. If you enable it for an AZ, you cannot disable it for individual volumes or snapshots in that AZ
* You can encrypt an existing unencrypted volume or snapshot by using AWS Key Management Service (KMS) AWS SDKs
* Encryption by default is a Region-specific setting. If you enable it for a Region, you cannot disable it for individual volumes or snapshots in that Region
* A volume restored from an encrypted snapshot, or a copy of an encrypted snapshot is always encrypted

### Question 2:
You have been asked by your Team Lead to enable detailed monitoring of the Amazon EC2 instances your team uses. As a Developer working on AWS CLI, which of the below command will you run?
* aws ec2 monitor-instances --instance-ids i-1234567890abcdef0
* aws ec2 run-instances --image-id ami-09092360 --monitoring State=enabled
* aws ec2 monitor-instances --instance-id i-1234567890abcdef0
* aws ec2 run-instances --image-id ami-09092360 --monitoring Enabled=true

### Question 3:
AWS CloudFormation helps model and provision all the cloud infrastructure resources needed for your business.
* AWS Elastic Beanstalk
* AWS Autoscaling
* AWS Serverless Application Model (AWS SAM)
* AWS CodeBuild
* AWS Lambda

### Question 4:
Amazon S3 achieves high availability by replicating data across multiple servers within AWS data centers. This implies, information about the changes must be replicated across Amazon S3, which can take some time. One gets to observe certain behavior of S3 because of this lag.
* A process deletes an existing object and immediately lists keys within its bucket. Until the deletion is fully propagated, Amazon S3 might list the deleted object
* A process writes a new object to Amazon S3 and immediately lists keys within its bucket. Until the change is fully propagated, the object might not appear in the list
* A process deletes an existing object and immediately tries to read it. Until the deletion is fully propagated, Amazon S3 might return the deleted data
* Amazon S3 supports object locking for concurrent updates

### Question 5:
Recently, you started an online learning platform using AWS Lambda and AWS Gateway API. Your first version was successful, and you began developing new features for the second version. You would like to gradually introduce the second version by routing only 10% of the incoming traffic to the new Lambda version.
* Use AWS Lambda aliases
* Use environment variables
* Use Tags to distinguish the different versions
* Deploy your Lambda in a VPC

### Question 6:
You are creating a mobile application that needs access to the AWS API Gateway. Users will need to register first before they can access your API and you would like the user management to be fully managed.
* Use API Gateway User Pools
* Use Cognito User Pools
* Use Lambda Authorizer
* Use IAM permissions with sigv4

### Question 7:
You are running a cloud file storage website with an Internet-facing Application Load Balancer, which routes requests from users over the internet to 10 registered Amazon EC2 instances. Users are complaining that your website always asks them to re-authenticate when they switch pages. You are puzzled because this behavior is not seen in your local machine or dev environment.
* Application Load Balancer is in slow-start mode, which gives ALB a little more time to read and write session data
* The Load Balancer does not have stickiness enabled
* The Load Balancer does not have TLS enabled
* The EC2 instances are logging out the users because the instances never have access to the client IPs because of the Load Balancer

### Question 8:
A multi-national enterprise uses AWS Organizations to manage its users across different divisions. Even though CloudTrail is enabled on the member accounts, managers have noticed that access issues to CloudTrail logs across different divisions and AWS Regions is becoming a bottleneck in troubleshooting issues. They have decided to use the organization trail to keep things simple.
* By default, CloudTrail tracks only bucket-level actions. To track object-level actions, you need to enable Amazon S3 data events
* Member accounts will be able to see the Organization trail, but cannot modify or delete it
* There is nothing called Organization Trail. The master account can, however, enable CloudTrail logging, to keep track of all activities across AWS accounts
* Member accounts do not have access to organization trail, neither do they have access to the Amazon S3 bucket that logs the files
* By default, CloudTrail event log files are not encrypted

### Question 9:
As a developer, you are looking at creating a custom configuration for Amazon EC2 instances running in an Auto Scaling group. The solution should allow the group to auto-scale based on the metric of 'average RAM usage' for your Amazon EC2 instances.
* Migrate your application to AWS Lambda
* Create a custom alarm for your ASG and make your instances trigger the alarm using PutAlarmData API
* Enable detailed monitoring for EC2 and ASG to get the RAM usage data and create a CloudWatch Alarm on top of it
* Create a custom metric in CloudWatch and make your instances send data to it using PutMetricData. Then, create an alarm based on this metric

### Question 10:
You company runs business logic on smaller software components that perform various functions. Some functions process information in a few seconds while others seem to take a long time to complete. Your manager asked you to decouple components that take a long time to ensure software applications stay responsive under load. You decide to configure Amazon Simple Queue Service (SQS) to work with your Elastic Beanstalk configuration.
* Single Instance with Elastic IP
* Single Instance Worker node
* Load-balancing, Autoscaling environment
* Dedicated worker environment

### Question 11:
You have a workflow process that pulls code from AWS CodeCommit and deploys to EC2 instances associated with tag group ProdBuilders. You would like to configure the instances to archive no more than two application revisions to conserve disk space.
* Integrate with AWS CodePipeline
* CodeDeploy Agent
* Have a load balancer in front of your instances
* AWS CloudWatch Log Agent

### Question 12:
You are a developer working with the AWS CLI to create Lambda functions that contain environment variables. Your functions will require over 50 environment variables consisting of sensitive information of database table names.
* The total size of all environment variables shouldn't exceed 4 KB. There is no limit on the number of variables
* The total size of all environment variables shouldn't exceed 4 KB. The maximum number of variables that can be created is 35
* The total size of all environment variables shouldn't exceed 8 KB. The maximum number of variables that can be created is 50
* The total size of all environment variables shouldn't exceed 8 KB. There is no limit on the number of variables

### Question 13:
A multi-national company maintains separate AWS accounts for different verticals in their organization. The project manager of a team wants to migrate the Elastic Beanstalk environment from Team A's AWS account into Team B's AWS account. As a Developer, you have been roped in to help him in this process.
* Create an export configuration from the Elastic Beanstalk console from Team A's account. This configuration has to be shared with the IAM Role of Team B's account. The import option of Team B's account will show the saved configuration, that can be used to create a new Beanstalk application
* Create a saved configuration in Team A's account and configure it to Export. Now, log into Team B's account and choose the Import option. Here, you need to specify the name of the saved configuration and allow the system to create the new application. This takes a little time based on the Regions the two accounts belong to
* Create a saved configuration in Team A's account and download it to your local machine. Make the account-specific parameter changes and upload to the S3 bucket in Team B's account. From Elastic Beanstalk console, create an application from 'Saved Configurations'
* It is not possible to migrate Elastic Beanstalk environment from one AWS account to the other

### Question 14:
A startup manages its Cloud resources with Elastic Beanstalk. The environment consists of few Amazon EC2 instances, an Auto Scaling Group (ASG), and an Elastic Load Balancer. Even after the Load Balancer marked an EC2 instance as unhealthy, the ASG has not replaced it with a healthy instance.
* Auto Scaling group doesn't automatically replace the unhealthy instances marked by the load balancer. They have to be manually replaced from AWS Console
* Health check parameters were configured for checking the instance health alone. The instance failed because of application failure which was not configured as a parameter for health check status
* The ping path field of the Load Balancer is configured incorrectly
* The health check type of your instance's Auto Scaling group, must be changed from EC2 to ELB by using a configuration file

### Question 15:
A HealthCare mobile app uses proprietary Machine Learning algorithms to provide early diagnosis using patient health metrics. To protect this sensitive data, the development team wants to transition to a scalable user management system with log-in/sign-up functionality that also supports Multi-Factor Authentication (MFA)
* Use Lambda functions and RDS to create a custom solution for user management
* Use Amazon SNS to send Multi-Factor Authentication (MFA) code via SMS to mobile app users
* Use Lambda functions and DynamoDB to create a custom solution for user management
* Use Amazon Cognito to enable Multi-Factor Authentication (MFA) when users log-in
* Use Amazon Cognito for user-management and facilitating the log-in/sign-up process

### Question 16:
As part of employee skills upgrade, the developers of your team have been delegated few responsibilities of DevOps engineers. Developers now have full control over modeling the entire software delivery process, from coding to deployment. As the team lead, you are now responsible for any manual approvals needed in the process.
* Create one CodePipeline for your entire flow and add a manual approval step
* Create deeply integrated AWS CodePipelines for each environment
* Create multiple CodePipelines for each environment and link them using AWS Lambda
* Use CodePipeline with Amazon Virtual Private Cloud

### Question 17:
Your company uses an Application Load Balancer to route incoming end-user traffic to applications hosted on Amazon EC2 instances. The applications capture incoming request information and store it in the Amazon Relational Database Service (RDS) running on Microsoft SQL Server DB engines.
* Use the header X-Forwarded-From
* You can get the Client IP addresses from Elastic Load Balancing logs
* Use the header X-Forwarded-For
* You can get the Client IP addresses from server access logs

### Question 18:
A junior developer working on ECS instances terminated a container instance in Amazon Elastic Container Service (Amazon ECS) as per instructions from the team lead. But the container instance continues to appear as a resource in the ECS cluster.
* You terminated the container instance while it was in STOPPED state, that lead to this synchronization issues
* You terminated the container instance while it was in RUNNING state, that lead to this synchronization issues
* A custom software on the container instance could have failed and resulted in the container hanging in an unhealthy state till restarted again
* The container instance has been terminated with AWS CLI, whereas, for ECS instances, Amazon ECS CLI should be used to avoid any synchronization issues

### Question 19:
A multi-national company runs its technology operations on AWS Cloud. As part of their storage solution, they use a large number of EBS volumes, with AWS Config and CloudTrail activated. A manager has tried to find the user name that created an EBS volume by searching CloudTrail events logs but wasn't successful.
* AWS CloudTrail event logs for 'ManageVolume' aren't available for EBS volumes created during an Amazon EC2 launch
* AWS CloudTrail event logs for 'CreateVolume' aren't available for EBS volumes created during an Amazon EC2 launch
* EBS volume status checks are disabled
* Amazon EBS CloudWatch metrics are disabled

### Question 20:
An intern at an IT company is getting started with AWS Cloud and wants to understand the following Amazon S3 bucket access policy:
* Allows IAM users to access their own home directory in Amazon S3, programmatically and in the console
* Allows full S3 access to an Amazon Cognito user, but explicitly denies access to the Production bucket if the Cognito user is not authenticated
* Allows full S3 access, but explicitly denies access to the Production bucket if the user has not signed in using MFA within the last thirty minutes
* Allows a user to manage a single Amazon S3 bucket and denies every other AWS action and resource if the user is not signed in using MFA within last thirty minutes

### Question 21:
Your company is planning to move away from reserving EC2 instances and would like to adopt a more agile form of serverless architecture.
* Amazon Elastic Kubernetes Service (Amazon EKS) on Fargate
* AWS Elastic Beanstalk
* Amazon Elastic Container Service (Amazon ECS) on EC2
* Amazon Elastic Container Service (Amazon ECS) on Fargate

### Question 22:
An organization is moving its on-premises resources to the cloud. Source code will be moved to AWS CodeCommit and AWS CodeBuild will be used for compiling the source code using Apache Maven as a build tool. The organization wants the build environment should allow for scaling and running builds in parallel.
* Enable CodeBuild Auto Scaling
* CodeBuild scales automatically, the organization does not have to do anything for scaling or for parallel builds
* Choose a high-performance instance type for your CodeBuild instances
* Run CodeBuild in an Auto Scaling group

### Question 23:
As a Senior Developer, you manage 10 Amazon EC2 instances that make read-heavy database requests to the Amazon RDS for PostgreSQL. You need to make this architecture resilient for disaster recovery.
* Use RDS Provisioned IOPS (SSD) Storage in place of General Purpose (SSD) Storage
* Use database cloning feature of the RDS DB cluster
* Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups across multiple Regions
* Use cross-Region Read Replicas
* Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups in a single AWS Region

### Question 24:
Your team-mate has configured an Amazon S3 event notification for an S3 bucket that holds sensitive audit data of a firm. As the Team Lead, you are receiving the SNS notifications for every event in this bucket. After validating the event data, you realized that few events are missing.
* Someone could have created a new notification configuration and that has overridden your existing configuration
* Your notification action is writing to the same bucket that triggers the notification
* If two writes are made to a single non-versioned object at the same time, it is possible that only a single event notification will be sent
* Versioning is enabled on the S3 bucket and event notifications are getting fired for only one version

### Question 25:
Your organization has developers that merge code changes regularly to an AWS CodeCommit repository. Your pipeline has AWS CodeCommit as the source and you would like to configure a rule that reacts to changes in CodeCommit.
* Use Lambda function with Amazon Simple Notification Service (SNS)
* Use CloudWatch Event Rules
* Use Lambda Event Rules
* Use CloudTrail Event rules with Amazon Simple Email Service (SES)

### Question 26:
A company uses microservices-based infrastructure to process the API calls from clients, perform request filtering and cache requests using the AWS API Gateway. Users report receiving 501 error code and you have been contacted to find out what is failing.
* Use X-Ray service
* Use CloudWatch service
* Use CloudTrail service
* Use API Gateway service

### Question 27:
A company uses Amazon RDS as its database. For improved user experience, it has been decided that a highly reliable fully-managed caching layer has to be configured in front of RDS.
* Install Redis on an Amazon EC2 instance
* Implement Amazon ElastiCache Memcached
* Migrate the database to Amazon Redshift
* Implement Amazon ElastiCache Redis in Cluster Mode

### Question 28:
You team maintains a public API Gateway that is accessed by clients from another domain. Usage has been consistent for the last few months but recently it has more than doubled. As a result, your costs have gone up and would like to prevent other unauthorized domains from accessing your API.
* Assign a Security Group to your API Gateway
* Use Mapping Templates
* Restrict access by using CORS
* Use Account-level throttling

### Question 29:
A large firm stores its static data assets on Amazon S3 buckets. Each service line of the firm has its own AWS account. For a business use case, the Finance department needs to give access to their S3 bucket's data to the Human Resources department.
* Use Cross-account IAM roles for programmatic and console access to S3 bucket objects
* Use Access Control List (ACL) and IAM policies for programmatic-only access to S3 bucket objects
* Use IAM roles and resource-based policies delegate access across accounts within different partitions via programmatic access only
* Use Resource-based policies and AWS Identity and Access Management (IAM) policies for programmatic-only access to S3 bucket objects

### Question 30:
A company has a workload that requires 14,000 consistent IOPS for data that must be durable and secure. The compliance standards of the company state that the data should be secure at every stage of its lifecycle on all of the EBS volumes they use.
* EBS volumes don't support any encryption
* EBS volumes do not support in-flight encryption but do support encryption at rest using KMS
* EBS volumes support in-flight encryption but does not support encryption at rest
* EBS volumes support both in-flight encryption and encryption at rest using KMS

### Question 31:
An AWS CodePipeline was configured to be triggered by Amazon CloudWatch Events. Recently the pipeline failed and upon investigation, the Team Lead noticed that the source was changed from AWS CodeCommit to Amazon Simple Storage Service (S3). The Team Lead has requested you to find the user who had made the changes.
* AWS CloudTrail
* Amazon Inspector
* Amazon CloudWatch
* AWS X-Ray

### Question 32:
Your web application reads and writes data to your DynamoDB table. The table is provisioned with 400 Write Capacity Units (WCU’s) shared across 4 partitions. One of the partitions receives 250 WCU/second while others receive much less. You receive the error 'ProvisionedThroughputExceededException'.
* You have a hot partition
* Configured IAM policy is wrong
* Write Capacity Units (WCU’s) are applied across to all your DynamoDB tables and this needs reconfiguration
* CloudWatch monitoring is lagging

### Question 33:
A leading financial services company offers data aggregation services for Wall Street trading firms. The company bills its clients based on per unit of clickstream data provided to the clients. As the company operates in a regulated industry, it needs to have the same ordered clickstream data available for auditing within a window of 7 days.
* AWS Kinesis Data Analytics
* AWS Kinesis Data Firehose
* Amazon SQS
* AWS Kinesis Data Streams

### Question 34:
A company has their entire stack integrated with AWS X-Ray. A manager at the company noticed the skyrocketing AWS monthly usage charges for the X-Ray service. He tracked the abnormal bills to the high volume of input data going into X-Ray. As a Developer, you have been given the responsibility to fix this issue as quickly as possible, with minimal disruptions.
* Enable X-Ray Sampling
* Send only the required data from client-side
* Enable X-Ray Deep linking to send only the most useful data to X-Ray
* Custom configuration of the X-Ray agents

### Question 35:
A digital marketing company has its website hosted on an Amazon S3 bucket A. The development team notices that the static JavaScript files, that are hosted on another S3 bucket B, are not loading correctly on the website.
* Update bucket policies on both bucket A and bucket B to allow successful loading of the JavaScript files on the website
* Enable versioning on both the buckets to facilitate correct functioning of the website
* Configure CORS on the bucket B that is hosting the JavaScript files to allow Bucket A origin to make the requests
* Configure CORS on the bucket A that is hosting the website to allow any origin to respond to requests

### Question 36:
The development team at a social media company is considering using Amazon ElastiCache to boost the performance of their existing databases.
* Use ElastiCache to run highly complex JOIN queries
* Use ElastiCache to improve latency and throughput for write-heavy application workloads
* Use ElastiCache to improve performance of compute-intensive workloads
* Use ElastiCache to improve latency and throughput for read-heavy application workloads
* Use ElastiCache to improve performance of Extract-Transform-Load (ETL) workloads

### Question 37:
Your company hosts a static website on Amazon Simple Storage Service (S3) written in HTML5. The website targets aviation enthusiasts and it has grown a worldwide audience with hundreds of thousands of visitors accessing the website now on a monthly basis. While users in the United States have a great user experience, users from other parts of the world are experiencing slow responses and lag.
* Use Amazon CloudFront
* Use Amazon S3 Caching
* Use Amazon ElastiCache for Redis
* Use Amazon S3 Transfer Acceleration

### Question 38:
A high-frequency stock trading firm is migrating their messaging queues from self-managed message-oriented middleware systems to Amazon SQS. The development team at the company wants to minimize the costs of using SQS.
* Use SQS long polling to retrieve messages from your Amazon SQS queues
* Use SQS message timer to retrieve messages from your Amazon SQS queues
* Use SQS short polling to retrieve messages from your Amazon SQS queues
* Use SQS visibility timeout to retrieve messages from your Amazon SQS queues

### Question 39:
You have an Auto Scaling group configured to a minimum capacity of 1 and a maximum capacity of 5, designed to launch EC2 instances across 3 Availability Zones. During a low utilization period, an entire Availability Zone went down and your application experienced downtime.
* Increase the minimum instance capacity of the Auto Scaling Group to 2
* Change the scaling metric of auto-scaling policy to network bytes
* Enable RDS Multi-AZ
* Configure ASG fast failover

### Question 40:
An e-commerce company has an order processing workflow with several tasks to be done in parallel as well as decision steps to be evaluated for successful processing of the order. All the tasks are implemented via Lambda functions.
* Use AWS Step Functions activities to orchestrate the workflow
* Use AWS Glue to orchestrate the workflow
* Use AWS Batch to orchestrate the workflow
* Use AWS Step Functions state machines to orchestrate the workflow

### Question 41:
A recruit has created an Amazon Simple Storage Service (S3) bucket. He needs assistance in getting the security principles right for this bucket.
* Use of IAM Roles
* Use of Access Control Lists (ACLs)
* Use of Security Groups
* Use of Bucket Policies

### Question 42:
An application runs on an EC2 instance and processes orders on a nightly basis. This EC2 instance needs to access the orders that are stored in S3.
* Create an IAM programmatic user and store the access key and secret access key on the EC2 ~/.aws/credentials file.
* Use EC2 User Data
* Use an IAM role
* Create an S3 bucket policy that authorises public access

### Question 43:
You have a three-tier web application consisting of a web layer using AngularJS, an application layer using an AWS API Gateway and a data layer in an Amazon Relational Database Service (RDS) database. Your web application allows visitors to look up popular movies from the past. The company is looking at reducing the number of calls made to endpoint and improve latency to the API.
* Use Stage Variables
* Use Amazon Kinesis Data Streams to stream incoming data and reduce the burden on Gateway APIs
* Enable API Gateway Caching
* Use Mapping Templates

### Question 44:
As a Developer, you are working on a mobile application that utilizes Amazon Simple Queue Service (SQS) for sending messages to downstream systems for further processing. One of the requirements is that the messages should be stored in the queue for a period of 12 days.
* The maximum retention period of SQS messages is 7 days, therefore retention period of 12 days is not possible
* Enable Long Polling for the SQS queue
* Use a FIFO SQS queue
* Change the queue message retention setting

### Question 45:
An IT company has its serverless stack integrated with AWS X-Ray. The developer at the company has noticed a high volume of data going into X-Ray and the AWS monthly usage charges have skyrocketed as a result. The developer has requested changes to mitigate the issue.
* Custom configuration for the X-Ray agents
* Implement a network sampling rule
* Enable X-Ray sampling
* Use Filter Expressions in the X-Ray console

### Question 46:
An organization with high data volume workloads have successfully moved to DynamoDB after having many issues with traditional database systems. However, a few months into production, DynamoDB tables are consistently recording high latency.
* Increase the request timeout settings, so the client gets enough time to complete the requests, thereby reducing retries on the system
* Consider using Global tables if your application is accessed by globally distributed users
* Use DynamoDB Accelerator (DAX) for businesses with heavy write-only workloads
* Reduce connection pooling, which keeps the connections alive even when user requests are not present, thereby, blocking the services
* Use eventually consistent reads in place of strongly consistent reads whenever possible

### Question 47:
You have migrated an on-premise SQL Server database to an Amazon Relational Database Service (RDS) database attached to a VPC inside a private subnet. Also, the related Java application, hosted on-premise, has been moved to an Amazon Lambda function.
* Use Lambda layers to connect to the internet and RDS separately
* Configure Lambda to connect to VPC with private subnet and Security Group needed to access RDS
* Use Environment variables to pass in the RDS connection string
* Configure lambda to connect to the public subnet that will give internet access and use Security Group to access RDS inside the private subnet

### Question 48:
Your team lead has requested code review of your code for Lambda functions. Your code is written in Python and makes use of the Amazon Simple Storage Service (S3) to upload logs to an S3 bucket. After the review, your team lead has recommended reuse of execution context to improve the Lambda performance.
* Use environment variables to pass operational parameters
* Enable X-Ray integration
* Assign more RAM to the function
* Move the Amazon S3 client initialization, out of your function handler

### Question 49:
A company’s e-commerce website is expecting hundreds of thousands of visitors on Black Friday. The marketing department is concerned that high volumes of orders might stress SQS leading to message failures. The company has approached you for the steps to be taken as a precautionary measure against the high volumes.
* Enable auto-scaling in the SQS queue
* Convert the queue into FIFO ordered queue, since messages to the down system will be processed faster once they are ordered
* Pre-configure the SQS queue to increase the capacity when messages hit a certain threshold
* Amazon SQS is highly scalable and does not need any intervention to handle the expected high volumes

### Question 50:
Your web application architecture consists of multiple Amazon EC2 instances running behind an Elastic Load Balancer with an Auto Scaling group having the desired capacity of 5 EC2 instances. You would like to integrate AWS CodeDeploy for automating application deployment. The deployment should re-route traffic from your application's original environment to the new environment.
* Opt for Blue/Green deployment
* Opt for In-place deployment
* Opt for Rolling deployment
* Opt for Immutable deployment

### Question 51:
A media company uses Amazon Simple Queue Service (SQS) queue to manage their transactions. With changing business needs, the payload size of the messages is increasing. The Team Lead of the project is worried about the 256 KB message size limit that SQS has.
* Use the MultiPart API
* Use the SQS Extended Client
* Use gzip compression
* Get a service limit increase from AWS

### Question 52:
You have deployed a traditional 3-tier web application architecture with a Classic Load Balancer, an Auto Scaling group, and an Amazon Relational Database Service (RDS) database. Users are reporting that they have to re-authenticate into the website often.
* Use Elastic IP
* Enable RDS read replicas
* Add an ElastiCache Cluster
* Enable Load Balancer stickiness

### Question 53:
You are working for a shipping company that is automating the creation of ECS clusters with an Auto Scaling Group using an AWS CloudFormation template that accepts cluster name as its parameters. Initially, you launch the template with input value 'MainCluster', which deployed five instances across two availability zones. The second time, you launch the template with an input value 'SecondCluster'. However, the instances created in the second run were also launched in 'MainCluster' even after specifying a different cluster name.
* The security groups on the EC2 instance are pointing to the wrong ECS cluster
* The cluster name Parameter has not been updated in the file /etc/ecs/ecs.config during bootstrap
* The ECS agent Docker image must be re-built to connect to the other clusters
* The EC2 instance is missing IAM permissions to join the other clusters

### Question 54:
As part of their on-boarding, the employees at an IT company need to upload their profile photos in a private S3 bucket. The company wants to build an in-house web application hosted on an EC2 instance that should display the profile photos in a secure way when the employees mark their attendance.
* Make the S3 bucket public so that the application can reference the image URL for display
* Save the S3 key for each user's profile photo in a DynamoDB table and use a lambda function to dynamically generate a pre-signed URL. Reference this URL for display via the web application
* Keep each user's profile image encoded in base64 format in a DynamoDB table and reference it from the application for display
* Keep each user's profile image encoded in base64 format in an RDS table and reference it from the application for display

### Question 55:
A telecommunications company that provides internet service for mobile device users maintains over 100 c4.large instances in the us-east-1 region. The EC2 instances run complex algorithms. The manager would like to track CPU utilization of the EC2 instances as frequently as every 10 seconds.
* Enable EC2 detailed monitoring
* Open a support ticket with AWS
* Create a high-resolution custom metric and push the data using a script triggered every 10 seconds
* Simply get it from the CloudWatch Metrics

### Question 56:
A financial services company wants to ensure that the customer data is always kept encrypted on Amazon S3 but wants a fully managed solution to create, rotate and remove the encryption keys.
* Server-Side Encryption with Secrets Manager
* Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3)
* Server-Side Encryption with Customer-Provided Keys (SSE-C)
* Server-Side Encryption with Customer Master Keys (CMKs) Stored in AWS Key Management Service (SSE-KMS)

### Question 57:
Your company has a three-year contract with a healthcare provider. The contract states that monthly database backups must be retained for the duration of the contract for compliance purposes. Currently, the limit on backup retention for automated backups, on Amazon Relational Database Service (RDS), does not meet your requirements.
* Enable RDS automatic backups
* Enable RDS Multi-AZ
* Enable RDS Read replicas
* Create a cron event in CloudWatch, which triggers an AWS Lambda function that triggers the database snapshot

### Question 58:
Your application is deployed automatically using AWS Elastic Beanstalk. Your YAML configuration files are stored in the folder .ebextensions and new files are added or updated often. The DevOps team does not want to re-deploy the application every time there are configuration changes, instead, they would rather manage configuration externally, securely, and have it load dynamically into the application at runtime.
* Use SSM Parameter Store
* Use S3
* Use Environment variables
* Use Stage Variables

### Question 59:
You are a system administrator whose company recently moved its production application to AWS and migrated data from MySQL to AWS DynamoDB. You are adding new tables to AWS DynamoDB and need to allow your application to query your data by the primary key and an alternate key. This option must be added when first creating tables otherwise changes cannot be made afterward.
* Create a GSI
* Call Scan
* Migrate away from DynamoDB
* Create a LSI

### Question 60:
An IT company has migrated to a serverless application stack on the AWS Cloud with the compute layer being implemented via Lambda functions. The engineering managers would like to actively troubleshoot any failures in the Lambda functions.
* Use CloudWatch Events to identify and notify any failures in the Lambda code
* Use CodeDeploy to identify and notify any failures in the Lambda code
* Use CodeCommit to identify and notify any failures in the Lambda code
* The developers should insert logging statements in the Lambda function code which are then available via CloudWatch logs

### Question 61:
A developer from your team has configured the load balancer to route traffic equally between instances or across Availability Zones. However, Elastic Load Balancing (ELB) routes more traffic to one instance or Availability Zone than the others.
* Sticky sessions are enabled for the load balancer
* There could be short-lived TCP connections between clients and instances
* Instances of a specific capacity type aren’t equally distributed across Availability Zones
* For Application Load Balancers, cross-zone load balancing is disabled by default
* After you disable an Availability Zone, the targets in that Availability Zone remain registered with the load balancer, thereby receiving random bursts of traffic

### Question 62:
A mobile gaming company is experiencing heavy read traffic to its Amazon Relational Database Service (RDS) database that retrieves player’s scores and stats. The company is using RDS database instance type db.m5.12xlarge, which is not cost-effective for their budget. They would like to implement a strategy to deal with the high volume of read traffic, reduce latency, and also downsize the instance size to cut costs.
* Setup RDS Read Replicas
* Move to Amazon Redshift
* Setup ElastiCache in front of RDS
* Switch application code to AWS Lambda for better performance

### Question 63:
A cybersecurity company is running a serverless backend with several compute-heavy workflows running on Lambda functions. The development team has noticed a performance lag after analyzing the performance metrics for the Lambda functions.
* Use provisioned concurrency to account for the compute-heavy workflows
* Increase the amount of memory available to the Lambda functions
* Invoke the Lambda functions asynchronously to process the compute-heavy workflows
* Use reserved concurrency to account for the compute-heavy workflows

### Question 64:
A new member of your team is working on creating Dead Letter Queue (DLQ) for AWS Lambda functions.
* The Lambda function invocation failed only once but succeeded thereafter
* The Lambda function invocation is asynchronous
* The event has been processed successfully
* The Lambda function invocation is synchronous
* The event fails all processing attempts

### Question 65:
Two policies are attached to an IAM user. The first policy states that the user has explicitly been denied all access to EC2 instances. The second policy states that the user has been allowed permission for EC2:Describe action.
* The order of the policy matters. If policy 1 is before 2, then the user is denied access. If policy 2 is before 1, then the user is allowed access
* The user will be denied access because one of the policies has an explicit deny on it
* The IAM user stands in an invalid state, because of conflicting policies
* The user will get access because it has an explicit allow

# Exam 4

### Question 1:
Your company has been hired to build a resilient mobile voting app for an upcoming music award show that expects to have 5 to 20 million viewers. The mobile voting app will be marketed heavily months in advance so you are expected to handle millions of messages in the system. You are configuring Amazon Simple Queue Service (SQS) queues for your architecture that should receive messages from 20 KB to 200 KB.
* Yes, the max message size is 256KB
* Yes, the max message size is 512KB
* No, the max message size is 64KB
* No, the max message size is 128KB

### Question 2:
You are working on a project that has over 100 dependencies. Every time your AWS CodeBuild runs a build step it has to resolve Java dependencies from external Ivy repositories which take a long time. Your manager wants to speed this process up in AWS CodeBuild.
* Use Instance Store type of EC2 instances to facilitate internal dependency cache
* Ship all the dependencies as part of the source code
* Reduce the number of dependencies
* Cache dependencies on S3

### Question 3:
Your AWS CodeDeploy deployment to T2 instances succeed. The new application revision makes API calls to Amazon S3 however the application is not working as expected due to authorization exceptions and you were assigned to troubleshoot the issue.
* Fix the IAM permissions for the CodeDeploy service role
* Make the S3 bucket public
* Fix the IAM permissions for the EC2 instance role
* Enable CodeDeploy Proxy

### Question 4:
A developer is migrating an on-premises application to AWS Cloud. The application currently processes user uploads and uploads them to a local directory on the server. All such file uploads must be saved and then made available to all instances in an Auto Scaling group.
* Use Amazon S3 and make code changes in the application so all uploads are put on S3
* Use Amazon EBS and configure the application AMI to use a snapshot of the same EBS instance while launching new instances
* Use Instance Store type of EC2 instances and share the files via file synchronization software
* Use Amazon EBS as the storage volume and share the files via file synchronization software

### Question 5:
You are a manager for a tech company that has just hired a team of developers to work on the company's AWS infrastructure. All the developers are reporting to you that when using the AWS CLI to execute commands it fails with the following exception: You are not authorized to perform this operation. Encoded authorization failure message: 6h34GtpmGjJJUm946eDVBfzWQJk6z5GePbbGDs9Z2T8xZj9EZtEduSnTbmrR7pMqpJrVYJCew2m8YBZQf4HRWEtrpncANrZMsnzk.
* AWS IAM decode-authorization-message
* Use KMS decode-authorization-message
* AWS STS decode-authorization-message
* AWS Cognito Decoder

### Question 6:
You are getting ready for an event to show off your Alexa skill written in JavaScript. As you are testing your voice activation commands you find that some intents are not invoking as they should and you are struggling to figure out what is happening. You included the following code console.log(JSON.stringify(this.event)) in hopes of getting more details about the request to your Alexa skill.
* Use CloudWatch integration feature with Glue
* Use CloudWatch integration feature with S3
* Use CloudWatch integration feature with Lambda
* Use CloudWatch integration feature with Kinesis

### Question 7:
As a Full-stack Web Developer, you are involved with every aspect of a company’s platform from development with PHP and JavaScript to the configuration of NoSQL databases with Amazon DynamoDB. You are not concerned about your response receiving stale data from your database and need to perform 16 eventually consistent reads per second of 12 KB in size each.
* 12
* 48
* 192
* 24

### Question 8:
Your company manages MySQL databases on EC2 instances to have full control. Applications on other EC2 instances managed by an ASG make requests to these databases to get information that displays data on dashboards viewed on mobile phones, tablets, and web browsers.
* Attach additional Elastic File Storage
* You create a CloudWatch custom metric and build an alarm to scale your ASG
* You enable detailed monitoring and use that to scale your ASG
* Attach an Elastic Load Balancer

### Question 9:
As a site reliability engineer, you are responsible for improving the company’s deployment by scaling and automating applications. As new application versions are ready for production you ensure that the application gets deployed to different sets of EC2 instances at different times allowing for a smooth transition.
* Define multiple CodeDeploy Applications
* CodeDeploy Hooks
* CodeDeploy Agent
* CodeDeploy Deployment Groups

### Question 10:
You have moved your on-premise infrastructure to AWS and are in the process of configuring an AWS Elastic Beanstalk deployment environment for production, development, and testing. You have configured your production environment to use a rolling deployment to prevent your application from becoming unavailable to users. For the development and testing environment, you would like to deploy quickly and are not concerned about downtime.
* Immutable
* Rolling
* All at once
* Rolling with additional batches

### Question 11:
An e-commerce company has implemented AWS CodeDeploy as part of its AWS cloud CI/CD strategy. The company has configured automatic rollbacks while deploying a new version of its flagship application to Amazon EC2.
* A new deployment of the last known working version of the application is deployed with a new deployment ID
* AWS CodePipeline promotes the most recent working deployment with a SUCCEEDED status to production
* The last known working deployment is automatically restored using the snapshot stored in Amazon S3
* CodeDeploy switches the Route 53 alias records back to the known good green deployment and terminates the failed blue deployment

### Question 12:
A communication platform serves millions of customers and deploys features in a production environment on AWS via CodeDeploy. You are reviewing scripts for the deployment process located in the AppSec file.
* ValidateService => BeforeInstall =>DownloadBundle => ApplicationStart
* BeforeInstall => ApplicationStart => DownloadBundle => ValidateService
* BeforeInstall => ValidateService =>DownloadBundle => ApplicationStart
* DownloadBundle => BeforeInstall => ApplicationStart => ValidateService

### Question 13:
After reviewing your monthly AWS bill you notice that the cost of using Amazon SQS has gone up substantially after creating new queues; however, you know that your queue clients do not have a lot of traffic and are receiving empty responses.
* Use a FIFO queue
* Decrease DelaySeconds
* Use LongPolling
* Increase the VisibilityTimeout

### Question 14:
Your company stores confidential data on an Amazon Simple Storage Service (S3) bucket. New security compliance guidelines require that files be stored with server-side encryption. The encryption used must be Advanced Encryption Standard (AES-256) and the company does not want to manage S3 encryption keys.
* SSE-C
* SSE-S3
* Client Side Encryption
* SSE-KMS

### Question 15:
Your mobile application needs to perform API calls to DynamoDB. You do not want to store AWS secret and access keys onto the mobile devices and need all the calls to DynamoDB made with a different identity per mobile device.
* Cognito User Pools
* Cognito Sync
* IAM
* Cognito Identity Pools

### Question 16:
Your development team uses the AWS SDK for Java on a web application that uploads files to several Amazon Simple Storage Service (S3) buckets using the SSE-KMS encryption mechanism. Developers are reporting that they are receiving permission errors when trying to push their objects over HTTP. Which of the following headers should they include in their request?
* 'x-amz-server-side-encryption': 'SSE-KMS'
* 'x-amz-server-side-encryption': 'SSE-S3'
* 'x-amz-server-side-encryption': 'aws:kms'
* 'x-amz-server-side-encryption': 'AES256'

### Question 17:
You have been hired at a company that needs an experienced developer to help with a continuous integration/continuous delivery (CI/CD) workflow on AWS. You configure the company’s workflow to run an AWS CodePipeline pipeline whenever the application’s source code changes in a repository hosted in AWS Code Commit and compiles source code with AWS Code Build. You are configuring ProjectArtifacts in your build stage.
* Contact AWS Support to allow AWS CodePipeline to manage build outputs
* Configure AWS CodeBuild to store output artifacts on EC2 servers
* Give AWS CodeBuild permissions to upload the build output to your Amazon S3 bucket
* Give AWS CodeCommit permissions to upload the build output to your Amazon S3 bucket

### Question 18:
An IT company has a web application running on Amazon EC2 instances that needs read-only access to an Amazon DynamoDB table.
* Create an IAM user with Administrator access and configure AWS credentials for this user on the given EC2 instance
* Run application code with AWS account root user credentials to ensure full access to all AWS services
* Create an IAM role with an AmazonDynamoDBReadOnlyAccess policy and apply it to the EC2 instance profile
* Create a new IAM user with access keys. Attach an inline policy to the IAM user with read-only access to DynamoDB. Place the keys in the code. For security, redeploy the code whenever the keys rotate

### Question 19:
You are working for a technology startup building web and mobile applications. You would like to pull Docker images from the ECR repository called demo so you can start running local tests against the latest application version.
* aws docker push 1234567890.dkr.ecr.eu-west-1.amazonaws.com/demo:latest
* $(aws ecr get-login --no-include-email)
* docker build -t 1234567890.dkr.ecr.eu-west-1.amazonaws.com/demo:latest
* docker pull 1234567890.dkr.ecr.eu-west-1.amazonaws.com/demo:latest
* docker login -u $AWS_ACCESS_KEY_ID -p $AWS_SECRET_ACCESS_KEY

### Question 20:
The development team at a company wants to insert vendor records into an Amazon DynamoDB table as soon as the vendor uploads a new file into an Amazon S3 bucket.
* Develop a Lambda function that will poll the S3 bucket and then insert the records into DynamoDB
* Write a cron job that will execute a Lambda function at a scheduled time and insert the records into DynamoDB
* Create an S3 event to invoke a Lambda function that inserts records into DynamoDB
* Set up an event with Amazon CloudWatch Events that will monitor the S3 bucket and then insert the records into DynamoDB

### Question 21:
A voting system hosted on-premise was recently migrated to AWS to lower cost, gain scalability, and to better serve thousands of concurrent users. When one of the AWS resource state changes, it generates an event and will need to trigger AWS Lambda. The AWS resource whose state changes and AWS Lambda does not have direct integration.
* CloudWatch Events Rules with AWS Lambda
* Cron jobs to trigger AWS Lambda to check the state of your service
* Open a support ticket with AWS
* AWS Lambda Custom Sources

### Question 22:
A firm maintains a highly available application that receives HTTPS traffic from mobile devices and web browsers. The main Developer would like to set up the Load Balancer routing to route traffic from web servers to smart.com/api and from mobile devices to smart.com/mobile. A developer advises that the previous recommendation is not needed and that requests should be sent to api.smart.com and mobile.smart.com instead.
* Web browser version
* Client IP
* Host based
* Path based
* Cookie value

### Question 23:
You manage a group of developers that are experienced with the AWS SDK for Java. You have given them a requirement to build a state machine workflow where each state executes an AWS Lambda function written in Java. Data payloads of 1KB in size will be passed between states and should allow for two retry attempts if the state fails.
* CloudWatch Rules
* AWS Step Functions
* Amazon Simple Workflow Service
* AWS ECS

### Question 24:
A financial services company with over 10,000 employees has hired you as the new Senior Developer. Initially caching was enabled to reduce the number of calls made to all API endpoints and improve the latency of requests to the company’s API Gateway.
* Using the Header Bypass-Cache=1
* Using the Header Cache-Control: max-age=0
* Use the Request parameter: ?bypass_cache=1
* Using the request parameter ?cache-control-max-age=0

### Question 25:
An e-commerce company uses Amazon SQS queues to decouple their application architecture. The development team has observed message processing failures for an edge case scenario when a user places an order for a particular product ID, but the product ID is deleted, thereby causing the application code to fail.
* Use short polling to handle message processing failures
* Use a dead-letter queue to handle message processing failures
* Use long polling to handle message processing failures
* Use a temporary queue to handle message processing failures

### Question 26:
You work as a developer doing contract work for the government on AWS gov cloud. Your applications use Amazon Simple Queue Service (SQS) for its message queue service. Due to recent hacking attempts, security measures have become stricter and require you to store data in encrypted queues.
* Use Secrets Manager
* Use the SSL endpoint
* Use Client side encryption
* Enable SQS KMS encryption

### Question 27:
DevOps engineers are developing an order processing system where notifications are sent to a department whenever an order is placed for a product. The system also pushes identical notifications of the new order to a processing module that would allow EC2 instances to handle the fulfillment of the order. In the case of processing errors, the messages should be allowed to be re-processed at a later stage and never lost.
* SQS + SES
* SNS + SQS
* SNS + Lambda
* SNS + Kinesis

### Question 28:
You are a software engineer working for an IT company and are asked to contribute to a growing internal application that includes dashboards for data visualization. You are provisioning your AWS DynamoDB table and need to perform 10 strongly consistent reads per second of 4 KB in size each.
* 20
* 10
* 5
* 40

### Question 29:
A developer has pushed a Lambda function that pushes data into an RDS MySQL database with the following Python code:
* Upgrade the MySQL instance type
* Change the runtime to Node.js
* Increase the Lambda function RAM
* Move the database connection out of the handler

### Question 30:
An organization uses Alexa as its intelligent assistant to improve productivity throughout the organization. A group of developers manages custom Alexa Skills written in Node.Js to control conference-room equipment settings and start meetings using voice activation. The manager has requested developers that all functions code should be monitored for error rates with the possibility of creating alarms on top of them.
* CloudTrail
* SSM
* X-Ray
* CloudWatch Metrics
* CloudWatch Alarms

### Question 31:
You are designing a high-performance application that requires millions of connections. You have several EC2 instances running Apache2 web servers and the application will require capturing the user’s source IP address and source port without the use of X-Forwarded-For.
* Application Load Balancer
* Network Load Balancer
* Classic Load Balancer
* Elastic Load Balancer

### Question 32:
Your application sends messages to an Amazon Simple Queue Service (SQS) queue frequently, which are then polled by another application that specifies which message to retrieve.
* 20
* 5
* 10
* 100

### Question 33:
A data analytics company with its IT infrastructure on the AWS Cloud wants to build and deploy its flagship application as soon as there are any changes to the source code.
* Keep the source code in Amazon EFS and start AWS CodePipeline whenever a file is updated
* Keep the source code in an Amazon S3 bucket and start AWS CodePipeline whenever a file in the S3 bucket is updated
* Keep the source code in an Amazon EBS volume and start AWS CodePipeline whenever there are updates to the source code
* Keep the source code in an AWS CodeCommit repository and start AWS CodePipeline whenever a change is pushed to the CodeCommit repository
* Keep the source code in an Amazon S3 bucket and set up AWS CodePipeline to recur at an interval of every 15 minutes

### Question 34:
A senior cloud engineer designs and deploys online fraud detection solutions for credit card companies processing millions of transactions daily. The Elastic Beanstalk application sends files to Amazon S3 and then sends a message to an Amazon SQS queue containing the path of the uploaded file in S3. A solution architect recommended that since PUTS of existing objects in S3 deliver eventual consistency and we want to minimize the risk of consumers reading old data, it would be preferable to introduce a per-message lag so that consumers won't find a message in SQS until it has been in the queue for at least 10 seconds.
* Use DelaySeconds parameter
* Implement application-side delay
* Use visibility timeout parameter
* Enable LongPolling

### Question 35:
Your company leverages Amazon CloudFront to provide content via the internet to customers with low latency. Aside from latency, security is another concern and you are looking for help in enforcing end-to-end connections using HTTPS so that content is protected.
* Between clients and CloudFront only
* Neither between clients and CloudFront nor between CloudFront and backend
* Between clients and CloudFront as well as between CloudFront and backend
* Between CloudFront and backend only

### Question 36:
You have a Java-based application running on EC2 instances loaded with AWS CodeDeploy agents. You are considering different options for deployment, one is the flexibility that allows for incremental deployment of your new application versions and replaces existing versions in the EC2 instances. The other option is a strategy in which an Auto Scaling group is used to perform a deployment.
* Cattle Deployment
* Blue/green Deployment
* Warm Standby Deployment
* In-place Deployment
* Pilot Light Deployment

### Question 37:
An IT company uses a blue/green deployment policy to provision new Amazon EC2 instances in an Auto Scaling group behind a new Application Load Balancer for each new application version. The current set up requires the users to log in after every new deployment.
* Use ElastiCache to maintain user sessions
* Use rolling updates instead of a blue/green deployment
* Enable sticky sessions in the Application Load Balancer
* Use multicast to replicate session information

### Question 38:
Your company manages hundreds of EC2 instances running on Linux OS. The instances are configured in several Availability Zones in the eu-west-3 region. Your manager has requested to collect system memory metrics on all EC2 instances using a script.
* Extract RAM statistics using the instance metadata
* Extract RAM statistics from the standard CloudWatch metrics for EC2 instances
* Use a cron job on the instances that pushes the EC2 RAM statistics as a Custom metric into CloudWatch
* Extract RAM statistics using X-Ray

### Question 39:
A firm uses AWS DynamoDB to store information about people’s favorite sports teams and allow the information to be searchable from their home page. There is a daily requirement that all 10 million records in the table should be deleted then re-loaded at 2:00 AM each night.
* Delete then re-create the table
* Call PurgeTable
* Scan and call BatchDeleteItem
* Scan and call DeleteItem

### Question 40:
An analytics company is using Kinesis Data Streams (KDS) to process automobile health-status data from the taxis managed by a taxi ride-hailing service. Multiple consumer applications are using the incoming data streams and the engineers have noticed a performance lag for the data delivery speed between producers and consumers of the data streams.
* Swap out Kinesis Data Streams with Kinesis Data Firehose
* Swap out Kinesis Data Streams with SQS FIFO queues
* Use Enhanced Fanout feature of Kinesis Data Streams
* Swap out Kinesis Data Streams with SQS Standard queues

### Question 41:
Your organization is looking into making a change to all virtual machines in the cloud. They would like to take advantage of running a bootstrap script for their Windows Server 2012 Base AMI virtual machines when they first boot.
* Mount EFS network drives
* EC2 Meta Data
* Custom AMI
* EC2 User Data

### Question 42:
You have a popular web application that accesses data stored in an Amazon Simple Storage Service (S3) bucket. Developers use the SDK to maintain the application and add new features. Security compliance requests that all new objects uploaded to S3 be encrypted using SSE-S3 at the time of upload. Which of the following headers must the developers add to their request?
* 'x-amz-server-side-encryption': 'aws:kms'
* 'x-amz-server-side-encryption': 'AES256'
* 'x-amz-server-side-encryption': 'SSE-S3'
* 'x-amz-server-side-encryption': 'SSE-KMS'

### Question 43:
An organization recently began using AWS CodeCommit for its source control service. A compliance security team visiting the organization was auditing the software development process and noticed developers making many git push commands within their development machines. The compliance team requires that encryption be used for this activity.
* Repositories are automatically encrypted at rest
* Use AWS Lambda as a hook to encrypt the pushed code
* Enable KMS encryption
* Use a git command line hook to encrypt the code client side

### Question 44:
A company has configured an Auto Scaling group with health checks. The configuration is set to the desired capacity value of 3 and maximum capacity value of 3. The EC2 instances of your Auto Scaling group are configured to scale when CPU utilization is at 60 percent and is now running at 80 percent utilization.
* The desired capacity will go up to 4 and the maximum capacity will also go up to 4
* System will trigger CloudWatch alarms to AWS support
* System will keep running as is
* The desired capacity will go up to 4 and the maximum capacity will stay at 3

### Question 45:
As part of internal regulations, you must ensure that all communications to Amazon S3 are encrypted.
* SSE-S3
* SSE-KMS
* SSE-C
* Client Side Encryption

### Question 46:
An IT company is using AWS CloudFormation to manage its IT infrastructure. It has created a template to provision a stack with a VPC and a subnet. The output value of this subnet has to be used in another stack.
* Use Fn::ImportValue
* Use 'Export' field in the Output section of the stack's template
* Use 'Expose' field in the Output section of the stack's template
* Use Fn::Transform

### Question 47:
Your company is in the process of building a DevOps culture and is moving all of its on-premise resources to the cloud using serverless architectures and automated deployments. You have created a CloudFormation template in YAML that uses an AWS Lambda function to pull HTML files from GitHub and place them into an Amazon Simple Storage Service (S3) bucket that you specify.
* cloudformation zip and cloudformation upload
* cloudformation package and cloudformation deploy
* cloudformation package and cloudformation upload
* cloudformation zip and cloudformation deploy

### Question 48:
You're a developer maintaining a web application written in .NET. The application makes references to public objects in a public S3 accessible bucket using a public URL. While doing a code review your colleague advises that the approach is not a best practice because some of the objects contain private data. After the administrator makes the S3 bucket private you can no longer access the S3 objects but you would like to create an application that will enable people to access some objects as needed with a time policy constraint.
* Using Routing Policy
* Using IAM policy
* Using pre-signed URL
* Using bucket policy

### Question 49:
You are planning to build a fleet of EBS-optimized EC2 instances to handle the load of your new application. Due to security compliance, your organization wants any secret strings used in the application to be encrypted to prevent exposing values as clear text.
* Encrypt first with KMS then store in SSM Parameter store
* Audit using SSM Audit Trail
* Store the secret as PlainText in SSM Parameter Store
* Store the secret as SecureString in SSM Parameter Store
* Audit using CloudTrail

### Question 50:
You have a popular three-tier web application that is used by users throughout the globe receiving thousands of incoming requests daily. You have AWS Route 53 policies to automatically distribute weighted traffic to the API resources located at URL api.global.com.
* Auto Scaling
* ELB
* S3
* CloudFront

### Question 51:
You have an Amazon Kinesis Data Stream with 10 shards, and from the metrics, you are well below the throughput utilization of 10 MB per second to send data. You send 3 MB per second of data and yet you are receiving ProvisionedThroughputExceededException errors frequently.
* The partition key that you have selected isn't distributed enough
* The data retention period is too long
* Metrics are slow to update
* You have too many shards

### Question 52:
A development team has inherited a web application running in the us-east-1 region with three availability zones (us-east-1a, us-east1-b, and us-east-1c) whose incoming web traffic is routed by a load balancer. When one of the EC2 instances hosting the web application crashes, the team realizes that the load balancer continues to route traffic to that instance causing intermittent issues.
* Enable SSL
* Enable Multi AZ deployments
* Enable Health Checks
* Enable Stickiness

### Question 53:
A .NET developer team works with many ASP.NET web applications that use EC2 instances to host them on IIS. The deployment process needs to be configured so that multiple versions of the application can run in AWS Elastic Beanstalk. One version would be used for development, testing, and another version for load testing.
* Use only one Beanstalk environment and perform configuration changes using an Ansible script
* You cannot have multiple development environments in Elastic Beanstalk, just one development and one production environment
* Create an Application Load Balancer to route based on hostname so you can pass on parameters to the development Elastic Beanstalk environment. Create a file in .ebextensions/ to know how to handle the traffic coming from the ALB
* Define a dev environment with a single instance and a 'load test' environment that has settings close to production environment

### Question 54:
You are assigned as the new project lead for a web application that processes orders for customers. You want to integrate event-driven processing anytime data is modified or deleted and use a serverless approach using AWS Lambda for processing stream events.
* RDS
* Kinesis
* DynamoDB
* ElastiCache

### Question 55:
As a site reliability engineer, you work on building and running large-scale, distributed, fault-tolerant systems in the cloud using automation. You have just replaced the company's Jenkins based CI/CD platform with AWS CodeBuild and would like to programmatically define your build steps.
* Define a buildspec.yml file in the codebuild/ directory
* Define an appspec.yml file in the root directory
* Define a buildspec.yml file in the root directory
* Define an appspec.yml file in the codebuild/ directory

### Question 56:
You have a web application hosted on EC2 that makes GET and PUT requests for objects stored in Amazon Simple Storage Service (S3) using the SDK for PHP. As the security team completed the final review of your application for vulnerabilities, they noticed that your application uses hardcoded IAM access key and secret access key to gain access to AWS services. They recommend you leverage a more secure setup, which should use temporary credentials if possible.
* Use an IAM Instance Role
* Hardcode the credentials in the application code
* Use environment variables
* Use the SSM parameter store

### Question 57:
You are storing your video files in a separate S3 bucket than your main static website in an S3 bucket. When accessing the video URLs directly the users can view the videos on the browser, but they can't play the videos while visiting the main website.
* Amend the IAM policy
* Disable Server-Side Encryption
* Change the bucket policy
* Enable CORS

### Question 58:
A cybersecurity company is publishing critical log data to a log group in Amazon CloudWatch Logs, which was created 3 months ago. The company must encrypt the log data using an AWS KMS customer master key (CMK), so any future data can be encrypted to meet the company’s security guidelines.
* Use the AWS CLI create-log-group command and specify the KMS key ARN
* Enable the encrypt feature on the log group via the CloudWatch Logs console
* Use the AWS CLI describe-log-groups command and specify the KMS key ARN
* Use the AWS CLI associate-kms-key command and specify the KMS key ARN

### Question 59:
You are revising options that would be best for monitoring a few EC2 instances you currently manage. Amazon CloudWatch has metrics available to monitor your EC2 instances for CPU load, I/O, and network I/O. Your budget does not allow for spending on monitoring so using the default monitoring available is your preferred choice.
* 2 minutes
* 5 minutes
* 10 minutes
* 1 minute

### Question 60:
You are a system administrator whose company recently moved its production application to AWS and migrated data from MySQL to AWS DynamoDB. You are adding new tables to AWS DynamoDB and need to allow your application to query your data by the primary key and an alternate key. This option must be added when first creating tables otherwise changes cannot be made afterward.
* Call Scan
* Create a LSI
* Migrate away from DynamoDB
* Create a GSI

### Question 61:
You have uploaded a zip file to AWS Lambda that contains code files written in Node.Js. When your function is executed you receive the following output, 'Error: Memory Size: 3008 MB Max Memory Used'.
* Your Lambda function ran out of RAM
* Your zip file is corrupt
* The uncompressed zip file exceeds AWS Lambda limits
* You have uploaded a zip file larger than 50 MB to AWS Lambda

### Question 62:
A development team uses the AWS SDK for Java to maintain an application that stores data in AWS DynamoDB. The application makes use of Scan operations to return several items from a 25 GB table. There is no possibility of creating indexes to retrieve these items predictably. Developers are trying to get these specific rows from DynamoDB as fast as possible.
* Use a Query
* Use a ProjectionExpression
* Use parallel scans
* Use a FilterExpression

### Question 63:
A company developed an app-based service for citizens to book transportation rides in the local community. The platform is running on AWS EC2 instances and uses Amazon Relational Database Service (RDS) for storing transportation data. A new feature has been requested where receipts would be emailed to customers with PDF attachments retrieved from Amazon Simple Storage Service (S3).
* Run aws configure on the EC2 instance
* EC2 User Data
* CloudFormation
* Create an IAM Role for EC2

### Question 64:
A media company is building an application that needs to store video files in Amazon S3. Management requires that the files be encrypted before they are sent to Amazon S3 for storage. The encryption keys need to be managed by an in-house security team but the key itself is stored on AWS.
* Use server-side encryption with a client-side master key
* Use client-side encryption with Amazon S3 managed key
* Use server-side encryption with customer-provided encryption key (SSE-C)
* Use client-side encryption with an AWS KMS managed customer master key (CMK)

### Question 65:
Your company has a load balancer in a VPC configured to be internet facing. The public DNS name assigned to the load balancer is myDns-1234567890.us-east-1.elb.amazonaws.com. When your client applications first load they capture the load balancer DNS name and then resolve the IP address for the load balancer so that they can directly reference the underlying IP.
* The load balancer is highly available and its public IP may change. The DNS name is constant
* You need to enable stickiness
* Your security groups are not stable
* You need to disable multi-AZ deployments

# Exam 5

### Question 1:
A financial services company has developed a REST API which is deployed in an Auto Scaling Group behind an Application Load Balancer. The API stores the data payload in DynamoDB and the static content is served through S3. Upon analyzing the usage pattern, it's found that 80% of the read requests are shared across all users.
* Enable DAX for DynamoDB and ElastiCache Memcached for S3
* Enable DynamoDB Accelerator (DAX) for DynamoDB and CloudFront for S3
* Enable ElastiCache Redis for DynamoDB and CloudFront for S3
* Enable ElastiCache Redis for DynamoDB and ElastiCache Memcached for S3

### Question 2:
Your client has tasked you with finding a service that would enable you to get cross-account tracing and visualization.
* CloudTrail
* AWS X-Ray
* CloudWatch Events
* VPC Flow Logs

### Question 3:
You would like to have a one-stop dashboard for all the CI/CD needs of one of your projects. You don't need heavy control of the individual configuration of each component in your CI/CD, but need to be able to get a holistic view of your projects.
* CodeStar
* CodeDeploy
* CodeBuild
* CodePipeline

### Question 4:
Your company is new to cloud computing and would like to host a static HTML5 website on the cloud and be able to access it via domain www.mycompany.com. You have created a bucket in Amazon Simple Storage Service (S3), enabled website hosting, and set the index.html as the default page. Finally, you create an Alias record in Amazon Route 53 that points to the S3 website endpoint of your S3 bucket.
* Create an IAM role
* Create a bucket policy
* Enable CORS
* Enable Encryption

### Question 5:
Your AWS account is now growing to 200 users and you would like to provide each of these users a personal space in the S3 bucket 'my_company_space' with the prefix /home/<username>, where they have read/write access.
* Create one customer-managed policy per user and attach them to the relevant users
* Create an S3 bucket policy and change it as users are added and removed
* Create one customer-managed policy with policy variables and attach it to a group of all users
* Create inline policies for each user as they are onboarded

### Question 6:
You are a developer working on AWS Lambda functions that are triggered by Amazon API Gateway and would like to perform testing on a low volume of traffic for new API versions.
* Custom Authorizers
* Stage Variables
* Mapping Templates
* Canary Deployment

### Question 7:
Applications running on EC2 instances process messages from an SQS queue but sometimes they experience errors due to messages not being processed.
* Implement a Dead Letter Queue
* Increase the VisibilityTimeout
* Reduce the VisibilityTimeout
* Use DeleteMessage

### Question 8:
Your company likes to operate multiple AWS accounts so that teams have their environments. Services deployed across these accounts interact with one another, and now there's a requirement to implement X-Ray traces across all your applications deployed on EC2 instances and AWS accounts.
* Configure the X-Ray daemon to use an IAM instance role
* Enable Cross Account collection in the X-Ray console
* Configure the X-Ray daemon to use access and secret keys
* Create a user in the target unified account and generate access and secret keys
* Create a role in the target unified account and allow roles in each sub-account to assume the role.

### Question 9:
A security company is requiring all developers to perform server-side encryption with customer-provided encryption keys when performing operations in AWS S3. Developers should write software with C# using the AWS SDK and implement the requirement in the PUT, GET, Head, and Copy operations.
* SSE-S3
* Client-Side Encryption
* SSE-C
* SSE-KMS

### Question 10:
You are looking to invoke an AWS Lambda function every hour (similar to a cron job) in a serverless way.
* CloudWatch Events
* SQS
* Kinesis
* Amazon S3

### Question 11:
Your company has developers worldwide with access to the company's Amazon Simple Storage Service (S3) buckets. The objects in the buckets are encrypted at the server-side but need more flexibility with access control, auditing, rotation, and deletion of keys. You would also like to limit who can use the key.
* SSE-C
* SSE-S3
* Client Side Encryption
* SSE-KMS

### Question 12:
You would like to paginate the results of an S3 List to show 100 results per page to your users and minimize the number of API calls that you will use.
* --page-size
* --starting-token
* --next-token
* --max-items
* --limit

### Question 13:
You are running a video website and provide users with S3 pre-signed URLs allowing your users to securely upload their video content onto your buckets. The average file size uploaded to your buckets is 500MB and you would like your users to efficiently send the content.
* Use SSE-S3 encryption
* Upload as one part
* Zip the video file before sending
* Do a multi-part upload

### Question 14:
Your web application front end consists of 5 EC2 instances behind an Application Load Balancer. You have configured your web application to capture the IP address of the client making requests. When viewing the data captured you notice that every IP address being captured is the same, which also happens to be the IP address of the Application Load Balancer.
* Look into the X-Forwarded-Proto header in the backend
* Look into the client's cookie
* Modify the front-end of the website so that the users send their IP in the requests
* Look into the X-Forwarded-For header in the backend

### Question 15:
Your Lambda function must use the Node.js drivers to connect to your RDS PostgreSQL database in your VPC.
* Put the function and the dependencies in one folder and zip them together
* Zip the function and the dependencies separately and upload them in AWS Lambda as two parts
* Upload the code through the AWS console and upload the dependencies as a zip
* Zip the function as-is with a package.json file so that AWS Lambda can resolve the dependencies for you

### Question 16:
You've just deployed an AWS Lambda function. The lambda function will be invoked via the API Gateway. The API Gateway will need to control access to it.
* Lambda Authorizer
* IAM permissions with sigv4
* STS
* Cognito User Pools

### Question 17:
You are running a web application where users can author blogs and share them with their followers. Most of the workflow is read based, but when a blog is updated, you would like to ensure that the latest data is served to the users (no stale data). The Developer has already suggested using ElastiCache to cope with the read load but has asked you to implement a caching strategy that complies with the requirements of the site.
* Use a Lazy Loading strategy with TTL
* Use DAX
* Use a Write Through strategy
* Use a Lazy Loading strategy without TTL

### Question 18:
You are working for a small organization that does not have a database administrator and the organization needs to install a database on the cloud quickly to support an accounting application used by thousands of users. The application will act as a backend and will perform (CRUD) operations such as create, read, update and delete as well as inner joins.
* DynamoDB
* ElastiCache
* Redshift
* RDS

### Question 19:
Your organization has a single Amazon Simple Storage Service (S3) bucket that contains folders labeled with customer names. Several administrators have IAM access to the S3 bucket and versioning is enabled to easily recover from unintended user actions.
* Versioning can be enabled only for a specific folder
* Overwriting a file increases its versions
* Any file that was unversioned before enabling versioning will have the 'null' version
* Deleting a file is a recoverable operation

### Question 20:
Which of the following CLI options will allow you to retrieve a subset of the attributes coming from a DynamoDB scan?
* --projection-expression
* --page-size
* --max-items
* --filter-expression

### Question 21:
Your Lambda function processes files for your customers and as part of that process, it creates a lot of intermediary files it needs to store on its disk and then discard.
* Use an S3 bucket
* Use the local directory /tmp
* Create a tmp/ directory in the source zip file and use it
* Use the local directory /opt

### Question 22:
You are deploying Lambda functions that operate on your S3 buckets to read files and extract key metadata. The Lambda functions are managed using SAM.
* S3ReadPolicy
* S3CrudPolicy
* LambdaInvokePolicy
* SQSPollerPolicy

### Question 23:
When your company first created an AWS account, you began with a single sign-in principal called a root user account that had complete access to all AWS services and resources.
* It should be accessible by one admin only after enabling Multi-factor authentication
* It should be accessible by no one, throw away the passwords after creating the account
* It should be accessible by 3 to 6 members of the IT team
* It should be accessible using the access key id and secret access key

### Question 24:
A popular mobile app retrieves data from an AWS DynamoDB table that was provisioned with read-capacity units (RCU’s) that are evenly shared across four partitions. One of those partitions is receiving more traffic than the other partitions, causing hot partition issues.
* More partitions
* DynamoDB DAX
* ElastiCache
* DynamoDB Streams

### Question 25:
Your team has just signed up an year-long contract with a client maintaining a three-tier web application, that needs to be moved to AWS Cloud. The application has steady traffic throughout the day and needs to be on a reliable system with no down-time or access issues. The solution needs to be cost-optimal for this startup.
* Amazon EC2 On Demand Instances
* Amazon EC2 Spot Instances
* Amazon EC2 Reserved Instances
* On-premise EC2 instance

### Question 26:
You are using AWS SQS FIFO queues to get the ordering of messages on a per user_id basis. On top of this, you would like to make sure that duplicate messages should not be sent to SQS as this would cause application failure.
* MessageDeduplicationId
* ReceiveRequestAttemptId
* ContentBasedDeduplication
* MessageGroupId

### Question 27:
You are storing bids information on your betting application and you would like to automatically expire DynamoDB table data after one week.
* Use DynamoDB Streams
* Use a Lambda function
* Use TTL
* Use DAX

### Question 28:
Your company is shifting towards Elastic Container Service (ECS) to deploy applications. The process should be automated using the AWS CLI to create a service where at least ten instances of a task definition are kept running under the default cluster.
* aws ecr create-service --service-name ecs-simple-service --task-definition ecs-demo --desired-count 10
* aws ecs run-task --cluster default --task-definition ecs-demo
* aws ecs create-service --service-name ecs-simple-service --task-definition ecs-demo --desired-count 10
* docker-compose create ecs-simple-service

### Question 29:
You have created a test environment in Elastic Beanstalk and as part of that environment, you have created an RDS database.
* Convert the Elastic Beanstalk environment to a worker environment
* Change the Elastic Beanstalk environment variables
* Make a selective delete in Elastic Beanstalk
* Make a snapshot of the database before it gets deleted

### Question 30:
You are using AWS SQS FIFO queues to get the ordering of messages on a per user_id basis.
* MessageGroupId
* MessageOrderId
* MessageDeduplicationId
* MessageHash

### Question 31:
You were assigned to a project that requires the use of the AWS CLI to build a project with AWS CodeBuild. Your project's root directory includes the buildspec.yml file to run build commands and would like your build artifacts to be automatically encrypted at the end.
* Use In Flight encryption (SSL)
* Use the AWS Encryption SDK
* Specify a KMS key to use
* Use an AWS Lambda Hook

### Question 32:
You would like to deploy a Lambda function globally so that requests are filtered at the AWS edge locations.
* Use a Lambda@Edge
* Deploy Lambda in a Global VPC
* Use a Global DynamoDB table as a Lambda source
* Deploy Lambda in S3

### Question 33:
As part of your video processing application, you are looking to perform a set of repetitive and scheduled tasks asynchronously. Your application is deployed on Elastic Beanstalk.
* Setup a Worker environment and a cron.yaml file
* Setup a Worker environment and a .ebextensions file
* Setup a Web Server environment and a .ebextensions file
* Setup a Web Server environment and a cron.yaml file

### Question 34:
You are creating a web application in which users can follow each other. Some users will be more popular than others and thus their data will be requested very often. Currently, the user data sits in RDS and it has been recommended by your Developer to use ElastiCache as a caching layer to improve the read performance. The whole dataset of users cannot sit in ElastiCache without incurring tremendous costs and therefore you would like to cache only the most often requested users profiles there. As your website is high traffic, it is accepted to have stale data for users for a while, as long as the stale data is less than a minute old.
* Use a Write Through strategy without TTL
* Use a Lazy Loading strategy with TTL
* Use a Lazy Loading strategy without TTL
* Use a Write Through strategy with TTL

### Question 35:
Your e-commerce company needs to improve its software delivery process and is moving away from the waterfall methodology. You decided that every application should be built using the best CI/CD practices and every application should be packaged and deployed as a Docker container. The Docker images should be stored in ECR and pushed with AWS CodePipeline and AWS CodeBuild.
* The ECR repository is stale, you must delete and re-create it
* The IAM permissions are wrong for the CodeBuild service
* The ECS instances are misconfigured and must contain additional data in /etc/ecs/ecs.config
* CodeBuild cannot talk to ECR because of security group issues

### Question 36:
You would like your Elastic Beanstalk environment to expose an HTTPS endpoint instead of an HTTP endpoint to get in-flight encryption between your clients and your web servers.
* Use a separate CloudFormation template to load the SSL certificate onto the Load Balancer
* Open up the port 80 for the security group
* Create an .ebextensions file to configure the Load Balancer
* Configure Health Checks

### Question 37:
You have been collecting AWS X-Ray traces across multiple applications and you would now like to index your XRay traces to search and filter through them efficiently.
* Segments
* Annotations
* Metadata
* Sampling

### Question 38:
You are a cloud security engineer working for a popular cyber-forensics company that offers vulnerability scanning solutions to government contractors. The scanning solutions are integrated with AWS resources to monitor EC2 and S3 API calls which then display results to users on an analytical dashboard.
* S3 Access Logs
* VPC Flow Logs
* CloudTrail
* IAM

### Question 39:
You would like your Elastic Beanstalk environment to expose an HTTPS endpoint and an HTTP endpoint. The HTTPS endpoint should be used to get in-flight encryption between your clients and your web servers, while the HTTP endpoint should only be used to redirect traffic to HTTPS and support URLs starting with http://.
* Open up port 80 & port 443
* Only open up port 443
* Configure your EC2 instances to redirect HTTP traffic to HTTPS
* Configure your EC2 instances to redirect HTTPS traffic to HTTP
* Assign an SSL certificate to the Load Balancer
* Only open up port 80

### Question 40:
You are a DynamoDB developer for an aerospace company that requires you to write 6 objects per second of 4.5KB in size each.
* 15
* 24
* 46
* 30

### Question 41:
A development team has a mix of applications hosted on-premises as well as on EC2 instances. The on-premises application controls all applications deployed on the EC2 instances. In case of any errors, the team wants to leverage Amazon CloudWatch to monitor and troubleshoot the on-premises application.
* Upload log files from the on-premises server to S3 and let CloudWatch process the files from S3
* Configure CloudWatch Logs to directly read the logs from the on-premises server
* Upload log files from the on-premises server to an EC2 instance which further forwards the logs to CloudWatch
* Configure the CloudWatch agent on the on-premises server by using IAM user credentials with permissions for CloudWatch

### Question 42:
A developer created an online shopping application that runs on EC2 instances behind load balancers. The same web application version is hosted on several EC2 instances and the instances run in an Auto Scaling group. The application uses STS to request credentials but after an hour your application stops working.
* A lambda function revokes your access every hour
* Your IAM policy is wrong
* The IAM service is experiencing downtime once an hour
* Your application needs to renew the credentials after 1 hour when they expire

### Question 43:
A development team has created AWS CloudFormation templates that are reusable by taking advantage of input parameters to name resources based on client names.
* EBS
* EFS
* ECR
* S3

### Question 44:
You have created a DynamoDB table to support your application and provisioned RCU and WCU to it so that your application has been running for over a year now without any throttling issues. Your application now requires a second type of query over your table and as such, you have decided to create an LSI and a GSI on a new table to support that use case. One month after having implemented such indexes, it seems your table is experiencing throttling.
* The GSI is throttling so you need to provision more RCU and WCU to the GSI
* Metrics are lagging in your CloudWatch dashboard and you should see the RCU and WCU peaking for the main table in a few minutes
* Adding both an LSI and a GSI to a table is not recommended by AWS best practices as this is a known cause for creating throttles
* The LSI is throttling so you need to provision more RCU and WCU to the LSI

### Question 45:
You would like to retrieve a subset of your dataset stored in S3 with the CSV format. You would like to retrieve a month of data and only 3 columns out of the 10.
* S3 Analytics
* S3 Inventory
* S3 Access Logs
* S3 Select

### Question 46:
Your client wants to deploy a service on EC2 instances, and as EC2 instances are added into an ASG, each EC2 instance should be running 3 different Docker Containers simultaneously.
* Third-party platform
* Custom platform
* Docker multi-container platform
* Docker single-container platform

### Question 47:
An IT company leverages CodePipeline to automate its release pipelines. The development team wants to write a Lambda function that will send notifications for state changes within the pipeline.
* Set up an Amazon CloudWatch alarm that monitors status changes in Code Pipeline and triggers the Lambda function
* Set up an Amazon CloudWatch Events rule that uses CodePipeline as an event source with the target as the Lambda function
* Use the Lambda console to configure a trigger that invokes the Lambda function with CodePipeline as the event source
* Use the CodePipeline console to set up a trigger for the Lambda function

### Question 48:
A data analytics company ingests a large number of messages and stores them in an RDS database using Lambda. Because of the increased payload size, it is taking more than 15 minutes to process each message.
* Use DynamoDB instead of RDS as database
* Provision EC2 instances in an Auto Scaling group to poll the messages from an SQS queue
* Provision an EC2 instance to poll the messages from an SQS queue
* Contact AWS Support to increase the Lambda timeout to 60 minutes

### Question 49:
You would like to run the X-Ray daemon for your Docker containers deployed using AWS Fargate.
* Deploy the X-Ray daemon agent as a process on your EC2 instance
* Deploy the X-Ray daemon agent as a sidecar container
* Provide the correct IAM task role to the X-Ray container
* Provide the correct IAM instance role to the EC2 instance
* Deploy the X-Ray daemon agent as a daemon set on ECS

### Question 50:
A media analytics company has built a streaming application on Lambda using Serverless Application Model (SAM).
* Develop the SAM template locally => upload the template to Lambda => deploy your application to the cloud
* Develop the SAM template locally => upload the template to CodeCommit => deploy your application to CodeDeploy
* Develop the SAM template locally => deploy the template to S3 => use your application in the cloud
* Develop the SAM template locally => upload the template to S3 => deploy your application to the cloud

### Question 51:
You are responsible for an application that runs on multiple Amazon EC2 instances. In front of the instances is an Internet-facing load balancer that takes requests from clients over the internet and distributes them to the EC2 instances. A health check is configured to ping the index.html page found in the root directory for the health status. When accessing the website via the internet visitors of the website receive timeout errors.
* IAM Roles
* The ALB is warming up
* Security Groups
* The application is down

### Question 52:
You are running a public DNS service on an EC2 instance where the DNS name is pointing to the IP address of the instance. You wish to upgrade your DNS service but would like to do it without any downtime.
* Use Route 53
* Elastic IP
* Provide a static private IP
* Create a Load Balancer and an auto scaling group

### Question 53:
Your company wants to move away from manually managing Lambda in the AWS console and wants to upload and update them using AWS CloudFormation.
* Write the AWS Lambda code inline in CloudFormation in the AWS::Lambda::Function block and reference the dependencies as a zip file stored in S3
* Upload all the code as a folder to S3 and refer the folder in AWS::Lambda::Function block
* Upload all the code as a zip to S3 and refer the object in AWS::Lambda::Function block
* Write the AWS Lambda code inline in CloudFormation in the AWS::Lambda::Function block as long as there are no third-party dependencies
* Upload all the code to CodeCommit and refer to the CodeCommit Repository in AWS::Lambda::Function block

### Question 54:
A media company wants to migrate a video editing service to Amazon EC2 while following security best practices. The videos are sourced and read from a non-public S3 bucket.
* Set up an EC2 service role with read-only permissions for the S3 bucket and attach the role to the EC2 instance profile
* Set up an IAM user with read-only permissions for the S3 bucket. Configure AWS credentials for this user via AWS CLI on the EC2 instance
* Set up an S3 service role with read-only permissions for the S3 bucket and attach the role to the EC2 instance profile
* Set up an IAM user with read-only permissions for the S3 bucket. Configure the IAM user credentials in the user data of the EC2 instance

### Question 55:
Your organization has set up a full CI/CD pipeline leveraging CodePipeline and the deployment is done on Elastic Beanstalk. This pipeline has worked for over a year now but you are approaching the limits of Elastic Beanstalk in terms of how many versions can be stored in the service.
* Setup an .ebextensions file
* Use a Lifecycle Policy
* Define a Lambda function
* Use Worker Environments

### Question 56:
Your team lead has finished creating a CodeBuild project in the management console and a build spec has been defined for the project. After the build is run, CodeBuild fails to pull a Docker image into the build environment.
* The Docker image is too big
* CodeBuild cannot work with custom Docker images
* Missing IAM permissions for the CodeBuild Service
* The Docker image is missing some tags

### Question 57:
Your development team has created a popular mobile app written for Android. The team is looking for a technology that can send messages to mobile devices using a mobile app.
* SQS
* SES
* Kinesis
* SNS

### Question 58:
One of your Kinesis Stream is experiencing increased traffic due to a sale day. Therefore your Kinesis Administrator has split shards and thus you went from having 6 shards to having 10 shards in your Kinesis Stream. Your consuming application is running a KCL-based application on EC2 instances.
* 1
* 6
* 10
* 20

### Question 59:
Which environment variable can be used by AWS X-Ray SDK to ensure that the daemon is correctly discovered on ECS?
* AWS_XRAY_DEBUG_MODE
* AWS_XRAY_CONTEXT_MISSING
* AWS_XRAY_DAEMON_ADDRESS
* AWS_XRAY_TRACING_NAME

### Question 60:
The development team at an e-commerce company is preparing for the upcoming Thanksgiving sale. The product manager wants the development team to implement appropriate caching strategy on Amazon ElastiCache to withstand traffic spikes on the website during the sale. A key requirement is to facilitate consistent updates to the product prices and product description, so that the cache never goes out of sync with the backend.
* Use a caching strategy to write to the cache directly and sync the backend at a later time
* Use a caching strategy to write to the backend first and wait for the cache to expire via TTL
* Use a caching strategy to write to the backend first and then invalidate the cache
* Use a caching strategy to update the cache and the backend at the same time

### Question 61:
You are working with a t2.small instance bastion host that has the AWS CLI installed to help manage all the AWS services installed on it. You would like to know the security group and the instance id of the current instance.
* Create an IAM role and attach it to your EC2 instance that helps you perform a 'describe' API call
* Query the user data at http://169.254.169.254/latest/user-data
* Query the metadata at http://169.254.169.254/latest/meta-data
* Query the user data at http://254.169.254.169/latest/meta-data

### Question 62:
You are implementing a banking application in which you need to update the Exchanges DynamoDB table and the AccountBalance DynamoDB table at the same time or not at all.
* DynamoDB Streams
* DynamoDB Transactions
* DynamoDB TTL
* DynamoDB Indexes

### Question 63:
You need to load SSL certificates onto your Load Balancers and also have EC2 instances dynamically retrieve them when needed for service to service two-way TLS communication.
* ACM
* KMS
* S3
* IAM

### Question 64:
An EC2 instance has an IAM instance role attached to it, providing it read and write access to the S3 bucket 'my_bucket'. You have tested the IAM instance role and both reads and writes are working. You then remove the IAM role from the EC2 instance and test both read and write again. Writes stopped working but reads are still working.
* When a read is done on a bucket, there's a grace period of 5 minutes to do the same read again
* Removing an instance role from an EC2 instance can take a few minutes before being active
* The EC2 instance is using cached temporary IAM credentials
* The S3 bucket policy authorizes reads

### Question 65:
An IT company uses AWS CloudFormation templates to provision their AWS infrastructure for Amazon EC2, Amazon VPC, and Amazon S3 resources. Using cross-stack referencing, a developer creates a stack called NetworkStack which will export the subnetId that can be used when creating EC2 instances in another stack.
* !Ref
* !ImportValue
* !Sub
* !GetAtt




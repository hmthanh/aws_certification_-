# AWS Certified Solutions Architect Professional

# Exam 1

### Question 1:
A global biomedicine company has built a Genomics Solution on AWS Cloud to advance neurological disease research and identify potential new disease therapies, find new gene targets and better understand neurological disease biology. The company's labs generate hundreds of terabytes of research data daily. To further accelerate the innovation process, the engineering team at the company wants to move most of the on-premises data into Amazon S3, Amazon EFS, and Amazon FSx for Windows File Server easily, quickly, and cost-effectively. The team would like to automate and accelerate online data transfers to these AWS storage services.
* Use AWS Snowball Edge Storage Optimized device to automate and accelerate online data transfers to the given AWS storage services
* Use AWS DataSync to automate and accelerate online data transfers to the given AWS storage services
* Use File Gateway to automate and accelerate online data transfers to the given AWS storage services
* Use AWS Transfer Family to automate and accelerate online data transfers to the given AWS storage services

### Question 2:
A global healthcare company wants to develop a solution called Health Information Systems (HIS) on AWS Cloud that would allow the providers, payers, and government agencies to collaborate, anticipate and navigate the changing healthcare landscape. While pursuing this endeavor, the company would like to decrease its IT operational overhead so it could focus more intently on its core business - healthcare analytics. The solution should help the company eliminate the bottleneck created by manual provisioning of development pipelines while adhering to crucial governance and control requirements. As a means to this end, the company has set up "AWS Organizations" to manage several of these scenarios and would like to use Service Control Policies (SCP) for central control over the maximum available permissions for the various accounts in their organization. This allows the organization to ensure that all accounts stay within the organization’s access control guidelines.
* SCPs affect all users and roles in attached accounts, excluding the root user
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can't perform that action
* SCPs do not affect service-linked role
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can still perform that action
* SCPs affect service-linked roles
* SCPs affect all users and roles in attached accounts, including the root user

### Question 3:
A retail company has hired you as an AWS Certified Solutions Architect Professional to provide consultancy for managing a serverless application that consists of multiple API gateways, Lambda functions, S3 buckets and DynamoDB tables. The company is getting reports from customers that some of the application components seem to be lagging while loading dynamic images and some are timing out with the "504 Gateway Timeout" error. As part of your investigations to identify the root cause behind this issue, you can confirm that DynamoDB monitoring metrics are at acceptable levels.
* Enable execution logging for the API Gateway. Process and analyze the execution logs in the API Gateway for HTTP errors to determine the root cause of the errors
* Process and analyze the VPC Flow Logs to determine if there is packet loss between the Lambda function and S3
* Process and analyze the AWS X-Ray traces and analyze HTTP methods to determine the root cause of the HTTP errors
* Enable access logging for the API Gateway. Process and analyze the access logs in the API Gateway for HTTP errors to determine the root cause of the errors
* Process and analyze the Amazon CloudWatch Logs for Lambda function to determine processing times for requested images at pre-configured intervals

### Question 4:
The DevOps team for a CRM SaaS company wants to implement a patching plan on AWS Cloud for a large mixed fleet of Windows and Linux servers. The patching plan has to be auditable and must be implemented securely to ensure compliance with the company's business requirements.
* Set up an OS-native patching service to manage the update frequency and release approval for all instances. Set up AWS Config to provide audit and compliance reporting
* Configure OpsWorks automatic patching support for all applications which will keep the OS up-to-date following the initial installation. Set up AWS Config to provide audit and compliance reporting
* Apply patch baselines using the AWS-ApplyPatchBaseline SSM document
* Set up Systems Manager Agent on all instances to manage patching. Test patches in pre-production and then deploy as a maintenance window task with the appropriate approval
* Apply patch baselines using the AWS-RunPatchBaseline SSM document

### Question 5:
A leading club in the Major League Baseball runs a web platform that boasts over 50,000 pages and over 100 million digitized photographs. It is available in six languages and maintains up-to-date information for the season. The engineering team has built a notification system on the web platform using SNS notifications which are then handled by a Lambda function for end-user delivery. During the off-season, the notification systems need to handle about 100 requests per second. During the peak baseball season, the rate touches about 5000 requests per second and it is noticed that a significant number of the notifications are not being delivered to the end-users on the web platform.
* The engineering team needs to provision more servers running the SNS service
* Amazon SNS has hit a concurrency limit, so the team needs to contact AWS support to raise the account limit
* The engineering team needs to provision more servers running the Lambda service
* Amazon SNS message deliveries to AWS Lambda have crossed the account concurrency quota for Lambda, so the team needs to contact AWS support to raise the account limit

### Question 6:
A leading mobility company wants to use AWS for its connected cab application that would collect sensor data from its electric cab fleet to give drivers dynamically updated map information. The company would like to build its new sensor service by leveraging fully serverless components that are provisioned and managed automatically by AWS. The development team at the company does not want an option that requires the capacity to be manually provisioned, as it does not want to respond manually to changing volumes of sensor data. The company has hired you as an AWS Certified Solutions Architect Professional to provide consultancy for this strategic initiative.
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in a Kinesis Data Stream, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in a Kinesis Data Stream, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing

### Question 7:
A retail company recently saw a huge spike in its monthly AWS spend. Upon further investigation, it was found that some developers had accidentally launched Amazon RDS instances in unexpected Regions. The company has hired you as an AWS Certified Solutions Architect Professional to establish best practices around least privileges for developers and control access to on-premises as well as AWS Cloud resources using Active Directory. The company has mandated you to institute a mechanism to control costs by restricting the level of access that developers have to the AWS Management Console without impacting their productivity. The company would also like to allow developers to launch RDS instances only in us-east-1 Region without limiting access to other services in any Region.
* Configure SAML-based authentication tied to an IAM role that has the PowerUserAccess managed policy attached to it. Attach a customer-managed policy that denies access to RDS in any AWS Region except us-east-1
* Configure SAML-based authentication tied to an IAM role that has the AdministrativeAccess managed policy attached to it. Attach a customer-managed policy that denies access to RDS in any AWS Region except us-east-1
* Set up an IAM user for each developer and add them to the developer IAM group that has the PowerUserAccess managed policy attached to it. Attach a customer-managed policy that allows the developers access to RDS only in us-east-1 Region
* Configure SAML-based authentication tied to an IAM role that has a PowerUserAccess managed policy and a customer-managed policy that denies all the developers access to any AWS services except AWS Service Catalog. Within AWS Service Catalog, create a product containing only RDS service in us-east-1 region

### Question 8:
A digital marketing company uses S3 to store artifacts that may only be accessible to an EC2 instance X in a given VPC. The security team at the company is apprehensive about an attack vector wherein any team member with access to this instance could also set up an EC2 instance in another VPC to access these artifacts.
* Set up a highly restricted Security Group for the EC2 instance X and create an S3 bucket policy to allow access only from this Security Group
* Configure an S3 VPC endpoint and create an S3 bucket policy to allow access only from this VPC endpoint
* Set up an IAM role that allows access to the artifacts in S3 and create an S3 bucket policy to allow access only from this role attached to the instance profile
* Attach an Elastic IP to the EC2 instance X and create an S3 bucket policy to allow access only from this Elastic IP

### Question 9:
An e-commerce company has hired an AWS Certified Solutions Architect Professional to design a dual-tier storage layer for its flagship application running on EC2 instances. One of the tiers of this storage layer is a data tier that should support a POSIX file system shared across many systems. The other tier of this storage layer is a service tier that supports static file content that requires block storage with more than 100k IOPS.
* Use EBS volumes with Provisioned IOPS as the service tier of the storage layer
* Use EC2 Instance Store as the service tier of the storage layer
* Use EC2 Instance Store as the data tier of the storage layer
* Use EFS as the data tier of the storage layer
* Use Amazon S3 as the data tier of the storage layer

### Question 10:
A leading internet television network company uses AWS Cloud for analytics, recommendation engines and video transcoding. To monitor and optimize this network, the engineering team at the company has developed a solution for ingesting, augmenting, and analyzing the multiple terabytes of data its network generates daily in the form of virtual private cloud (VPC) flow logs. This would enable the company to identify performance-improvement opportunities such as identifying apps that are communicating across regions and collocating them. The VPC flow logs data is funneled into Kinesis Data Streams which further acts as the source of a delivery stream for Kinesis Firehose. The engineering team has now configured a Kinesis Agent to send the VPC flow logs data from another set of network devices to the same Firehose delivery stream. They noticed that data is not reaching Firehose as expected.
* Kinesis Firehose delivery stream has reached its limit and needs to be scaled manually
* Kinesis Agent cannot write to a Kinesis Firehose for which the delivery stream source is already set as Kinesis Data Streams
* The data sent by Kinesis Agent is lost because of a configuration error
* Kinesis Agent can only write to Kinesis Data Streams, not to Kinesis Firehose

# Exam 2

### Question 1:
An Internet-of-Things (IoT) company has developed an end-to-end cloud-based solution that provides customers with integrated IoT functionality in devices including baby monitors, security cameras and entertainment systems. The company is using Kinesis Data Streams (KDS) to process IoT data from these devices. Multiple consumer applications are using the incoming data streams and the engineers have noticed a performance lag for the data delivery speed between producers and consumers of the data streams.
* Swap out Kinesis Data Streams with SQS FIFO queues to support the desired read throughput for the downstream applications
* Swap out Kinesis Data Streams with SQS Standard queues to support the desired read throughput for the downstream applications
* Use Enhanced Fanout feature of Kinesis Data Streams to support the desired read throughput for the downstream applications
* Swap out Kinesis Data Streams with Kinesis Data Firehose to support the desired read throughput for the downstream applications

### Question 2:
A global healthcare company wants to develop a solution called Health Information Systems (HIS) on AWS Cloud that would allow the providers, payers, and government agencies to collaborate, anticipate and navigate the changing healthcare landscape. While pursuing this endeavor, the company would like to decrease its IT operational overhead so it could focus more intently on its core business - healthcare analytics. The solution should help the company eliminate the bottleneck created by manual provisioning of development pipelines while adhering to crucial governance and control requirements. As a means to this end, the company has set up "AWS Organizations" to manage several of these scenarios and would like to use Service Control Policies (SCP) for central control over the maximum available permissions for the various accounts in their organization. This allows the organization to ensure that all accounts stay within the organization’s access control guidelines.
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can't perform that action
* SCPs affect all users and roles in attached accounts, including the root user
* SCPs affect all users and roles in attached accounts, excluding the root user
* SCPs do not affect service-linked role
* SCPs affect service-linked roles
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can still perform that action

### Question 3:
A big data analytics company analyzes customer movement data for brick-and-mortar retailers to help them optimize marketing, merchandising, and operations performance by measuring foot traffic, store visits, walk-by conversion, bounce rate, visit duration, and customer loyalty. The company leverages its proprietary analytics workflows built on Redshift to correlate traffic with marketing campaigns and to help retailers optimize hours for peak traffic, among other activities. The company has hired you as an AWS Certified Solutions Architect Professional to review the company's Redshift cluster, which has now become an integral part of its technology solutions. You have been asked to improve the reliability and availability of the cluster in case of a disaster and provide options to ensure that if an issue arises, the cluster can either operate or be restored within five hours.
* Set up two identical Amazon Redshift clusters in different regions in a primary-secondary configuration. Develop a solution using the Kinesis Data Streams to collect the data prior to ingestion into the primary Redshift cluster and stream the data to the secondary cluster
* Set up a CloudFormation stack set for Redshift cluster creation so it can be launched in another Region and configure Amazon Redshift to automatically copy snapshots for the cluster to the other AWS Region. In case of a disaster, restore the cluster in the other AWS Region from that Region's snapshot
* Configure the Amazon Redshift cluster to make use of Auto Scaling groups with the nodes in the cluster spread across multiple Availability Zones (AZs). In case of a disaster, the nodes in the other AZs will ensure reliability and availability
* Set up two identical Amazon Redshift clusters in different regions in a primary-secondary configuration. Create a cron job to run the UNLOAD command every five hours to export data for all tables in primary cluster to S3. Use cross-region replication from the primary region to secondary region. Create another cron job to ingest the data for all tables from S3 into the secondary cluster using the LOAD command

### Question 4:
A solo entrepreneur is working on a new digital media startup and wants to have a hands-on understanding of the comparative pricing for various storage types available on AWS Cloud. The entrepreneur has created a test file of size 5 GB with some random data. Next, he uploads this test file into AWS S3 Standard storage class, provisions an EBS volume (General Purpose SSD (gp2)) with 50 GB of provisioned storage and copies the test file into the EBS volume, and lastly copies the test file into an EFS Standard Storage filesystem. At the end of the month, he analyses the bill for costs incurred on the respective storage types for the test file.
* Cost of test file storage on EBS < Cost of test file storage on S3 Standard < Cost of test file storage on EFS
* Cost of test file storage on EFS < Cost of test file storage on S3 Standard < Cost of test file storage on EBS
* Cost of test file storage on S3 Standard < Cost of test file storage on EBS < Cost of test file storage on EFS
* Cost of test file storage on S3 Standard < Cost of test file storage on EFS < Cost of test file storage on EBS

### Question 5:
A leading club in the Major League Baseball runs a web platform that boasts over 50,000 pages and over 100 million digitized photographs. It is available in six languages and maintains up-to-date information for the season. The engineering team has built a notification system on the web platform using SNS notifications which are then handled by a Lambda function for end-user delivery. During the off-season, the notification systems need to handle about 100 requests per second. During the peak baseball season, the rate touches about 5000 requests per second and it is noticed that a significant number of the notifications are not being delivered to the end-users on the web platform.
* The engineering team needs to provision more servers running the Lambda service
* Amazon SNS message deliveries to AWS Lambda have crossed the account concurrency quota for Lambda, so the team needs to contact AWS support to raise the account limit
* Amazon SNS has hit a concurrency limit, so the team needs to contact AWS support to raise the account limit
* The engineering team needs to provision more servers running the SNS service

### Question 6:
A medical technology company has recently set up a hybrid cloud between its on-premises data centers and AWS Cloud. The engineering team at the company has developed a Media Archiving and Communication System application that runs on AWS to support real-time collaboration among radiologists and other specialists. The company uses Amazon S3 to aggregate the raw medical images and video footage from its research teams across the world to discover tremendous medical insights. The technical teams at the overseas research facilities have reported huge delays in uploading large video files to the destination S3 bucket.
* Use Amazon S3 Transfer Acceleration to enable faster file uploads into the destination S3 bucket
* Use multipart uploads for faster file uploads into the destination S3 bucket
* Create multiple AWS direct connect connections between the AWS Cloud and research facilities running in the on-premises data centers. Use the direct connect connections for faster file uploads into S3
* Create multiple site-to-site VPN connections between the AWS Cloud and research facilities running in the on-premises data centers. Use these VPN connections for faster file uploads into S3
* Use AWS Global Accelerator for faster file uploads into the destination S3 bucket

### Question 7:
A leading gaming company runs multiple game platforms that need to store game state, player data, session history, and leaderboards. The company is looking to move to AWS Cloud to scale reliably to millions of concurrent users and requests while ensuring consistently low latency measured in single-digit milliseconds. The engineering team at the company is evaluating multiple in-memory data stores with the ability to power its on-demand, live leaderboard. The company's leaderboard requires high availability, low latency, and real-time processing to deliver customizable user data for the community of its users.
* Develop the leaderboard using RDS Aurora as it meets the in-memory, high availability, low latency requirements
* Develop the leaderboard using ElastiCache Redis as it meets the in-memory, high availability, low latency requirements
* Develop the leaderboard using DynamoDB with DynamoDB Accelerator (DAX) as it meets the in-memory, high availability, low latency requirements
* Develop the leaderboard using AWS Neptune as it meets the in-memory, high availability, low latency requirements
* Develop the leaderboard using DynamoDB as it meets the in-memory, high availability, low latency requirements

### Question 8:
An e-commerce company is planning to migrate its IT infrastructure from the on-premises data center to AWS Cloud to ramp up its capabilities well in time for the upcoming Holiday Sale season. The company’s CTO has hired you as an AWS Certified Solutions Architect Professional to design a distributed, highly available and loosely coupled order processing application. The application is responsible for receiving and processing orders before storing them in a DynamoDB table. The application has seen sporadic traffic spikes in the past and the CTO wants the application to be able to scale during marketing campaigns to process the orders with minimal disruption.
* Ingest the orders via a Step Function state machine and trigger an ECS container to process them
* Ingest the orders in an SQS queue and trigger a Lambda function to process them
* Push the orders to an SNS topic and subscribe a Lambda function to process them
* Push the orders to Kinesis Data Streams and use Amazon EC2 instances to process them

### Question 9:
A US-based retailer wants to ensure website availability as the company’s traditional infrastructure hasn’t been easy to scale. By moving its e-commerce platform to AWS, the company, which sees 880,000 unique visitors/day, can scale with demand and has improved availability. Last year, the company handled record Black Friday orders of nearly 10,000 orders/hour. The engineering team at the company now wants to finetune the disaster recovery strategy for its database tier. To kick-off the engagement, as an AWS Certified Solutions Architect Professional, you have been asked to implement a disaster recovery strategy for all the Amazon RDS databases that the company owns.
* You can share automated Amazon RDS snapshots with up to 20 AWS accounts
* Similar to an Amazon RDS Multi-AZ configuration, failover to a Read Replica is an automated process that requires no manual intervention after initial configurations
* Database snapshots are user-initiated backups of your complete DB instance that serve as full backups. These snapshots can be copied and shared to different Regions and accounts
* Recovery time objective (RTO), expressed in hours, represents how much data you could lose when a disaster happens
* Automated backups are limited to a single AWS Region while manual snapshots and Read Replicas are supported across multiple Regions
* Recovery time objective (RTO) represents the number of hours it takes, to return the Amazon RDS database to a working state after a disaster

### Question 10:
The DevOps team at a leading SaaS company is planning to release the major upgrade of its flagship CRM application in a week. The team is testing the alpha release of the application running on 20 EC2 instances managed by an Auto Scaling group in subnet 172.20.0.0/24 within VPC X with CIDR block 172.20.0.0/16. The team has noticed connection timeout errors in the application logs while connecting to a MySQL database running on an EC2 instance in the same region in subnet 172.30.0.0/24 within VPC Y with CIDR block 172.30.0.0/16. The IP of the database instance is hard-coded in the application instances.
* Create and attach virtual private gateways for both VPCs and set up default routes to the customer gateways for both VPCs. Assign an Elastic IP for the EC2 instance running MySQL database in VPC Y. Update the application instances to connect to this Elastic IP
* Create and attach NAT gateways for both VPCs and set up routes to the NAT gateways for both VPCs. Assign an Elastic IP for the EC2 instance running MySQL database in VPC Y. Update the application instances to connect to this Elastic IP
* Create and attach internet gateways for both VPCs and set up default routes to the Internet gateways for both VPCs. Assign an Elastic IP for the EC2 instance running MySQL database in VPC Y. Update the application instances to connect to this Elastic IP
* Set up a VPC peering connection between the two VPCs and add a route to the routing table of VPC X that points to the IP address range of 172.30.0.0/16
* Set up a VPC peering connection between the two VPCs and add a route to the routing table of VPC Y that points to the IP address range of 172.20.0.0/16

### Question 11:
A gaming company runs its flagship application with an SLA of 99.99%. Global users access the application 24/7. The application is currently hosted on the on-premises data centers and it routinely fails to meet its SLA, especially when hundreds of thousands of users access the application concurrently. The engineering team has also received complaints from some users about high latency.
* Configure Route 53 round-robin routing policy to distribute load evenly across all Regions and activate the health checks. Host the website behind a Network Load Balancer (NLB) with targets as ECS containers using Fargate. Repeat this configuration of NLB with ECS containers using Fargate in multiple Regions. Use Aurora Global database as the data layer
* Configure Route 53 geolocation-based routing to route to the nearest Region and activate the health checks. Host the website behind a Network Load Balancer (NLB) with targets as ECS containers using Fargate. Repeat this configuration of NLB with ECS containers using Fargate in multiple Regions. Use Aurora Global database as the data layer
* Configure a combination of Route 53 failover routing with geolocation-based routing. Host the website behind an Application Load Balancer (ALB) with targets as EC2 instances that are automatically scaled via Auto-Scaling Group (ASG). Repeat this configuration of ALB with EC2 instances as targets that are scaled via ASG in multiple Regions. Use a Multi-AZ deployment with RDS MySQL as the data layer
* Configure Route 53 latency-based routing to route to the nearest Region and activate the health checks. Host the website on S3 in each Region and use API Gateway with AWS Lambda for the application layer. Set up the data layer using DynamoDB global tables with DAX for caching

### Question 12:
A multi-national retail company wants to modernize its applications and minimize its data center infrastructure. The company wants to explore a hybrid cloud environment with AWS so that it can start leveraging AWS services for some of its data analytics workflows. The engineering team at the retail company wants to establish a dedicated, encrypted, low latency, and high throughput connection between its data center and AWS Cloud. The engineering team has set aside sufficient time to account for the operational overhead of establishing this connection.
* Use VPC transit gateway to establish a connection between the data center and AWS Cloud
* Use AWS Direct Connect along with a site-to-site VPN to establish a connection between the data center and AWS Cloud
* Use AWS Direct Connect to establish a connection between the data center and AWS Cloud
* Use site-to-site VPN to establish a connection between the data center and AWS Cloud

### Question 13:
A silicon valley based unicorn startup recently launched a video-sharing social networking service called KitKot. The startup uses AWS Cloud to manage the IT infrastructure. Users upload video files up to 1 GB in size to a single EC2 instance based application server which stores them on a shared EFS file system. Another set of EC2 instances managed via an Auto Scaling group, periodically scans the EFS share directory for new files to process and generate new videos (for thumbnails and composite visual effects) according to the video processing instructions that are uploaded alongside the raw video files. Post-processing, the raw video files are deleted from the EFS file system and the results are stored in an S3 bucket. Links to the processed video files are sent via in-app notifications to the users. The startup has recently found that even as more instances are added to the Auto Scaling Group, many files are processed twice, therefore image processing speed is not improved.
* Refactor the application to run from S3 instead of EFS and upload the video files directly to an S3 bucket. Set CloudWatch Events to trigger a Lambda function on each file upload that puts a message in an SQS queue containing the link and the video processing instructions. Change the video processing application to read from SQS queue for new files and configure the queue depth metric to scale instances in the video processing Auto Scaling group. Leverage CloudWatch Events to trigger an SNS notification to the user containing the links to the processed files
* Create an hourly cron job on the application server to synchronize the contents of the EFS share with S3. Trigger a Lambda function every time a file is uploaded to S3 and process the video file to store the results in another S3 bucket. Once the file is processed, leverage CloudWatch Events to trigger an SNS notification to send an in-app notification to the user containing the links to the processed files
* Refactor the application to run from S3 instead of EFS and upload the video files directly to an S3 bucket. Configure an S3 trigger to invoke a Lambda function on each video file upload to S3 that puts a message in an SQS queue containing the link and the video processing instructions. Change the video processing application to read from the SQS queue and the S3 bucket. Configure the queue depth metric to scale the size of the Auto Scaling group for video processing instances. Leverage CloudWatch Events to trigger an SNS notification to the user containing the links to the processed files
* Refactor the application to run from Amazon S3 instead of the EFS file system and upload the video files directly to an S3 bucket via an API Gateway based REST API. Configure an S3 trigger to invoke a Lambda function each time a file is uploaded and the Lambda in turn processes the video and stores the processed files in another bucket. Leverage CloudWatch Events to trigger an SNS notification to send an in-app notification to the user containing the links to the processed files

### Question 14:
An analytics company has developed a solution for location intelligence for mobile advertising wherein the company’s flagship product extracts contextual intelligence generated from large amounts of location based data such as place data, event data, digital, mobile and social data – as well as a diversity of other location specific information. The product then performs a series of data cleansing, normalization, analysis, and machine learning processes to extract an understanding of the type of audience present in a specific location at a specific time – enabling the ability to audience target in mobile highly effectively. The company wants to leverage ElastiCache for Redis in cluster mode to enhance the performance and scalability of its existing two-tier application architecture. The ElastiCache cluster is configured to listen on port 6379. The company has hired you as an AWS Certified Solutions Architect Professional to build a secure solution so that the cache data is secure and protected from unauthorized access.
* Enable CloudWatch Logs to monitor the security credentials for the ElastiCache cluster
* Enable CloudTrail to monitor the API Calls for the ElastiCache cluster
* Create the cluster with auth-token parameter and make sure that the parameter is included in all subsequent commands to the cluster
* Configure the security group for the ElastiCache cluster with the required rules to allow inbound traffic from the cluster itself as well as from the cluster's clients on port 6379
* Configure the ElastiCache cluster to have both in-transit as well as at-rest encryption
* Configure the security group for the ElastiCache cluster with the required rules to allow outbound traffic to the cluster's clients on port 6379

### Question 15:
A big data analytics company is leveraging AWS Cloud to process Internet of Things (IoT) sensor data from the field devices of an agricultural sciences company. The analytics company stores the IoT sensor data in Amazon DynamoDB tables. To detect anomalous behaviors and respond quickly, all changes to the items stored in the DynamoDB tables must be logged in near real-time.
* Configure event patterns in CloudWatch Events to capture DynamoDB API call events and set up Lambda function as a target to analyze anomalous behavior. Send SNS notifications when anomalous behaviors are detected
* Set up CloudTrail to capture all API calls that update the DynamoDB tables. Leverage CloudTrail event filtering to analyze anomalous behaviors and send SNS notifications in case anomalies are detected
* Set up DynamoDB Streams to capture and send updates to a Lambda function that outputs records directly to Kinesis Data Analytics (KDA). Detect and analyze anomalies in KDA and send notifications via SNS
* Set up DynamoDB Streams to capture and send updates to a Lambda function that outputs records to Kinesis Data Analytics (KDA) via Kinesis Data Streams (KDS). Detect and analyze anomalies in KDA and send notifications via SNS

### Question 16:
A social media company has a serverless application stack that consists of CloudFront, API Gateway and Lambda functions. The company has hired you as an AWS Certified Solutions Architect Professional to improve the current deployment process which creates a new version of the Lambda function and then runs an AWS CLI script for deployment. In case the new version errors out, then another CLI script is invoked to deploy the previous working version of the Lambda function. The company has mandated you to decrease the time to deploy new versions of the Lambda functions and also reduce the time to detect and rollback when errors are identified.
* Set up and deploy nested CloudFormation stacks with the CloudFront distribution as well as the API Gateway in the parent stack. Create and deploy a child stack containing the Lambda functions. To address any changes in a Lambda function, create a CloudFormation change set and deploy. Use pre-traffic and post-traffic test functions of the change set to verify the deployment. Rollback in case CloudWatch alarms are triggered
* Set up and deploy a CloudFormation stack containing a new API Gateway endpoint that points to the new Lambda version. Test the updated CloudFront origin that points to this new API Gateway endpoint and in case errors are detected then revert the CloudFront origin to the previous working API Gateway endpoint
* Use Serverless Application Model (SAM) and leverage the built-in traffic-shifting feature of SAM to deploy the new Lambda version via CodeDeploy and use pre-traffic and post-traffic test functions to verify code. Rollback in case CloudWatch alarms are triggered
* Set up and deploy nested CloudFormation stacks with the CloudFront distribution as well as the API Gateway in the parent stack. Create and deploy a child stack containing the Lambda functions. To address any changes in a Lambda function, create a CloudFormation change set and deploy. In case the Lambda function errors out, rollback the CloudFormation change set to the previous version

### Question 17:
A web hosting company's CFO recently analyzed the company's monthly bill for the AWS account for the development environment and identified an opportunity to reduce the cost for AWS Elastic Beanstalk infrastructure in use. The CFO in consultation with the CTO has hired you as an AWS Certified Solutions Architect Professional to design a highly available solution that will provision an Elastic Beanstalk environment in the morning and terminate it at the end of the day. The solution should be designed with minimal operational overhead with a focus on minimizing costs. The solution should also facilitate the increased use of Elastic Beanstalk environments among different development teams and must provide a one-stop scheduler solution for all teams to keep the operational costs as low as possible.
* Provision an EC2 Micro instance. Configure an IAM role with the required Elastic Beanstalk environment permissions and attach it to the instance profile. Create scripts on the instance to provision and terminate the Elastic Beanstalk environment. Set up cron jobs on the instance to execute the scripts
* Configure the Elastic Beanstalk environment to use custom commands in the EC2 instance user data. Leverage the scheduled action for an Auto Scaling group to scale-out EC2 instances in the morning and scale-in the instance count to 0 to terminate the EC2 instances at the end of the day
* Leverage the activity task of an AWS Step Function to provision and terminate the Elastic Beanstalk environment. Create a role for the Step Function to allow it to provision and terminate the Elastic Beanstalk environment. Execute the Step Function daily and use the "wait state" to control the start and stop time
* Set up separate Lambda functions to provision and terminate the Elastic Beanstalk environment. Configure a Lambda execution role granting the required Elastic Beanstalk environment permissions and assign the role to the Lambda functions. Configure cron expression based Amazon CloudWatch Events rules to trigger the Lambda functions

### Question 18:
A project uses two AWS accounts for accessing various AWS services. The engineering team has just configured an Amazon S3 bucket in the first AWS account for writing data from the Amazon Redshift cluster provisioned in the second AWS account. The team has noticed that the files created in the S3 bucket using UNLOAD command from the Redshift cluster are not accessible to the users present in the same AWS account as the S3 bucket.
* The owner of an S3 bucket has implicit access to all objects in his bucket. Permissions are set on objects after they are completely copied to the target location. Since the owner is unable to access the uploaded files, it is possible that the write operation is still in progress
* When objects are uploaded to S3 bucket from a different AWS account, the S3 bucket owner will get implicit permissions to access these objects. It is an upload error that can be fixed by providing manual access from AWS console
* By default, an S3 object is owned by the AWS account that uploaded it. So the S3 bucket owner will not implicitly have access to the objects written by Redshift cluster
* When two different AWS accounts are accessing an S3 bucket, both the accounts need to share the bucket policies, explicitly defining the actions possible for each account. An erroneous policy can lead to such permission failures

### Question 19:
A global IoT technology company develops solutions using connected sensors and intelligent analytics to empower more than 17,000 municipalities in 50 countries to be smarter by improving transportation capacity, safety, cost-effectiveness and performance. The product team at the company is looking to build features to simplify each step of building an API and streamline collaboration so you can create better APIs. As part of its research, the product team has figured out a market need to support both stateful and stateless client-server communications via the APIs developed using its platform.
* API Gateway creates RESTful APIs that enable stateless client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateless client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateful client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateful client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server

### Question 20:
A web development studio runs hundreds of Proof-of-Concept (PoC) and demo applications on virtual machines running on an on-premises server. Many of the applications are simple PHP, JavaScript or Python web applications which are no longer actively developed and serve little traffic.
* Leverage AWS Server Migration Service (SMS) to create AMIs for each virtual machine and run each application on a dedicated EC2 instance
* Leverage VM Import/Export to create AMIs for each virtual machine and run them in single-instance AWS Elastic Beanstalk environments by configuring a custom image
* Dockerize each application and then deploy to an ECS cluster running behind an Application Load Balancer
* Migrate the application code to use a serverless stack comprising of Lambda functions and DynamoDB

### Question 21:
The engineering team at a data analytics company is currently optimizing a production workload on AWS that is I/O intensive with frequent read/write/update operations and it's currently constrained on the IOPS. This workload consists of a single-tier with 15 r6g.8xlarge instances, each with 3 TB gp2 volume. The number of processing jobs has increased recently, resulting in an increase in latency as well. The team has concluded that they need to increase the IOPS by 3,000 for each of the instances for the application to perform efficiently.
* Modify the type of Amazon EBS volume on each instance from gp2 to io1 and set provisioned IOPS to 12,000
* Modify the size of the gp2 volume for each instance from 3 TB to 4 TB
* Provision a new EFS file system and migrate all the data to this new file system. Mount this file system on all 15 instances
* Set up a new Amazon S3 bucket and migrate all the data to this new bucket. Configure each instance to access this S3 bucket and use it for storage

### Question 22:
A digital media company wants to use AWS Cloudfront to manage its content. Firstly, it would like to allow only those new users who have paid the annual subscription fee the ability to download the application installation file. Secondly, only the subscribers should be able to view the files in the members' area.
* Require HTTPS for communication between CloudFront and your S3 origin
* Use CloudFront signed cookies to restrict access to the application installation file
* Use CloudFront signed cookies to restrict access to all the files in the members' area of the website
* Use CloudFront signed URLs to restrict access to all the files in the members' area of the website
* Use CloudFront signed URLs to restrict access to the application installation file

### Question 23:
A global biomedicine company has built a Genomics Solution on AWS Cloud to advance neurological disease research and identify potential new disease therapies, find new gene targets and better understand neurological disease biology. The company's labs generate hundreds of terabytes of research data daily. To further accelerate the innovation process, the engineering team at the company wants to move most of the on-premises data into Amazon S3, Amazon EFS, and Amazon FSx for Windows File Server easily, quickly, and cost-effectively. The team would like to automate and accelerate online data transfers to these AWS storage services.
* Use File Gateway to automate and accelerate online data transfers to the given AWS storage services
* Use AWS Transfer Family to automate and accelerate online data transfers to the given AWS storage services
* Use AWS Snowball Edge Storage Optimized device to automate and accelerate online data transfers to the given AWS storage services
* Use AWS DataSync to automate and accelerate online data transfers to the given AWS storage services

### Question 24:
A financial services company runs more than 400 core-banking microservices on AWS, using services including Amazon Elastic Compute Cloud (Amazon EC2), Amazon Elastic Block Store (Amazon EBS), and Amazon Simple Storage Service (Amazon S3). The company also segregates parts of its infrastructure using separate AWS accounts, so if one account is compromised, critical parts of the infrastructure in other accounts remain unaffected. The bank uses one account for production, one for non-production, and one for storing and managing users’ login information and roles within AWS. The privileges that are assigned in the user account then allow users to read or write to production and non-production accounts. The company has set up "AWS Organizations" to manage several of these scenarios. The company wants to provide shared and centrally-managed VPCs to all business units for certain applications that need a high degree of interconnectivity.
* Use VPC sharing to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC sharing to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC peering to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC peering to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations

### Question 25:
A leading hotel reviews website has a repository of more than one million high-quality digital images. When this massive volume of images became too cumbersome to handle in-house, the company decided to offload the content to a central repository on Amazon S3 as part of its hybrid cloud strategy. The company now wants to reprocess its entire collection of photographic images to change the watermarks. The company wants to use Amazon EC2 instances and Amazon SQS in an integrated workflow to generate the sizes they need for each photo. The team wants to process a few thousand photos each night, using Amazon EC2 Spot Instances. The team uses Amazon SQS to communicate the photos that need to be processed and the status of the jobs. To handle certain sensitive photos, the team wants to postpone the delivery of certain messages to the queue by one minute while all other messages need to be delivered immediately to the queue.
* Use message timers to postpone the delivery of certain messages to the queue by one minute
* Use dead-letter queues to postpone the delivery of certain messages to the queue by one minute
* Use visibility timeout to postpone the delivery of certain messages to the queue by one minute
* Use delay queues to postpone the delivery of certain messages to the queue by one minute

### Question 26:
A mobility company in Latin America uses Elastic Load Balancing to distribute traffic across multiple Amazon EC2 instances. Auto Scaling groups start and stop Amazon EC2 machines based on the number of incoming requests. The company has recently started operations in a new AWS Region and is setting up an Application Load Balancer for its fleet of EC2 instances spread across two Availability Zones, with one instance as a target in Availability Zone X and four instances as targets in Availability Zone Y. The company is doing benchmarking for server performance in the new Region for the case when cross-zone load balancing is enabled compared to the case when cross-zone load balancing is disabled.
* With cross-zone load balancing enabled, one instance in Availability Zone X receives 50% traffic and four instances in Availability Zone Y receive 12.5% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone X receives 20% traffic and four instances in Availability Zone Y receive 20% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone X receives 20% traffic and four instances in Availability Zone Y receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone X receives 50% traffic and four instances in Availability Zone Y receive 12.5% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone X receives 20% traffic and four instances in Availability Zone Y receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone X receives no traffic and four instances in Availability Zone Y receive 25% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone X receives no traffic and four instances in Availability Zone Y receive 25% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone X receives 50% traffic and four instances in Availability Zone Y receive 12.5% traffic each

### Question 27:
The engineering team at a retail company has deployed a fleet of EC2 instances under an Auto Scaling group (ASG). The instances under the ASG span two Availability Zones (AZ) within the eu-west-1 region. All the incoming requests are handled by an Application Load Balancer (ALB) that routes the requests to the EC2 instances under the ASG. A planned migration went wrong last week when two instances (belonging to AZ 1) were manually terminated and desired capacity was reduced causing the Availability Zones to become unbalanced. Later that day, another instance (belonging to AZ 2) was detected as unhealthy by the Application Load Balancer's health check.
* Amazon EC2 Auto Scaling creates a new scaling activity to terminate the unhealthy instance and launch the new instance simultaneously
* Amazon EC2 Auto Scaling creates a new scaling activity for launching a new instance to replace the unhealthy instance. Later, EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it
* As the Availability Zones got unbalanced, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling launches new instances before terminating the old ones, so that rebalancing does not compromise the performance or availability of your application
* Amazon EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it. Later, another scaling activity launches a new instance to replace the terminated instance
* As the Availability Zones got unbalanced, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling terminates old instances before launching new instances, so that rebalancing does not cause extra instances to be launched

### Question 28:
A leading mobility company wants to use AWS for its connected cab application that would collect sensor data from its electric cab fleet to give drivers dynamically updated map information. The company would like to build its new sensor service by leveraging fully serverless components that are provisioned and managed automatically by AWS. The development team at the company does not want an option that requires the capacity to be manually provisioned, as it does not want to respond manually to changing volumes of sensor data. The company has hired you as an AWS Certified Solutions Architect Professional to provide consultancy for this strategic initiative.
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in a Kinesis Data Stream, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in a Kinesis Data Stream, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing

### Question 29:
A leading pharmaceutical company has significant investments in running Oracle and PostgreSQL services on Amazon RDS which provide their scientists with near real-time analysis of millions of rows of manufacturing data generated by continuous manufacturing equipment with 1,600 data points per row. The business analytics team has been running ad-hoc queries on these databases to prepare daily reports for senior management. The engineering team has observed that the database performance takes a hit whenever these reports are run by the analytics team. To facilitate the business analytics reporting, the engineering team now wants to replicate this data with high availability and consolidate these databases into a petabyte-scale data warehouse by streaming data to Amazon Redshift.
* Use AWS Database Migration Service to replicate the data from the databases into Amazon Redshift
* Use Amazon Kinesis Data Streams to replicate the data from the databases into Amazon Redshift
* Use Amazon EMR to replicate the data from the databases into Amazon Redshift
* Use AWS Glue to replicate the data from the databases into Amazon Redshift

### Question 30:
A digital media company has hired you as an AWS Certified Solutions Architect Professional to optimize the architecture for its backup solution for applications running on the AWS Cloud. Currently, all of the applications running on AWS use at least two Availability Zones (AZs). The updated backup policy at the company mandates that all nightly backups for its data are durably stored in at least two geographically distinct Regions for Production and Disaster Recovery (DR) and the backup processes for both Regions must be fully automated. The new backup solution must ensure that the backup is available to be restored immediately for the Production Region and should be restored within 24 hours in the DR Region.
* Create a backup process to persist all the data to an S3 bucket A using S3 standard storage class in the Production Region. Set up cross-Region replication of this S3 bucket A to an S3 bucket B using S3 standard-IA storage class in the DR Region and set up a lifecycle policy in the DR Region to immediately move this data to Amazon Glacier
* Create a backup process to persist all the data to an S3 bucket A using S3 standard storage class in the Production Region. Set up cross-Region replication of this S3 bucket A to an S3 bucket B using S3 standard storage class in the DR Region and set up a lifecycle policy in the DR Region to immediately move this data to Amazon Glacier
* Create a backup process to persist all the data to Amazon Glacier in the Production Region. Set up cross-Region replication of this data to Amazon Glacier in the DR Region to ensure minimum possible costs in both Regions
* Create a backup process to persist all the data to a large Amazon EBS volume attached to the backup server in the Production Region. Run nightly cron jobs to snapshot these volumes and then copy these snapshots to the DR Region

### Question 31:
A web-hosting startup manages more than 500 public web applications on AWS Cloud which are deployed in a single AWS Region. The fully qualified domain names (FQDNs) of all of the applications are configured to use HTTPS and are served via Application Load Balancers (ALBs). These ALBs are configured to use public SSL/TLS certificates. The startup has hired you as an AWS Certified Solutions Architect Professional to migrate the web applications to a multi-Region architecture. You must ensure that all HTTPS services continue to work without interruption.
* Generate a separate certificate for each FQDN in each AWS Region using AWS Certificate Manager. Associate the certificates with the corresponding ALBs in the relevant AWS Region
* Generate a separate certificate for each FQDN in each AWS Region using AWS KMS. Associate the certificates with the corresponding ALBs in the relevant AWS Region
* Generate a certificate for each FQDN via AWS Certificate Manager. Associate the same FQDN certificate with the ALBs in the relevant AWS Regions
* Set up the key pairs and then generate the certificate for each FQDN via AWS KMS. Associate the same FQDN certificate with the ALBs in the relevant AWS Regions

### Question 32:
The CTO at a multi-national retail company is pursuing an IT re-engineering effort to set up a hybrid network architecture that would facilitate the company's envisaged long-term data center migration from multiple on-premises data centers to the AWS Cloud. The current on-premises data centers are in different locations and are inter-linked via a private fiber. Due to the unique constraints of the existing legacy applications, using NAT is not an option. During the migration period, many critical applications will need access to other applications deployed in both the on-premises data centers and AWS Cloud.
* Set up multiple software VPN connections between AWS cloud and the on-premises data centers. Configure each subnet's traffic through different VPN connections for redundancy. Make sure that no VPC CIDR blocks overlap one another or the on-premises network
* Set up a Direct Connect to each on-premises data center from different service providers and configure routing to failover to the other on-premises data center's Direct Connect in case one connection fails. Make sure that no VPC CIDR blocks overlap one another or the on-premises network
* Set up a Direct Connect as primary connection for all on-premises data centers with another VPN as backup. Configure both connections to use the same virtual private gateway and BGP. Make sure that no VPC CIDR blocks overlap one another or the on-premises network
* Set up multiple hardware VPN connections between AWS cloud and the on-premises data centers. Configure each subnet's traffic through different VPN connections for redundancy. Make sure that no VPC CIDR blocks overlap one another or the on-premises network

### Question 33:
A leading Internet-of-Things (IoT) solutions company needs to develop a platform that would analyze real-time clickstream events from embedded sensors in consumer electronic devices. The company has hired you as an AWS Certified Solutions Architect Professional to consult the engineering team and develop a solution using the AWS Cloud. The company wants to use clickstream data to perform data science, develop algorithms, and create visualizations and dashboards to support the business stakeholders. Each of these groups would work independently and would need real-time access to this clickstream data for their applications.
* Use AWS Kinesis Data Analytics to facilitate multiple applications consume and analyze same streaming data concurrently and independently
* Use AWS Kinesis Data Streams to facilitate multiple applications consume same streaming data concurrently and independently
* Use Amazon SQS to facilitate multiple applications process same streaming data concurrently and independently
* Use AWS Kinesis Data Firehose to allow applications to consume the same streaming data concurrently and independently

### Question 34:
An e-commerce company has hired an AWS Certified Solutions Architect Professional to transform a standard three-tier web application architecture in AWS. Currently, the web and application tiers run on EC2 instances and the database tier runs on RDS MySQL. The company wants to redesign the web and application tiers to use API Gateway with Lambda Functions with the final goal of deploying the new application within 6 months. As an immediate short-term task, the Engineering Manager has mandated the Solutions Architect to reduce costs for the existing stack.
* Provision Reserved Instances for the web and application tiers and On-Demand Instances for the database tier
* Provision Spot Instances for the web and application tiers and Reserved Instances for the database tier
* Provision Reserved Instances for the web, application and database tiers
* Provision On-Demand Instances for the web and application tiers and Reserved Instances for the database tier

### Question 35:
A world-leading video creation and distribution company has recently migrated to AWS Cloud for digitally transforming their movie business. The company wants to speed up its media distribution process and improve data security while also reducing costs and eliminating errors. The company wants to set up a Digital Cinema Network that would allow it to connect the space-constrained movie theater environment to content stored in Amazon S3 as well as to accelerate the online distribution of movies and advertising to theaters in 38 key media markets worldwide. The company also wants to do an accelerated online migration of hundreds of terabytes of files from their on-premises data center to Amazon S3 and then establish a mechanism to access the migrated data for ongoing updates from the on-premises applications.
* Use S3 Transfer Acceleration to migrate existing data to Amazon S3 and then use DataSync for ongoing updates from the on-premises applications
* Use AWS DataSync to migrate existing data to Amazon S3 and then use File Gateway to retain access to the migrated data for ongoing updates from the on-premises applications
* Use File Gateway configuration of AWS Storage Gateway to migrate data to Amazon S3 and then use S3 Transfer Acceleration for ongoing updates from the on-premises applications
* Use AWS DataSync to migrate existing data to Amazon S3 as well as access the S3 data for ongoing updates

### Question 36:
An international integrated property management company wants to improve employee communication and productivity by using SharePoint to deploy a content and collaboration platform with document and records management functionality. The company wants to establish an AWS Direct Connect link to connect the AWS Cloud with the internal corporate network using AWS Storage Gateway. Using AWS Direct Connect would enable the company to deliver on its performance benchmark requirements including a three second or less response time for sending small documents across the internal network. To facilitate this goal, the company wants to be able to resolve DNS queries for any resources in the on-premises network from the AWS VPC and also resolve any DNS queries for resources in the AWS VPC from the on-premises network.
* Create a universal endpoint on Route 53 Resolver and then Route 53 Resolver can receive and forward queries to resolvers on the on-premises network via this endpoint
* Create an outbound endpoint on Route 53 Resolver and then Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint
* Create an inbound endpoint on Route 53 Resolver and then Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint
* Create an inbound endpoint on Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Route 53 Resolver via this endpoint
* Create an outbound endpoint on Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Route 53 Resolver via this endpoint

### Question 37:
A Big Data Analytics company has built a custom data warehousing solution for a large airline by using Amazon Redshift. The solution helps the airline to analyze the international and domestic flight reservations, ticket issuing and boarding information, aircraft operation records, and cargo transportation records. As part of the cost optimizations, the airline now wants to move any historical data (any data older than a year) into S3, as the daily analytical reports consume data for just the last one year. However, the analysts at multiple divisions of the airline want to retain the ability to cross-reference this historical data along with the daily reports. The airline wants to develop a solution with the LEAST amount of effort and MINIMUM cost.
* Use the Redshift COPY command to load the S3 based historical data into Redshift. Once the ad-hoc queries are run for the historic data, it can be removed from Redshift
* Use Redshift Spectrum to create Redshift cluster tables pointing to the underlying historical data in S3. The analytics team can then query this historical data to cross-reference with the daily reports from Redshift
* Set up access to the historical data via Athena. The analytics team can run historical data queries on Athena and continue the daily reporting on Redshift. In case the reports need to be cross-referenced, the analytics team needs to export these in flat files and then do further analysis
* Use Glue ETL job to load the S3 based historical data into Redshift. Once the ad-hoc queries are run for the historic data, it can be removed from Redshift

### Question 38:
A multi-national retail company has built a hub-and-spoke network with AWS Transit Gateway. VPCs have been provisioned into multiple AWS accounts to facilitate network isolation and to enable delegated network administration. The organization is looking at a cost-effective, quick and secure way of maintaining this distributed architecture so that it provides access to services required by workloads in each of the VPCs.
* Use VPCs connected with AWS Direct Connect
* Use Fully meshed VPC Peers
* Use Centralized VPC Endpoints for connecting with multiple VPCs, also known as shared services VPC
* Use Transit VPC to reduce cost and share the resources across VPCs

### Question 39:
A social media company has configured a CloudFront distribution to distribute both static and dynamic content from a web application that needs user authorization and session tracking for dynamic content. The web application is running behind an Application Load Balancer. The cache behavior for the CloudFront distribution has been configured to forward the Authorization, Host, and Date HTTP whitelist headers as well as forward a session cookie to the origin. All other cache behavior settings are set to their default value. A valid ACM certificate is applied to the CloudFront distribution as well as to the HTTPS listener for the Application Load Balancer with the CloudFront origin protocol policy configured to HTTPS only.
* Remove the Date and Authorization HTTPS headers from the whitelist headers section of the cache behavior. Then update the cache behavior to use presigned cookies for authorization
* Create separate cache behaviors for static and dynamic content. Remove the Date HTTP header from the whitelist headers section on both of the cache behaviors. Remove the session cookie from the whitelist cookies section for static content as well as the Authorization HTTP header from the whitelist headers section for cache behavior configured for static content
* Remove the Host HTTP header from the whitelist headers section and remove the session cookie from the whitelist cookies section for the default cache behavior. Enable automatic object compression and use Lambda@Edge viewer request events for user authorization
* Create separate cache behaviors for static and dynamic content. Remove the Date as well as Host HTTP headers from the whitelist headers section on both of the cache behaviors. Remove the session cookie from the whitelist cookies section for static content as well as the Authorization HTTP header from the whitelist headers section for cache behavior configured for static content

### Question 40:
An oncology research company has a goal to eradicate cancer by developing personalized immunotherapies to fight multiple cancer types. Recently the company has migrated some of its IT infrastructure to AWS Cloud and is looking for a solution to enable real-time data transfer between AWS and its data centers to reduce the turnaround time for patient results thereby enabling the company to identify tumor antigens and manufacture personalized immunotherapies faster. The company wants to build a patient results archival solution such that only the most frequently accessed results are available as cached data locally while backing up all results on Amazon S3.
* Use AWS direct connect to store the most frequently accessed results locally for low-latency access while storing the full backup of results in an Amazon S3 bucket
* Use AWS Snowball Edge Storage Optimized device to store the most frequently accessed results locally for low-latency access while storing the full backup of results in an Amazon S3 bucket
* Use AWS Volume Gateway - Stored Volume - to store the most frequently accessed results locally for low-latency access while storing the full volume with all results in its Amazon S3 service bucket
* Use AWS Volume Gateway - Cached Volume - to store the most frequently accessed results locally for low-latency access while storing the full volume with all results in its Amazon S3 service bucket

### Question 41:
A social learning platform allows students to connect with other students as well as experts and professionals from academic, research institutes and industry. The goal of the company’s platform, developed on AWS Cloud, is to assist students pursuing higher education learn and develop skills in a manner unencumbered by socio-economic, location and resource barriers. The engineering team at the company manages 5 Amazon EC2 instances that make read-heavy database requests to the Amazon RDS for PostgreSQL DB cluster. As an AWS Certified Solutions Architect Professional, you have been asked to make the database cluster resilient from a disaster recovery perspective.
* Use cross-Region Read Replicas
* Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups in a single AWS Region
* Enable the automated backup feature of Amazon RDS in a multi-AZ deployment that creates backups across multiple Regions
* Use database cloning feature of the RDS DB cluster
* Use RDS Provisioned IOPS (SSD) Storage in place of General Purpose (SSD) Storage

### Question 42:
The DevOps team for a CRM SaaS company wants to implement a patching plan on AWS Cloud for a large mixed fleet of Windows and Linux servers. The patching plan has to be auditable and must be implemented securely to ensure compliance with the company's business requirements.
* Apply patch baselines using the AWS-ApplyPatchBaseline SSM document
* Set up Systems Manager Agent on all instances to manage patching. Test patches in pre-production and then deploy as a maintenance window task with the appropriate approval
* Set up an OS-native patching service to manage the update frequency and release approval for all instances. Set up AWS Config to provide audit and compliance reporting
* Configure OpsWorks automatic patching support for all applications which will keep the OS up-to-date following the initial installation. Set up AWS Config to provide audit and compliance reporting
* Apply patch baselines using the AWS-RunPatchBaseline SSM document

### Question 43:
An IT company wants to move all its clients belonging to the regulated and security-sensitive industries such as financial services and healthcare to the AWS Cloud as it wants to leverage the out-of-box security-specific capabilities offered by AWS. The Security team at the company is developing a framework to validate the adoption of AWS best practices and industry-recognized compliance standards. The AWS Management Console is the preferred method for the in-house teams wanting to provision resources. You have been hired as an AWS Certified Solutions Architect Professional to spearhead this strategic initiative.
* Leverage CloudTrail integration with SNS to automatically notify unauthorized API activities. Ensure that CloudTrail is enabled for all accounts as well as all available AWS services. Use Lambda functions to automatically revert non-authorized changes in AWS resources
* Leverage CloudWatch Logs agent to collect all the AWS SDK logs. Search the log data using a pre-defined set of filter patterns that match mutating API calls. Use CloudWatch alarms to send notifications via SNS when unintended changes are performed. Archive log data by using a batch export to Amazon S3 and analyze via Athena
* Leverage CloudWatch Events near-real-time capabilities to monitor system events patterns to trigger Lambda functions to automatically revert non-authorized changes in AWS resources. Send notifications via SNS topics to improve the incidence response time
* Leverage Config rules to audit changes to AWS resources and monitor the compliance of the configuration by running the evaluations for the rule at a frequency that you choose. Develop AWS Config custom rules to establish a test-driven development approach by triggering the evaluation when any resource that matches the rule's scope changes in configuration
* Enable trails and set up CloudTrail events to review and monitor management activities of all AWS accounts by logging these activities into CloudWatch Logs using a KMS key. Ensure that CloudTrail is enabled for all accounts as well as all available AWS services

### Question 44:
A leading community marketplace company allows property owners and travelers to connect with each other for the purpose of renting unique vacation spaces around the world. The engineering team at the company uses Amazon MySQL RDS DB cluster because it simplifies much of the time-consuming administrative tasks typically associated with databases. The team uses Multi-Availability Zone (Multi-AZ) deployment to further automate its database replication and augment data durability. The current cluster configuration also uses Read Replicas. An intern has joined the team and wants to understand the replication capabilities for Multi-AZ as well as Read Replicas for the given RDS cluster.
* Multi-AZ follows asynchronous replication and spans one Availability Zone within a single region. Read Replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows synchronous replication and spans at least two Availability Zones within a single region. Read Replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read Replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read Replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region

### Question 45:
A social media company has its corporate headquarters in New York with an on-premises data center using an AWS Direct Connect connection to the AWS VPC. The branch offices in San Francisco and Miami use Site-to-Site VPN connections to connect to the AWS VPC. The company is looking for a solution to have the branch offices send and receive data with each other as well as with their corporate headquarters.
* Configure VPC Endpoints between branch offices and corporate headquarters which will enable branch offices to send and receive data with each other as well as with their corporate headquarters
* Set up VPC Peering between branch offices and corporate headquarters which will enable branch offices to send and receive data with each other as well as with their corporate headquarters
* Configure Public Virtual Interfaces (VIFs) between branch offices and corporate headquarters which will enable branch offices to send and receive data with each other as well as with their corporate headquarters
* Set up VPC CloudHub between branch offices and corporate headquarters which will enable branch offices to send and receive data with each other as well as with their corporate headquarters

### Question 46:
A Wall Street based trading firm is modernizing its message queuing system by migrating from self-managed message-oriented middleware systems to Amazon SQS. The firm is using SQS to migrate several trading applications to the cloud to ensure high availability and cost efficiency while simplifying administrative complexity and overhead. The development team at the firm expects a peak rate of about 2,400 transactions per second to be processed via SQS. It is important that the messages are processed in the order they are received.
* Use Amazon SQS FIFO queue in batch mode of 4 transactions per operation to process the transactions at the peak rate
* Use Amazon SQS standard queue to process the messages
* Use Amazon SQS FIFO queue in batch mode of 12 transactions per operation to process the transactions at the peak rate
* Use Amazon SQS FIFO queue in batch mode of 8 transactions per operation to process the transactions at the peak rate

### Question 47:
A health and beauty online retailer ships thousands of orders daily to 85 countries worldwide with more than 25,000 items and carries inventory from 600 different manufacturers. The company processes thousands of online orders each day from these countries and its website is localized in 15 languages. As a global online business, the company’s website faces continual security threats and challenges in the form of HTTP flood attacks, distributed denial of service (DDoS) attacks, rogue robots that flood its website with traffic, SQL-injection attacks designed to extract data and cross-site scripting attacks (XSS). Most of these attacks originate from certain countries. Therefore, the company wants to block access to its application from specific countries; however, the company wants to allow its remote development team (from one of the blocked countries) to have access to the application. The application is deployed on EC2 instances running under an Application Load Balancer (ALB) with AWS WAF.
* Use ALB IP set statement that specifies the IP addresses that you want to allow through
* Create a deny rule for the blocked countries in the NACL associated with each of the EC2 instances
* Use ALB geo match statement listing the countries that you want to block
* Use WAF geo match statement listing the countries that you want to block
* Use WAF IP set statement that specifies the IP addresses that you want to allow through

### Question 48:
A data analytics company needs to set up a data lake on Amazon S3 for a financial services client. The data lake is split in raw and curated zones. For compliance reasons, the source data needs to be kept for a minimum of 5 years. The source data arrives in the raw zone and is then processed via an AWS Glue based ETL job into the curated zone. The business analysts run ad-hoc queries only on the data in the curated zone using Athena. The team is concerned about the cost of data storage in both the raw and curated zones as the data is increasing at a rate of 2 TB daily in each zone.
* Use Glue ETL job to write the transformed data in the curated zone using a compressed file format
* Setup a lifecycle policy to transition the curated zone data into Glacier Deep Archive after 1 day of object creation
* Setup a lifecycle policy to transition the raw zone data into Glacier Deep Archive after 1 day of object creation
* Create a Lambda function based job to delete the raw zone data after 1 day
* Use Glue ETL job to write the transformed data in the curated zone using CSV format

### Question 49:
The engineering team at a social media company is building an ElasticSearch based index for all the existing files in S3. To build this index, it only needs to read the first 250 bytes of each object in S3, which contains some metadata about the content of the file itself. There are over 100,000 files in your S3 bucket, adding up to 50TB of data.
* Use the ElasticSearch Import feature to load the entire data from S3 to ElasticSearch and then ElasticSearch would automatically build the index
* Create an application that will traverse the S3 bucket, issue a Byte Range Fetch for the first 250 bytes, and store that information in ElasticSearch
* Create an application that will traverse the S3 bucket, read the entire files one by one, extract the first 250 bytes, and store that information in ElasticSearch
* Use the Database Migration Service to load the entire data from S3 to ElasticSearch and then ElasticSearch would automatically build the index
* Create an application that will use the S3 Select ScanRange parameter to get the first 250 bytes and store that information in ElasticSearch

### Question 50:
A leading internet television network company uses AWS Cloud for analytics, recommendation engines and video transcoding. To monitor and optimize this network, the engineering team at the company has developed a solution for ingesting, augmenting, and analyzing the multiple terabytes of data its network generates daily in the form of virtual private cloud (VPC) flow logs. This would enable the company to identify performance-improvement opportunities such as identifying apps that are communicating across regions and collocating them. The VPC flow logs data is funneled into Kinesis Data Streams which further acts as the source of a delivery stream for Kinesis Firehose. The engineering team has now configured a Kinesis Agent to send the VPC flow logs data from another set of network devices to the same Firehose delivery stream. They noticed that data is not reaching Firehose as expected.
* The data sent by Kinesis Agent is lost because of a configuration error
* Kinesis Agent cannot write to a Kinesis Firehose for which the delivery stream source is already set as Kinesis Data Streams
* Kinesis Firehose delivery stream has reached its limit and needs to be scaled manually
* Kinesis Agent can only write to Kinesis Data Streams, not to Kinesis Firehose

### Question 51:
A Silicon Valley based education technology startup is moving its IT operations from an on-premises data center to AWS Cloud. Its flagship product is a comprehensive learning management system that is offered in three configurations: on-premises, hosted, and fully managed software as a service (SaaS). For its SaaS version, the startup was initially using a major commercial database in a managed-hosting environment. However, this resulted in high licensing costs and required the startup to invest significant resources in day-to-day database management. That’s why it chose to migrate to the open-source MySQL database running on Amazon RDS. The engineering team at the startup is evaluating the Multi-AZ and Read Replica capabilities of RDS MySQL vs Aurora MySQL before they implement the solution in their production environment. The startup has hired you as an AWS Certified Solutions Architect Professional to provide a detailed report on this technical requirement.
* Read Replicas can be manually promoted to a standalone database instance for RDS MySQL whereas Read Replicas for Aurora MySQL can be promoted to the primary instance
* Multi-AZ deployments for Aurora MySQL follow synchronous replication whereas Multi-AZ deployments for RDS MySQL follow asynchronous replication
* The primary and standby DB instances are upgraded at the same time for RDS MySQL Multi-AZ. All instances are upgraded at the same time for Aurora MySQL
* Multi-AZ deployments for both RDS MySQL and Aurora MySQL follow synchronous replication
* Read Replicas can be manually promoted to a standalone database instance for Aurora MySQL whereas Read Replicas for RDS MySQL can be promoted to the primary instance
* Database engine version upgrades happen on primary for Aurora MySQL whereas all instances are updated together for RDS MySQL

### Question 52:
A retail company has hired you as an AWS Certified Solutions Architect Professional to provide consultancy for managing a serverless application that consists of multiple API gateways, Lambda functions, S3 buckets and DynamoDB tables. The company is getting reports from customers that some of the application components seem to be lagging while loading dynamic images and some are timing out with the "504 Gateway Timeout" error. As part of your investigations to identify the root cause behind this issue, you can confirm that DynamoDB monitoring metrics are at acceptable levels.
* Process and analyze the Amazon CloudWatch Logs for Lambda function to determine processing times for requested images at pre-configured intervals
* Process and analyze the AWS X-Ray traces and analyze HTTP methods to determine the root cause of the HTTP errors
* Process and analyze the VPC Flow Logs to determine if there is packet loss between the Lambda function and S3
* Enable execution logging for the API Gateway. Process and analyze the execution logs in the API Gateway for HTTP errors to determine the root cause of the errors
* Enable access logging for the API Gateway. Process and analyze the access logs in the API Gateway for HTTP errors to determine the root cause of the errors

### Question 53:
A leading medical imaging equipment and diagnostic imaging solutions provider uses AWS Cloud to run its healthcare data flows through more than 500,000 medical imaging devices globally. The solutions provider stores close to one petabyte of medical imaging data on Amazon S3 to provide the durability and reliability needed for their critical data. A research assistant working with the radiology department is trying to upload a high-resolution image into S3 via the public internet. The image size is approximately 5GB. The research assistant is using S3 Transfer Acceleration (S3TA) for faster image upload. It turns out that S3TA did not result in an accelerated transfer.
* The research assistant only needs to pay S3TA transfer charges for the image upload
* The research assistant does not need to pay any transfer charges for the image upload
* The research assistant only needs to pay S3 transfer charges for the image upload
* The research assistant needs to pay both S3 transfer charges and S3TA transfer charges for the image upload

### Question 54:
An e-commerce company wants to test its blue-green deployment on the customer base in the next couple of days. Most of the customers use mobile phones which are prone to DNS caching. The company has only two days left before the big sale will be launched.
* Use AWS CodeDeploy deployment options to choose the right deployment
* Use AWS Global Accelerator to distribute a portion of traffic to a particular deployment
* Use Elastic Load Balancer to distribute traffic across deployments
* Use Route 53 weighted routing to spread traffic across different deployments

### Question 55:
A leading car information and shopping platform helps more than 20 million web and mobile users each month browse automobile dealer inventory, read vehicle reviews, and consume other automobile-related content by leveraging its library of 50 million vehicle photos uploaded by auto dealers. The company is planning a key update with even better image quality and faster load times on the company's website as well as mobile apps but the existing image-handling solution based on Cloudera MapReduce clusters is not the right tool for the job. The company now wants to switch to a serverless solution on AWS Cloud. As part of this process, the engineering team has been studying various best practices for serverless solutions. They intend to use AWS Lambda extensively and are looking at the salient features to consider when using Lambda as the backbone for the serverless architecture.
* The bigger your deployment package, the slower your Lambda function will cold-start. Hence, AWS suggests packaging dependencies as a separate package from the actual Lambda package
* Serverless architecture and containers complement each other and you should leverage Docker containers within the Lambda functions
* Lambda allocates compute power in proportion to the memory you allocate to your function. AWS, thus recommends to over provision your function time out settings for the proper performance of Lambda functions
* By default, Lambda functions always operate from an AWS-owned VPC and hence have access to any public internet address or public AWS APIs. Once a Lambda function is VPC-enabled, it will need a route through a NAT gateway in a public subnet to access public resources
* Since Lambda functions can scale extremely quickly, it's a good idea to deploy a CloudWatch Alarm that notifies your team when function metrics such as ConcurrentExecutions or Invocations exceeds the expected threshold
* If you intend to reuse code in more than one Lambda function, you should consider creating a Lambda Layer for the reusable code

### Question 56:
An e-commerce company has hired an AWS Certified Solutions Architect Professional to design a dual-tier storage layer for its flagship application running on EC2 instances. One of the tiers of this storage layer is a data tier that should support a POSIX file system shared across many systems. The other tier of this storage layer is a service tier that supports static file content that requires block storage with more than 100k IOPS.
* Use EFS as the data tier of the storage layer
* Use Amazon S3 as the data tier of the storage layer
* Use EC2 Instance Store as the data tier of the storage layer
* Use EBS volumes with Provisioned IOPS as the service tier of the storage layer
* Use EC2 Instance Store as the service tier of the storage layer

### Question 57:
A social media company is transitioning its IT infrastructure from its on-premises data center to the AWS Cloud. The company wants to move its data artifacts, 200 TB in total size, to Amazon S3 on the AWS Cloud in the shortest possible time. The company has hired you as an AWS Certified Solutions Architect Professional to provide consultancy for this data migration. In terms of the networking infrastructure, the company has a 500 Mbps Direct Connect connection to the AWS Cloud as well as an IPSec based AWS VPN connection using the public internet that supports a bandwidth of 1 Gbps.
* Leverage the 1Gbps IPSec based AWS VPN connection to transfer the data to S3 over the public internet
* Order three AWS Snowball Edge appliances, split and transfer the data to these three appliances and ship them to AWS which will then copy the data from the Snowball Edge appliances to S3
* Leverage S3 Transfer Acceleration to transfer the data to S3
* Leverage the 500 Mbps Direct Connect connection to transfer the data to S3 over the dedicated connection

### Question 58:
A multi-national digital media company wants to exit out of the business of owning and maintaining its own IT infrastructure so it can redeploy resources toward innovation in Artificial Intelligence and other areas to create a better customer experience. As part of this digital transformation, the media company wants to archive about 9 PB of data in its on-premises data center to durable long term storage.
* Transfer the on-premises data into a Snowmobile device. Copy the Snowmobile data into Amazon S3 and create a lifecycle policy to transition the data into AWS Glacier
* Transfer the on-premises data into a Snowmobile device. Copy the Snowmobile data directly into AWS Glacier
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data into Amazon S3 and create a lifecycle policy to transition the data into AWS Glacier
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data directly into AWS Glacier

### Question 59:
A global SaaS company has recently migrated its technology infrastructure from its on-premises data center to AWS Cloud. The engineering team has provisioned an RDS MySQL DB cluster for the company's flagship application. An analytics workload also runs on the same database which publishes near real-time reports for the management of the company. When the analytics workload runs, it slows down the SaaS application as well, resulting in bad user experience.
* For Disaster Recovery purposes, create a Read Replica in another Region as the Master database and point the analytics workload there
* Create a Read Replica in the same Region as the Master database and point the analytics workload there
* Migrate the analytics application to AWS Lambda
* Enable Multi-AZ for the RDS database and run the analytics workload on the standby database

### Question 60:
A Wall Street based trading firm uses AWS Cloud for its IT infrastructure. The firm runs several trading-risk simulation applications, developing complex algorithms to simulate diverse scenarios in order to evaluate the financial health of its customers. The firm stores customers' financial records on Amazon S3. The engineering team needs to implement an archival solution based on Amazon S3 Glacier to enforce regulatory and compliance controls on data access.
* Use S3 Glacier to store the sensitive archived data and then use an S3 Access Control List to enforce compliance controls
* Use S3 Glacier vault to store the sensitive archived data and then use an S3 Access Control List to enforce compliance controls
* Use S3 Glacier vault to store the sensitive archived data and then use a vault lock policy to enforce compliance controls
* Use S3 Glacier to store the sensitive archived data and then use an S3 lifecycle policy to enforce compliance controls

### Question 61:
An e-commerce company runs a data archival workflow once a month for its on-premises data center which is connected to the AWS Cloud over a minimally used 10-Gbps Direct Connect connection using a private virtual interface to its virtual private cloud (VPC). The company internet connection is 200 Mbps, and the usual archive size is around 140 TB that is created on the first Friday of a month. The archive must be transferred and available in Amazon S3 by the next Monday morning.
* Configure a public virtual interface on the 10-Gbps Direct Connect connection and then copy the data to S3 over the connection
* Order multiple AWS Snowball Edge appliances, transfer the data in parallel to these appliances and ship them to AWS which will then copy the data from the Snowball Edge appliances to S3
* Configure a private virtual interface on the 10-Gbps Direct Connect connection and then copy the data securely to S3 over the connection
* Configure a VPC endpoint for S3 and then leverage the Direct Connect connection for data transfer with VPC endpoint as the target

### Question 62:
A retail company recently saw a huge spike in its monthly AWS spend. Upon further investigation, it was found that some developers had accidentally launched Amazon RDS instances in unexpected Regions. The company has hired you as an AWS Certified Solutions Architect Professional to establish best practices around least privileges for developers and control access to on-premises as well as AWS Cloud resources using Active Directory. The company has mandated you to institute a mechanism to control costs by restricting the level of access that developers have to the AWS Management Console without impacting their productivity. The company would also like to allow developers to launch RDS instances only in us-east-1 Region without limiting access to other services in any Region.
* Configure SAML-based authentication tied to an IAM role that has the AdministrativeAccess managed policy attached to it. Attach a customer-managed policy that denies access to RDS in any AWS Region except us-east-1
* Configure SAML-based authentication tied to an IAM role that has the PowerUserAccess managed policy attached to it. Attach a customer-managed policy that denies access to RDS in any AWS Region except us-east-1
* Set up an IAM user for each developer and add them to the developer IAM group that has the PowerUserAccess managed policy attached to it. Attach a customer-managed policy that allows the developers access to RDS only in us-east-1 Region
* Configure SAML-based authentication tied to an IAM role that has a PowerUserAccess managed policy and a customer-managed policy that denies all the developers access to any AWS services except AWS Service Catalog. Within AWS Service Catalog, create a product containing only RDS service in us-east-1 region

### Question 63:
A healthcare company provides solutions for diagnostic, treatment and preventative care in the US. The company uses data to drive decisions, and when its on-premises database solutions couldn’t handle the amount of data in 37 million records, the company migrated to Amazon Redshift. The engineering team at the company is now working on the Disaster Recovery (DR) plans for the Redshift cluster deployed in the eu-west-1 Region. The existing cluster is encrypted via AWS KMS and the team wants to copy the Redshift snapshots to another Region to meet the DR requirements.
* Create an IAM role in destination Region with access to the KMS key in the source Region. Create a snapshot copy grant in the destination Region for this KMS key in the source Region. Configure Redshift cross-Region snapshots in the source Region
* Create a snapshot copy grant in the destination Region for a KMS key in the destination Region. Configure Redshift cross-Region replication in the source Region
* Create a snapshot copy grant in the destination Region for a KMS key in the destination Region. Configure Redshift cross-Region snapshots in the source Region
* Create a snapshot copy grant in the source Region for a KMS key in the source Region. Configure Redshift cross-Region snapshots in the destination Region

### Question 64:
A digital marketing company uses S3 to store artifacts that may only be accessible to an EC2 instance X in a given VPC. The security team at the company is apprehensive about an attack vector wherein any team member with access to this instance could also set up an EC2 instance in another VPC to access these artifacts.
* Set up a highly restricted Security Group for the EC2 instance X and create an S3 bucket policy to allow access only from this Security Group
* Configure an S3 VPC endpoint and create an S3 bucket policy to allow access only from this VPC endpoint
* Set up an IAM role that allows access to the artifacts in S3 and create an S3 bucket policy to allow access only from this role attached to the instance profile
* Attach an Elastic IP to the EC2 instance X and create an S3 bucket policy to allow access only from this Elastic IP

### Question 65:
The world’s largest cable company uses AWS in a hybrid environment to innovate and deploy features for its flagship video product, XFINITY X1, several times a week. The company uses AWS products such as Amazon Virtual Private Cloud (Amazon VPC) and Amazon Direct Connect to deliver the scalability and security needed for rapidly innovating in a hybrid environment. As part of an internal product roadmap, the engineering team at the company has created a private hosted zone and associated it with a virtual private cloud (VPC). However, the domain names remain unresolved, resulting in errors.
* DNS hostnames and DNS resolution should be enabled for private hosted zones
* There is a private hosted zone and a Resolver rule that routes traffic to your network for the same domain name resulting in an ambiguous routing rule
* The private and public hosted zones should not have overlapping namespaces
* Name server (NS) record and Start Of Authority (SOA) records should have the correct configurations

### Question 66:
A blog hosting company has an existing SaaS product architected as an on-premises three-tier web application. The blog content is posted and updated several times a day by multiple authors, so the Linux web servers serve content from a centralized file share on a NAS server. The CTO at the company has done an extensive technical review and highlighted to the company management that the existing infrastructure is not optimized. The company would like to migrate to AWS so that the resources can be dynamically scaled in response to load. The on-premises infrastructure and AWS Cloud are connected using Direct Connect.
* Provision a cluster of EC2 instances based web servers running behind an Application Load Balancer on AWS. Share an EBS volume among all instances for accessing the content. Develop custom code to periodically synchronize this volume with the NAS server
* Provision EC2 instances based web servers with an Auto Scaling group. Create a nightly data transfer batch job to update the web server instances from the NAS server
* Set up an on-premises file gateway using Storage Gateway to replace the NAS server and then replicate the existing content to AWS. On the AWS Cloud, mount the same Storage Gateway bucket to the EC2 instance based web servers to serve the content
* Attach an EFS file system to the on-premises servers to act as the NAS server. Mount the same EFS file system to the AWS based web servers running on EC2 instances to serve the content

### Question 67:
A financial services company has multiple AWS accounts hosting its portfolio of IT applications that serve the company's retail and enterprise customers. A CloudWatch Logs agent is installed on each of the EC2 instances running these IT applications. The company wants to aggregate all security events in a centralized AWS account dedicated to log storage. The centralized operations team at the company needs to perform near-real-time gathering and collating events across multiple AWS accounts.
* Set up CloudWatch Logs agents to publish data to a Kinesis Data Firehose stream in the centralized logging AWS account. Create a Lambda function to read messages from the stream and push messages to Kinesis Data Firehose and then store the data in S3
* Set up Kinesis Data Streams in the logging account and then subscribe the stream to CloudWatch Logs streams in each application AWS account via subscription filters. Configure an Amazon Kinesis Data Firehose delivery stream with the Data Streams as its source and persist the log data in an Amazon S3 bucket inside the logging AWS account
* Set up CloudWatch Logs streams in each application AWS account to forward events to CloudWatch Logs in the centralized logging AWS account. In the centralized logging AWS account, subscribe a Kinesis Data Firehose stream to Amazon CloudWatch Events and further use the Firehose stream to store the log data in S3
* Set up a new IAM role in each application AWS account with permissions to view CloudWatch Logs. Create a Lambda function to assume this new role and perform an hourly export of each AWS account's CloudWatch Logs data to an S3 bucket in the centralized logging AWS account

### Question 68:
A mobile app based social media company is using Amazon CloudFront to deliver media-rich content to its audience across the world. The Content Delivery Network (CDN) offers a multi-tier cache by default, with regional edge caches that improve latency and lower the load on the origin servers when the object is not already cached at the edge. However, there are certain content types that bypass the regional edge cache and go directly to the origin.
* E-commerce assets such as product photos
* Static content such as style sheets, JavaScript files
* User-generated videos
* Proxy methods PUT/POST/PATCH/OPTIONS/DELETE go directly to the origin
* Dynamic content, as determined at request time (cache-behavior configured to forward all headers)

### Question 69:
A leading telecommunications company has built a portfolio of Software-as-a-Service applications focusing on voice, video, chat, contact center, and enterprise-class API solutions powered by one global cloud communications platform. As part of this strategy, they have developed their multi-cloud storage (MCS) solution on Amazon RDS for MySQL but it's running into performance issues despite using Read Replicas. The company has hired you as an AWS Certified Solutions Architect Professional to address these performance-related challenges on an urgent basis without moving away from the underlying relational database schema. The company has branch offices across the world, and it needs the solution to work on a global scale.
* Use Amazon Aurora Global Database to enable fast local reads with low latency in each region
* Use Amazon DynamoDB Global Tables to provide fast, local, read and write performance in each region
* Spin up EC2 instances in each AWS region, install MySQL databases and migrate the existing data into these new databases
* Spin up a Redshift cluster in each AWS region. Migrate the existing data into Redshift clusters

### Question 70:
A financial services provider recently migrated to AWS Cloud as it needed high-powered computing to run financial simulations to value and manage insurance retirement products by leveraging its financial simulation platform to reduce simulation time by leveraging GPU optimized instances. The DevOps team at the company has provisioned a new GPU optimized EC2 instance X by choosing the default security group of the default VPC. The team can ping instance X from other instances in the VPC. The other instances were also created using the default security group. The next day, the team launches another GPU optimized instance Y by creating a new security group and attaching it to instance Y. All other configuration options for instance Y are chosen as default. However, the team is not able to ping instance Y from other instances in the VPC.
* Instance X is in the default security group. The default rules for the default security group allow no inbound traffic from network interfaces (and their associated instances) that are assigned to the same security group. Instance Y is in a new security group. The default rules for a security group that you create allow inbound traffic from all sources
* Instance X is in the default security group. The default rules for the default security group allow inbound traffic from all sources. Instance Y is in a new security group. The default rules for a security group that you create allow no inbound traffic
* Instance X is in the default security group. The default rules for the default security group allow inbound traffic from network interfaces (and their associated instances) that are assigned to the same security group. Instance Y is in a new security group. The default rules for a security group that you create allow no inbound traffic
* Instance X is in the default security group. The default rules for the default security group allow no inbound traffic from all sources. Instance Y is in a new security group. The default rules for a security group that you create allow inbound traffic from all sources

### Question 71:
A healthcare technology solutions company recently faced a security event resulting in an S3 bucket with sensitive data containing Personally Identifiable Information (PII) for patients being made public. The company policy mandates never to have public S3 objects so the Governance and Compliance team must be notified immediately as soon as any public objects are identified. The company has hired you as an AWS Certified Solutions Architect Professional to help build a solution that detects the presence of a public S3 object, which in turn sets off an alarm to trigger notifications and then automatically remediates the said object.
* Enable object-level logging for S3. When a PutObject API call is made with a public-read permission, use S3 event notifications to trigger a Lambda that sends a notification via SNS
* Leverage AWS Access Analyzer to check for S3 bucket public-read permissions and invoke a Lambda function to send a notification via SNS as soon as a public object is uploaded
* Configure a Lambda function as one of the SNS topic subscribers, which is invoked to secure the objects in the S3 bucket
* Enable object-level logging for S3. Set up a CloudWatch event pattern when a PutObject API call with public-read permission is detected in the AWS CloudTrail logs and set the target as an SNS topic for downstream notifications
* Leverage AWS Trusted Advisor to check for S3 bucket public-read permissions and invoke a Lambda function to send a notification via SNS as soon as a public object is uploaded

### Question 72:
A global apparel, footwear, and accessories retailer uses Amazon S3 for centralized storage of the static media assets such as images and videos for its products. The product planning specialists typically upload and download video files (about 100MB each) to the same S3 bucket as part of their day to day work. Initially, the product planning specialists were based out of a single region and there were no performance issues. However, as the company grew and started running offices from multiple countries, it resulted in poor latency while accessing data from S3 and uploading data to S3. The company wants to continue with the serverless solution for its storage requirements but wants to improve its performance.
* Create new S3 buckets in every region where the company has an office, so that each office can maintain its storage for the media assets
* Spin up EC2 instances in each region where the company has an office. Create a daily job to transfer S3 data into EBS volumes attached to the EC2 instances
* Use Amazon CloudFront distribution with origin as the S3 bucket. This would speed up uploads as well as downloads for the video files
* Move S3 data into EFS file system created in a US region, connect to EFS file system from EC2 instances in other AWS regions using an inter-region VPC peering connection
* Enable Amazon S3 Transfer Acceleration for the S3 bucket. This would speed up uploads as well as downloads for the video files

### Question 73:
An online florist and gift retailer serves customers in the US as well as Europe. The company recently decided to go all-in on AWS and use the platform to host its website, order and stock management systems and fulfillment applications. The company wants to migrate its on-premises Oracle database to Aurora MySQL. The company has hired an AWS Certified Solutions Architect Professional to carry out the migration with minimal downtime using AWS DMS. The company has mandated that the migration must have minimal impact on the performance of the source database and the Solutions Architect must validate that the data was migrated accurately from the source to the target before the cutover.
* Use AWS Schema Conversion Tool for the migration task so it can compare the source and target data and report any mismatches
* Configure DMS premigration assessment on the migration task so the assessment can compare the source and target data and report any mismatches
* Configure DMS data validation on the migration task so it can compare the source and target data for the DMS task and report any mismatches
* Use the table metrics of the DMS task to verify the statistics for tables being migrated including the DDL statements completed

### Question 74:
The DevOps team at a leading social media company uses Chef to automate the configurations of servers in the on-premises data center. The CTO at the company now wants to migrate the IT infrastructure to AWS Cloud with minimal changes to the server configuration workflows and at the same time account for less operational overhead post-migration to AWS. The company has hired you as an AWS Certified Solutions Architect Professional to recommend a solution for this migration.
* Rehost the IT infrastructure to AWS Cloud by leveraging AWS Elastic Beanstalk as a configuration management service to automate the configurations of servers on AWS
* Replatform the IT infrastructure to AWS Cloud by leveraging AWS OpsWorks as a configuration management service to automate the configurations of servers on AWS
* Rehost the IT infrastructure to AWS Cloud by leveraging AWS OpsWorks as a configuration management service to automate the configurations of servers on AWS
* Replatform the IT infrastructure to AWS Cloud by leveraging AWS Config as a configuration management service to automate the configurations of servers on AWS

### Question 75:
A multi-national bank has recently migrated to AWS Cloud to utilize dedicated instances that are physically isolated at the host hardware level from instances that belong to other AWS accounts. The bank's flagship application is hosted on a fleet of EC2 instances which are part of an Auto Scaling group (ASG). The ASG uses a Launch Configuration (LC-A) with "dedicated" instance placement tenancy but the VPC (VPC-A) used by the Launch Configuration LC-A has the instance tenancy set to default. Later the engineering team creates a new Launch Configuration (LC-B) with "default" instance placement tenancy but the VPC (VPC-B) used by the Launch Configuration LC-B has the instance tenancy set to dedicated.
* The instances launched by both Launch Configuration LC-A and Launch Configuration LC-B will have default instance tenancy
* The instances launched by both Launch Configuration LC-A and Launch Configuration LC-B will have dedicated instance tenancy
* The instances launched by Launch Configuration LC-A will have default instance tenancy while the instances launched by the Launch Configuration LC-B will have dedicated instance tenancy
* The instances launched by Launch Configuration LC-A will have dedicated instance tenancy while the instances launched by the Launch Configuration LC-B will have default instance tenancy
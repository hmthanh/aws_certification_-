# Begin_AWS Certified Solutions Architect Associate

# Exam 1

### Question 1:
The planetary research program at an ivy-league university is assisting NASA to find potential landing sites for exploration vehicles of unmanned missions to our neighboring planets. The program uses High Performance Computing (HPC) driven application architecture to identify these landing sites.
* The EC2 instances should be deployed in an Auto Scaling group so that application meets high availability requirements
* The EC2 instances should be deployed in a partition placement group so that distributed workloads can be handled effectively
* The EC2 instances should be deployed in a cluster placement group so that the underlying workload can benefit from low network latency and high network throughput
* The EC2 instances should be deployed in a spread placement group so that there are no correlated failures

### Question 2:
A social photo-sharing company uses Amazon S3 to store the images uploaded by the users. These images are kept encrypted in S3 by using AWS-KMS and the company manages its own Customer Master Key (CMK) for encryption. A member of the DevOps team accidentally deleted the CMK a day ago, thereby rendering the user's photo data unrecoverable. You have been contacted by the company to consult them on possible solutions to this crisis.
* As the CMK was deleted a day ago, it must be in the 'pending deletion' status and hence you can just cancel the CMK deletion and recover the key
* The company should issue a notification on its web application informing the users about the loss of their data
* Contact AWS support to retrieve the CMK from their backup
* The CMK can be recovered by the AWS root account user

### Question 3:
A media company wants to get out of the business of owning and maintaining its own IT infrastructure. As part of this digital transformation, the media company wants to archive about 5PB of data in its on-premises data center to durable long term storage.
* Setup Site-to-Site VPN connection between the on-premises data center and AWS Cloud. Use this connection to transfer the data into AWS Glacier
* Setup AWS direct connect between the on-premises data center and AWS Cloud. Use this connection to transfer the data into AWS Glacier
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data into Amazon S3 and create a lifecycle policy to transition the data into AWS Glacier
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data into AWS Glacier

### Question 4:
An IT consultant is helping the owner of a medium-sized business set up an AWS account. What are the security recommendations he must follow while creating the AWS account root user? (Select two)
* Send an email to the business owner with details of the login username and password for the AWS root user. This will help the business owner to troubleshoot any login issues in future
* Enable Multi Factor Authentication (MFA) for the AWS account root user account
* Create a strong password for the AWS account root user
* Encrypt the access keys and save them on Amazon S3
* Create AWS account root user access keys and share those keys only with the business owner

### Question 5:
A silicon valley based startup focused on the advertising technology (ad tech) space uses DynamoDB as a data store for storing various kinds of marketing data, such as user profiles, user events, clicks, and visited links. Some of these use-cases require a high request rate (millions of requests per second), low predictable latency, and reliability. The startup now wants to add a caching layer to support high read volumes.
* RDS
* ElastiCache
* Redshift
* Elasticsearch
* DynamoDB Accelerator (DAX)

### Question 6:
A US-based non-profit organization develops learning methods for primary and secondary vocational education, delivered through digital learning platforms, which are hosted on AWS under a hybrid cloud setup. After experiencing stability issues with their cluster of self-managed RabbitMQ message brokers, the organization wants to explore an alternate solution on AWS.
* Amazon Simple Notification Service (Amazon SNS)
* Amazon SQS Standard
* Amazon SQS FIFO (First-In-First-Out)
* Amazon MQ

### Question 7:
A leading carmaker would like to build a new car-as-a-sensor service by leveraging fully serverless components that are provisioned and managed automatically by AWS. The development team at the carmaker does not want an option that requires the capacity to be manually provisioned, as it does not want to respond manually to changing volumes of sensor data.
* Ingest the sensor data in a Kinesis Data Stream, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in a Kinesis Data Stream, which is polled by a Lambda function in batches and the data is written into an auto-scaled DynamoDB table for downstream processing
* Ingest the sensor data in an Amazon SQS standard queue, which is polled by an application running on an EC2 instance and the data is written into an auto-scaled DynamoDB table for downstream processing

### Question 8:
The engineering team at an in-home fitness company is evaluating multiple in-memory data stores with the ability to power its on-demand, live leaderboard. The company's leaderboard requires high availability, low latency, and real-time processing to deliver customizable user data for the community of users working out together virtually from the comfort of their home.
* Power the on-demand, live leaderboard using DynamoDB with DynamoDB Accelerator (DAX) as it meets the in-memory, high availability, low latency requirements
* Power the on-demand, live leaderboard using AWS Neptune as it meets the in-memory, high availability, low latency requirements
* Power the on-demand, live leaderboard using RDS Aurora as it meets the in-memory, high availability, low latency requirements
* Power the on-demand, live leaderboard using ElastiCache Redis as it meets the in-memory, high availability, low latency requirements
* Power the on-demand, live leaderboard using DynamoDB as it meets the in-memory, high availability, low latency requirements

### Question 9:
One of the largest healthcare solutions provider in the world uses Amazon S3 to store and protect a petabyte of critical medical imaging data for its AWS based Health Cloud service, which connects hundreds of thousands of imaging machines and other medical devices. The engineering team has observed that while some of the objects in the imaging data bucket are frequently accessed, others sit idle for a considerable span of time.
* Store the objects in the imaging data bucket using the S3 Standard-IA storage class
* Store the objects in the imaging data bucket using the S3 Intelligent-Tiering storage class
* Create a data monitoring application on an EC2 instance in the same region as the imaging data bucket. The application is triggered daily via CloudWatch and it changes the storage class of infrequently accessed objects to S3 One Zone-IA and the frequently accessed objects are migrated to S3 Standard class
* Create a data monitoring application on an EC2 instance in the same region as the imaging data bucket. The application is triggered daily via CloudWatch and it changes the storage class of infrequently accessed objects to S3 Standard-IA and the frequently accessed objects are migrated to S3 Standard class

### Question 10:
The DevOps team at an analytics company has noticed that the performance of its proprietary Machine Learning workflow has deteriorated ever since a new Auto Scaling group was deployed a few days back. Upon investigation, the team found out that the Launch Configuration selected for the Auto Scaling group is using the incorrect instance type that is not optimized to handle the Machine Learning workflow.
* Modify the launch configuration to use the correct instance type and continue to use the existing Auto Scaling group
* No need to modify the launch configuration. Just modify the Auto Scaling group to use the correct instance type
* Create a new launch configuration to use the correct instance type. Modify the Auto Scaling group to use this new launch configuration. Delete the old launch configuration as it is no longer needed
* No need to modify the launch configuration. Just modify the Auto Scaling group to use more number of existing instance types. More instances may offset the loss of performance

### Question 11:
A silicon valley based research group is working on a High Performance Computing (HPC) application in the area of Computational Fluid Dynamics. The application carries out simulations of the external aerodynamics around a car and needs to be deployed on EC2 instances with a requirement for high levels of inter-node communications and high network traffic between the instances.
* Deploy EC2 instances behind a Network Load Balancer
* Deploy EC2 instances in a partition placement group
* Deploy EC2 instances in a spread placement group
* Deploy EC2 instances in a cluster placement group
* Deploy EC2 instances with Elastic Fabric Adapter

### Question 12:
The engineering team at a Spanish professional football club has built a notification system on the web platform using Amazon SNS notifications which are then handled by a Lambda function for end-user delivery. During the off-season, the notification systems need to handle about 100 requests per second. During the peak football season, the rate touches about 5000 requests per second and it is noticed that a significant number of the notifications are not being delivered to the end-users on the web platform.
* Amazon SNS message deliveries to AWS Lambda have crossed the account concurrency quota for Lambda, so the team needs to contact AWS support to raise the account limit
* The engineering team needs to provision more servers running the SNS service
* The engineering team needs to provision more servers running the Lambda service
* Amazon SNS has hit a scalability limit, so the team needs to contact AWS support to raise the account limit

### Question 13:
A software engineering intern at an e-commerce company is documenting the process flow to provision EC2 instances via the Amazon EC2 API. These instances are to be used for an internal application that processes HR payroll data. He wants to highlight those volume types that cannot be used as a boot volume.
* Throughput Optimized HDD (st1)
* Cold HDD (sc1)
* Instance Store
* General Purpose SSD (gp2)
* Provisioned IOPS SSD (io1)

### Question 14:
A streaming solutions company is building a video streaming product by using an Application Load Balancer (ALB) that routes the requests to the underlying EC2 instances. The engineering team has noticed a peculiar pattern. The ALB removes an instance whenever it is detected as unhealthy but the Auto Scaling group fails to kick-in and provision the replacement instance.
* The Auto Scaling group is using EC2 based health check and the Application Load Balancer is using ALB based health check
* Both the Auto Scaling group and Application Load Balancer are using EC2 based health check
* The Auto Scaling group is using ALB based health check and the Application Load Balancer is using EC2 based health check
* Both the Auto Scaling group and Application Load Balancer are using ALB based health check

### Question 15:
The engineering team at a leading online real estate marketplace uses Amazon MySQL RDS because it simplifies much of the time-consuming administrative tasks typically associated with databases. The team uses Multi-Availability Zone (Multi-AZ) deployment to further automate its database replication and augment data durability and also deploys read replicas. A new DevOps engineer has joined the team and wants to understand the replication capabilities for Multi-AZ as well as Read-replicas.
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows synchronous replication and spans at least two Availability Zones within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans one Availability Zone within a single region. Read replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region

### Question 16:
An IT Company wants to move all the compute components of its AWS Cloud infrastructure into serverless architecture. Their development stack comprises a mix of backend programming languages and the company would like to explore the support offered by the AWS Lambda runtime for their programming languages stack.
* C#/.NET
* C
* Go
* PHP
* R

### Question 17:
A file hosting startup offers cloud storage and file synchronization services to its end users. The file-hosting service uses Amazon S3 under the hood to power its storage offerings. Currently all the customer files are uploaded directly under a single S3 bucket. The engineering team has started seeing scalability issues where customer file uploads have started failing during the peak access hours in the evening with more than 5000 requests per second.
* Change the application architecture to use EFS instead of Amazon S3 for storing the customers' uploaded files
* Change the application architecture to create a new S3 bucket for each customer and then upload each customer's files directly under the respective buckets
* Change the application architecture to create a new S3 bucket for each day's data and then upload the daily files directly under that day's bucket
* Change the application architecture to create customer-specific custom prefixes within the single bucket and then upload the daily files into those prefixed locations

### Question 18:
A social media analytics company uses a fleet of EC2 servers to manage its analytics workflow. These EC2 servers operate under an Auto Scaling group. The engineers at the company want to be able to download log files whenever an instance terminates because of a scale-in event from an auto-scaling policy.
* Auto Scaling group lifecycle hook
* EC2 instance meta data
* Auto Scaling group scheduled action
* EC2 instance user data

### Question 19:
A large financial institution operates an on-premises data center with hundreds of PB of data managed on Microsoft’s Distributed File System (DFS). The CTO wants the organization to transition into a hybrid cloud environment and run data-intensive analytics workloads that support DFS.
* Microsoft SQL Server on Amazon
* AWS Managed Microsoft AD
* Amazon FSx for Lustre
* Amazon FSx for Windows File Server

### Question 20:
The engineering team at an e-commerce company wants to set up a custom domain for internal usage such as internaldomainexample.com. The team wants to use the private hosted zones feature of Route 53 to accomplish this.
* enableVpcHostnames
* enableDnsSupport
* enableVpcSupport
* enableDnsDomain
* enableDnsHostnames

### Question 21:
A silicon valley based startup uses a fleet of EC2 servers to manage its CRM application. These EC2 servers are behind an Elastic Load Balancer (ELB). Which of the following configurations are NOT allowed for the Elastic Load Balancer?
* Use the ELB to distribute traffic for four EC2 instances. All the four instances are deployed in Availability Zone B of us-west-1 region
* Use the ELB to distribute traffic for four EC2 instances. All the four instances are deployed across two Availability Zones of us-east-1 region
* Use the ELB to distribute traffic for four EC2 instances. Two of these instances are deployed in Availability Zone A of us-east-1 region and the other two instances are deployed in Availability Zone B of us-west-1 region
* Use the ELB to distribute traffic for four EC2 instances. All the four instances are deployed in Availability Zone A of us-east-1 region

### Question 22:
A global media company is using Amazon CloudFront to deliver media-rich content to its audience across the world. The Content Delivery Network (CDN) offers a multi-tier cache by default, with regional edge caches that improve latency and lower the load on the origin servers when the object is not already cached at the edge. However there are certain content types that bypass the regional edge cache, and go directly to the origin.
* Static content such as style sheets, JavaScript files
* User-generated videos
* E-commerce assets such as product photos
* Proxy methods PUT/POST/PATCH/OPTIONS/DELETE go directly to the origin
* Dynamic content, as determined at request time (cache-behavior configured to forward all headers)

### Question 23:
A video analytics organization has been acquired by a leading media company. The analytics organization has 10 independent applications with an on-premises data footprint of about 70TB for each application. The media company has its IT infrastructure on the AWS Cloud. The terms of the acquisition mandate that the on-premises data should be migrated into AWS Cloud and the two organizations establish connectivity so that collaborative development efforts can be pursued. The CTO of the media company has set a timeline of one month to carry out this transition.
* Order 10 Snowball Edge Storage Optimized devices to complete the one-time data transfer
* Setup AWS direct connect to establish connectivity between the on-premises data center and AWS Cloud
* Order 70 Snowball Edge Storage Optimized devices to complete the one-time data transfer
* Order 1 Snowmobile to complete the one-time data transfer
* Setup Site-to-Site VPN to establish connectivity between the on-premises data center and AWS Cloud

### Question 24:
A biotechnology company wants to seamlessly integrate its on-premises data center with AWS cloud-based IT systems which would be critical to manage as well as scale-up the complex planning and execution of every stage of its drug development process. As part of a pilot program, the company wants to integrate data files from its analytical instruments into AWS via an NFS interface.
* AWS Storage Gateway - Volume Gateway
* AWS Storage Gateway - Tape Gateway
* AWS Site-to-Site VPN
* AWS Storage Gateway - File Gateway

### Question 25:
A leading social media analytics company is contemplating moving its dockerized application stack into AWS Cloud. The company is not sure about the pricing for using Elastic Container Service (ECS) with the EC2 launch type compared to the Elastic Container Service (ECS) with the Fargate launch type.
* ECS with EC2 launch type is charged based on EC2 instances and EBS volumes used. ECS with Fargate launch type is charged based on vCPU and memory resources that the containerized application requests
* Both ECS with EC2 launch type and ECS with Fargate launch type are charged based on EC2 instances and EBS volumes used
* Both ECS with EC2 launch type and ECS with Fargate launch type are just charged based on Elastic Container Service used per hour
* Both ECS with EC2 launch type and ECS with Fargate launch type are charged based on vCPU and memory resources that the containerized application requests

### Question 26:
The development team at an e-commerce startup has set up multiple microservices running on EC2 instances under an Application Load Balancer. The team wants to route traffic to multiple back-end services based on the URL path of the HTTP header. So it wants requests for https://www.example.com/orders to go to a specific microservice and requests for https://www.example.com/products to go to another microservice.
* Path-based Routing
* Host-based Routing
* HTTP header-based routing
* Query string parameter-based routing

### Question 27:
A gaming company uses Amazon Aurora as its primary database service. The company has now deployed 5 multi-AZ read replicas to increase the read throughput and for use as failover target. The replicas have been assigned the following failover priority tiers and corresponding sizes are given in parentheses: tier-1 (16TB), tier-1 (32TB), tier-10 (16TB), tier-15 (16TB), tier-15 (32TB).
* Tier-10 (16TB)
* Tier-1 (16TB)
* Tier-15 (32TB)
* Tier-1 (32TB)

### Question 28:
One of the biggest football leagues in Europe has granted the distribution rights for live streaming its matches in the US to a silicon valley based streaming services company. As per the terms of distribution, the company must make sure that only users from the US are able to live stream the matches on their platform. Users from other countries in the world must be denied access to these live-streamed matches.
* Use Route 53 based weighted routing policy to restrict distribution of content to only the locations in which you have distribution rights
* Use Route 53 based failover routing policy to restrict distribution of content to only the locations in which you have distribution rights
* Use Route 53 based geolocation routing policy to restrict distribution of content to only the locations in which you have distribution rights
* Use georestriction to prevent users in specific geographic locations from accessing content that you're distributing through a CloudFront web distribution
* Use Route 53 based latency routing policy to restrict distribution of content to only the locations in which you have distribution rights

### Question 29:
The data engineering team at an e-commerce company has set up a workflow to ingest the clickstream data into the raw zone of the S3 data lake. The team wants to run some SQL based data sanity checks on the raw zone of the data lake.
* Load the incremental raw zone data into Redshift on an hourly basis and run the SQL based sanity checks
* Use Athena to run SQL based analytics against S3 data
* Load the incremental raw zone data into RDS on an hourly basis and run the SQL based sanity checks
* Load the incremental raw zone data into an EMR based Spark Cluster on an hourly basis and use SparkSQL to run the SQL based sanity checks

### Question 30:
The audit department at one of the leading consultancy firms generates and accesses the audit reports only during the last month of a financial year. The department uses AWS Step Functions to orchestrate the report creating process with failover and retry scenarios built into the solution and the data should be available with millisecond latency. The underlying data to create these audit reports is stored on S3 and runs into hundreds of Terabytes.
* Amazon S3 Glacier (S3 Glacier)
* Amazon S3 Standard-Infrequent Access (S3 Standard-IA)
* Amazon S3 Intelligent-Tiering (S3 Intelligent-Tiering)
* Amazon S3 Standard

### Question 31:
The DevOps team at an e-commerce company wants to perform some maintenance work on a specific EC2 instance that is part of an Auto Scaling group using a step scaling policy. The team is facing a maintenance challenge - every time the team deploys a maintenance patch, the instance health check status shows as out of service for a few minutes. This causes the Auto Scaling group to provision another replacement instance immediately.
* Put the instance into the Standby state and then update the instance by applying the maintenance patch. Once the instance is ready, you can exit the Standby state and then return the instance to service
* Take a snapshot of the instance, create a new AMI and then launch a new instance using this AMI. Apply the maintenance patch to this new instance and then add it back to the Auto Scaling Group by using the manual scaling policy. Terminate the earlier instance that had the maintenance issue
* Suspend the ReplaceUnhealthy process type for the Auto Scaling group and apply the maintenance patch to the instance. Once the instance is ready, you can activate the ReplaceUnhealthy process type again
* Delete the Auto Scaling group and apply the maintenance fix to the given instance. Create a new Auto Scaling group and add all the instances again using the manual scaling policy
* Suspend the ScheduledActions process type for the Auto Scaling group and apply the maintenance patch to the instance. Once the instance is ready, you can activate the ScheduledActions process type again

### Question 32:
The engineering team at an online fashion retailer uses AWS Cloud to manage its technology infrastructure. The EC2 server fleet is behind an Application Load Balancer and the fleet strength is managed by an Auto Scaling group. Based on the historical data, the team is anticipating a huge traffic spike during the upcoming Thanksgiving sale.
* Auto Scaling group lifecycle hook
* Auto Scaling group scheduled action
* Auto Scaling group step scaling policy
* Auto Scaling group target tracking scaling policy

### Question 33:
The sourcing team at the US headquarters of a global e-commerce company is preparing a spreadsheet of the new product catalog. The spreadsheet is saved on an EFS file system created in us-east-1 region. The sourcing team counterparts from other AWS regions such as Asia Pacific and Europe also want to collaborate on this spreadsheet.
* The spreadsheet will have to be copied into EFS file systems of other AWS regions as EFS is a regional service and it does not allow access from other AWS regions
* The spreadsheet will have to be copied in Amazon S3 which can then be accessed from any AWS region
* The spreadsheet on the EFS file system can be accessed from EC2 instances running in other AWS regions by using an inter-region VPC peering connection
* The spreadsheet data will have to be moved into an RDS MySQL database which can then be accessed from any AWS region

### Question 34:
The CTO of an online home rental marketplace wants to re-engineer the caching layer of the current architecture for its relational database. He wants the caching layer to have replication and archival support built into the architecture.
* ElastiCache for Redis
* ElastiCache for Memcached
* DocumentDB
* DynamoDB Accelerator (DAX)

### Question 35:
A geological research agency maintains the seismological data for the last 100 years. The data has a velocity of 1GB per minute. You would like to store the data with only the most relevant attributes to build a predictive model for earthquakes.
* Ingest the data in Kinesis Data Analytics and use SQL queries to filter and transform the data before writing to S3
* Ingest the data in Kinesis Data Firehose and use a Lambda function to filter and transform the incoming stream before the output is dumped on S3
* Ingest the data in AWS Glue job and use Spark transformations before writing to S3
* Ingest the data in a Spark Streaming Cluster on EMR use Spark Streaming transformations before writing to S3

### Question 36:
A new DevOps engineer has joined a large financial services company recently. As part of his onboarding, the IT department is conducting a review of the checklist for tasks related to AWS Identity and Access Management.
* Enable MFA for privileged users
* Grant maximum privileges to avoid assigning privileges again
* Configure AWS CloudTrail to log all IAM actions
* Create a minimum number of accounts and share these account credentials among employees
* Use user credentials to provide access specific permissions for Amazon EC2 instances

### Question 37:
An IT company has built a custom data warehousing solution for a retail organization by using Amazon Redshift. As part of the cost optimizations, the company wants to move any historical data (any data older than a year) into S3, as the daily analytical reports consume data for just the last one year. However the analysts want to retain the ability to cross-reference this historical data along with the daily reports. The company wants to develop a solution with the LEAST amount of effort and MINIMUM cost.
* Use the Redshift COPY command to load the S3 based historical data into Redshift. Once the ad-hoc queries are run for the historic data, it can be removed from Redshift
* Use Redshift Spectrum to create Redshift cluster tables pointing to the underlying historical data in S3. The analytics team can then query this historical data to cross-reference with the daily reports from Redshift
* Use Glue ETL job to load the S3 based historical data into Redshift. Once the ad-hoc queries are run for the historic data, it can be removed from Redshift
* Setup access to the historical data via Athena. The analytics team can run historical data queries on Athena and continue the daily reporting on Redshift. In case the reports need to be cross-referenced, the analytics team need to export these in flat files and then do further analysis

### Question 38:
The DevOps team at an e-commerce company has deployed a fleet of EC2 instances under an Auto Scaling group (ASG). The instances under the ASG span two Availability Zones (AZ) within the us-east-1 region. All the incoming requests are handled by an Application Load Balancer (ALB) that routes the requests to the EC2 instances under the ASG. As part of a test run, two instances (instance 1 and 2, belonging to AZ A) were manually terminated by the DevOps team causing the Availability Zones to become unbalanced. Later that day, another instance (belonging to AZ B) was detected as unhealthy by the Application Load Balancer's health check.
* As the Availability Zones got unbalanced, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling terminates old instances before launching new instances, so that rebalancing does not cause extra instances to be launched
* Amazon EC2 Auto Scaling creates a new scaling activity to terminate the unhealthy instance and launch the new instance simultaneously
* Amazon EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it. Later, another scaling activity launches a new instance to replace the terminated instance
* Amazon EC2 Auto Scaling creates a new scaling activity for launching a new instance to replace the unhealthy instance. Later, EC2 Auto Scaling creates a new scaling activity for terminating the unhealthy instance and then terminates it
* As the Availability Zones got unbalanced, Amazon EC2 Auto Scaling will compensate by rebalancing the Availability Zones. When rebalancing, Amazon EC2 Auto Scaling launches new instances before terminating the old ones, so that rebalancing does not compromise the performance or availability of your application

### Question 39:
The DevOps team at a major financial services company uses Multi-Availability Zone (Multi-AZ) deployment for its MySQL RDS database in order to automate its database replication and augment data durability. The DevOps team has scheduled a maintenance window for a database engine level upgrade for the coming weekend.
* Any database engine level upgrade for an RDS DB instance with Multi-AZ deployment triggers both the primary and standby DB instances to be upgraded at the same time. This causes downtime until the upgrade is complete
* Any database engine level upgrade for an RDS DB instance with Multi-AZ deployment triggers the primary DB instance to be upgraded which is then followed by the upgrade of the standby DB instance. This does not cause any downtime for the duration of the upgrade
* Any database engine level upgrade for an RDS DB instance with Multi-AZ deployment triggers both the primary and standby DB instances to be upgraded at the same time. However, this does not cause any downtime until the upgrade is complete
* Any database engine level upgrade for an RDS DB instance with Multi-AZ deployment triggers the standby DB instance to be upgraded which is then followed by the upgrade of the primary DB instance. This does not cause any downtime for the duration of the upgrade

### Question 40:
A news network uses Amazon S3 to aggregate the raw video footage from its reporting teams across the US. The news network has recently expanded into new geographies in Europe and Asia. The technical teams at the overseas branch offices have reported huge delays in uploading large video files to the destination S3 bucket.
* Use Amazon S3 Transfer Acceleration to enable faster file uploads into the destination S3 bucket
* Create multiple site-to-site VPN connections between the AWS Cloud and branch offices in Europe and Asia. Use these VPN connections for faster file uploads into S3
* Use AWS Global Accelerator for faster file uploads into the destination S3 bucket
* Create multiple AWS direct connect connections between the AWS Cloud and branch offices in Europe and Asia. Use the direct connect connections for faster file uploads into S3
* Use multipart uploads for faster file uploads into the destination S3 bucket

### Question 41:
A DevOps engineer at an IT company was recently added to the admin group of the company's AWS account. The AdministratorAccess managed policy is attached to this group.
* Change the password for his own IAM user account
* Configure an Amazon S3 bucket to enable MFA (Multi Factor Authentication) delete
* Delete the IAM user for his manager
* Close the company's AWS account
* Delete an S3 bucket from the production environment

### Question 42:
A technology blogger wants to write a review on the comparative pricing for various storage types available on AWS Cloud. The blogger has created a test file of size 1GB with some random data. Next he copies this test file into AWS S3 Standard storage class, provisions an EBS volume (General Purpose SSD (gp2)) with 100GB of provisioned storage and copies the test file into the EBS volume, and lastly copies the test file into an EFS Standard Storage filesystem. At the end of the month, he analyses the bill for costs incurred on the respective storage types for the test file.
* Cost of test file storage on EBS < Cost of test file storage on S3 Standard < Cost of test file storage on EFS
* Cost of test file storage on EFS < Cost of test file storage on S3 Standard < Cost of test file storage on EBS
* Cost of test file storage on S3 Standard < Cost of test file storage on EFS < Cost of test file storage on EBS
* Cost of test file storage on S3 Standard < Cost of test file storage on EBS < Cost of test file storage on EFS

### Question 43:
An organization wants to delegate access to a set of users from the development environment so that they can access some resources in the production environment which is managed under another AWS account.
* Create new IAM user credentials for the production environment and share these credentials with the set of users from the development environment
* It is not possible to access cross-account resources
* Both IAM roles and IAM users can be used interchangeably for cross-account access
* Create a new IAM role with the required permissions to access the resources in the production environment. The users can then assume this IAM role while accessing the resources from the production environment

### Question 44:
A silicon valley based startup wants to be the global collaboration platform for API development. The product team at the startup has figured out a market need to support both stateful and stateless client-server communications via the APIs developed using its platform. You have been hired by the startup as an AWS solutions architect to build a Proof-of-Concept to fulfill this market need using AWS API Gateway.
* API Gateway creates RESTful APIs that enable stateless client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateful client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateful client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateful, full-duplex communication between client and server
* API Gateway creates RESTful APIs that enable stateless client-server communication and API Gateway also creates WebSocket APIs that adhere to the WebSocket protocol, which enables stateless, full-duplex communication between client and server

### Question 45:
A leading video streaming service delivers billions of hours of content from Amazon S3 to customers around the world. Amazon S3 also serves as the data lake for its big data analytics solution. The data lake has a staging zone where intermediary query results are kept only for 24 hours. These results are also heavily referenced by other parts of the analytics pipeline.
* Store the intermediary query results in S3 One Zone-Infrequent Access storage class
* Store the intermediary query results in S3 Standard storage class
* Store the intermediary query results in S3 Standard-Infrequent Access storage class
* Store the intermediary query results in S3 Intelligent-Tiering storage class

### Question 46:
A junior scientist working with the Deep Space Research Laboratory at NASA is trying to upload a high-resolution image of a nebula into Amazon S3. The image size is approximately 3GB. The junior scientist is using S3 Transfer Acceleration (S3TA) for faster image upload. It turns out that S3TA did not result in an accelerated transfer.
* The junior scientist does not need to pay any transfer charges for the image upload
* The junior scientist only needs to pay S3TA transfer charges for the image upload
* The junior scientist only needs to pay S3 transfer charges for the image upload
* The junior scientist needs to pay both S3 transfer charges and S3TA transfer charges for the image upload

### Question 47:
A chip design startup is running an Electronic Design Automation (EDA) application, which is a high-performance workflow used to simulate performance and failures during the design phase of silicon chip production. The application produces massive volumes of data that can be divided into two categories. The 'hot data' needs to be both processed and stored quickly in a parallel and distributed fashion. The 'cold data' needs to be kept for reference with quick access for reads and updates at a low cost.
* Amazon FSx for Lustre
* Amazon FSx for Windows File Server
* AWS Glue
* Amazon EMR

### Question 48:
The solo founder at a tech startup has just created a brand new AWS account. The founder has provisioned an EC2 instance 1A which is running in region A. Later, he takes a snapshot of the instance 1A and then creates a new AMI in region A from this snapshot. This AMI is then copied into another region B. The founder provisions an instance 1B in region B using this new AMI in region B.
* 1 EC2 instance and 1 AMI exist in region B
* 1 EC2 instance and 1 snapshot exist in region B
* 1 EC2 instance and 2 AMIs exist in region B
* 1 EC2 instance, 1 AMI and 1 snapshot exist in region B

### Question 49:
A company has multiple EC2 instances operating in a private subnet which is part of a custom VPC. These instances are running an image processing application that needs to access images stored on S3. Once each image is processed, the status of the corresponding record needs to be marked as completed in a DynamoDB table.
* Create a separate interface endpoint for S3 and DynamoDB each. Then connect to these services using the private IP address
* Create a gateway endpoint for DynamoDB and add it as a target in the route table of the custom VPC. Create an interface endpoint for S3 and then connect to the S3 service using the private IP address
* Create a gateway endpoint for S3 and add it as a target in the route table of the custom VPC. Create an interface endpoint for DynamoDB and then connect to the DynamoDB service using the private IP address
* Create a separate gateway endpoint for S3 and DynamoDB each. Add two new target entries for these two gateway endpoints in the route table of the custom VPC

### Question 50:
An IT company wants to review its security best-practices after an incident was reported where a new developer on the team was assigned full access to DynamoDB. The developer accidentally deleted a couple of tables from the production environment while building out a new feature.
* The CTO should review the permissions for each new developer's IAM user so that such incidents don't recur
* Remove full database access for all IAM users in the organization
* Only root user should have full database access in the organization
* Use permissions boundary to control the maximum permissions employees can grant to the IAM principals

### Question 51:
The IT department at a consulting firm is conducting a training workshop for new developers. As part of an evaluation exercise on Amazon S3, the new developers were asked to identify the invalid storage class lifecycle transitions for objects stored on S3.
* S3 Standard-IA => S3 Intelligent-Tiering
* S3 Standard-IA => S3 One Zone-IA
* S3 Standard => S3 Intelligent-Tiering
* S3 One Zone-IA => S3 Standard-IA
* S3 Intelligent-Tiering => S3 Standard

### Question 52:
A research group at an ivy-league university needs a fleet of EC2 instances operating in a fault-tolerant architecture for a specialized task that must deliver high random I/O performance. Each instance in the fleet would have access to a dataset that is replicated across the instances. Because of the resilient architecture, the specialized task would continue to be processed even if any of the instances goes down as the underlying application architecture would ensure the replacement instance has access to the required dataset.
* Use EC2 instances with access to S3 based storage
* Use EBS based EC2 instances
* Use Instance Store based EC2 instances
* Use EC2 instances with EFS mount points

### Question 53:
A healthcare startup needs to enforce compliance and regulatory guidelines for objects stored in Amazon S3. One of the key requirements is to provide adequate protection against accidental deletion of objects.
* Establish a process to get managerial approval for deleting S3 objects
* Change the configuration on AWS S3 console so that the user needs to provide additional confirmation while deleting any S3 object
* Enable MFA delete on the bucket
* Create an event trigger on deleting any S3 object. The event invokes an SNS notification via email to the IT manager
* Enable versioning on the bucket

### Question 54:
A digital media streaming company wants to use AWS Cloudfront to distribute its content only to its service subscribers. As a solutions architect, which of the following solutions would you suggest in order to deliver restricted content to the bona fide end users? (Select two)
* Forward HTTPS requests to the origin server by using the ECDSA or RSA ciphers
* Use CloudFront signed cookies
* Require HTTPS for communication between CloudFront and your S3 origin
* Require HTTPS for communication between CloudFront and your custom origin
* Use CloudFront signed URLs

### Question 55:
The payroll department at a company initiates several computationally intensive workloads on EC2 instances at a designated hour on the last day of every month. The payroll department has noticed a trend of severe performance lag during this hour. The engineering team has figured out a solution by using Auto Scaling Group for these EC2 instances and making sure that 10 EC2 instances are available during this peak usage hour. For normal operations only 2 EC2 instances are enough to cater to the workload.
* Configure your Auto Scaling group by creating a scheduled action that kicks-off at the designated hour on the last day of the month. Set the min count as well as the max count of instances to 10. This causes the scale-out to happen before peak traffic kicks in at the designated hour
* Configure your Auto Scaling group by creating a simple tracking policy and setting the instance count to 10 at the designated hour. This causes the scale-out to happen before peak traffic kicks in at the designated hour
* Configure your Auto Scaling group by creating a target tracking policy and setting the instance count to 10 at the designated hour. This causes the scale-out to happen before peak traffic kicks in at the designated hour
* Configure your Auto Scaling group by creating a scheduled action that kicks-off at the designated hour on the last day of the month. Set the desired capacity of instances to 10. This causes the scale-out to happen before peak traffic kicks in at the designated hour

### Question 56:
A cyber forensics company runs its EC2 servers behind an Application Load Balancer along with an Auto Scaling group. The engineers at the company want to be able to install proprietary forensic tools on each instance and perform a pre-activation status check of these tools whenever an instance is provisioned because of a scale-out event from an auto-scaling policy.
* Use the Auto Scaling group lifecycle hook to put the instance in a wait state and launch a custom script that installs the proprietary forensic tools and performs a pre-activation status check
* Use the Auto Scaling group scheduled action to put the instance in a wait state and launch a custom script that installs the proprietary forensic tools and performs a pre-activation status check
* Use the EC2 instance meta data to put the instance in a wait state and launch a custom script that installs the proprietary forensic tools and performs a pre-activation status check
* Use the EC2 instance user data to put the instance in a wait state and launch a custom script that installs the proprietary forensic tools and performs a pre-activation status check

### Question 57:
The engineering team at a data analytics company has observed that its flagship application functions at its peak performance when the underlying EC2 instances have a CPU utilization of about 50%. The application is built on a fleet of EC2 instances managed under an Auto Scaling group. The workflow requests are handled by an internal Application Load Balancer that routes the requests to the instances.
* Configure the Auto Scaling group to use a Cloudwatch alarm triggered on a CPU utilization threshold of 50%
* Configure the Auto Scaling group to use simple scaling policy and set the CPU utilization as the target metric with a target value of 50%
* Configure the Auto Scaling group to use target tracking policy and set the CPU utilization as the target metric with a target value of 50%
* Configure the Auto Scaling group to use step scaling policy and set the CPU utilization as the target metric with a target value of 50%

### Question 58:
A social gaming startup has its flagship application hosted on a fleet of EC2 servers running behind an Elastic Load Balancer. These servers are part of an Auto Scaling Group. 90% of the users start logging into the system at 6 pm every day and continue till midnight. The engineering team at the startup has observed that there is a significant performance lag during the initial hour from 6 pm to 7 pm. The application is able to function normally thereafter.
* Configure your Auto Scaling group by creating a step scaling policy. This causes the scale-out to happen even before peak traffic kicks in at 6 pm
* Configure your Auto Scaling group by creating a scheduled action that kicks-off before 6 pm. This causes the scale-out to happen even before peak traffic kicks in at 6 pm
* Configure your Auto Scaling group by creating a target tracking policy. This causes the scale-out to happen even before peak traffic kicks in at 6 pm
* Configure your Auto Scaling group by creating a lifecycle hook that kicks-off before 6 pm. This causes the scale-out to happen even before peak traffic kicks in at 6 pm

### Question 59:
A cyber security company is running a mission critical application using a single Spread placement group of EC2 instances. The company needs 15 Amazon EC2 instances for optimal performance.
* 14
* 3
* 15
* 7

### Question 60:
Which of the following is true regarding cross-zone load balancing as seen in Application Load Balancer versus Network Load Balancer?
* By default, cross-zone load balancing is enabled for Application Load Balancer and disabled for Network Load Balancer
* By default, cross-zone load balancing is disabled for both Application Load Balancer and Network Load Balancer
* By default, cross-zone load balancing is disabled for Application Load Balancer and enabled for Network Load Balancer
* By default, cross-zone load balancing is enabled for both Application Load Balancer and Network Load Balancer

### Question 61:
A US-based healthcare startup is building an interactive diagnostic tool for COVID-19 related assessments. The users would be required to capture their personal health records via this tool. As this is sensitive health information, the backup of the user data must be kept encrypted in S3. The startup does not want to provide its own encryption keys but still wants to maintain an audit trail of when an encryption key was used and by whom.
* Use client-side encryption with client provided keys and then upload the encrypted user data to S3
* Use SSE-C to encrypt the user data on S3
* Use SSE-KMS to encrypt the user data on S3
* Use SSE-S3 to encrypt the user data on S3

### Question 62:
A leading video streaming provider is migrating to AWS Cloud infrastructure for delivering its content to users across the world. The company wants to make sure that the solution supports at least a million requests per second for its EC2 server farm.
* Classic Load Balancer
* Infrastructure Load Balancer
* Network Load Balancer
* Application Load Balancer

### Question 63:
An e-commerce company wants to explore a hybrid cloud environment with AWS so that it can start leveraging AWS services for some of its data analytics workflows. The engineering team at the e-commerce company wants to establish a dedicated, encrypted, low latency, and high throughput connection between its data center and AWS Cloud. The engineering team has set aside sufficient time to account for the operational overhead of establishing this connection.
* Use AWS Direct Connect to establish a connection between the data center and AWS Cloud
* Use VPC transit gateway to establish a connection between the data center and AWS Cloud
* Use site-to-site VPN to establish a connection between the data center and AWS Cloud
* Use AWS Direct Connect plus VPN to establish a connection between the data center and AWS Cloud

### Question 64:
Which of the following features of an Amazon S3 bucket can only be suspended once they have been enabled?
* Static Website Hosting
* Server Access Logging
* Versioning
* Requester Pays

### Question 65:
A major bank is using SQS to migrate several core banking applications to the cloud to ensure high availability and cost efficiency while simplifying administrative complexity and overhead. The development team at the bank expects a peak rate of about 1000 messages per second to be processed via SQS. It is important that the messages are processed in order.
* Use Amazon SQS standard queue to process the messages
* Use Amazon SQS FIFO queue to process the messages
* Use Amazon SQS FIFO queue in batch mode of 4 messages per operation to process the messages at the peak rate
* Use Amazon SQS FIFO queue in batch mode of 2 messages per operation to process the messages at the peak rate



# Exam 2

### Question 1:
A weather forecast agency collects key weather metrics across multiple cities in the US and sends this data in the form of key-value pairs to AWS Cloud at a one-minute frequency.
* ElastiCache
* RDS
* DynamoDB
* Lambda
* Redshift

### Question 2:
Upon a security review of your AWS account, an AWS consultant has found that a few RDS databases are un-encrypted. As a Solutions Architect, what steps must be taken to encrypt the RDS databases?
* Enable Multi-AZ for the database, and make sure the standby instance is encrypted. Stop the main database to that the standby database kicks in, then disable Multi-AZ
* Create a Read Replica of the database, and encrypt the read replica. Promote the read replica as a standalone database, and terminate the previous database
* Enable encryption on the RDS database using the AWS Console
* Take a snapshot of the database, copy it as an encrypted snapshot, and restore a database from the encrypted snapshot. Terminate the previous database

### Question 3:
The engineering team at an IT company is deploying an Online Transactional Processing (OLTP) application, which will have unpredictable spikes of usage, that they do not know in advance.
* DynamoDB with On-Demand Capacity
* Amazon ElastiCache
* Aurora Serverless
* DynamoDB with Provisioned Capacity and Auto Scaling

### Question 4:
A company has many VPC in various accounts, that need to be connected in a star network with one another and connected with on-premises networks through Direct Connect. What do you recommend?
* Transit Gateway
* VPN Gateway
* VPC Peering
* Private Link

### Question 5:
You have deployed a database technology that has a synchronous replication mode to survive disasters in data centers. The database is therefore deployed on two EC2 instances in two Availability Zones. The database must be publicly available so you have deployed the EC2 instances in public subnets. The replication protocol currently uses the EC2 public IP addresses.
* Use the EC2 instances private IP for the replication
* Assign Elastic IPs to the EC2 instances and use them for the replication
* Create a Private Link between the two EC2 instances
* Use an Elastic Fabric Adapter

### Question 6:
A popular real estate website in the United States provides the latest market information to tens of millions of buyers and sellers every day. A primary feature of the website is the home-valuation tool that provides buyers and sellers with the estimated market value for a specific home. The inputs to the home-valuation tool are updated via a flexible nightly process which runs for 1 hour using Python and is currently running on-premises. It needs to be migrated to AWS.
* Run on a Spot Instance with Spot Block
* Run on EMR
* Run on Lambda
* Run on an Application Load Balancer

### Question 7:
Your company has an on-premises Distributed File System Replication (DFSR) service to keep files synchronized on multiple Windows servers, and would like to migrate to AWS cloud.
* EFS
* FSx for Lustre
* FSx for Windows
* Amazon S3

### Question 8:
You have a team of developers in your company, and you would like to ensure they can quickly experiment with AWS Managed Policies by attaching them to their accounts, but you would like to prevent them from doing an escalation of privileges, by granting themselves the AdministratorAccess managed policy. How should you proceed?
* Create a Service Control Policy (SCP) on your AWS account that restricts developers from attaching themselves the AdministratorAccess policy
* Attach an IAM policy to your developers, that prevents them from attaching the AdministratorAccess policy
* For each developer, define an IAM permission boundary that will restrict the managed policies they can attach to themselves
* Put the developers into an IAM group, and then define an IAM permission boundary on the group that will restrict the managed policies they can attach to themselves

### Question 9:
The DevOps team at a leading social media company uses AWS OpsWorks, which is a fully managed configuration management service. OpsWorks eliminates the need to operate your configuration management systems or worry about maintaining its infrastructure.
* Salt
* Chef
* CFEngine
* Puppet
* Ansible

### Question 10:
A Hollywood studio is planning a series of promotional events leading up to the launch of the trailer of its next sci-fi thriller. The executives at the studio want to create a static website with lots of animations in line with the theme of the movie. The studio has hired you as a solutions architect to build a scalable serverless solution.
* Host the website on AWS Lambda. Create a CloudFront distribution with Lambda as the origin
* Host the website on an instance in the studio's on-premises data center. Create a CloudFront distribution with this instance as the custom origin
* Host the website on an EC2 instance. Create a CloudFront distribution with the EC2 instance as the custom origin
* Build the website as a static website hosted on Amazon S3. Create a CloudFront distribution with Amazon S3 as the origin. Use Amazon Route 53 to create an alias record that points to your CloudFront distribution

### Question 11:
An IT company is working on client engagement to build a real-time data analytics tool for the Internet of Things (IoT) data. The IoT data is funneled into Kinesis Data Streams which further acts as the source of a delivery stream for Kinesis Firehose. The engineering team has now configured a Kinesis Agent to send IoT data from another set of devices to the same Firehose delivery stream. They noticed that data is not reaching Firehose as expected.
* Kinesis Agent can only write to Kinesis Data Streams, not to Kinesis Firehose
* Kinesis Agent cannot write to a Kinesis Firehose for which the delivery stream source is already set as Kinesis Data Streams
* The data sent by Kinesis Agent is lost because of a configuration error
* Kinesis Firehose delivery stream has reached its limit and needs to be scaled manually

### Question 12:
A financial services firm uses a high-frequency trading system and wants to write the log files into Amazon S3. The system will also read these log files in parallel on a near real-time basis. The engineering team is apprehensive of any data discrepancies that might arise when the trading system overwrites an existing log file and then tries to read that specific log file.
* A process replaces an existing object and immediately tries to read it. Until the change is fully propagated, Amazon S3 does not return any data
* A process replaces an existing object and immediately tries to read it. Until the change is fully propagated, Amazon S3 might return the new data
* A process replaces an existing object and immediately tries to read it. Amazon S3 always returns the latest version of the object
* A process replaces an existing object and immediately tries to read it. Until the change is fully propagated, Amazon S3 might return the previous data

### Question 13:
A social photo-sharing web application is hosted on EC2 instances behind an Elastic Load Balancer. The app gives the users the ability to upload their photos and also shows a leaderboard on the homepage of the app. The uploaded photos are stored in S3 and the leaderboard data is maintained in DynamoDB. The EC2 instances need to access both S3 and DynamoDB for these features.
* Encrypt the AWS credentials via a custom encryption library and save it in a secret directory on the EC2 instances. The application code can then safely decrypt the AWS credentials to make the API calls to S3 and DynamoDB
* Configure AWS CLI on the EC2 instances using a valid IAM user's credentials. The application code can then invoke shell scripts to access S3 and DynamoDB via AWS CLI
* Save the AWS credentials (access key Id and secret access token) in a configuration file within the application code on the EC2 instances. EC2 instances can use these credentials to access S3 and DynamoDB
* Attach the appropriate IAM role to the EC2 instance profile so that the instance can access S3 and DynamoDB

### Question 14:
A junior DevOps engineer wants to change the default configuration for EBS volume termination. By default, the root volume of an EC2 instance for an EBS-backed AMI is deleted when the instance terminates.
* Set the TerminateOnDelete attribute to true
* Set the DeleteOnTermination attribute to true
* Set the TerminateOnDelete attribute to false
* Set the DeleteOnTermination attribute to false

### Question 15:
Your application is deployed on EC2 instances fronted by an Application Load Balancer. Recently, your infrastructure has come under attack. Attackers perform over 100 requests per second, while your normal users only make about 5 requests per second.
* Configure Sticky Sessions on the Application Load Balancer
* Use a Web Application Firewall and setup a rate-based rule
* Define a Network ACL (NACL) on your Application Load Balancer
* Use AWS Shield Advanced and setup a rate-based rule

### Question 16:
What does this IAM policy do?
* It allows starting EC2 instances only when the IP where the call originates is within the 34.50.31.0/24 CIDR block
* It allows starting EC2 instances only when they have a Public IP within the 34.50.31.0/24 CIDR block
* It allows starting EC2 instances only when they have an Elastic IP within the 34.50.31.0/24 CIDR block
* It allows starting EC2 instances only when they have a Private IP within the 34.50.31.0/24 CIDR block

### Question 17:
A cybersecurity company uses a fleet of EC2 instances to run a proprietary application. The infrastructure maintenance group at the company wants to be notified via an email whenever the CPU utilization for any of the EC2 instances breaches a certain threshold.
* Amazon SNS
* AWS Lambda
* Amazon CloudWatch
* Amazon SQS
* AWS Step Functions

### Question 18:
You would like to mount a network file system on Linux instances, where files will be stored and accessed frequently at first, and then infrequently. What solution is the MOST cost-effective?
* Glacier Deep Archive
* S3 Intelligent Tiering
* EFS IA
* FSx for Lustre

### Question 19:
Researchers at a pharma company are working on developing a vaccine for the COVID-19 pandemic. They have identified multiple candidates as potential vaccines and they need to analyze healthcare data of individuals in the US to identify the first batch of recipients for the initial trials. For faster processing, the data processing application needs to parse through this healthcare data in an in-memory database that is highly available as well as HIPAA compliant.
* ElastiCache for Redis
* DynamoDB
* ElastiCache for Memcached
* DocumentDB

### Question 20:
You would like to deploy an application behind an Application Load Balancer, that will have some Auto Scaling capability and efficiently leverage a mix of Spot Instances and On-Demand instances to meet demand.
* Create an ASG with a launch configuration
* Create a Spot Fleet Request
* Create an ASG with a launch template
* Create a Spot Instance Request

### Question 21:
A financial services company is looking to transition its IT infrastructure from on-premises to AWS Cloud. They are moving towards a single log processing model for all their log files (consisting of system logs, application logs, database logs, etc) that can be processed in a serverless fashion and then durably stored for downstream analytics. They want to use an AWS managed service that automatically scales to match the throughput of the log data and requires no ongoing administration.
* Kinesis Data Streams
* AWS Lambda
* Amazon EMR
* Kinesis Data Firehose

### Question 22:
The infrastructure team at a company maintains 5 different VPCs (let's call these VPCs A, B, C, D, E) for resource isolation. Due to the changed organizational structure, the team wants to interconnect all VPCs together. To facilitate this, the team has set up VPC peering connections between VPC A and all other VPCs in a hub and spoke model with VPC A at the center. However, the team has still failed to establish connectivity between all VPCs.
* Establish VPC peering connections between all VPCs
* Use an internet gateway to interconnect the VPCs
* Use a VPC endpoint to interconnect the VPCs
* Use a transit gateway to interconnect the VPCs

### Question 23:
An HTTP application is deployed on an Auto Scaling Group, is accessible from an Application Load Balancer that provides HTTPS termination, and accesses a PostgreSQL database managed by RDS. How should you configure the security groups? (Select three)
* The security group of the EC2 instances should have an inbound rule from the security group of the ALB on port 80
* The security group of RDS should have an inbound rule from the security group of the EC2 instances in the ASG on port 5432
* The security group of the ALB should have an inbound rule from anywhere on port 443
* The security group of RDS should have an inbound rule from the security group of the EC2 instances in the ASG on port 80
* The security group of the ALB should have an inbound rule from anywhere on port 80
* The security group of the EC2 instances should have an inbound rule from the security group of the RDS database on port 5432

### Question 24:
A Machine Learning research group uses a proprietary computer vision application hosted on an EC2 instance. Every time the instance needs to be stopped and started again, the application takes about 3 minutes to start as some auxiliary software programs need to be executed so that the application can function. The research group would like to minimize the application boostrap time whenever the system needs to be stopped and then started at a later point in time.
* Use EC2 Meta-Data
* Use EC2 Instance Hibernate
* Use EC2 User-Data
* Create an AMI and launch your EC2 instances from that

### Question 25:
To improve the performance and security of the application, the engineering team at a company has created a CloudFront distribution with an Application Load Balancer as the custom origin. The team has also set up a Web Application Firewall (WAF) with CloudFront distribution. The security team at the company has noticed a surge in malicious attacks from a specific IP address to steal sensitive data stored on the EC2 instances.
* Create a deny rule for the malicious IP in the NACL associated with each of the instances
* Create an IP match condition in the WAF to block the malicious IP address
* Create a ticket with AWS support to take action against the malicious IP
* Create a deny rule for the malicious IP in the Security Groups associated with each of the instances

### Question 26:
A global media company uses a fleet of EC2 instances (behind an Application Load Balancer) to power its video streaming application. To improve the performance of the application, the engineering team has also created a CloudFront distribution with the Application Load Balancer as the custom origin. The security team at the company has noticed a spike in the number and types of SQL injection and cross-site scripting attack vectors on the application.
* Use Security Hub with CloudFront distribution
* Use Route 53 with CloudFront distribution
* Use Web Application Firewall (WAF) with CloudFront distribution
* Use AWS Firewall Manager with CloudFront distribution

### Question 27:
An application is currently hosted on four EC2 instances (behind Application Load Balancer) deployed in a single Availability Zone (AZ). To maintain an acceptable level of end-user experience, the application needs at least 4 instances to be always available.
* Deploy the instances in three Availability Zones. Launch two instances in each Availability Zone
* Deploy the instances in one Availability Zones. Launch two instances in the Availability Zone
* Deploy the instances in two Availability Zones. Launch two instances in each Availability Zone
* Deploy the instances in two Availability Zones. Launch four instances in each Availability Zone

### Question 28:
You would like to store a database password in a secure place, and enable automatic rotation of that password every 90 days. What do you recommend?
* Key Management Service (KMS)
* Secrets Manager
* SSM Parameter Store
* CloudHSM

### Question 29:
A startup has just developed a video backup service hosted on a fleet of EC2 instances. The EC2 instances are behind an Application Load Balancer and the instances are using EBS volumes for storage. The service provides authenticated users the ability to upload videos that are then saved on the EBS volume attached to a given instance. On the first day of the beta launch, users start complaining that they can see only some of the videos in their uploaded videos backup. Every time the users log into the website, they claim to see a different subset of their uploaded videos.
* Write a one time job to copy the videos from all EBS volumes to RDS and then modify the application to use RDS for storing the videos
* Write a one time job to copy the videos from all EBS volumes to S3 Glacier Deep Archive and then modify the application to use S3 Glacier Deep Archive for storing the videos
* Mount EFS on all EC2 instances. Write a one time job to copy the videos from all EBS volumes to EFS. Modify the application to use EFS for storing the videos
* Write a one time job to copy the videos from all EBS volumes to DynamoDB and then modify the application to use DynamoDB for storing the videos
* Write a one time job to copy the videos from all EBS volumes to S3 and then modify the application to use Amazon S3 standard for storing the videos

### Question 30:
You would like to use Snowball to move on-premises backups into a long term archival tier on AWS. Which solution provides the MOST cost savings?
* Create a Snowball job and target an S3 bucket. Create a lifecycle policy to immediately move data to Glacier
* Create a Snowball job and target an S3 bucket. Create a lifecycle policy to immediately move data to Glacier Deep Archive
* Create a Snowball job and target a Glacier Deep Archive Vault
* Create a Snowball job and target a Glacier Vault

### Question 31:
A big-data consulting firm is working on a client engagement where the ETL workloads are currently handled via a Hadoop cluster deployed in the on-premises data center. The client wants to migrate their ETL workloads to AWS Cloud. The AWS Cloud solution needs to be highly available with about 50 EC2 instances per Availability Zone.
* Both Spread placement group and Partition placement group
* Spread placement group
* Cluster placement group
* Partition placement group

### Question 32:
The engineering team at a startup is running a Proof-of-Concept to move their business to AWS Cloud. The team wants to store business-critical data on Elastic Block Storage (EBS) volumes which provide persistent storage independent of EC2 instances. During a test run, the team found out that on terminating an Amazon EC2 instance, the attached Elastic Block Storage (EBS) volume was also lost, which was contrary to their assumptions.
* The EBS volume was configured as the root volume of Amazon EC2 instance. On termination of the instance, the default behavior is to also terminate the attached root volume
* The EBS volumes were not backed up on EFS file system storage, resulting in the loss of volume
* The EBS volumes were not backed up on Amazon S3 storage, resulting in the loss of volume
* On termination of an EC2 instance, all the attached EBS volumes are always terminated

### Question 33:
Which of the following IAM policies provides read-only access to the S3 bucket mybucket and its content?

### Question 34:
An IT company has an Access Control Management (ACM) application that uses Amazon RDS for MySQL but is running into performance issues despite using Read Replicas. The company has hired you as a solutions architect to address these performance-related challenges on an urgent basis without moving away from the underlying relational database schema. The company has branch offices across the world, and it needs the solution to work on a global scale.
* Use Amazon Aurora Global Database to enable fast local reads with low latency in each region
* Spin up a Redshift cluster in each AWS region. Migrate the existing data into Redshift clusters
* Spin up EC2 instances in each AWS region, install MySQL databases and migrate the existing data into these new databases
* Use Amazon DynamoDB Global Tables to provide fast, local, read and write performance in each region

### Question 35:
A medium-sized business has a taxi dispatch application deployed on an EC2 instance. Because of an unknown bug, the application causes the instance to freeze regularly. Then, the instance has to be manually restarted via the AWS management console.
* Setup a CloudWatch alarm to monitor the health status of the instance. In case of an Instance Health Check failure, CloudWatch Alarm can publish to an SNS event which can then trigger a lambda function. The lambda function can use AWS EC2 API to reboot the instance
* Use CloudWatch events to trigger a Lambda function to reboot the instance status every 5 minutes
* Setup a CloudWatch alarm to monitor the health status of the instance. In case of an Instance Health Check failure, an EC2 Reboot CloudWatch Alarm Action can be used to reboot the instance
* Use CloudWatch events to trigger a Lambda function to check the instance status every 5 minutes. In the case of Instance Health Check failure, the lambda function can use AWS EC2 API to reboot the instance

### Question 36:
A junior developer is learning to build websites using HTML, CSS, and JavaScript. He has created a static website and then deployed it on Amazon S3. Now he can't seem to figure out the endpoint for his super cool website.
* http://s3-website.Region.bucket-name.amazonaws.com
* http://bucket-name.Region.s3-website.amazonaws.com
* http://s3-website-Region.bucket-name.amazonaws.com
* http://bucket-name.s3-website.Region.amazonaws.com
* http://bucket-name.s3-website-Region.amazonaws.com

### Question 37:
An application runs big data workloads on EC2 instances. The application needs at least 20 instances to maintain a minimum acceptable performance threshold and the application needs 300 instances to handle spikes in the workload. Based on historical workloads processed by the application, it needs 80 instances 80% of the time.
* Purchase 80 reserved instances. Provision additional on-demand and spot instances per the workload demand (Use Auto Scaling Group with launch template to provision the mix of on-demand and spot instances)
* Purchase 80 on-demand instances. Provision additional on-demand and spot instances per the workload demand (Use Auto Scaling Group with launch template to provision the mix of on-demand and spot instances)
* Purchase 80 spot instances. Use Auto Scaling Group to provision the remaining instances as on-demand instances per the workload demand
* Purchase 80 on-demand instances. Use Auto Scaling Group to provision the remaining instances as spot instances per the workload demand

### Question 38:
A big data consulting firm needs to set up a data lake on Amazon S3 for a Health-Care client. The data lake is split in raw and refined zones. For compliance reasons, the source data needs to be kept for a minimum of 5 years. The source data arrives in the raw zone and is then processed via an AWS Glue based ETL job into the refined zone. The business analysts run ad-hoc queries only on the data in the refined zone using AWS Athena. The team is concerned about the cost of data storage in both the raw and refined zones as the data is increasing at a rate of 1TB daily in each zone.
* Create a Lambda function based job to delete the raw zone data after 1 day
* Use Glue ETL job to write the transformed data in the refined zone using CSV format
* Use Glue ETL job to write the transformed data in the refined zone using a compressed file format
* Setup a lifecycle policy to transition the raw zone data into Glacier Deep Archive after 1 day of object creation
* Setup a lifecycle policy to transition the refined zone data into Glacier Deep Archive after 1 day of object creation

### Question 39:
You would like to migrate an AWS account from an AWS Organization A to an AWS Organization B. What are the steps do to it?
* Send an invite to the new organization. Accept the invite to the new organization from the member account. Remove the member account from the old organization
* Send an invite to the new organization. Remove the member account from the old organization. Accept the invite to the new organization from the member account
* Open an AWS Support ticket to ask them to migrate the account
* Remove the member account from the old organization. Send an invite to the new organization. Accept the invite to the new organization from the member account

### Question 40:
A financial services company has to retain the activity logs for each of their customers to meet regulatory and compliance guidelines. Depending on the business line, the company wants to retain the logs for 5-10 years in highly available and durable storage on AWS. The overall data size is expected to be in PetaBytes. In case of an audit, the data would need to be accessible within a timeframe of up to 48 hours.
* Amazon S3 Glacier Deep Archive
* Amazon S3 Glacier
* Third party tape storage
* Amazon S3 Standard storage

### Question 41:
You are deploying a critical monolith application that must be deployed on a single web server, as it hasn't been created to work in distributed mode. Still, you want to make sure your setup can automatically recover from the failure of an AZ.
* Create a Spot Fleet request
* Create an auto-scaling group that spans across 2 AZ, which min=1, max=2, desired=2
* Assign an EC2 Instance Role to perform the necessary API calls
* Create an Elastic IP and use the EC2 user-data script to attach it
* Create an Application Load Balancer and a target group with the instance(s) of the Auto Scaling Group
* Create an auto-scaling group that spans across 2 AZ, which min=1, max=1, desired=1

### Question 42:
A DevOps engineer at an organization is debugging issues related to an Amazon EC2 instance. The engineer has SSH'ed into the instance and he needs to retrieve the instance public IP from within a shell script running on the instance command line.
* http://254.169.254.169/latest/meta-data/public-ipv4
* http://169.254.169.254/latest/user-data/public-ipv4
* http://254.169.254.169/latest/user-data/public-ipv4
* http://169.254.169.254/latest/meta-data/public-ipv4

### Question 43:
A media publishing company is looking at moving their on-premises infrastructure to AWS Cloud. Their flagship application uses a massive PostgreSQL database and the engineering team would like to retain control over managing the patches, version upgrades for the database, and consistent performance with high IOPS. The team wants to install the database on an EC2 instance with the optimal storage type on the attached EBS volume.
* Amazon EC2 with EBS volume of Provisioned IOPS SSD (io1) type
* Amazon EC2 with EBS volume of cold HDD (sc1) type
* Amazon EC2 with EBS volume of General Purpose SSD (gp2) type
* Amazon EC2 with EBS volume of Throughput Optimized HDD (st1) type

### Question 44:
An Industrial Appliances company has just moved a significant percentage of its existing workloads to the AWS Cloud, and all departments now use some AWS solutions. Although these changes have helped the company to become more flexible, but the DevOps team still needs to ramp up on IT security. Currently, the team wants to enable a highly available architecture for a bastion host solution.
* Create an Elastic IP and assign it to all EC2 instances that are bastion hosts managed by an ASG
* Create a public Network Load Balancer that links to EC2 instances that are bastion hosts managed by an ASG
* Create a public Application Load Balancer that links to EC2 instances that are bastion hosts managed by an ASG
* Create a VPC Endpoint for a fleet of EC2 instances that are bastion hosts managed by an ASG

### Question 45:
The development team at an e-commerce startup has set up multiple microservices running on EC2 instances under an Elastic Load Balancer. The team wants to route traffic to multiple back-end services based on the content of the request.
* Application Load Balancer
* Classic Load Balancer
* Network Load Balancer
* Both Application Load Balancer and Network Load Balancer

### Question 46:
What is true about RDS Read Replicas encryption?
* If the master database is unencrypted, the read replicas are encrypted
* If the master database is unencrypted, the read replicas can be either encrypted or unencrypted
* If the master database is encrypted, the read replicas are encrypted
* If the master database is encrypted, the read replicas can be either encrypted or unencrypted

### Question 47:
One of the largest biotechnology companies in the world uses Amazon S3 to store and protect terabytes of critical research data for its AWS based Drug Discovery application, which allows thousands of universities to collaborate. The engineering team wants to publish an event into an SQS queue whenever a new research paper is uploaded on S3.
* FIFO SQS queue is only allowed as an Amazon S3 event notification destination, whereas Standard SQS queue is not allowed
* Both Standard SQS queue and FIFO SQS queue are allowed as an Amazon S3 event notification destination
* Standard SQS queue is only allowed as an Amazon S3 event notification destination, whereas FIFO SQS queue is not allowed
* Neither Standard SQS queue nor FIFO SQS queue are allowed as an Amazon S3 event notification destination

### Question 48:
An IT company wants to optimize the costs incurred on its fleet of 100 EC2 instances for the next year. Based on historical analyses, the engineering team observed that 70 of these instances handle the compute services of its flagship application and need to be always available. The other 30 instances are used to handle batch jobs that can afford a delay in processing.
* Purchase 70 on-demand instances and 30 spot instances
* Purchase 70 on-demand instances and 30 reserved instances
* Purchase 70 reserved instances and 30 spot instances
* Purchase 70 reserved instances and 30 on-demand instances

### Question 49:
The DevOps team at a startup has provisioned a new EC2 instance A by choosing all default options in the AWS management console. The team can ping instance A from other instances in the VPC. The other instances were also created using the default options. The next day, the team launches another instance B by creating a new security group and attaching it to instance B. All other configuration options for instance B are chosen as default. However, the team is not able to ping instance B from other instances in the VPC.
* Instance A is in the default security group. The default rules for the default security group allow no inbound traffic from all sources. Instance B is in a new security group. The default rules for a security group that you create allow inbound traffic from all sources
* Instance A is in the default security group. The default rules for the default security group allow inbound traffic from network interfaces (and their associated instances) that are assigned to the same security group. Instance B is in a new security group. The default rules for a security group that you create allow no inbound traffic
* Instance A is in the default security group. The default rules for the default security group allow no inbound traffic from network interfaces (and their associated instances) that are assigned to the same security group. Instance B is in a new security group. The default rules for a security group that you create allow inbound traffic from all sources
* Instance A is in the default security group. The default rules for the default security group allow inbound traffic from all sources. Instance B is in a new security group. The default rules for a security group that you create allow no inbound traffic

### Question 50:
Your e-commerce application is using an RDS PostgreSQL database and an analytics workload also runs on the same database. When the analytics workload is run, your e-commerce application slows down which further affects your sales.
* Create a Read Replica in the same AZ as the Master database and point the analytics workload there
* Enable Multi-AZ for the RDS database and run the analytics workload on the standby database
* Migrate the analytics application to AWS Lambda
* Create a Read Replica in another AZ as the Master database and point the analytics workload there

### Question 51:
A silicon valley based startup has a content management application with the web-tier running on EC2 instances and the database tier running on Amazon Aurora. Currently, the entire infrastructure is located in us-east-1 region. The startup has 90% of its customers in the US and Europe. The engineering team is getting reports of deteriorated application performance from customers in Europe with high application load time.
* Setup another fleet of EC2 instances for the web tier in the eu-west-1 region. Enable failover routing policy in Route 53
* Create Amazon Aurora Multi-AZ standby instance in the eu-west-1 region
* Create Amazon Aurora read replicas in the eu-west-1 region
* Setup another fleet of EC2 instances for the web tier in the eu-west-1 region. Enable geolocation routing policy in Route 53
* Setup another fleet of EC2 instances for the web tier in the eu-west-1 region. Enable latency routing policy in Route 53

### Question 52:
A silicon valley based startup has a two-tier architecture using EC2 instances for its flagship application. The web servers (listening on port 443), which have been assigned security group A, are in public subnets across two Availability Zones and the MSSQL based database instances (listening on port 1433), which have been assigned security group B, are in two private subnets across two Availability Zones. The DevOps team wants to review the security configurations of the application architecture.
* For security group B: Add an inbound rule that allows traffic only from all sources on port 1433
* For security group B: Add an inbound rule that allows traffic only from security group A on port 1433
* For security group B: Add an inbound rule that allows traffic only from security group A on port 443
* For security group A: Add an inbound rule that allows traffic from all sources on port 443. Add an outbound rule with the destination as security group B on port 443
* For security group A: Add an inbound rule that allows traffic from all sources on port 443. Add an outbound rule with the destination as security group B on port 1433

### Question 53:
A social photo-sharing company is storing user profile pictures in an S3 bucket and an image analysis application is deployed on four EC2 instances. A solutions architect would like to trigger an image analysis procedure only on one of the four EC2 instances for each photo uploaded. What do you recommend?
* Create an S3 Event Notification that sends a message to an SQS queue. Make the EC2 instances read from the SQS queue
* Create a CloudWatch Event that reacts to objects uploads in S3 and invokes one of the EC2 instances
* Create an S3 Event Notification that sends a message to an SNS topic. Subscribe the EC2 instances to the SNS topic
* Subscribe the EC2 instances to the S3 Inventory stream

### Question 54:
A tax computation software runs on Amazon EC2 instances behind a Classic Load Balancer. The instances are managed by an Auto Scaling Group. The tax computation software has an optimization module, which can take up to 10 minutes to find the optimal answer.
* Enable ELB health checks on the ASG
* Enable Stickiness on the CLB
* Create an ASG Scheduled Action
* Increase the deregistration delay to more than 10 minutes

### Question 55:
You have an in-memory database launched on an EC2 instance and you would like to be able to stop and start the EC2 instance without losing the in-memory state of your database. What do you recommend?
* Create an AMI from the instance
* Use EC2 Instance Hibernate
* Use an EC2 Instance Store
* Mount an in-memory EBS Volume

### Question 56:
Your company has a monthly big data workload, running for about 2 hours, which can be efficiently distributed across various servers of various sizes, with a variable number of CPU, and that can withstand server failures.
* Run the workload on a Spot Fleet
* Run the workload on Spot Instances
* Run the workload on Dedicated Hosts
* Run the workload on Reserved Instances

### Question 57:
What does this IAM policy do?
* It allows running EC2 instances only in the eu-west-1 region, and the API call can be made from anywhere in the world
* It allows to run EC2 instances in the eu-west-1 region, when the API call is made from the eu-west-1 region
* It allows running EC2 instances in any region when the API call is originating from the eu-west-1 region
* It allows running EC2 instances anywhere but in the eu-west-1 region

### Question 58:
A large news agency uses Amazon S3 for centralized storage of the static media assets such as video reports. Reporters typically upload and download video files (about 500MB each) to the same S3 bucket as part of their day to day work. As the agency has started running offices from remote branches, it has resulted in poor latency for accessing and uploading data to/from S3. The agency wants to continue with the serverless solution for its storage requirements but wants to improve the performance.
* Use Amazon CloudFront distribution with origin as the S3 bucket. This would speed up uploads as well as downloads for the video files
* Create new S3 buckets in every region where the agency has a remote office, so that each office can maintain its storage for the media assets
* Enable Amazon S3 Transfer Acceleration for the S3 bucket. This would speed up uploads as well as downloads for the video files
* Spin up EC2 instances in each region where the agency has a remote office. Create a daily job to transfer S3 data into EBS volumes attached to the EC2 instances
* Move S3 data into EFS file system created in a US region, connect to EFS file system from EC2 instances in other AWS regions using an inter-region VPC peering connection

### Question 59:
You are looking to build an index of your files in S3, using Amazon RDS PostgreSQL. To build this index, it is necessary to read the first 250 bytes of each object in S3, which contains some metadata about the content of the file itself. There are over 100,000 files in your S3 bucket, amounting to 50TB of data.
* Create an application that will traverse the S3 bucket, then use S3 Select Byte Range Fetch parameter to get the first 250 bytes, and store that information in RDS
* Use the RDS Import feature to load the data from S3 to PostgreSQL, and run a SQL query to build the index
* Create an application that will traverse the S3 bucket, read all the files one by one, extract the first 250 bytes, and store that information in RDS
* Create an application that will traverse the S3 bucket, issue a Byte Range Fetch for the first 250 bytes, and store that information in RDS

### Question 60:
You have multiple AWS accounts within a single AWS Region managed by AWS Organizations and you would like to ensure all EC2 instances in all these accounts can communicate privately. Which of the following solutions provides the capability at the CHEAPEST cost?
* Create a Transit Gateway and link all the VPC in all the accounts together
* Create a VPC peering connection between all VPCs
* Create a VPC in an account and share one or more of its subnets with the other accounts using Resource Access Manager
* Create a Private Link between all the EC2 instances

### Question 61:
You are building an application that will be deployed on 10 EC2 instances using Amazon Linux 2 AMI. The application needs access to a shared network file system that is POSIX compliant. What do you recommend?
* EFS
* EBS
* S3
* Instance Store

### Question 62:
An e-commerce website hosted on an EC2 instance consumes messages from an SQS queue which has records for pending orders. The SQS queue has a visibility timeout of 30 minutes. The EC2 instance sends out an email once an order has been processed. The development team observes that 12 emails have been sent but only 4 orders have been placed.
* Queue is set to long polling so the messages are being picked up multiple times by the consumer application
* Queue is set to short polling so the messages are being picked up multiple times by the consumer application
* Because of a configuration issue, the consumer application is not deleting the messages in the SQS queue after it has processed them
* Queue is set to distributed mode forcing delivery of duplicate messages

### Question 63:
The engineering team at an e-commerce company is working on cost optimizations for EC2 instances. The team wants to manage the workload using a mix of on-demand and spot instances across multiple instance types. They would like to create an Auto Scaling group with a mix of these instances.
* You can use a launch configuration or a launch template to provision capacity across multiple instance types using both On-Demand Instances and Spot Instances to achieve the desired scale, performance, and cost
* You can only use a launch configuration to provision capacity across multiple instance types using both On-Demand Instances and Spot Instances to achieve the desired scale, performance, and cost
* You can neither use a launch configuration nor a launch template to provision capacity across multiple instance types using both On-Demand Instances and Spot Instances to achieve the desired scale, performance, and cost
* You can only use a launch template to provision capacity across multiple instance types using both On-Demand Instances and Spot Instances to achieve the desired scale, performance, and cost

### Question 64:
An IT company is working on a client project to build a Supply Chain Management application. The web-tier of the application runs on an EC2 instance and the database tier is on Amazon RDS MySQL. For beta testing, all the resources are currently deployed in a single Availability Zone. The development team wants to improve application availability before the go-live.
* Deploy the web-tier EC2 instances in two regions, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in Multi-AZ configuration
* Deploy the web-tier EC2 instances in two regions, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in read replica configuration
* Deploy the web-tier EC2 instances in two Availability Zones, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in Multi-AZ configuration
* Deploy the web-tier EC2 instances in two Availability Zones, behind an Elastic Load Balancer. Deploy the Amazon RDS MySQL database in read replica configuration

### Question 65:
You are establishing a monitoring solution for desktop systems, that will be sending telemetry data into AWS every 1 minute. Data for each system must be processed in order, independently, and you would like to scale the number of consumers to be possibly equal to the number of desktop systems that are being monitored. What do you recommend?
* Use an SQS FIFO queue, and send the telemetry data as is
* Use a Kinesis Data Stream, and send the telemetry data with a Partition ID that uses the value of the Desktop ID
* Use an SQS standard queue, and send the telemetry data as is
* Use an SQS FIFO queue, and make sure the telemetry data is sent with a Group ID attribute representing the value of the Desktop ID



# Exam 3

### Question 1:
A Hollywood production studio is looking at transferring their existing digital media assets of around 20PB to AWS Cloud in the shortest possible timeframe.
* AWS Snowball
* AWS Snowmobile
* AWS Direct Connect
* AWS Storage Gateway

### Question 2:
A retail company has connected its on-premises data center to the AWS Cloud via AWS Direct Connect. The company wants to be able to resolve DNS queries for any resources in the on-premises network from the AWS VPC and also resolve any DNS queries for resources in the AWS VPC from the on-premises network.
* Create an inbound endpoint on Route 53 Resolver and then Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint
* Create an outbound endpoint on Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Route 53 Resolver via this endpoint
* Create a universal endpoint on Route 53 Resolver and then Route 53 Resolver can receive and forward queries to resolvers on the on-premises network via this endpoint
* Create an inbound endpoint on Route 53 Resolver and then DNS resolvers on the on-premises network can forward DNS queries to Route 53 Resolver via this endpoint
* Create an outbound endpoint on Route 53 Resolver and then Route 53 Resolver can conditionally forward queries to resolvers on the on-premises network via this endpoint

### Question 3:
The engineering team at a company manages the Auto Scaling group and the Launch Configuration for EC2 instances (in us-east-1 region) via a shell script using the AWS CLI. The billing department at the company has noticed that all instances created via this Launch Configuration have detailed monitoring enabled and have been incurring additional costs. To verify this behavior, the lead engineer logs into the AWS management console and creates another Launch Configuration with the same settings but finds that the instances created via this new Launch Configuration have only basic monitoring enabled.
* By default, basic monitoring is enabled when you use the AWS management console to create a launch configuration. Detailed monitoring is enabled by default when you create a launch configuration using the AWS CLI
* By default, detailed monitoring is enabled when you use the AWS management console or AWS CLI to create a launch configuration. For the given use-case, the basic monitoring option for the instances must have been explicitly set to enabled while creating the Launch Configuration from the AWS management console
* This seems to be an issue with the us-east-1 region. The issue can be resolved by moving the instances to us-west-1 region
* By default, basic monitoring is enabled when you use the AWS management console or AWS CLI to create a launch configuration. For the given use-case, the detailed monitoring option for the instances must have been explicitly set to enabled while creating the Launch Configuration from the AWS CLI

### Question 4:
A CRM application is facing user experience issues with users reporting frequent sign-in requests from the application. The application is currently hosted on multiple EC2 instances behind an Application Load Balancer. The engineering team has identified the root cause as unhealthy servers causing session data to be lost. The team would like to implement a distributed in-memory cache-based session management solution.
* Use DynamoDB for distributed in-memory cache based session management
* Use Elasticache for distributed in-memory cache based session management
* Use Application Load Balancer sticky sessions
* Use RDS for distributed in-memory cache based session management

### Question 5:
An IT consultant is helping a small business revamp their technology infrastructure on the AWS Cloud. The business has two AWS accounts and all resources are provisioned in the us-west-2 region. The IT consultant is trying to launch an EC2 instance in each of the two AWS accounts such that the instances are in the same Availability Zone of the us-west-2 region. Even after selecting the same default subnet (us-west-2a) while launching the instances in each of the AWS accounts, the IT consultant notices that the Availability Zones are still different.
* Use AZ ID to uniquely identify the Availability Zones across the two AWS Accounts
* Use the default VPC to uniquely identify the Availability Zones across the two AWS Accounts
* Use the default subnet to uniquely identify the Availability Zones across the two AWS Accounts
* Reach out to AWS Support for creating the EC2 instances in the same Availability Zone across the two AWS accounts

### Question 6:
A global pharmaceutical company generates hundreds of terabytes of research data daily. To further accelerate the innovation process, the engineering team at the company wants to move most of the on-premises data into Amazon S3, Amazon EFS, and Amazon FSx for Windows File Server easily, quickly, and cost-effectively. The team would like to automate and accelerate online data transfers to these AWS storage services.
* Use File Gateway to automate and accelerate online data transfers to the given AWS storage services
* Use AWS Snowball Edge Storage Optimized device to automate and accelerate online data transfers to the given AWS storage services
* Use AWS Transfer Family to automate and accelerate online data transfers to the given AWS storage services
* Use AWS DataSync to automate and accelerate online data transfers to the given AWS storage services

### Question 7:
The DevOps team at an IT company has created a custom VPC (V1) and attached an Internet Gateway (I1) to the VPC. The team has also created a subnet (S1) in this custom VPC and added a route to this subnet's route table (R1) that directs internet-bound traffic to the Internet Gateway. Now the team launches an EC2 instance (E1) in the subnet S1 and assigns a public IPv4 address to this instance. Next the team also launches a NAT instance (N1) in the subnet S1.
* Internet Gateway (I1)
* Route Table (R1)
* Subnet (S1)
* NAT instance (N1)

### Question 8:
The engineering team at a social media company wants to use Amazon CloudWatch alarms to automatically recover EC2 instances if they become impaired. The team has hired you as a solutions architect to provide subject matter expertise.
* If your instance has a public IPv4 address, it retains the public IPv4 address after recovery
* A recovered instance is identical to the original instance, including the instance ID, private IP addresses, Elastic IP addresses, and all instance metadata
* Terminated EC2 instances can be recovered if they are configured at the launch of instance
* During instance recovery, the instance is migrated during an instance reboot, and any data that is in-memory is retained
* If your instance has a public IPv4 address, it does not retain the public IPv4 address after recovery

### Question 9:
A media company has its corporate headquarters in Los Angeles with an on-premises data center using an AWS Direct Connect connection to the AWS VPC. The branch offices in San Francisco and Miami use Site-to-Site VPN connections to connect to the AWS VPC. The company is looking for a solution to have the branch offices send and receive data with each other as well as with their corporate headquarters.
* Software VPN
* VPN CloudHub
* VPC Endpoint
* VPC Peering

### Question 10:
A financial services company is moving its IT infrastructure to AWS Cloud and wants to enforce adequate data protection mechanisms on Amazon S3 to meet compliance guidelines. The engineering team has hired you as a solutions architect to help them understand the encryption capabilities on S3.
* S3 can encrypt object metadata by using Server-Side Encryption
* S3 can encrypt data in transit using HTTPS (TLS)
* S3 can protect data at rest using Client-Side Encryption
* S3 can protect data at rest using Server-Side Encryption

### Question 11:
A leading Software as a Service (SaaS) TeleHealth services company has deployed its IT infrastructure on the AWS Cloud. The flagship application is hosted on multiple EC2 instances within a single VPC in the us-east-1 region. The engineering team at the company wants to use Amazon SQS to decouple some of the underlying processes but the team is concerned about accessing SQS over the public internet.
* Use VPC endpoint to access Amazon SQS
* Use VPN connection to access Amazon SQS
* Use Network Address Translation (NAT) instance to access Amazon SQS
* Use Internet Gateway to access Amazon SQS

### Question 12:
A financial services company has recently migrated from on-premises infrastructure to AWS Cloud. The DevOps team wants to implement a solution that allows all resource configurations to be reviewed and make sure that they meet compliance guidelines. Also, the solution should be able to offer the capability to look into the resource configuration history across the application stack.
* Use Amazon CloudWatch to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes
* Use AWS CloudTrail to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes
* Use AWS Config to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes
* Use AWS Systems Manager to review resource configurations to meet compliance guidelines and maintain a history of resource configuration changes

### Question 13:
The business analytics team at a company has been running ad-hoc queries on Oracle and PostgreSQL services on Amazon RDS to prepare daily reports for senior management. To facilitate the business analytics reporting, the engineering team now wants to replicate this data with high availability and consolidate these databases into a petabyte-scale data warehouse by streaming data to Amazon Redshift.
* Use AWS Database Migration Service to replicate the data from the databases into Amazon Redshift
* Use AWS Glue to replicate the data from the databases into Amazon Redshift
* Use Amazon Kinesis Data Streams to replicate the data from the databases into Amazon Redshift
* Use AWS EMR to replicate the data from the databases into Amazon Redshift

### Question 14:
The CTO at a retail company wants to optimize the cost of EC2 instances. He wants to move certain nightly batch jobs to spot instances. He has hired you as a solutions architect to provide the initial guidance.
* If a spot request is persistent, then it is opened again after you stop the Spot Instance
* Spot blocks are designed to be interrupted, just like a spot instance
* Spot blocks are designed not to be interrupted
* If a spot request is persistent, then it is opened again after your Spot Instance is interrupted
* When you cancel an active spot request, it does not terminate the associated instance
* When you cancel an active spot request, it terminates the associated instance as well

### Question 15:
The DevOps team at an IT company has recently migrated to AWS and they are configuring security groups for their two-tier application with public web servers and private database servers. The team wants to understand the allowed configuration options for an inbound rule for a security group.
* You can use a range of IP addresses in CIDR block notation as the custom source for the inbound rule
* You can use an IP address as the custom source for the inbound rule
* You can use an Internet Gateway ID as the custom source for the inbound rule
* You can use a security group as the custom source for the inbound rule

### Question 16:
A retail company uses AWS Cloud to manage its IT infrastructure. The company has set up "AWS Organizations" to manage several departments running their AWS accounts and using resources such as EC2 instances and RDS databases. The company wants to provide shared and centrally-managed VPCs to all departments using applications that need a high degree of interconnectivity.
* Use VPC sharing to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC peering to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC peering to share one or more subnets with other AWS accounts belonging to the same parent organization from AWS Organizations
* Use VPC sharing to share a VPC with other AWS accounts belonging to the same parent organization from AWS Organizations

### Question 17:
The DevOps team at an IT company is provisioning a two-tier application in a VPC with a public subnet and a private subnet. The team wants to use either a NAT instance or a NAT gateway in the public subnet to enable instances in the private subnet to initiate outbound IPv4 traffic to the internet but needs some technical assistance in terms of the configuration options available for the NAT instance and the NAT gateway.
* NAT gateway supports port forwarding
* Security Groups can be associated with a NAT gateway
* Security Groups can be associated with a NAT instance
* NAT instance can be used as a bastion server
* NAT gateway can be used as a bastion server
* NAT instance supports port forwarding

### Question 18:
A media streaming company is looking to migrate its on-premises infrastructure into the AWS Cloud. The engineering team is looking for a fully managed NoSQL persistent data store with in-memory caching to maintain low latency that is critical for real-time scenarios such as video streaming and interactive content. The team expects the number of concurrent users to touch up to a million so the database should be able to scale elastically.
* ElastiCache
* RDS
* DocumentDB
* DynamoDB

### Question 19:
A freelance developer has built a Python based web application. The developer would like to upload his code to AWS Cloud and have AWS handle the deployment automatically. He also wants access to the underlying operating system for further enhancements.
* Amazon EC2
* AWS Elastic Container Service (ECS)
* AWS CloudFormation
* AWS Elastic Beanstalk

### Question 20:
An IT company is looking to move its on-premises infrastructure to AWS Cloud. The company has a portfolio of applications with a few of them using server bound licenses that are valid for the next year. To utilize the licenses, the CTO wants to use dedicated hosts for a one year term and then migrate the given instances to default tenancy thereafter.
* You can change the tenancy of an instance from host to dedicated
* You can change the tenancy of an instance from default to host
* You can change the tenancy of an instance from dedicated to host
* You can change the tenancy of an instance from default to dedicated
* You can change the tenancy of an instance from dedicated to default

### Question 21:
A leading hotel reviews business uses Amazon Web Services to store and process images for their website. The team uses Amazon EC2 and Amazon SQS in an integrated workflow to generate the sizes they need for each photo. SQS communicates the photos that need to be processed and the status of the jobs. Because of changes in the business processes, the engineering team is now migrating from SQS Standard queues to FIFO queues with batching.
* Make sure that the name of the FIFO queue ends with the .fifo suffix
* Make sure that the throughput for the target FIFO queue does not exceed 3,000 messages per second
* Delete the existing standard queue and recreate it as a FIFO queue
* Convert the existing standard queue into a FIFO queue
* Make sure that the name of the FIFO queue is the same as the standard queue
* Make sure that the throughput for the target FIFO queue does not exceed 300 messages per second

### Question 22:
The DevOps team at a multi-national company is helping its subsidiaries standardize EC2 instances by using the same Amazon Machine Image (AMI). Some of these subsidiaries are in the same AWS region but use different AWS accounts whereas others are in different AWS regions but use the same AWS account as the parent company. The DevOps team has hired you as a solutions architect for this project.
* Copying an AMI backed by an encrypted snapshot cannot result in an unencrypted target snapshot
* You can share an AMI with another AWS account
* You cannot share an AMI with another AWS account
* You cannot copy an AMI across AWS Regions
* You can copy an AMI across AWS Regions
* Copying an AMI backed by an encrypted snapshot results in an unencrypted target snapshot

### Question 23:
The data science team at a mobility company wants to analyze real-time location data of rides. The company is using Kinesis Data Firehose for delivering the location-specific streaming data into targets for downstream analytics.
* Amazon RedShift
* Amazon S3
* Amazon EMR
* Amazon Elasticsearch

### Question 24:
A multi-national company uses AWS Cloud to manage its IT infrastructure. The company has set up "AWS Organizations" to manage several departments running their AWS accounts. The departments operate from different countries and are spread across various AWS regions. The company wants to set up a consistent resource provisioning process across departments so that each resource follows pre-defined configurations such as using a specific type of EC2 instances, specific IAM roles for Lambda functions, etc.
* Use AWS CloudFormation StackSets to deploy the same template across AWS accounts and regions
* Use AWS CloudFormation templates to deploy the same template across AWS accounts and regions
* Use AWS CloudFormation stacks to deploy the same template across AWS accounts and regions
* Use AWS Resource Access Manager (RAM) to deploy the same template across AWS accounts and regions

### Question 25:
A data analytics company is running a proprietary database on an EC2 instance using EBS volumes. The database is heavily I/O bound. As a solutions architect, which of the following RAID configurations would you recommend improving the I/O performance?
* Amazon EBS does not support the standard RAID configurations
* Use RAID 0 when I/O performance is more important than fault tolerance
* Both RAID 0 and RAID 1 provide equally good I/O performance
* Use RAID 1 when I/O performance is more important than fault tolerance

### Question 26:
A startup has created a new web application for users to complete a risk assessment survey for COVID-19 symptoms via a self-administered questionnaire. The startup has purchased the domain covid19survey.com using Route 53. The web development team would like to create a Route 53 record so that all traffic for covid19survey.com is routed to www.covid19survey.com.
* Create an alias record for covid19survey.com that routes traffic to www.covid19survey.com
* Create an NS record for covid19survey.com that routes traffic to www.covid19survey.com
* Create an MX record for covid19survey.com that routes traffic to www.covid19survey.com
* Create a CNAME record for covid19survey.com that routes traffic to www.covid19survey.com

### Question 27:
A retail company has its flagship application running on a fleet of EC2 instances behind an Elastic Load Balancer (ELB). The engineering team has been seeing recurrent issues wherein the in-flight requests from the ELB to the EC2 instances are getting dropped when an instance becomes unhealthy.
* Cross Zone load balancing
* Sticky Sessions
* Idle Timeout
* Connection Draining

### Question 28:
An e-commerce company is planning to migrate their two-tier application from on-premises infrastructure to AWS Cloud. As the engineering team at the company is new to the AWS Cloud, they are planning to use the Amazon VPC console wizard to set up the networking configuration for the two-tier application having public web servers and private database servers.
* VPC with a public subnet only and AWS Site-to-Site VPN access
* VPC with public and private subnets and AWS Site-to-Site VPN access
* VPC with a single public subnet
* VPC with public and private subnets (NAT)

### Question 29:
A multi-national company is looking at optimizing their AWS resources across various countries and regions. They want to understand the best practices on cost optimization, performance, and security for their system architecture spanning across multiple business units.
* AWS Systems Manager
* AWS Management Console
* AWS Trusted Advisor
* AWS Config

### Question 30:
A silicon valley based healthcare startup uses AWS Cloud for its IT infrastructure. The startup stores patient health records on Amazon S3. The engineering team needs to implement an archival solution based on Amazon S3 Glacier to enforce regulatory and compliance controls on data access.
* Use S3 Glacier to store the sensitive archived data and then use an S3 Access Control List to enforce compliance controls
* Use S3 Glacier to store the sensitive archived data and then use an S3 lifecycle policy to enforce compliance controls
* Use S3 Glacier vault to store the sensitive archived data and then use an S3 Access Control List to enforce compliance controls
* Use S3 Glacier vault to store the sensitive archived data and then use a vault lock policy to enforce compliance controls

### Question 31:
A data analytics company is using SQS queues for decoupling the various processes of an application workflow. The company wants to postpone the delivery of certain messages to the queue by one minute while all other messages need to be delivered immediately to the queue.
* Use delay queues to postpone the delivery of certain messages to the queue by one minute
* Use message timers to postpone the delivery of certain messages to the queue by one minute
* Use dead-letter queues to postpone the delivery of certain messages to the queue by one minute
* Use visibility timeout to postpone the delivery of certain messages to the queue by one minute

### Question 32:
Which of the following S3 storage classes supports encryption by default for both data at rest as well as in-transit?
* Amazon S3 Glacier
* Amazon S3 One Zone-IA
* Amazon S3 Standard-Infrequent Access
* Amazon S3 Intelligent Tiering

### Question 33:
A big data consulting firm needs to set up a data lake on Amazon S3 for a retail client. The data lake is split in raw and refined zones. The source data arrives in the raw zone and is then processed via an AWS Glue based ETL job into the refined zone. The workflow also involves multiple lambda functions that perform data hygiene and data completeness checks in both the raw and refined zones. The firm is looking for an orchestration solution to manage this end to end workflow.
* Amazon EMR
* Amazon Simple Workflow Service (SWF)
* AWS Batch
* AWS Step Functions

### Question 34:
An e-commerce company is using an Elastic Load Balancer for its fleet of EC2 instances spread across two Availability Zones, with one instance as a target in Availability Zone A and four instances as targets in Availability Zone B. The company is doing benchmarking for server performance when cross-zone load balancing is enabled compared to the case when cross-zone load balancing is disabled.
* With cross-zone load balancing enabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives no traffic and four instances in Availability Zone B receive 25% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone A receives 20% traffic and four instances in Availability Zone B receive 20% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each
* With cross-zone load balancing enabled, one instance in Availability Zone A receives no traffic and four instances in Availability Zone B receive 25% traffic each. With cross-zone load balancing disabled, one instance in Availability Zone A receives 50% traffic and four instances in Availability Zone B receive 12.5% traffic each

### Question 35:
Computer vision researchers at a university are trying to optimize the I/O bound processes for a proprietary algorithm running on EC2 instances. The ideal storage would facilitate high-performance IOPS when doing file processing in a temporary storage space before uploading the results back into Amazon S3.
* Use EC2 instances with EBS Provisioned IOPS SSD (io1) as the storage option
* Use EC2 instances with EBS General Purpose SSD (gp2) as the storage option
* Use EC2 instances with Instance Store as the storage option
* Use EC2 instances with EBS Throughput Optimized HDD (st1) as the storage option

### Question 36:
A financial services company is migrating their messaging queues from self-managed message-oriented middleware systems to Amazon SQS. The development team at the company wants to minimize the costs of using SQS.
* Use SQS short polling to retrieve messages from your Amazon SQS queues
* Use SQS message timer to retrieve messages from your Amazon SQS queues
* Use SQS visibility timeout to retrieve messages from your Amazon SQS queues
* Use SQS long polling to retrieve messages from your Amazon SQS queues

### Question 37:
A social media company uses Amazon SQS queues to decouple their application architecture. The engineering team has observed message processing failures for an edge case scenario where comments posted to a story remain unprocessed if the original story itself is deleted by the author while the comments were being posted.
* Use a temporary queue to handle message processing failures
* Use long polling to handle message processing failures
* Use short polling to handle message processing failures
* Use a dead-letter queue to handle message processing failures

### Question 38:
An AWS Organization is using Service Control Policies (SCP) for central control over the maximum available permissions for all accounts in their organization. This allows the organization to ensure that all accounts stay within the organization’s access control guidelines.
* SCPs affect service-linked roles
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can still perform that action
* SCPs do not affect service-linked role
* If a user or role has an IAM permission policy that grants access to an action that is either not allowed or explicitly denied by the applicable SCPs, the user or role can't perform that action
* SCPs affect all users and roles in attached accounts, excluding the root user
* SCPs affect all users and roles in attached accounts, including the root user

### Question 39:
A pharmaceutical company is considering moving to AWS Cloud to accelerate the research and development process. Most of the daily workflows would be centered around running batch jobs on EC2 instances with storage on EBS volumes. The CTO is concerned about meeting HIPAA compliance norms for sensitive data stored on EBS.
* Any snapshot created from the volume is encrypted
* Data at rest inside the volume is NOT encrypted
* Data moving between the volume and the instance is encrypted
* Data moving between the volume and the instance is NOT encrypted
* Any snapshot created from the volume is NOT encrypted
* Data at rest inside the volume is encrypted

### Question 40:
A leading bank has moved its IT infrastructure to AWS Cloud and they have been using Amazon EC2 Auto Scaling for their web servers. This has helped them deal with traffic spikes effectively. But, their relational database has now become a bottleneck and they urgently need a fully managed auto scaling solution for their relational database to address any unpredictable changes in the traffic.
* Amazon DynamoDB
* Amazon Aurora Serverless
* Amazon Relational Database Service (Amazon RDS)
* Amazon Aurora

### Question 41:
A big data analytics company is looking to archive the on-premises data into a POSIX compliant file storage system on AWS Cloud. The archived data would be accessed for just about a week in a year.
* EFS Standard
* EFS Infrequent Access
* S3 Standard-IA
* S3 Standard

### Question 42:
A leading news aggregation company offers hundreds of digital products and services for customers ranging from law firms to banks to consumers. The company bills its clients based on per unit of clickstream data provided to the clients. As the company operates in a regulated industry, it needs to have the same ordered clickstream data available for auditing within a window of 7 days.
* AWS Kinesis Data Analytics
* Amazon SQS
* AWS Kinesis Data Firehose
* AWS Kinesis Data Streams

### Question 43:
An online gaming company wants to block access to its application from specific countries; however, the company wants to allow its remote development team (from one of the blocked countries) to have access to the application. The application is deployed on EC2 instances running under an Application Load Balancer (ALB) with AWS WAF.
* Use ALB IP set statement that specifies the IP addresses that you want to allow through
* Create a deny rule for the blocked countries in the NACL associated with each of the EC2 instances
* Use WAF IP set statement that specifies the IP addresses that you want to allow through
* Use WAF geo match statement listing the countries that you want to block
* Use ALB geo match statement listing the countries that you want to block

### Question 44:
A big data analytics company is using Kinesis Data Streams (KDS) to process IoT data from the field devices of an agricultural sciences company. Multiple consumer applications are using the incoming data streams and the engineers have noticed a performance lag for the data delivery speed between producers and consumers of the data streams.
* Swap out Kinesis Data Streams with Kinesis Data Firehose
* Swap out Kinesis Data Streams with SQS Standard queues
* Use Enhanced Fanout feature of Kinesis Data Streams
* Swap out Kinesis Data Streams with SQS FIFO queues

### Question 45:
An e-commerce company uses Microsoft Active Directory to provide users and groups with access to resources on the on-premises infrastructure. The company has extended its IT infrastructure to AWS in the form of a hybrid cloud. The engineering team at the company wants to run directory-aware workloads on AWS for a SQL Server-based application. The team also wants to configure a trust relationship to enable single sign-on (SSO) for its users to access resources in either domain.
* Simple AD
* AWS Managed Microsoft AD
* Amazon Cloud Directory
* AD Connector

### Question 46:
A financial services company wants to move the Windows file server clusters out of their datacenters. They are looking for cloud file storage offerings that provide full Windows compatibility. Can you identify the AWS storage services that provide highly reliable file storage that is accessible over the industry-standard Server Message Block (SMB) protocol compatible with Windows systems? (Select two)
* Amazon FSx for Windows File Server
* Elastic File System
* Elastic Block Storage
* Simple Storage Service (Amazon S3)
* File Gateway Configuration of AWS Storage Gateway

### Question 47:
A leading online gaming company is migrating its flagship application to AWS Cloud for delivering its online games to users across the world. The company would like to use a Network Load Balancer (NLB) to handle millions of requests per second. The engineering team has provisioned multiple instances in a public subnet and specified these instance IDs as the targets for the NLB.
* Traffic is routed to instances using the primary elastic IP address specified in the primary network interface for the instance
* Traffic is routed to instances using the primary public IP address specified in the primary network interface for the instance
* Traffic is routed to instances using the primary private IP address specified in the primary network interface for the instance
* Traffic is routed to instances using the instance ID specified in the primary network interface for the instance

### Question 48:
A software genomics company provides end-to-end genomic data analysis and reporting solutions to hospitals and labs. The company has multiple High Performance Computing (HPC) workflows that quickly and accurately process and analyze whole genomes and gene panels for hereditary diseases. The company is looking to migrate these workflows from their on-premises infrastructure to AWS Cloud.
* Elastic Fabric Adapter
* Elastic Network Interface
* Elastic Network Adapter
* Elastic IP Address

### Question 49:
A leading global measurement and data analytics company measures what the consumers watch and what advertising they’re exposed to. This real-time data is ingested into its on-premises data center and subsequently the daily data feed is compressed into a single file and uploaded on Amazon S3 for backup. The typical compressed file size is around 2 GB.
* Upload the compressed file using multipart upload with S3 transfer acceleration
* Upload the compressed file using multipart upload
* FTP the compressed file into an EC2 instance that runs in the same region as the S3 bucket. Then transfer the file from EC2 instance into the S3 bucket
* Upload the compressed file in a single operation

### Question 50:
A retail company wants to establish encrypted network connectivity between its on-premises data center and AWS Cloud. The company wants to get the solution up and running in the fastest possible time and it should also support encryption in transit.
* Use AWS Data Sync to establish encrypted network connectivity between the on-premises data center and AWS Cloud
* Use AWS Direct Connect to establish encrypted network connectivity between the on-premises data center and AWS Cloud
* Use AWS Secrets Manager to establish encrypted network connectivity between the on-premises data center and AWS Cloud
* Use Site-to-Site VPN to establish encrypted network connectivity between the on-premises data center and AWS Cloud

### Question 51:
A leading media company wants to do an accelerated online migration of hundreds of terabytes of files from their on-premises data center to Amazon S3 and then establish a mechanism to access the migrated data for ongoing updates from the on-premises applications.
* Use S3 Transfer Acceleration to migrate existing data to Amazon S3 and then use DataSync for ongoing updates from the on-premises applications
* Use AWS DataSync to migrate existing data to Amazon S3 and then use File Gateway to retain access to the migrated data for ongoing updates from the on-premises applications
* Use AWS DataSync to migrate existing data to Amazon S3 as well as access the S3 data for ongoing updates
* Use File Gateway configuration of AWS Storage Gateway to migrate data to Amazon S3 and then use S3 Transfer Acceleration for ongoing updates from the on-premises applications

### Question 52:
An e-commerce company runs its web application on EC2 instances in an Auto Scaling group and it's configured to handle consumer orders in an SQS queue for downstream processing. The DevOps team has observed that the performance of the application goes down in case of a sudden spike in orders received.
* Use a scheduled scaling policy based on a custom Amazon SQS queue metric
* Use a simple scaling policy based on a custom Amazon SQS queue metric
* Use a target tracking scaling policy based on a custom Amazon SQS queue metric
* Use a step scaling policy based on a custom Amazon SQS queue metric

### Question 53:
A video conferencing application is hosted on a fleet of EC2 instances which are part of an Auto Scaling group (ASG). The ASG uses a Launch Configuration (LC1) with "dedicated" instance placement tenancy but the VPC (V1) used by the Launch Configuration LC1 has the instance tenancy set to default. Later the DevOps team creates a new Launch Configuration (LC2) with "default" instance placement tenancy but the VPC (V2) used by the Launch Configuration LC2 has the instance tenancy set to dedicated.
* The instances launched by Launch Configuration LC1 will have default instance tenancy while the instances launched by the Launch Configuration LC2 will have dedicated instance tenancy
* The instances launched by Launch Configuration LC1 will have dedicated instance tenancy while the instances launched by the Launch Configuration LC2 will have default instance tenancy
* The instances launched by both Launch Configuration LC1 and Launch Configuration LC2 will have dedicated instance tenancy
* The instances launched by both Launch Configuration LC1 and Launch Configuration LC2 will have default instance tenancy

### Question 54:
A financial services company is looking to move its on-premises IT infrastructure to AWS Cloud. The company has multiple long-term server bound licenses across the application stack and the CTO wants to continue to utilize those licenses while moving to AWS.
* Use EC2 dedicated instances
* Use EC2 dedicated hosts
* Use EC2 on-demand instances
* Use EC2 reserved instances

### Question 55:
A social media company runs its IT infrastructure on the AWS Cloud. The company has a batch job running at 1 am daily that takes a backup of the media assets uploaded for the past day and the entire job takes about 3 hours to run. The company wants to use the MOST cost-effective long-term purchasing option for EC2 instances such that the job is guaranteed to run during the defined time window.
* On-Demand Instances
* Spot Instances
* Scheduled Reserved Instances
* Dedicated Instances

### Question 56:
A sports data company is delivering real-time data to media companies, sports federations, and the betting industry using its IT infrastructure on AWS Cloud. The company wants an urgent solution that provides a low-latency way to ingest live sports results regardless of where in the world their sports journalists are sitting. The live sports results are delivered via a proprietary application using UDP protocol.
* Use Auto Scaling group to provide a low latency way to ingest live sports results
* Use CloudFront to provide a low latency way to ingest live sports results
* Use Global Accelerator to provide a low latency way to ingest live sports results
* Use Elastic Load Balancer to provide a low latency way to ingest live sports results

### Question 57:
An AI research group at a university uses a proprietary speech synthesis application hosted on an EC2 instance. When started, the instance takes a long time to build a memory footprint for all the auxiliary software libraries required for the application to function. The research group would like to pre-warm the instances so they can launch the analysis right away when needed.
* Create an Auto Scaling Group (ASG) with capacity 0
* Use a custom AMI with auxiliary software libraries pre-installed
* Use EC2 hibernate
* Use Spot Instances

### Question 58:
A big data analytics company is working on a real-time vehicle tracking solution. The data processing workflow involves both I/O intensive and throughput intensive database workloads. The development team needs to store this real-time data in a NoSQL database hosted on an EC2 instance and needs to support up to 25,000 IOPS per volume.
* Throughput Optimized HDD (st1)
* Cold HDD (sc1)
* General Purpose SSD (gp2)
* Provisioned IOPS SSD (io1)

### Question 59:
An IT company is using SQS queues for decoupling the various components of application architecture. As the consuming components need additional time to process SQS messages, the company wants to postpone the delivery of new messages to the queue for a few seconds.
* Use visibility timeout to postpone the delivery of new messages to the queue for a few seconds
* Use FIFO queues to postpone the delivery of new messages to the queue for a few seconds
* Use delay queues to postpone the delivery of new messages to the queue for a few seconds
* Use dead-letter queues to postpone the delivery of new messages to the queue for a few seconds

### Question 60:
The CTO at an IT company wants to move away from license-based, expensive, and legacy commercial database solutions deployed at the on-premises data center to more efficient, open-source, and cost-effective options on AWS Cloud. At the same time, the CTO is concerned about identifying areas for data-conversion that require special attention during migration since the on-premises databases have multiple active complex configurations such as secondary indexes, foreign keys, and stored procedures.
* Basic Schema Copy
* AWS Snowball Edge
* AWS Database Migration Service
* AWS Schema Conversion Tool
* AWS Glue

### Question 61:
A DevOps engineer at an IT company just upgraded an EC2 instance type from t2.nano (0.5G of RAM, 1 vCPU) to u-12tb1.metal (12.3 TB of RAM, 448 vCPUs). How would you categorize this upgrade?
* This is a scale-out example of vertical scalability
* This is a scale-up example of horizontal scalability
* This is an example of high availability
* This is a scale-up example of vertical scalability

### Question 62:
A retail organization is moving some of its on-premises data to AWS Cloud. The DevOps team at the organization has set up an AWS Managed IPSec VPN Connection between their remote on-premises network and their Amazon VPC over the internet.
* Create a Virtual Private Gateway on the on-premises side of the VPN and a Customer Gateway on the AWS side of the VPN
* Create a Virtual Private Gateway on both the AWS side of the VPN as well as the on-premises side of the VPN
* Create a Customer Gateway on both the AWS side of the VPN as well as the on-premises side of the VPN
* Create a Virtual Private Gateway on the AWS side of the VPN and a Customer Gateway on the on-premises side of the VPN

### Question 63:
A media company wants to use clickstream for data science tasks, develop algorithms, and create visualizations and dashboards to support the business stakeholders. Each of these groups work independently and would need real-time access to this clickstream data for their applications.
* AWS Kinesis Data Firehose
* Amazon SQS
* AWS Kinesis Data Streams
* AWS Kinesis Data Analytics

### Question 64:
A leading interactive entertainment company for the mobile world has a hybrid cloud structure for its on-premises data center and AWS Cloud infrastructure. The company wants to build a web log archival solution such that only the most frequently accessed logs are available as cached data locally while backing up all logs on Amazon S3.
* Use AWS Snowball Edge Storage Optimized device to store the most frequently accessed logs locally for low-latency access while storing the full backup of logs in an Amazon S3 bucket
* Use AWS direct connect to store the most frequently accessed logs locally for low-latency access while storing the full backup of logs in an Amazon S3 bucket
* Use AWS Volume Gateway - Cached Volume - to store the most frequently accessed logs locally for low-latency access while storing the full volume with all logs in its Amazon S3 service bucket
* Use AWS Volume Gateway - Stored Volume - to store the most frequently accessed logs locally for low-latency access while storing the full volume with all logs in its Amazon S3 service bucket

### Question 65:
A social media startup uses AWS Cloud to manage its IT infrastructure. The engineering team at the startup wants to perform weekly database rollovers for a MySQL database server using a serverless cron job that typically takes about 5 minutes to execute the database rollover script written in Python. The database rollover will archive the past week’s data from the production database to keep the database small while still keeping its data accessible.
* Create a time-based schedule option within an AWS Glue job to invoke itself every week and run the database rollover script
* Schedule a weekly CloudWatch event cron expression to invoke a Lambda function that runs the database rollover job
* Provision an EC2 scheduled reserved instance to run the database rollover script to be run via an OS-based weekly cron expression
* Provision an EC2 spot instance to run the database rollover script to be run via an OS-based weekly cron expression



# Exam 4

### Question 1:
You have an S3 bucket that contains files in different subfolders, for example `s3://my-bucket/images` and `s3://my-bucket/thumbnails`. When an image is first uploaded and new, it is viewed several times. But after 45 days, analytics prove that image files are on average rarely requested, but the thumbnails still are. After 180 days, you would like to archive the image files and the thumbnails. Overall you would like to remain highly available to prevent disasters happening against a whole AZ.
* Create a Lifecycle Policy to transition objects to S3 One Zone IA using a prefix after 45 days
* Create a Lifecycle Policy to transition objects to Glacier using a prefix after 180 days
* Create a Lifecycle Policy to transition all objects to S3 Standard IA after 45 days
* Create a Lifecycle Policy to transition objects to S3 Standard IA using a prefix after 45 days
* Create a Lifecycle Policy to transition all objects to Glacier after 180 days

### Question 2:
A niche social media application allows users to connect with sports athletes. As a solutions architect, you've designed the architecture of the application to be fully serverless using API Gateway & AWS Lambda. The backend is leveraging a DynamoDB table. Some of the star athletes using the application are highly popular, and therefore DynamoDB has increased the RCUs. Still, hotkey experiencing a hot partition problem.
* Use DynamoDB Global Tables
* Use Amazon ElastiCache
* Use DynamoDB DAX
* Use DynamoDB Streams

### Question 3:
A company runs a popular dating website on the AWS Cloud. As a Solutions Architect, you've designed the architecture of the website to follow a serverless pattern on the AWS Cloud using API Gateway and AWS Lambda. The backend is leveraging an RDS PostgreSQL database. Currently, you are using a classic username and password combination to connect the Lambda function to the RDS database.
* Attach an AWS Identity and Access Management (IAM) role to AWS Lambda
* Deploy AWS Lambda in a VPC
* Restrict the RDS database security group to the Lambda's security group
* Use IAM authentication from Lambda to RDS PostgreSQL
* Embed a credential rotation logic in the AWS Lambda, retrieving them from SSM

### Question 4:
You are working as an AWS architect for a government facility that manages a critical application for the government. You are asked to set up a Disaster Recovery (DR) mechanism with minimum costs to make sure that there is no loss of critical data in case of failure.
* Warm Standby
* Pilot Light
* Multi-Site
* Backup and Restore

### Question 5:
A digital media company needs to manage uploads of around 1TB from an application being used by a partner company.
* Use Direct Connect to provide extra bandwidth
* Use Amazon S3 Versioning
* Use AWS Snowball
* Use multi-part upload feature of Amazon S3

### Question 6:
Your company is building a music sharing platform on which users can upload the songs of their choice. As a solutions architect for the platform, you have designed an architecture that will leverage a Network Load Balancer linked to an Auto Scaling Group across multiple availability zones. You are currently running with 100 Amazon EC2 instances with an Auto Scaling Group that needs to be able to share the storage layer for the music files.
* Amazon Elastic File System (Amazon EFS)
* EBS volumes mounted in RAID 1
* Instance Store
* EBS volumes mounted in RAID 0

### Question 7:
One of the biggest global oil and gas companies has recently migrated to the AWS Cloud. To reap the benefits of speed of data collection, flexibility, and rapid experimentation via the Internet of Things (IoT) devices, the company is planning on distributing a sensor to install at individual residents to measure the temperature and make adjustments to the heating system. To provide adjustment commands, the company would like to have a streaming system that performs real-time analytics on the data. Once the analytics are done, the company would like to send notifications back to the mobile applications of the users.
* Amazon Kinesis with Amazon Simple Notification Service (SNS)
* Amazon Kinesis with Simple Email Service (Amazon SES)
* Amazon Simple Queue Service (SQS) with Amazon Simple Notification Service (SNS)
* Amazon Kinesis with Simple Queue Service (SQS)

### Question 8:
Your company runs a website for evaluating coding skills. As a Solutions Architect, you've designed the architecture of the website to follow a serverless pattern on the AWS Cloud using API Gateway and AWS Lambda. The backend is leveraging an RDS PostgreSQL database. Caching is implemented using a Redis ElastiCache cluster. You would like to increase the security of your authentication to Redis from the Lambda function, leveraging a username and password combination.
* Use Redis Auth
* Enable KMS Encryption
* Use IAM Auth and attach an IAM role to Lambda
* Create an inbound rule to restrict access to Redis Auth only from the Lambda security group

### Question 9:
A company hosting a Network File System on-premise, has managed it well till date. However, the teams have realized that it is getting challenging to manage the entire process and the company is looking to adopt an hybrid cloud strategy to connect their on-premise applications to an AWS NFS that is backed by Amazon S3.
* Storage Gateway File
* Amazon Elastic File System (Amazon EFS)
* Storage Gateway Tape
* Storage Gateway Volume

### Question 10:
A Big Data processing company has created a distributed data processing framework that performs best if the network performance between the processing machines is high. The application has to be deployed on AWS, and the company is only looking at performance as its key measure.
* Use Spot Instances
* Use a Cluster placement group
* Use a Spread placement group
* Optimize the EC2 kernel using EC2 User Data

### Question 11:
A company has been evolving towards creating sandbox environments for developers. The entire infrastructure is managed by AWS CloudFormation to easily recreate stack. An RDS database is managed by CloudFormation in a "dev" environment and has been costing a lot, as it has been mirroring the production setup. After running cost analysis reports, you realize that the storage layer (io1) accounts for 90% of the cost, and the remaining 10% is used by EC2 instance. The CloudWatch metrics report that both the EC2 instance and the EBS volume are under-utilized. The CloudWatch metrics show the EBS volume does frequent IO bursts, but the database is rarely steadily used.
* Convert the Amazon EC2 instance EBS volume to gp2
* Change the Amazon EC2 instance type to something much smaller
* Keep the EBS volume to io1 and reduce the IOPS
* Don't use a CloudFormation template to create the database as the CloudFormation service incurs greater service charges

### Question 12:
An IT company is working on an engagement to revamp a monolith CRM application into a modern de-coupled application built on AWS Cloud. From a solutions architecture perspective, the new application has been written from scratch keeping in mind the best practices for performance and resilience. To finalize the migration to the new architecture, you have updated a Route 53 simple record to point "myapp.mydomain.com" from the old Load Balancer to the new one.
* The health checks are failing
* The CNAME Record is misconfigured
* The TTL is still in effect
* The Alias Record is misconfigured

### Question 13:
You are working for a SaaS (Software as a Service) company as a solutions architect and help design solutions for the company's customers. One of the customers is a bank and has a requirement to whitelist up to two public IPs when the bank is accessing external services across the internet.
* Use a Network Load Balancer with an Auto Scaling Group (ASG)
* Use an Auto Scaling Group (ASG) with Dynamic Elastic IPs attachment
* Use an Application Load Balancer with an Auto Scaling Group (ASG)
* Use a Classic Load Balancer with an Auto Scaling Group (ASG)

### Question 14:
A company has grown from a small startup to an enterprise employing over 1000 people. As part of the scaling up of the AWS Cloud teams, the company has observed some strange behavior with S3 buckets settings being changed regularly.
* Implement an IAM policy to forbid users to change S3 bucket settings
* Use S3 access logs to analyze user access using Athena
* Implement a bucket policy requiring MFA for all operations
* Use CloudTrail to analyze API calls

### Question 15:
You started a new job as a Solutions Architect in a big company that has both AWS experts and people learning AWS. You would like to have everyone empowered for building and configuring best-practices driven architecture without making manual mistakes. Recently, an intern misconfigured a newly created RDS database which resulted in a production outage.
* Attach an IAM policy to interns preventing them from creating an RDS database
* Store your recommendations in a custom Trusted Advisor rule
* Use CloudFormation to manage RDS databases
* Create a Lambda function which sends emails when it finds misconfigured RDS databases

### Question 16:
Your firm has implemented a multi-tiered networking structure within the VPC - two public and two private subnets. The public subnets are used to deploy the Application Load Balancers, while the two private subnets are used to deploy the application on Amazon EC2 instances. As part of the firm's security and compliance needs, they need the Amazon EC2 instances to have access to the internet.
* Egress-Only Internet Gateways deployed in your private subnet
* NAT Instances deployed in your public subnet
* Internet Gateways deployed in your private subnet
* NAT Gateways deployed in your public subnet

### Question 17:
An e-commerce website is migrating towards a microservices-based approach for their website and plans to expose their website from the same load balancer, linked to different target groups with different URLs: checkout.mycorp.com, www.mycorp.com, mycorp.com/products, and mycorp.com/orders. The website would like to use ECS on the backend to manage these microservices and possibly host the same container of the application multiple times on the same EC2 instance.
* Application Load Balancer + dynamic port mapping
* Application Load Balancer + Reverse Proxy running as a Docker daemon on each ECS host
* Classic Load Balancer + dynamic port mapping
* Network Load Balancer + dynamic port mapping

### Question 18:
A junior developer has downloaded a sample Amazon S3 bucket policy to make changes to it based on new company-wide access policies. He has requested your help in understanding this bucket policy.
* It authorizes an IP address and a CIDR to access the S3 bucket
* It ensures the S3 bucket is exposing an external IP within the CIDR range specified, except one IP
* It ensures EC2 instances that have inherited a security group can access the bucket
* It authorizes an entire CIDR except one IP address to access the S3 bucket

### Question 19:
One of the largest consumer electronics companies has a suite of smart products and services which feature Artificial Intelligence (AI) technology. The company embeds Wi-Fi chips in these smart products, which allows these products to communicate with each other while learning about their user’s behavioral patterns and environment. The company is planning on distributing a master sensor in people's homes to measure the key metrics from these smart products and make adjustments to the default settings for these products. In order to provide adjustment commands, the company would like to have a streaming system that supports ordered data based on the sensor's key, and also sustains high throughput messages (thousands of messages per second).
* Amazon Simple Queue Service (SQS)
* Amazon Simple Notification Service (SNS)
* Amazon Kinesis Data Streams (KDS)
* AWS Lambda

### Question 20:
A financial services firm has traditionally operated with an on-premise data center and would like to create a disaster recovery strategy leveraging the AWS Cloud.
* Backup and Restore
* Multi Site
* Warm Standby
* Pilot Light

### Question 21:
As a solutions architect, you have created a solution that utilizes an Application Load Balancer with stickiness and an Auto Scaling Group (ASG). The ASG spawns across 2 Availability Zones (AZ). AZ-A has 3 EC2 instances and AZ-B has 4 EC2 instances. The ASG is about to go into a scale-in event due to the triggering of a CloudWatch alarm.
* A random instance in the AZ-A will be terminated
* The instance with the oldest launch configuration will be terminated in AZ-B
* An instance in the AZ-A will be created
* A random instance will be terminated in AZ-B

### Question 22:
A silicon valley based startup helps its users legally sign highly confidential contracts. In order to meet the strong industry requirements and governance guidelines, the startup must ensure that the signed contracts are encrypted using the AES-256 algorithm via an encryption key that is generated internally. The startup is now migrating to AWS Cloud and would like you, a Solution Architect, to advise them on the encryption scheme to adopt. The startup wants to continue using their existing encryption key generation mechanism.
* SSE-S3
* Client-Side Encryption
* SSE-KMS
* SSE-C

### Question 23:
A company runs a niche e-commerce website on the AWS Cloud. As a Solutions Architect, you've designed the architecture of the website to follow some serverless pattern on the API side, with API Gateway and AWS Lambda. The backend is leveraging an RDS Aurora MySQL database. The web portal was initially launched in the Americas, and it has been doing well and the company would like to expand it to Europe, where a read-only version will be available to improve latency. You plan on deploying the API Gateway and AWS Lambda using CloudFormation, but would like to have a read-only copy of your data in Europe as well.
* Create a Lambda function to periodically back up and restore the Aurora database in another region
* Use Aurora Multi-AZ
* Use a DynamoDB Streams
* Use Aurora Read Replicas

### Question 24:
Your company is evolving towards a microservice approach for their website. The company plans to expose the website from the same load balancer, linked to different target groups with different URLs, that are similar to these - checkout.mycorp.com, www.mycorp.com, mycorp.com/profile, and mycorp.com/search.
* Create a Network Load Balancer
* Create an Application Load Balancer
* Create a Classic Load Balancer
* Create an NGINX based load balancer on an EC2 instance to have advanced routing capabilities

### Question 25:
A photo hosting service publishes a master pack of beautiful mountain images, every month, that are over 50 GB in size and downloaded all around the world. The content is currently hosted on EFS and distributed by Elastic Load Balancing (ELB) and Amazon EC2 instances. The website is experiencing high load each month and very high network costs.
* Host the master pack onto Amazon S3 for faster access
* Upgrade the Amazon EC2 instances
* Create a CloudFront distribution
* Enable ELB caching

### Question 26:
A team has around 200 users, each of these having an IAM user account in AWS. Currently, they all have read access to an Amazon S3 bucket. The team wants 50 among them to have write and read access to the buckets.
* Create a group, attach the policy to the group and place the users in the group
* Create a policy and assign it manually to the 50 users
* Update the S3 bucket policy
* Create an MFA user with read / write access and link 50 IAM with MFA

### Question 27:
Your company is deploying a website running on Elastic Beanstalk. The website takes over 45 minutes for the installation and contains both static as well as dynamic files that must be generated during the installation process.
* Use EC2 user data to install the application at boot time
* Store the installation files in S3 so they can be quickly retrieved
* Use EC2 user data to customize the dynamic installation parts at boot time
* Use Elastic Beanstalk deployment caching feature
* Create a Golden AMI with the static installation components already setup

### Question 28:
Your company runs a web portal to match developers to clients who need their help. As a solutions architect, you've designed the architecture of the website to be fully serverless with API Gateway & AWS Lambda. The backend is leveraging a DynamoDB table. You would like to automatically congratulate your developers on important milestones, such as - their first paid contract. All the contracts are stored in DynamoDB.
* Amazon SQS + Lambda
* DynamoDB DAX + API Gateway
* CloudWatch Events + Lambda
* DynamoDB Streams + Lambda

### Question 29:
As a Solutions Architect, you have set up a database on a single EC2 instance that has an EBS volume of type gp2. You currently have 300GB of space on the gp2 device. The EC2 instance is of type m5.large. The database performance has recently been poor and upon looking at CloudWatch, you realize the IOPS on the EBS volume is maxing out. The disk size of the database must not change because of a licensing issue.
* Stop the CloudWatch agent to improve performance
* Convert the EC2 instance to an i3.4xlarge
* Increase the IOPS on the gp2 volume
* Convert the gp2 volume to an io1

### Question 30:
As a Solutions Architect, you would like to completely secure the communications between your CloudFront distribution and your S3 bucket which contains the static files for your website. Users should only be able to access the S3 bucket through CloudFront and not directly.
* Create a bucket policy to only authorize the IAM role attached to the CloudFront distribution
* Update the S3 bucket security groups to only allow traffic from the CloudFront security group
* Create an origin access identity (OAI) and update the S3 Bucket Policy
* Make the S3 bucket public

### Question 31:
You are working as a Solutions Architect for a photo processing company that has a proprietary algorithm to compress an image without any loss in quality. Because of the efficiency of the algorithm, your clients are willing to wait for a response that carries their compressed images back. You also want to process these jobs asynchronously and scale quickly, to cater to the high demand. Additionally, you also want the job to be retried in case of failures.
* EC2 Spot Instances
* Amazon Simple Queue Service (SQS)
* EC2 Reserved Instances
* Amazon Simple Notification Service (SNS)
* EC2 On-Demand Instances

### Question 32:
The engineering team at a global e-commerce company is currently reviewing their disaster recovery strategy. The team has outlined that they need to be able to quickly recover their application stack with a Recovery Time Objective (RTO) of 5 minutes, in all of the AWS Regions that the application runs. The application stack currently takes over 45 minutes to install on a Linux system.
* Create an AMI after installing the software and copy the AMI across all Regions. Use this Region-specific AMI to run the recovery process in the respective Regions
* Use Amazon EC2 user data to speed up the installation process
* Create an AMI after installing the software and use this AMI to run the recovery process in other Regions
* Store the installation files in Amazon S3 for quicker retrieval

### Question 33:
The engineering team at a leading e-commerce company is anticipating a surge in the traffic because of a flash sale planned for the weekend. You have estimated the web traffic to be 10x. The content of your website is highly dynamic and changes very often.
* Deploy the website on S3
* Use a CloudFront distribution in front of your website
* Use a Route53 Multi Value record
* Use an Auto Scaling Group

### Question 34:
A leading social media startup has developed a mobile app that allows users to create custom animated videos and share it with their friends. The app has grown at a rate of 150% new users on a month by month basis over the last 1 year. The startup is now moving to AWS Cloud to better manage the IT infrastructure and scale efficiently. The engineering team is evaluating various AWS services as part of the solution stack for the data store layer. The AWS service should be able to handle some complicated queries such as "What are the number of likes on the videos that have been posted by friends of a user A?".
* Amazon Aurora
* Amazon ElasticSearch
* Amazon Neptune
* Amazon Redshift

### Question 35:
You are a long-time Solutions Architect for your company that has been traditionally operating with an on-premise data center. As part of the new strategic direction from the CTO, you are adopting hybrid cloud infrastructure to leverage some AWS services such as S3. Yet, your company needs strong security requirements to have a connection between your on-premise data center and AWS to be private. In case of failures though, it needs to guarantee uptime over security and is willing to use the public internet.
* Use Site to Site VPN as a backup connection
* Use Egress Only Internet Gateway as a backup connection
* Use Direct Connect as a primary connection
* Use Direct Connect as a backup connection
* Use Site to Site VPN as a primary connection

### Question 36:
You have built an application that is deployed with an Elastic Load Balancer and an Auto Scaling Group. As a Solutions Architect, you have configured aggressive CloudWatch alarms, making your Auto Scaling Group (ASG) scale in and out very quickly, renewing your fleet of Amazon EC2 instances on a daily basis. A production bug appeared two days ago, but the team is unable to SSH into the instance to debug the issue, because the instance has already been terminated by the ASG. The log files are saved on the EC2 instance.
* Use AWS Lambda to regularly SSH into the EC2 instances and copy the log files to S3
* Install a CloudWatch Logs agents on the EC2 instances to send logs to CloudWatch
* Make a snapshot of the EC2 instance just before it gets terminated
* Disable the Termination from the ASG any time a user reports an issue

### Question 37:
Your company has created a data warehouse using Redshift that is used to analyze data from Amazon S3. From the usage pattern, you have detected that after 30 days, the data is rarely queried in Redshift and it's not "hot data" anymore. You would like to preserve the SQL querying capability on your data and get the queries started immediately. Also, you want to adopt a pricing model that allows you to save the maximum amount of cost on Redshift.
* Migrate the Redshift underlying storage to S3 IA
* Move the data to S3 Standard IA after 30 days
* Analyze the cold data with Athena
* Move the data to S3 Glacier after 30 days
* Create a smaller Redshift Cluster with the cold data

### Question 38:
A developer in your team has set up a classic 3 tier architecture composed of an Application Load Balancer, an Auto Scaling group managing a fleet of EC2 instances, and an Aurora database. As a Solutions Architect, you would like to adhere to the security pillar of the well-architected framework.
* Add a rule authorizing the EC2 security group
* Add a rule authorizing the Aurora security group
* Add a rule authorizing the ASG's subnets CIDR
* Add a rule authorizing the ELB security group

### Question 39:
A company helps its customers legally sign highly confidential contracts. To meet the strong industry requirements, the company must ensure that the signed contracts are encrypted using the company's proprietary algorithm. The company is now migrating to AWS Cloud using AWS S3 and would like you, the solution architect, to advise them on the encryption scheme to adopt.
* SSE-KMS
* SSE-C
* Client Side Encryption
* SSE-S3

### Question 40:
A developer in your company has set up a classic 2 tier architecture consisting of an Application Load Balancer and an Auto Scaling group (ASG) managing a fleet of EC2 instances. The ALB is deployed in a subnet of size 10.0.1.0/18 and the ASG is deployed in a subnet of size 10.0.4.0/17.
* Add a rule to authorize the CIDR 10.0.4.0/17
* Add a rule to authorize the CIDR 10.0.1.0/18
* Add a rule to authorize the security group of the ALB
* Add a rule to authorize the security group of the ASG

### Question 41:
A leading e-commerce company runs its IT infrastructure on AWS Cloud. The company has a batch job running at 7 am daily on an RDS database. It processes shipping orders for the past day, and usually gets around 2000 records that need to be processed sequentially in a batch job via a shell script. The processing of each record takes about 3 seconds.
* Amazon EC2
* AWS Lambda
* AWS Glue
* Amazon Kinesis Data Streams

### Question 42:
One of the largest Ed-tech platforms boasts of a learning-management system being used by more than 100 million users across the globe. Of late, the company has been finding it difficult to scale its business. That’s because the company’s most popular applications, including the learning-management system, are hosted on more than 30 on-premises data centers throughout the world. The engineering team at the company wants to migrate to AWS Cloud and is currently evaluating Amazon RDS as its main database. To ensure High Availability, the team wants to go for Multi-AZ deployment and they would like to understand what happens when the primary instance in Multi-AZ goes down.
* The CNAME record will be updated to point to the standby DB
* The application will be down until the primary database has recovered itself
* An email will be sent to the System Administrator asking for manual intervention
* The URL to access the database will change to the standby DB

### Question 43:
As an e-sport tournament hosting company, you have servers that need to scale and be highly available. Therefore you have deployed an Elastic Load Balancer (ELB) with an Auto Scaling group (ASG) across 3 Availability Zones (AZs). When e-sport tournaments are running, the servers need to scale quickly. And when tournaments are done, the servers can be idle. As a general rule, you would like to be highly available, have the capacity to scale and optimize your costs.
* Use Reserved Instances for the minimum capacity
* Set the minimum capacity to 3
* Set the minimum capacity to 1
* Use Dedicated hosts for the minimum capacity
* Set the minimum capacity to 2

### Question 44:
As a Solutions Architect, you are responsible for all operations in the us-west-1 region, which has a complex infrastructure composed of several Lambda functions, API Gateways and DynamoDB tables. As part of the disaster recovery strategy, you would like to be in a position to quickly re-create your entire infrastructure in another region, if needed.
* AWS OpsWorks
* AWS CloudFormation
* AWS Elastic Beanstalk
* AWS Trusted Advisor

### Question 45:
A company's business logic is built on several microservices, running on-premise. They currently communicate using a message broker that supports the MQTT protocol. The company is looking at migrating these applications and the message broker to AWS Cloud without changing the application logic.
* Amazon Simple Notification Service (SNS)
* Amazon Kinesis Data Streams
* Amazon MQ
* Amazon Simple Queue Service (SQS)

### Question 46:
As part of the design of a mobile application, a firm has decided to use a traditional serverless architecture using AWS Lambda, API Gateway & DynamoDB. The firm is looking for a technology that allows the users to connect through a Google login and have the capability to turn on MFA (Multi-Factor Authentication) to have maximum security. Ideally, the solution should be fully managed by AWS.
* Enable the AWS Google Login Service
* AWS Identity and Access Management (IAM)
* Amazon Cognito
* Write a Lambda function with Auth0 3rd party integration

### Question 47:
A development team has deployed a microservice to the ECS. The application layer is in a Docker container that provides both static and dynamic content through an Application Load Balancer. With increasing load, the ECS cluster is experiencing higher network usage. The development team has drilled into the network usage and found that 90% of it is due to distributing static content of the application.
* Distribute the static content through Amazon EFS
* Distribute the dynamic content through Amazon S3
* Distribute the dynamic content through Amazon EFS
* Distribute the static content through Amazon S3

### Question 48:
An application deployed to Elastic Beanstalk uses Amazon DynamoDB as the data layer. Recently, your database has seen a spike in writes and your users often get errors from your application because of the writes being unsuccessful due to a throughput provisioned exception. You would like to prevent your users from seeing these errors while guaranteeing them that the data they're trying to write to the backend will be written. You have decided to de-couple the application layer from the database layer and dedicate a worker process to writing the data to DynamoDB.
* Amazon Simple Queue Service (SQS)
* Amazon Simple Notification Service (SNS)
* Kinesis Data Streams
* DynamoDB DAX

### Question 49:
A company has recently created a new department to handle their services workload. An IT team has been asked to create a custom VPC to isolate the resources created in this new department. They have set up the public subnet and internet gateway (IGW). However, they are not able to ping the Amazon EC2 instances with Elastic IP launched in the newly created VPC.
* Disable Source / Destination check on the EC2 instance
* Contact AWS support to map your VPC with subnet
* Create a secondary IGW to attach with public subnet and move the current IGW to private and write route tables
* Check if the route table is configured with IGW
* Check if the security groups allow ping from the source

### Question 50:
Your company has deployed an application that will perform a lot of overwrites and deletes on data and require the latest information to be available anytime data is read via queries on database tables.
* Amazon ElastiCache
* Amazon Neptune
* Amazon Simple Storage Service (Amazon S3)
* Amazon Relational Database Service (Amazon RDS)

### Question 51:
A CRM web application was written as a monolith in PHP and is facing scaling issues because of performance bottlenecks. The CTO wants to re-engineer towards microservices architecture and expose their website from the same load balancer, linked to different target groups with different URLs: checkout.mycorp.com, www.mycorp.com, mycorp.com/profile and mycorp.com/search. The CTO would like to expose all these URLs as HTTPS endpoints for security purposes.
* Change the ELB SSL Security Policy
* Use a wildcard SSL certificate
* Use SSL certificates with SNI
* Use an HTTP to HTTPS redirect

### Question 52:
Due to COVID-19 pandemic, a large social media company has asked more than 90% of its employees to work remotely. The rapid growth of remote and mobile workers has put tremendous pressure on IT to provide fast, easy access to corporate applications from the device of choice. The company is looking for an AWS service to help mobile and remote employees access the applications needed, by delivering a cloud desktop, accessible anywhere with an internet connection, using any supported device.
* AWS AppSync
* AWS Organizations
* AWS Single Sign-On (SSO)
* Amazon Workspaces

### Question 53:
As a Solutions Architect, you are tasked to design a distributed application that will run on various EC2 instances. This application needs to have the highest performance local disk to cache data. Also, data is copied through an EC2 to EC2 replication mechanism. It is acceptable if the instance loses its data when stopped or terminated.
* Amazon Elastic File System (Amazon EFS)
* Amazon Simple Storage Service (Amazon S3)
* Instance Store
* Amazon Elastic Block Store (EBS)

### Question 54:
Your company is building a video streaming service accessible to users who have paid an ongoing subscription. The subscription data is stored in DynamoDB. You would like to expose the users to a serverless architecture allowing them to request the video files that sit on Amazon S3 and are distributed by CloudFront and protected by an origin access identity (OAI).
* Use DynamoDB triggers to generate the URL
* Use AWS Lambda to generate the URL
* Generate an S3 pre-signed URL
* Use API Gateway to generate the URL
* Generate a CloudFront signed URL

### Question 55:
A small rental company had 5 employees, all working under the same AWS cloud account. These employees deployed their applications built for various functions- including billing, operations, finance, etc. Each of these employees has been operating in their own VPC. Now, there is a need to connect these VPCs so that the applications can communicate with each other.
* Use VPC Peering
* Use a NAT Gateway
* Use a Direct Connect
* Use an Internet Gateway

### Question 56:
You are using AWS Lambda to implement a batch job for a big data analytics workflow. Based on historical trends, a similar job runs for 30 minutes on average. The Lambda function pulls data from Amazon S3, processes it, and then writes the results back to S3. When you deployed your AWS Lambda function, you noticed an issue where the Lambda function abruptly failed after 15 minutes of execution.
* The AWS Lambda function is missing IAM permissions
* The AWS Lambda function is timing out
* The AWS Lambda function is running out of memory
* The AWS Lambda function chosen runtime is wrong

### Question 57:
Your company is building a music sharing platform on which users can upload their songs. As a solutions architect for the platform, you have designed an architecture that will leverage a Network Load Balancer linked to an Auto Scaling Group across multiple availability zones. The songs live on an FTP that your EC2 instances can easily access. You are currently running with 4 EC2 instances in your ASG, but when a very popular song is released, your Auto Scaling Group scales to 100 instances and you start to incur high network and compute fees.
* Move the songs to S3
* Leverage AWS Storage Gateway
* Use a CloudFront distribution
* Move the songs to Glacier

### Question 58:
A web hosting company has deployed their application behind a Network Load Balancer (NLB) and an Auto Scaling Group (ASG). The system administrator has now released a new cost-optimized AMI that should be used to launch instances for the Auto Scaling Group, going ahead.
* Launch a script on the EC2 instance to query the metadata service at http://169.254.169.254/meta-data/ami-update
* Create a new launch configuration with the new AMI ID
* Swap the underlying root EBS volumes for your instances
* Update the current launch configuration with the new AMI ID

### Question 59:
You have developed a new REST API leveraging the API Gateway, AWS Lambda and Aurora database services. Most of the workload on the website is read-heavy. The data rarely changes and it is acceptable to serve users outdated data for about 24 hours. Recently, the website has been experiencing high load and the costs incurred on the Aurora database have been very high.
* Enable API Gateway Caching
* Switch to using an Application Load Balancer
* Add Aurora Read Replicas
* Enable AWS Lambda In Memory Caching

### Question 60:
For security purposes, a team has decided to put their instances in a private subnet. They plan to deploy a VPC endpoint to access these services. The members of the team would like to know about the only two AWS services that require a Gateway Endpoint instead of an Interface Endpoint.
* Amazon Kinesis
* Amazon S3
* Amazon Simple Queue Service (SQS)
* DynamoDB
* Amazon Simple Notification Service (SNS)

### Question 61:
What does this CloudFormation snippet do? (Select three)
* It allows any IP to pass through on the HTTP port
* It only allows the IP 0.0.0.0 to reach HTTP
* It configures an NACL's inbound rules
* It lets traffic flow from one IP on port 22
* It configures a security group's outbound rules
* It prevents traffic from reaching on HTTP unless from the IP 192.168.1.1
* It configures a security group's inbound rules

### Question 62:
A digital advertising and marketing firm, segments users and customers based on the collection and analysis of non-personally identifiable data from browsing sessions. This requires applying data mining methods across historical clickstreams to identify effective segmentation and categorization algorithms and techniques. The engineering team at the firm wants to create a daily big data analysis job leveraging Spark for analyzing online/offline sales and customer loyalty data to create customized reports on a client-by-client basis. The big data analysis job needs to read the data from Amazon S3 and output it back to S3. Finally, the results need to be sent back to the firm's clients.
* Amazon Redshift
* Amazon EMR
* AWS Glue
* Amazon Athena

### Question 63:
One of the fastest-growing rideshare companies in the United States uses AWS Cloud for its IT infrastructure. The rideshare service is available in more than 200 cities facilitating millions of rides per month. The company uses AWS to move faster and manage its exponential growth, leveraging AWS products to support more than 100 microservices that enhance every element of its customers’ experience. The company wants to improve the ride-tracking system that stores GPS coordinates for all rides. The engineering team at the company is looking for a NoSQL database that has single-digit millisecond latency, can scale horizontally, and is serverless, so that they can perform high-frequency lookups reliably.
* Amazon DynamoDB
* Amazon ElastiCache
* Amazon Relational Database Service (Amazon RDS)
* Amazon Neptune

### Question 64:
A leading global consumer robot company, designs and builds robots that empower people to do more both inside and outside the home. The company’s engineers are building an ecosystem of robots to enable the idea of smart homes. The company is planning on distributing an additional sensor to install at people's homes, to measure and monitor the robotic movement. In order to provide adjustment commands, the sensors must insert the data in a database, from which a stream of changes will be analyzed and acted upon. The company would like this database to be horizontally scalable and highly available. The company would also like to have Auto Scaling capabilities and also able to handle any changes in data attributes over time, in case they update their devices.
* Amazon Redshift
* Amazon Relational Database Service (Amazon RDS)
* Amazon DynamoDB
* Amazon Aurora

### Question 65:
A company runs a popular photo-sharing website on the AWS Cloud. As a Solutions Architect, you've designed the architecture of the website to follow a serverless pattern on the AWS Cloud using API Gateway and AWS Lambda. The backend is leveraging an RDS PostgreSQL database. The website is experiencing high read traffic and the Lambda functions are putting an increased read load on the RDS database.
* Use Amazon RDS Multi-AZ feature
* Use Amazon RDS Read Replicas
* Use Amazon DynamoDB
* Use Amazon ElastiCache



# Exam 5

### Question 1:
A large retail company uses separate VPCs with different configurations for each of their lines of business. As part of the specific security requirement, an administrator had created a private hosted zone and associated it with the required virtual private cloud (VPC). However, the domain names remain unresolved thereby resulting in errors.
* You might have private and public hosted zones that have overlapping namespaces
* DNS hostnames and DNS resolution are required settings for private hosted zones
* Name server (NS) record and Start Of Authority (SOA) records are created with wrong configurations
* This error may happen when there is a private hosted zone and a Resolver rule that routes traffic to your network for the same domain name, resulting in ambiguity over the route to be taken

### Question 2:
You create an Auto Scaling group to work with an Application Load Balancer. The scaling group is configured with a minimum size value of 10, a maximum value of 30, and the desired capacity value of 20. One of the 20 EC2 instances has been reported as unhealthy.
* The ASG will format the root EBS drive on the EC2 instance and run the User Data again
* The ASG will terminate the EC2 Instance
* The ASG will detach the EC2 instance from the group, and leave it running
* The ASG will keep the instance running and re-start the application

### Question 3:
A health-care solutions company wants to run their applications on single-tenant hardware to meet regulatory guidelines.
* Dedicated Hosts
* Dedicated Instances
* On-Demand Instances
* Spot Instances

### Question 4:
A media company runs a photo-sharing web application that is currently accessed across three different countries. The application is deployed on several Amazon EC2 instances running behind an Application Load Balancer. With new government regulations, the company has been asked to block access from two countries and allow access only from the home country of the company.
* Configure the security group for the EC2 instances
* Use Geo Restriction feature of Amazon CloudFront in a VPC
* Configure the security group on the Application Load Balancer
* Configure AWS WAF on the Application Load Balancer in a VPC

### Question 5:
A media company has set up its technology infrastructure using AWS services such as Amazon EC2 instances, Lambda functions, Amazon S3 storage service and Amazon ElastiCache Redis to enhance the performance of its RDS database layer. The company has hired you as a Solutions Architect to implement a robust disaster recovery strategy for its caching layer so that it guarantees minimal downtime and data loss while ensuring top application performance.
* Schedule Manual backups using Redis append-only file (AOF)
* Add read-replicas across multiple availability zones to reduce the risk of potential data loss because of failure
* Opt for Multi-AZ configuration with automatic failover functionality to help mitigate failure
* Schedule daily automatic backups at a time when you expect low resource utilization for your cluster

### Question 6:
An automobile company is running its flagship application on a fleet of EC2 instances behind an Auto Scaling Group (ASG). The ASG has been configured more than a year ago. A young developer has just joined the development team and wants to understand the best practices to manage and configure an ASG.
* Data is not automatically copied from existing instances to a new dynamically created instance
* EC2 Auto Scaling groups can span Availability Zones, but not AWS regions
* If you configure the ASG to a certain base capacity, you cannot use a combined purchasing model to fulfill the instance requirements. You will need to choose either On-Demand instances or Reserved Instances only
* If you have an EC2 Auto Scaling group (ASG) with running instances and you choose to delete the ASG, the instances will be terminated and the ASG will be deleted
* You can only specify one launch configuration for an EC2 Auto Scaling group at a time. But, you can modify a launch configuration after you've created it
* Amazon EC2 Auto Scaling can automatically add a volume when the existing one is approaching capacity. This, however, is a configuration parameter and needs to be set explicitly

### Question 7:
A company has its application servers in the public subnet that connect to the RDS instances in the private subnet. For regular maintenance, the RDS instances need patch fixes that need to be downloaded from the internet.
* Configure an Egress-only internet gateway for the resources in the private subnet of the VPC
* Configure the Internet Gateway of the VPC to be accessible to the private subnet resources by changing the route tables
* Configure a NAT Gateway in the public subnet of the VPC
* Configure a NAT instance in the public subnet of the VPC

### Question 8:
An enterprise is planning their journey to AWS Cloud and the CTO has decided to move the secondary workloads such as backups and archives to AWS cloud. The CTO wishes to move the data stored on physical tapes to Cloud, without changing their current backup workflows. The company holds petabytes of data on tapes and needs a cost-optimized solution to move the huge chunks of data and store it cost-effectively.
* AWS DataSync makes it simple and fast to move large amounts of data online between on-premises storage and AWS Cloud. Data moved to Cloud can then be stored cost-effectively in Amazon S3 archiving storage classes
* Use AWS Direct Connect, a cloud service solution that makes it easy to establish a dedicated network connection from on-premises to AWS to transfer data. Once this is done, Amazon S3 can be used to store data at lesser costs
* Use AWS VPN connection between the on-premises datacenter and your Amazon VPC. Once this is established, you can use Amazon Elastic File System (Amazon EFS) to get a scalable, fully managed elastic NFS file system for use with AWS Cloud services and on-premises resources
* Tape Gateway can be used to move on-premises tape data onto AWS Cloud. From here, Amazon S3 archiving storage classes can be used to store data cost-effectively for years

### Question 9:
A social media company manages its flagship application on an EC2 server fleet running behind an Application Load Balancer and the traffic is fronted by a CloudFront distribution. The engineering team wants to decouple the user authentication process for the application so that the application servers can just focus on the business logic.
* Use Cognito Authentication via Cognito Identity Pools for your Application Load Balancer
* Use Cognito Authentication via Cognito User Pools for your Application Load Balancer
* Use Cognito Authentication via Cognito User Pools for your CloudFront distribution
* Use Cognito Authentication via Cognito Identity Pools for your CloudFront distribution

### Question 10:
A financial services company is looking at moving their on-premises infrastructure to AWS Cloud and leverage the serverless architecture. As part of this process, their engineering team has been studying various best practices for developing a serverless solution. They intend to use AWS Lambda extensively and want to focus on the key points to consider when using Lambda as a backbone for this architecture.
* By default, Lambda functions always operate from an AWS-owned VPC and hence have access to any public internet address or public AWS APIs. Once a Lambda function is VPC-enabled, it will need a route through a NAT gateway in a public subnet to access public resources
* Since Lambda functions can scale extremely quickly, it's a good idea to deploy a CloudWatch Alarm that notifies your team when function metrics such as ConcurrentExecutions or Invocations exceeds the expected threshold
* The bigger your deployment package, the slower your Lambda function will cold-start. Hence, AWS suggests packaging dependencies as a separate package from the actual Lambda package
* Lambda allocates compute power in proportion to the memory you allocate to your function. AWS, thus recommends to over provision your function time out settings for the proper performance of Lambda functions
* If you intend to reuse code in more than one Lambda function, you should consider creating a Lambda Layer for the reusable code
* Serverless architecture and containers complement each other and you should leverage Docker containers within the Lambda functions

### Question 11:
An e-commerce company has created a hub-and-spoke network with AWS Transit Gateway. VPCs have been provisioned into multiple AWS accounts to facilitate network isolation and delegate network administration. The company is looking for a cost-effective, easy, and secure way of maintaining this distributed architecture.
* Use VPCs connected with AWS Direct Connect
* Use Centralized VPC Endpoints for connecting with multiple VPCs, also known as shared services VPC
* Use Transit VPC to reduce cost and share the resources across VPCs
* Use Fully meshed VPC Peers

### Question 12:
A retail company has its business-critical data stored on the AWS Cloud in different forms such as files on a filesystem, object storage in S3, block storage and in relational databases. The company has hired you as a Solutions Architect to make this data available in alternate regions as part of the disaster recovery strategy.
* Amazon Elastic File System (Amazon EFS), used to store files, is scoped to individual AZ. You need to employ EFS File Sync to quickly replicate files across multiple AZs
* Amazon EBS volumes are regionally scoped. To ensure high availability, you should replicate your EBS Snapshots to another region
* For OS images, when using Amazon EC2 and Amazon EBS, the appropriate Amazon Machine Images (AMIs) are automatically copied and available in the alternate Region as specified by the user
* For data stored in databases, Amazon RDS Read Replicas provide enhanced performance and durability for database instances
* For application data, you must initiate and ensure the EBS Snapshots of your data volumes are configured for cross-region copy
* For static application data stored in Amazon S3, you need to enable Cross-Region Replication (CRR)

### Question 13:
The application maintenance team at a company has noticed that the production application is very slow when the business reports are run on the RDS database. These reports fetch a large amount of data and have complex queries with multiple joins, spanning across multiple business-critical core tables. CPU, memory, and storage metrics are around 50% of the total capacity.
* Create a read replica and connect the report generation tool/application to it
* Configure the RDS instance to be Multi-AZ DB instance, and connect the report generation tool to the DB instance in a different AZ
* Increase the size of RDS instance
* Migrate from General Purpose SSD to magnetic storage to enhance IOPS

### Question 14:
A health-care company runs its extremely critical web service on Amazon EC2 instances behind an Auto Scaling Group (ASG). The company provides ambulances for critical patients and needs the application to be reliable without issues. The workload of the company can be managed on 2 EC2 instances and can peak up to 6 instances when workload builds up.
* The ASG should be configured with the minimum capacity set to 4, with 2 instances each in two different AWS Regions. The maximum capacity of the ASG should be set to 6
* The ASG should be configured with the minimum capacity set to 2, with 1 instance each in two different Availability Zones. The maximum capacity of the ASG should be set to 6
* The ASG should be configured with the minimum capacity set to 4, with 2 instances each in two different Availability Zones. The maximum capacity of the ASG should be set to 6
* The ASG should be configured with the minimum capacity set to 2 and the maximum capacity set to 6 in a single Availability Zone

### Question 15:
A profitable small business has been running their IT systems using the on-premises infrastructure. With growing demand, the business is finding it difficult to manage the IT infrastructure, which is not their core competency. The business plans to move to AWS Cloud, in light of their plans of extending their operations to other countries.
* Host both the static and dynamic content of the web application on Amazon S3 and use Amazon CloudFront for distribution across diverse regions/countries
* Host both the static and dynamic content of the web application on Amazon EC2 with RDS as database. Amazon CloudFront should be configured to distribute the content across geographically disperse regions
* Host the static content on Amazon S3 and use Lambda with DynamoDB for the serverless web application that handles dynamic content. Amazon CloudFront will sit in front of Lambda for distribution across diverse regions
* Host the static content on Amazon S3 and use Amazon EC2 with RDS for generating the dynamic content. Amazon CloudFront can be configured in front of EC2 instance, to make global distribution easy

### Question 16:
A highly successful gaming company has consistently used the standard architecture of configuring an Application Load Balancer (ALB) in front of Amazon EC2 instances for different services and microservices. As they have expanded to different countries and additional features have been added, the architecture has become complex with too many ALBs in multiple regions. Security updates, firewall configurations, and traffic routing logic have become complex with too many IP addresses and configurations.
* Launch AWS Global Accelerator and create endpoints for all the Regions. Register the ALBs of each Region to the corresponding endpoints
* Set up a Network Load Balancer (NLB) with Elastic IPs. To this NLB, register the private IPs of all the ALBs as targets
* Assign an Elastic IP to an Auto Scaling Group (ASG), and set up multiple Amazon EC2 to run behind the ASGs, for each of the regions
* Configure Elastic IPs for each of the ALBs in each region

### Question 17:
While troubleshooting, a cloud architect realized that the Amazon EC2 instance is unable to connect to the Internet using the Internet Gateway.
* The network ACLs associated with the subnet must have rules to allow inbound and outbound traffic
* The instance's subnet is associated with multiple route tables with conflicting configurations
* The route table in the instance’s subnet should have a route to an Internet Gateway
* The instance's subnet is not associated with any route table
* The subnet has been configured to be Public and has no access to the internet

### Question 18:
A media company is evaluating the possibility of moving its IT infrastructure to the AWS Cloud. The company needs at least 10 TB of storage with the maximum possible I/O performance for processing certain files which are mostly large videos. The company also needs close to 450 TB of very durable storage for storing media content and almost double of it, i.e. 900 TB for archival of legacy data.
* Amazon EC2 instance store for maximum performance, AWS Storage Gateway for on-premises durable data access and Amazon S3 Glacier Deep Archive for archival storage
* Amazon S3 standard storage for maximum performance, Amazon S3 Intelligent-Tiering for intelligent, durable storage, and Amazon S3 Glacier Deep Archive for archival storage
* Amazon EC2 instance store for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage
* Amazon EBS for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage

### Question 19:
A company's cloud architect has set up a solution that uses Route 53 to configure the DNS records for the primary website with the domain pointing to the Application Load Balancer (ALB). The company wants a solution where users will be directed to a static error page, configured as a backup, in case of unavailability of the primary website.
* Use Route 53 Weighted routing to give minimum weight to Amazon S3 bucket that holds the error page to be displayed. In case of primary failure, the requests get routed to the error page
* Set up a Route 53 active-active failover configuration. If Route 53 health check determines the ALB endpoint as unhealthy, the traffic will be diverted to a static error page, hosted on Amazon S3 bucket
* Set up a Route 53 active-passive failover configuration. If Route 53 health check determines the ALB endpoint as unhealthy, the traffic will be diverted to a static error page, hosted on Amazon S3 bucket
* Use Route 53 Latency-based routing. Create a latency record to point to the Amazon S3 bucket that holds the error page to be displayed

### Question 20:
A financial services firm runs its technology operations on a fleet of Amazon EC2 instances. The firm needs a certain software to be available on the instances to support their daily workflows. The engineering team has been told to use the user data feature of EC2 instances to ensure new instances are ready for operations.
* By default, user data is executed every time an EC2 instance is re-started
* When an instance is running, you can update user data by using root user credentials
* By default, scripts entered as user data are executed with root user privileges
* By default, scripts entered as user data do not have root user privileges for executing
* By default, user data runs only during the boot cycle when you first launch an instance

### Question 21:
You are working as an Engineering Manager at a company and you manage several development teams and monitor their access across multiple accounts. To get the teams up and running quickly, you had initially created multiple roles with broad permissions that are based on job function in the development accounts. Now, the developers are ready to deploy workloads to production accounts and you only want to grant them minimum possible permissions that the developers would actually need.
* Use Access Advisor to know the action last accessed information for the last few months and create IAM Groups with the permissions gained from these insights
* Use Access Advisor to determine the permissions the developers have used in the last few months and only give those permissions (with new IAM roles) while reverting the rest
* Create service accounts for each of the teams and restrict the associated policy to only the permissions needed for the particular functionality
* Create IAM Roles with limited permissions for each of the teams. Any missing permissions can be added to these roles if developers face issues in accessing services they need

### Question 22:
An online gaming application has been built on AWS Cloud. Of late, a large chunk of traffic is coming from users who download the historic leaderboard reports and their game tactics for various games. The current infrastructure and design are unable to cope up with the traffic numbers and application freezes on most of the pages.
* Use Amazon CloudFront with S3 as the storage solution
* Use Amazon CloudFront with DynamoDB for greater speed and low latency access
* Use AWS Lambda with ElastiCache and Amazon RDS for serving content at high speed and low latency
* Configure AWS Lambda with an RDS database solution, to provide a serverless architecture

### Question 23:
A popular chatting application has millions of users. The engineering team responsible for the application has used ElastiCache to bolster the performance even as the user base has increased by two folds over the past six months. After due diligence, the team has chosen TTL (Time to Live) caching strategy for their requirements which has worked reasonably well so far. Recently, the database administrator has found sudden spikes in queries to the database that are fetching the same data. This effect may cripple the database as more users sign-up for the application thereby causing a bad user experience.
* TTL caching strategy is the right fit for this use case. Opt for Write-Through caching strategy. The write-through strategy adds or updates data in the cache whenever data is written to the database, making sure that the database never gets too many read requests
* Delete the existing cache keys and opt for Lazy loading cache technique for lesser hits on database
* ElastiCache seems to be preconfigured with an eviction policy that is forcing data out of the memory. Disable the eviction policy to remedy the fault
* When different application processes simultaneously request a cache key, get a cache miss, and then each hits the same database query for data, it results in the database getting swamped with identical queries. The solution is to prewarm the cache

### Question 24:
An online gaming company has global users accessing its flagship application in different AWS Regions. Few weeks ago, an Elastic Load Balancer (ELB) had malfunctioned in a region taking down all the traffic with it. The manual intervention cost the company significant time and resulted in a huge revenue loss. Additionally, the users have also complained of poor performance when accessing the application over the internet.
* Create S3 buckets in different AWS Regions and configure CloudFront to pick the nearest edge location to the user
* Set up AWS Direct Connect as the backbone for each of the AWS Regions where the application is deployed
* Set up an Amazon Route 53 geoproximity routing policy to route traffic
* Set up AWS Global Accelerator and add endpoints to cater to users in different geographic locations

### Question 25:
A startup has recently moved their monolithic web application to AWS Cloud. The application runs on a single EC2 instance. Currently, the user base is small and the startup does not want to spend effort on elaborate disaster recovery strategies or Auto Scaling Group. The application can afford a maximum downtime of 10 minutes.
* Configure an Amazon CloudWatch alarm that triggers the recovery of the EC2 instance, in case the instance fails. The instance, however, should only be configured with an EBS volume
* Configure AWS Trusted Advisor to monitor the health check of EC2 instance and provide a remedial action in case an unhealthy flag is detected
* Configure Amazon CloudWatch events that can trigger the recovery of the EC2 instance, in case the instance or the application fails
* Configure an Amazon CloudWatch alarm that triggers the recovery of the EC2 instance, in case the instance fails. The instance can be configured with EBS volume or with instance store volumes

### Question 26:
A health care startup has built their application on REST-based interface that receives near real-time data from the small devices connected to patients. Once the patient's health metrics flow in, the downstream applications process the data and generate a report of the diagnosis that is sent back to the doctor. The process worked well when the velocity of data ingestion was less. With the startup gaining traction and being used by more doctors, the system has become slow and sometimes even unresponsive as it does not have a retry mechanism. The startup is looking at a scalable solution that has minimal implementation overhead.
* Use Amazon API Gateway with the existing REST-based interface to create a high performing architecture
* Use Amazon Kinesis Data Streams to ingest the data. Process this data using AWS Lambda function or run analytics using Kinesis Data Analytics
* Use Amazon Simple Notification Service (Amazon SNS) for data ingestion and configure Lambda to trigger logic for downstream processing
* Use Amazon Simple Queue Service (SQS) for data ingestion and configure Lambda to trigger logic for downstream processing

### Question 27:
The engineering team at a logistics company is working on a shipments application deployed on a fleet of Amazon EC2 instances behind an Auto Scaling Group (ASG). While configuring new changes for an upcoming release, a team member has noticed that the ASG is not terminating an unhealthy instance.
* The instance maybe in Impaired status
* The health check grace period for the instance has not expired
* The EC2 instance could be a spot instance type, which cannot be terminated by ASG
* A user might have updated the configuration of ASG and increased the minimum number of instances forcing ASG to keep all instances alive
* A custom health check might have failed. ASG does not terminate instances that are set unhealthy by custom checks
* The instance has failed the ELB health check status

### Question 28:
The health check for a system monitors 100,000 servers on a distributed network. If a server is found to be unhealthy, an SNS notification is sent, along with a priority message on registered phone numbers. A major event had stalled 10,000 of these servers and the company realized that their design couldn't stand the load of firing thousands of notifications and updates simultaneously. They also understood that, even if half the servers go unhealthy, it will choke the network and the company will not be able to update the clients on-time about the status of their servers.
* The health check system should send the full snapshot of the current state of all the servers each time, denoting them as bits of data to reduce workload and keep spikes at bay
* Use AWS Lambda with SNS to speed up the processing of records
* The SNS service is not meant for heavy workloads of this order. Opting for SQS would have kept the system stable during server fails
* The health check system should send the current state of only the failed servers, denoting them as bits of data to reduce workload

### Question 29:
An IT company is working on a project that uses two separate AWS accounts for accessing different AWS services. The team has just configured an Amazon S3 bucket in the first AWS account for writing data from the Amazon Redshift cluster present in the second AWS account. The developer has noticed that the files created in the S3 bucket using the UNLOAD command from the Redshift cluster are not accessible to the S3 bucket owner.
* When objects are uploaded to S3 bucket from a different AWS account, the S3 bucket owner will get implicit permissions to access these objects. It is an upload error that can be fixed by providing manual access from AWS console
* When two different AWS accounts are accessing an S3 bucket, both the accounts need to share the bucket policies, explicitly defining the actions possible for each account. An erroneous policy can lead to such permission failures
* By default, an S3 object is owned by the AWS account that uploaded it. So the S3 bucket owner will not implicitly have access to the objects written by the Redshift cluster
* The owner of an S3 bucket has implicit access to all objects in his bucket. Permissions are set on objects after they are completely copied to the target location. Since the owner is unable to access the uploaded files, the write operation may be still in progress

### Question 30:
You are working as a Solutions Architect with a gaming company that has deployed an application that allows its customers to play games online. The application connects to an Amazon Aurora database, and the entire stack is currently deployed in the United States. The company has plans to expand to Europe and Asia for its operations. It needs the games table to be accessible globally but needs the users and games_played table to be regional only.
* Use an Amazon Aurora Global Database for the games table and use Amazon Aurora for the users and games_played tables
* Use an Amazon Aurora Global Database for the games table and use DynamoDB for the users and games_played tables
* Use a DynamoDB Global Table for the games table and use Amazon Aurora for the users and games_played tables
* Use a DynamoDB Global Table for the games table and use DynamoDB for the users and games_played tables

### Question 31:
A financial services company uses Amazon GuardDuty for analyzing their AWS account metadata to adhere to the compliance requirements mandated by the regulatory authorities. However, the company has now decided to stop using GuardDuty service. All the existing findings have to be deleted and cannot persist anywhere on AWS Cloud.
* Suspend the service in the general settings
* Disable the service in the general settings
* Raise a service request with Amazon to completely delete the data from all their backups
* De-register the service under services tab

### Question 32:
As an AWS Certified Solutions Architect Associate, you have been hired to work with the engineering team at a company to create a REST API using the serverless architecture.
* Fargate with Lambda at the front
* Route 53 with EC2 as backend
* Public-facing Application Load Balancer with ECS on Amazon EC2
* API Gateway exposing Lambda Functionality

### Question 33:
A legacy application is built using a tightly-coupled monolithic architecture. With an increased number of users, the company is unable to provide a good user experience. Performance, scalability, and security have become an issue, since a small change propagates to all the connected components, making it difficult to develop, test, and maintain the application features. The company has decided to decouple the architecture and adopt AWS microservices architecture. Some of the microservices handle need to handle fast running processes whereas other microservices need to handle slower processes.
* Upstream microservices should send their output to the configured Amazon SQS queue. The downstream slower microservices can pick messages from the respective queues for processing
* Upstream microservices can stream their output to Amazon Kinesis Data Streams. All the consumer microservices can fetch the data from these streams and work on them at their own pace
* Upstream microservices should publish their output to the configured Amazon SNS topic. The downstream, slower microservices will get the notifications for working on them to completion, at their own pace
* The upstream microservices can send their output to Amazon EventBridge, which can forward or distribute the work across different downstream microservices

### Question 34:
A Pharmaceuticals company has decided to move most of their IT infrastructure to AWS Cloud. Some of the applications, however, will remain on their on-premises data center to meet certain regulatory guidelines. The company is looking for a scalable solution to connect the on-premises applications to the ones on AWS Cloud.
* Use AWS Transit Gateway to connect the Amazon VPCs to the on-premises networks
* Use Transit VPC Solution to connect the Amazon VPCs to the on-premises networks
* Fully meshed VPC peering can be used to connect the Amazon VPCs to the on-premises networks
* Partially meshed VPC peering can be used to connect the Amazon VPCs to the on-premises networks

### Question 35:
A telecommunications company is looking at moving its real-time traffic analytics infrastructure to AWS Cloud. The company owns thousands of hardware devices like switches, routers, cables, and so on. The status of all these devices has to be fed into an analytics system for real-time processing. If a malfunction is detected, communication has to be initiated to the responsible team, to fix the hardware. Also, another application needs to read this same incoming data in parallel and analyze all the connecting lines that may go down because of the hardware failure.
* Amazon Kinesis Data Streams
* Amazon Simple Notification Service (SNS)
* Amazon Simple Queue Service (SQS) with Amazon Simple Notification Service (SNS)
* Amazon Simple Queue Service (SQS) with Amazon Simple Email Service (Amazon SES)

### Question 36:
The engineering team at a retail company has developed a REST API which is deployed in an Auto Scaling group behind an Application Load Balancer. The API stores the data payload in DynamoDB and the static content is served through S3. On analyzing the usage trends, it is found that 90% of the read requests are shared across all users.
* Enable DynamoDB Accelerator (DAX) for DynamoDB and CloudFront for S3
* Enable ElastiCache Redis for DynamoDB and ElastiCache Memcached for S3
* Enable ElastiCache Redis for DynamoDB and CloudFront for S3
* Enable DAX for DynamoDB and ElastiCache Memcached for S3

### Question 37:
A data analytics company uses custom data-integration services to produce data and log files in S3 buckets. As part of the process re-engineering, the company now wants to stream the existing data files and ongoing changes from Amazon S3 to Amazon Kinesis Data Streams. The timelines are quite stringent and the company is looking at implementing this functionality as soon as possible.
* Amazon S3 bucket actions can be directly configured to write data into Amazon Simple Notification Service (SNS). SNS can then be used to send the updates to Amazon Kinesis Data Streams
* Configure CloudWatch events for the bucket actions on Amazon S3. An AWS Lambda function can then be triggered from the CloudWatch event that will send the necessary data to Amazon Kinesis Data Streams
* Leverage AWS Database Migration Service (AWS DMS) as a bridge between Amazon S3 and Amazon Kinesis Data Streams
* Leverage S3 event notification to trigger a Lambda function for the file create event. The Lambda function will then send the necessary data to Amazon Kinesis Data Streams

### Question 38:
A media company uses Amazon S3 buckets for storing their business-critical files. Initially, the development team used to provide bucket access to specific users within the same account. With changing business requirements, cross-account S3 access requirements are also growing. The company is looking for a granular solution that can offer user level as well as account-level access permissions for the data stored in S3 buckets.
* Use Security Groups
* Use Amazon S3 Bucket Policies
* Use Identity and Access Management (IAM) policies
* Use Access Control Lists (ACLs)

### Question 39:
The lead engineer at a social media company has created an Elastic Load Balancer that has marked all the EC2 instances in the target group as unhealthy. Surprisingly, when he enters the IP address of the EC2 instances in the web browser, he can access the website.
* You need to attach Elastic IP to the EC2 instances
* Your web-app has a runtime that is not supported by the Application Load Balancer
* The security group of the EC2 instance does not allow for traffic from the security group of the Application Load Balancer
* The route for the health check is misconfigured
* The EBS volumes have been improperly mounted

### Question 40:
A retail company has built their AWS solution using serverless architecture by leveraging AWS Lambda and Amazon S3. The development team has a requirement to implement AWS Lambda across AWS accounts. The requirement entails using a Lambda function with an IAM role from an AWS account A to access an Amazon S3 bucket in AWS account B.
* Create an AWS Identity and Access Management (IAM) role for the Lambda function that also grants access to the S3 bucket. Set the IAM role as the Lambda function's execution role
* AWS Lambda cannot access resources across AWS accounts. Use Identity federation to work around this limitation of Lambda
* The S3 bucket owner can delegate permissions to users in the other AWS account
* Create an AWS Identity and Access Management (IAM) role for the Lambda function that also grants access to the S3 bucket. Set the IAM role as the Lambda function's execution role. Verify that the bucket policy grants access to the Lambda function's execution role

### Question 41:
You are a cloud architect in Silicon Valley. Many companies in this area have mobile apps that capture and send data to Amazon Kinesis Data Streams. They have been getting a ProvisionedThroughputExceededException exception. You have been contacted to help and upon careful analysis, you are seeing that messages are being sent one by one while being sent at a high rate.
* Decrease the Stream retention duration
* Increase the number of shards
* Batch messages
* Use Exponential Backoff

### Question 42:
A multi-national retail company has multiple business divisions with each division having its own AWS account. The engineering team at the company would like to debug and trace data across these AWS accounts and visualize it in a centralized account.
* X-Ray
* CloudTrail
* CloudWatch Events
* VPC Flow Logs

### Question 43:
A medical devices company extensively uses Amazon S3 buckets for their critical data storage. Hundreds of buckets are used to keep the images' data segregated and faster to access. During the company's monthly meetings, the finance team submitted a report with the high costs incurred on S3 storage. Upon analysis, the IT team realized that the lifecycle policies on the S3 buckets have not been applied most optimally.
* Use S3 Intelligent-Tiering storage class to optimize the S3 storage costs
* Configure Amazon Elastic File System (Amazon EFS) to provide a fast, cost-effective and sharable storage service
* Use S3 Outposts storage class to reduce the costs on S3 storage by storing the data on-premises
* Use S3 One Zone-Infrequent Access, to reduce the costs on S3 storage

### Question 44:
An Internet-of-Things(IoT) technology company has leveraged a distributed architecture to build its AWS Cloud based solution. This distributed system relies on communications networks to interconnect its three different service components - service A, service B and Service C. Service A invokes service B which in turn invokes service C for sending a response back to service A. During the testing phase, it has been noticed that the failure of service C results in the failure of service A too.
* Service B should return a static response, a simple alternative to returning an error when service C fails to respond
* Service B should return an error when service C fails
* Service B should re-compute the response using different means (or service) to replace the failure of service C
* Since service C is critical for the entire architecture, in the event of a failure, service C should have a standby to fall back on

### Question 45:
An IT company is looking at securing their APIs using AWS best practices. APIs are often targeted by attackers because of the operations that they can perform and the valuable data they can provide. The company has hired you as a Solutions Architect to advise the company on the various authentication/authorization mechanisms that AWS offers to authorize an API call within the API Gateway. The company would prefer to implement a solution that offers built-in user management.
* Use Amazon Cognito User Pools
* Use API Gateway Lambda authorizer
* Use Amazon Cognito Identity Pools
* Use AWS_IAM authorization

### Question 46:
A Silicon Valley startup's cloud infrastructure consists of a few Amazon EC2 instances, Amazon RDS instances and Amazon S3 storage. A year into their business operations, the startup is incurring costs that seem too high to support their business requirements.
* Use AWS Cost Explorer Resource Optimization to get a report of EC2 instances that are either idle or have low utilization and use AWS Compute Optimizer to look at instance type recommendations
* Use AWS Trusted Advisor checks on Amazon EC2 Reserved Instances to automatically renew Reserved Instances. Trusted advisor also suggests Amazon RDS idle DB instances
* Use Amazon S3 Storage class analysis to get recommendations for transitions of objects to S3 Glacier storage classes to reduce storage costs. You can also automate moving these objects into lower-cost storage tier using Lifecycle Policies
* Use AWS Compute Optimizer recommendations to help you choose the optimal Amazon EC2 purchasing options and help reserve your instance capacities at reduced costs

### Question 47:
A retail company manages its global application on AWS Cloud and their engineering team runs several deployments as part of phased rollouts. The digital marketing team wants to test its blue-green deployment on its customer base in the next couple of days. Most of the customers use mobile phones which are prone to DNS caching. The company has only two days left for the annual Thanksgiving sale to commence.
* Use Route 53 weighted routing to spread traffic across different deployments
* Use Elastic Load Balancer to distribute traffic across deployments
* Use AWS Global Accelerator to distribute a portion of traffic to a particular deployment
* Use AWS CodeDeploy deployment options to choose the right deployment

### Question 48:
You have just terminated an instance in the us-west-1a availability zone. The attached EBS volume is now available for attachment to other instances. An intern launches a new Linux EC2 instance in the us-west-1b availability zone and is attempting to attach the EBS volume. The intern informs you that it is not possible and needs your help.
* EBS volumes are AZ locked
* EBS volumes are region locked
* The EBS volume is encrypted
* The required IAM permissions are missing

### Question 49:
An e-commerce company is looking for a highly available architecture to migrate their flagship application which is planned to be hosted on a fleet of Amazon EC2 instances. The company is also looking at facilitating content-based routing in its architecture.
* Use an Auto Scaling group for distributing traffic to the EC2 instances spread across different Availability Zones. Configure a Public IP address to mask any failure of an instance
* Use an Application Load Balancer for distributing traffic to the EC2 instances spread across different Availability Zones. Configure Auto Scaling group to mask any failure of an instance
* Use a Network Load Balancer for distributing traffic to the EC2 instances spread across different Availability Zones. Configure a Private IP address to mask any failure of an instance
* Use an Auto Scaling group for distributing traffic to the EC2 instances spread across different Availability Zones. Configure an Elastic IP address to mask any failure of an instance

### Question 50:
A Big Data analytics company wants to set up an AWS cloud architecture that throttles requests in case of sudden traffic spikes. To augment its custom technology stack, the company is looking for AWS services that can be used for buffering or throttling to handle traffic variations.
* Amazon Gateway Endpoints, Amazon SQS and Amazon Kinesis
* Amazon SQS, Amazon SNS and AWS Lambda
* Elastic Load Balancer, Amazon SQS, AWS Lambda
* Amazon API Gateway, Amazon SQS and Amazon Kinesis

### Question 51:
The Development team at an e-commerce company is working on securing their databases.
* RDS Sequel Server
* RDS Maria DB
* RDS PostGreSQL
* RDS Oracle
* RDS MySQL

### Question 52:
A mobile chat application uses DynamoDB as its database service to provide low latency chat updates. A new developer has joined the team and is reviewing the configuration settings for DynamoDB which have been tweaked for certain technical requirements. CloudTrail service has been enabled on all the resources used for the project. Yet, DynamoDB encryption details are nowhere to be found.
* By default, all DynamoDB tables are encrypted under AWS managed CMKs, which do not write to CloudTrail logs
* By default, all DynamoDB tables are encrypted using Data keys, which do not write to CloudTrail logs
* By default, all DynamoDB tables are encrypted under Customer managed CMKs, which do not write to CloudTrail logs
* By default, all DynamoDB tables are encrypted under an AWS owned customer master key (CMK), which do not write to CloudTrail logs

### Question 53:
A CRM company is moving their IT infrastructure to AWS Cloud to take advantage of the scalability, flexibility and cost optimization it offers. The company has a SaaS (Software as a Service) CRM application that feeds updates to a multitude of other in-house applications as well as several third-party SaaS applications. These in-house applications are also being migrated to use AWS services and the company is looking at connecting the SaaS CRM with the in-house as well as third-party SaaS applications.
* Use Amazon Simple Queue Service (SQS), a fully managed message queuing service that enables you to asynchronously decouple and scale microservices, distributed systems, and serverless applications
* Use Amazon Simple Notification Service (SNS), a fully managed messaging service for both system-to-system and app-to-person (A2P) communication. It enables you to communicate between systems through publish/subscribe (pub/sub) patterns that enable asynchronous messaging between decoupled microservice applications or to communicate directly to users via SMS, mobile push and email
* Use Amazon EventBridge, which is a serverless event bus that makes it easy to connect applications and is event-based, works asynchronously to decouple the system architecture
* Use Elastic Load Balancing, that automatically distributes incoming application traffic across multiple targets, such as Amazon EC2 instances, containers, IP addresses, and Lambda functions for effective decoupling of system architecture

### Question 54:
A retail company manages its IT infrastructure on AWS Cloud. A fleet of Amazon EC2 instances sits behind an Auto Scaling Group (ASG) that helps manage the fleet size to meet the demand. After analyzing the application, the team has configured two metrics that control the scale-in and scale-out policy of ASG. One is a target tracking policy that uses a custom metric to add and remove two new instances, based on the number of SQS messages in the queue. The other is a step scaling policy that uses the Amazon CloudWatch CPUUtilization metric to launch one new instance when the existing instance exceeds 90 percent utilization for a specified length of time.
* Amazon EC2 Auto Scaling chooses the minimum capacity from each of the policies that meet the criteria. So, one new instance will be launched by the ASG
* Amazon EC2 Auto Scaling chooses the policy that provides the largest capacity, so policy with the custom metric is triggered, and two new instances will be launched by the ASG
* Amazon EC2 Auto Scaling chooses the sum of the capacity of all the policies that meet the criteria. So, three new instances will be launched by the ASG
* Amazon EC2 Auto Scaling chooses the latest policy after running the algorithm defined during ASG configuration. Based on this output, either of the policies will be chosen for scaling out

### Question 55:
A startup has created a cost-effective backup solution in another AWS Region. The application is running in warm standby mode and has Application Load Balancer (ALB) to support it from the front. The current failover process is manual and requires updating the DNS alias record to point to the secondary ALB in another Region in case of failure of the primary ALB.
* Enable an Amazon Route 53 health check
* Enable an EC2 instance health check
* Configure Trusted Advisor to check on unhealthy instances
* Enable an ALB health check

### Question 56:
An IT company hosts windows based applications on its on-premises data center. The company is looking at moving the business to the AWS Cloud. The cloud solution should offer shared storage space that multiple applications can access without a need for replication. Also, the solution should integrate with the company's self-managed Active Directory domain.
* Use Amazon Elastic File System (Amazon EFS) as a shared storage solution
* Use File Gateway of AWS Storage Gateway to create a hybrid storage solution
* Use Amazon FSx for Windows File Server, for shared storage space
* Use Amazon FSx for Lustre, for effective shared storage and millisecond latencies

### Question 57:
A call center used to hire experienced specialists to analyze the customer service calls attended by their small group of call center representatives. Each call center representative handles about 40-50 calls in a day. Over the years, as the company grew to more than a hundred employees, hiring specialists to analyze calls has not only become cumbersome but also ineffective. The company wants to move to AWS Cloud and is looking at an automated solution that can help them analyze the calls for sentiment and security analysis.
* Use Kinesis Data Streams to read in audio files into Amazon Alexa, which will convert the audio files into text. Kinesis Data Analytics can be used to analyze these files and Amazon Quicksight can be used to visualize and display the output
* Use Kinesis Data Streams to read in audio files as they are generated. Use Amazon provided machine learning (ML) algorithms to initially convert the audio files into text. These text files can be analyzed using various ML algorithms to generate reports for customer sentiment analysis
* Use Amazon Transcribe to convert audio files to text. Use Amazon Quicksight to run analysis on these text files to understand the underlying patterns. Visualize and display them onto user Dashboards for human analysis
* Use Amazon Transcribe to convert audio files to text. Run analysis on these text files using Amazon Athena to understand the underlying customer sentiments

### Question 58:
An IT training company hosted its website on Amazon S3 a couple of years ago. Due to COVID-19 related travel restrictions, the training website has suddenly gained traction. With an almost 300% increase in the requests served per day, the company's AWS costs have sky-rocketed for just the S3 outbound data costs.
* Configure S3 Batch Operations to read data in bulk at one go, to reduce the number of calls made to S3 buckets
* Use Amazon Elastic File System (Amazon EFS), as it provides a shared, scalable, fully managed elastic NFS file system for storing AWS Cloud or on-premises data
* Configure Amazon CloudFront to distribute the data hosted on Amazon S3 cost-effectively
* To reduce S3 cost, the data can be saved on an EBS volume connected to an EC2 instance that can host the application

### Question 59:
A solutions architect is tasked with a requirement to design a low-latency solution for a static, single-page application, accessed by users through a custom domain name. The solution must be serverless, provide in-transit data encryption and needs to be cost-effective.
* Host the application on Amazon EC2 instance with instance store volume for high performance of the application to provide low latency access to users
* Host the application on AWS Fargate and front it with an Elastic Load Balancer for an improved performance
* Configure Amazon S3 to store the static data and use AWS Fargate for hosting the application on serverless architecture
* Amazon S3 can be used to host the static website. While Amazon CloudFront can be used to distribute the content for low latency access

### Question 60:
The engineering team at a retail company uses EC2 instances, API Gateway, Amazon RDS, Elastic Load Balancer and CloudFront services. As per suggestions from a risk advisory group, all the development teams have been advised to ramp up the security of the applications by analyzing the data sources from AWS services that are part of their stack. The CTO at the company also wants the teams to assess the viability of using Amazon GuardDuty.
* ELB logs, DNS logs, CloudTrail events
* CloudFront logs, API Gateway logs, CloudTrail events
* VPC Flow Logs, DNS logs, CloudTrail events
* VPC Flow Logs, API Gateway logs, S3 access logs

### Question 61:
An IT company is working on multiple client projects and some of these projects span across multiple teams that use different AWS accounts. For one such project, two of the teams have a requirement to set up Amazon Simple Email Service (Amazon SES) event notification in one AWS account that needs to send data to an Amazon Kinesis data stream in another AWS account.
* AWS Lambda cannot write across accounts. So, Amazon SNS has to be set up in both the accounts that need to communicate. SNS topic from account one will write data to SNS topic of the second account. In the second account, use Lambda as a subscriber to SNS. When Lambda fires, it will update Amazon Kinesis data streams with the information payload
* From the SES account, configure SES to push data to the Lambda function. Lambda permissions need to be set up for both the accounts (to read from one and write to another). Set up Lambda to send data to Kinesis Data Streams, present in the second AWS account (Here, SES, SNS, and Lambda are present in SES account and Kinesis data streams is present in the second account)
* Configure SES for multiple AWS accounts. This way, SES can directly write to Amazon Kinesis Data streams in the other account
* From the SES account, configure SES to push data to an Amazon SNS topic. Subscribe a Lambda function to this SNS topic. Lambda permissions need to be set up for both the accounts (to read from one and write to another). Set up Lambda to send data to Kinesis Data Streams, present in the second AWS account (Here, SES, SNS, and Lambda are present in SES account and Kinesis data streams is present in the second account)

### Question 62:
A media agency stores its re-creatable artifacts on Amazon S3 buckets. The artifacts are accessed by a large volume of users for the first few days and the frequency of access falls down drastically after a week. Although the artifacts would be accessed occasionally after the first week, but they must continue to be immediately accessible when required. The cost of maintaining all the artifacts on S3 storage is turning out to be very expensive and the agency is looking at reducing costs as much as possible.
* Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days
* Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 7 days
* Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days
* Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 7 days

### Question 63:
A financial services application deployed on the on-premises infrastructure has recently been moved to Amazon EC2 instances. The application data contains critical personal information about all its customers and needs to be protected from all types of cyberattacks. The company is considering using the AWS Web Application Firewall (WAF) to handle this requirement.
* Create a CloudFront distribution for the application on Amazon EC2 instances. Deploy AWS WAF on Amazon CloudFront to provide the necessary safety measures
* Configure an Application Load Balancer (ALB) to balance the workload for all the EC2 instances. Configure CloudFront to distribute from an ALB since WAF cannot be directly configured on ALBs. This configuration not only provides necessary safety but is scalable too
* AWS WAF can be directly configured only on an Application Load Balancer (ALB) or an Amazon API Gateway. One of these two services can then be configured with Amazon EC2 to build the needed secure architecture
* AWS WAF can be directly configured on Amazon EC2 instances for ensuring the security of the underlying application data

### Question 64:
A media startup is looking at hosting their web application on AWS Cloud. The application will be accessed by users from different geographic regions of the world. The main feature of the application requires the upload and download of video files that can reach a maximum size of 10GB. The startup wants the solution to be cost-effective and scalable with the lowest possible latency for a great user experience.
* Use Amazon EC2 with ElastiCache for faster distribution of content, while Amazon S3 can be used as a storage service
* Use Amazon EC2 with Global Accelerator for faster distribution of content, while using Amazon S3 as storage service
* Use Amazon S3 for hosting the web application and use S3 Transfer Acceleration to reduce the latency that geographically dispersed users might face
* Use Amazon S3 for hosting the web application and use Amazon CloudFront for faster distribution of content to geographically dispersed users

### Question 65:
A multi-national company uses different AWS accounts for their distinct business divisions. The communication between these divisions is heavily based on Amazon Simple Notification Service (SNS). For a particular use case, the AWS account for the Human Resources division needs to have access to an Amazon SNS topic that falls under the AWS account of the Finance division.
* Create a group and add all IAM users under it (users from both the accounts). Add the appropriate policy to allow access to the topic
* Add the appropriate policy to all the IAM users of the Human Resources account that need access to the topic
* Add a policy to the topic under the Finance account, where the Resource is defined as the Human Resources account
* Add a policy to the topic under the Finance account, where the Principal is defined as the Human Resources account




# AWS Certified Solutions Architect Associate Practice

# Exam 1

### Question 1:
The database tier of a web application is running on a Windows server on-premises. The database is a Microsoft SQL Server database. The application owner would like to migrate the database to an Amazon RDS instance.

How can the migration be executed with minimal administrative effort and downtime?
* Use the AWS Database Migration Service (DMS) to directly migrate the database to RDS. Use the Schema Conversion Tool (SCT) to enable conversion from Microsoft SQL Server to Amazon RDS
* Use AWS DataSync to migrate the data from the database to Amazon S3. Use AWS Database Migration Service (DMS) to migrate the database to RDS
* Use the AWS Database Migration Service (DMS) to directly migrate the database to RDS
* Use the AWS Server Migration Service (SMS) to migrate the server to Amazon EC2. Use AWS Database Migration Service (DMS) to migrate the database to RDS

### Question 2:
A company uses Docker containers for many application workloads in an on-premise data center. The company is planning to deploy containers to AWS and the chief architect has mandated that the same configuration and administrative tools must be used across all containerized environments. The company also wishes to remain cloud agnostic to safeguard mitigate the impact of future changes in cloud strategy.

How can a Solutions Architect design a managed solution that will align with open-source software?
* Launch the containers on Amazon Elastic Kubernetes Service (EKS) and EKS worker nodes.
* Launch the containers on a fleet of Amazon EC2 instances in a cluster placement group.
* Launch the containers on Amazon Elastic Container Service (ECS) with AWS Fargate instances.
* Launch the containers on Amazon Elastic Container Service (ECS) with Amazon EC2 instance worker nodes.

### Question 3:
A solutions architect is designing the infrastructure to run an application on Amazon EC2 instances. The application requires high availability and must dynamically scale based on demand to be cost efficient.

What should the solutions architect do to meet these requirements?
* Configure an Application Load Balancer in front of an Auto Scaling group to deploy instances to multiple Regions
* Configure an Application Load Balancer in front of an Auto Scaling group to deploy instances to multiple Availability Zones
* Configure an Amazon API Gateway API in front of an Auto Scaling group to deploy instances to multiple Availability Zones
* Configure an Amazon CloudFront distribution in front of an Auto Scaling group to deploy instances to multiple Regions

### Question 4:
A company has two accounts for perform testing and each account has a single VPC: VPC-TEST1 and VPC-TEST2. The operations team require a method of securely copying files between Amazon EC2 instances in these VPCs. The connectivity should not have any single points of failure or bandwidth constraints.

Which solution should a Solutions Architect recommend?
* Attach a virtual private gateway to VPC-TEST1 and VPC-TEST2 and enable routing.
* Attach a Direct Connect gateway to VPC-TEST1 and VPC-TEST2 and enable routing.
* Create a VPC peering connection between VPC-TEST1 and VPC-TEST2.
* Create a VPC gateway endpoint for each EC2 instance and update route tables.

### Question 5:
A team are planning to run analytics jobs on log files each day and require a storage solution. The size and number of logs is unknown and data will persist for 24 hours only.

What is the MOST cost-effective solution?
* Amazon S3 Standard
* Amazon S3 Glacier Deep Archive
* Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA)
* Amazon S3 Intelligent-Tiering

### Question 6:
A company runs an application in an on-premises data center that collects environmental data from production machinery. The data consists of JSON files stored on network attached storage (NAS) and around 5 TB of data is collected each day. The company must upload this data to Amazon S3 where it can be processed by an analytics application. The data must be transferred securely.

Which solution offers the MOST reliable and time-efficient data transfer?
* AWS DataSync over AWS Direct Connect.
* AWS Database Migration Service over the Internet.
* Multiple AWS Snowcone devices.
* Amazon S3 Transfer Acceleration over the Internet.

### Question 7:
An AWS Organization has an OU with multiple member accounts in it. The company needs to restrict the ability to launch only specific Amazon EC2 instance types. How can this policy be applied across the accounts with the least effort?
* Use AWS Resource Access Manager to control which launch types can be used
* Create an SCP with an allow rule that allows launching the specific instance types
* Create an SCP with a deny rule that denies all but the specific instance types
* Create an IAM policy to deny launching all but the specific instance types

### Question 8:
A company's web application is using multiple Amazon EC2 Linux instances and storing data on Amazon EBS volumes. The company is looking for a solution to increase the resiliency of the application in case of a failure.

What should a solutions architect do to meet these requirements?
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Store data on Amazon EFS and mount a target on each instance
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Mount an instance store on each EC2 instance
* Launch the application on EC2 instances in each Availability Zone. Attach EBS volumes to each EC2 instance
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Store data using Amazon S3 One Zone-Infrequent Access (S3 One Zone-A)

### Question 9:
A company hosts an application on Amazon EC2 instances behind Application Load Balancers in several AWS Regions. Distribution rights for the content require that users in different geographies must be served content from specific regions.

Which configuration meets these requirements?
* Create Amazon Route 53 records with a geoproximity routing policy.
* Create Amazon Route 53 records with a geolocation routing policy.
* Configure Amazon CloudFront with multiple origins and AWS WAF.
* Configure Application Load Balancers with multi-Region routing.

### Question 10:
A solutions architect is creating a document submission application for a school. The application will use an Amazon S3 bucket for storage. The solution must prevent accidental deletion of the documents and ensure that all versions of the documents are available. Users must be able to upload and modify the documents.

Which combination of actions should be taken to meet these requirements? (Select TWO.)
* Enable versioning on the bucket
* Set read-only permissions on the bucket
* Enable MFA Delete on the bucket
* Attach an IAM policy to the bucket
* Encrypt the bucket using AWS SSE-S3

### Question 11:
An insurance company has a web application that serves users in the United Kingdom and Australia. The application includes a database tier using a MySQL database hosted in eu-west-2. The web tier runs from eu-west-2 and ap-southeast-2. Amazon Route 53 geoproximity routing is used to direct users to the closest web tier. It has been noted that Australian users receive slow response times to queries.

Which changes should be made to the database tier to improve performance?
* Migrate the database to Amazon RDS for MySQL. Configure Multi-AZ in the Australian Region
* Migrate the database to Amazon DynamoDB. Use DynamoDB global tables to enable replication to additional Regions
* Deploy MySQL instances in each Region. Deploy an Application Load Balancer in front of MySQL to reduce the load on the primary instance
* Migrate the database to an Amazon Aurora global database in MySQL compatibility mode. Configure read replicas in ap-southeast-2

### Question 12:
An application is being created that will use Amazon EC2 instances to generate and store data. Another set of EC2 instances will then analyze and modify the data. Storage requirements will be significant and will continue to grow over time. The application architects require a storage solution.

Which actions would meet these needs?
* Store the data in an Amazon EFS filesystem. Mount the file system on the application instances
* Store the data in AWS Storage Gateway. Setup AWS Direct Connect between the Gateway appliance and the EC2 instances
* Store the data in Amazon S3 Glacier. Update the vault policy to allow access to the application instances
* Store the data in an Amazon EBS volume. Mount the EBS volume on the application instances

### Question 13:
A recent security audit uncovered some poor deployment and configuration practices within your VPC. You need to ensure that applications are deployed in secure configurations.

How can this be achieved in the most operationally efficient manner?
* Remove the ability for staff to deploy applications
* Use CloudFormation with securely configured templates
* Manually check all application configurations before deployment
* Use AWS Inspector to apply secure configurations

### Question 14:
A new application will run across multiple Amazon ECS tasks. Front-end application logic will process data and then pass that data to a back-end ECS task to perform further processing and write the data to a datastore. The Architect would like to reduce-interdependencies so failures do no impact other components.

Which solution should the Architect use?
* Create an Amazon Kinesis Firehose delivery stream and configure the front-end to add data to the stream and the back-end to read data from the stream
* Create an Amazon SQS queue that pushes messages to the back-end. Configure the front-end to add messages to the queue
* Create an Amazon SQS queue and configure the front-end to add messages to the queue and the back-end to poll the queue for messages
* Create an Amazon Kinesis Firehose delivery stream that delivers data to an Amazon S3 bucket, configure the front-end to write data to the stream and the back-end to read data from Amazon S3

### Question 15:
A company's application is running on Amazon EC2 instances in a single Region. In the event of a disaster, a solutions architect needs to ensure that the resources can also be deployed to a second Region.

Which combination of actions should the solutions architect take to accomplish this? (Select TWO.)
* Launch a new EC2 instance from an Amazon Machine Image (AMI) in the second Region
* Detach a volume on an EC2 instance and copy it to an Amazon S3 bucket in the second Region
* Copy an Amazon Elastic Block Store (Amazon EBS) volume from Amazon S3 and launch an EC2 instance in the second Region using that EBS volume
* Copy an Amazon Machine Image (AMI) of an EC2 instance and specify the second Region for the destination
* Launch a new EC2 instance in the second Region and copy a volume from Amazon S3 to the new instance

### Question 16:
A company has deployed a new website on Amazon EC2 instances behind an Application Load Balancer (ALB). Amazon Route 53 is used for the DNS service. The company has asked a Solutions Architect to create a backup website with support contact details that users will be directed to automatically if the primary website is down.

How should the Solutions Architect deploy this solution cost-effectively?
* Configure a static website using Amazon S3 and create a Route 53 failover routing policy.
* Configure a static website using Amazon S3 and create a Route 53 weighted routing policy.
* Create the backup website on EC2 and ALB in another Region and create an AWS Global Accelerator endpoint.
* Deploy the backup website on EC2 and ALB in another Region and use Route 53 health checks for failover routing.

### Question 17:
Storage capacity has become an issue for a company that runs application servers on-premises. The servers are connected to a combination of block storage and NFS storage solutions. The company requires a solution that supports local caching without re-architecting its existing applications.

Which combination of changes can the company make to meet these requirements? (Select TWO.)
* Use the mount command on servers to mount Amazon S3 buckets using NFS.
* Use Amazon Elastic File System (EFS) volumes to replace the block storage.
* Use an AWS Storage Gateway file gateway to replace the NFS storage.
* Use AWS Direct Connect and mount an Amazon FSx for Windows File Server using iSCSI.
* Use an AWS Storage Gateway volume gateway to replace the block storage.

### Question 18:
A company runs a large batch processing job at the end of every quarter. The processing job runs for 5 days and uses 15 Amazon EC2 instances. The processing must run uninterrupted for 5 hours per day. The company is investigating ways to reduce the cost of the batch processing job.

Which pricing model should the company choose?
* Scheduled Reserved Instances
* Spot Block Instances
* Reserved Instances
* On-Demand Instances

### Question 19:
An organization has a large amount of data on Windows (SMB) file shares in their on-premises data center. The organization would like to move data into Amazon S3. They would like to automate the migration of data over their AWS Direct Connect link.

Which AWS service can assist them?
* AWS DataSync
* AWS CloudFormation
* AWS Database Migration Service (DMS)
* AWS Snowball

### Question 20:
An Amazon VPC contains several Amazon EC2 instances. The instances need to make API calls to Amazon DynamoDB. A solutions architect needs to ensure that the API calls do not traverse the internet.

How can this be accomplished? (Select TWO.)
* Create an ENI for the endpoint in each of the subnets of the VPC
* Create a route table entry for the endpoint
* Create a VPC peering connection between the VPC and DynamoDB
* Create a new DynamoDB table that uses the endpoint
* Create a gateway endpoint for DynamoDB

### Question 21:
A company hosts a multiplayer game on AWS. The application uses Amazon EC2 instances in a single Availability Zone and users connect over Layer 4. Solutions Architect has been tasked with making the architecture highly available and also more cost-effective.

How can the solutions architect best meet these requirements? (Select TWO.)
* Increase the number of instances and use smaller EC2 instance types
* Configure an Auto Scaling group to add or remove instances in the Availability Zone automatically
* Configure an Application Load Balancer in front of the EC2 instances
* Configure an Auto Scaling group to add or remove instances in multiple Availability Zones automatically
* Configure a Network Load Balancer in front of the EC2 instances

### Question 22:
A legacy tightly-coupled High Performance Computing (HPC) application will be migrated to AWS. Which network adapter type should be used?
* Elastic Network Adapter (ENA)
* Elastic IP Address
* Elastic Fabric Adapter (EFA)
* Elastic Network Interface (ENI)

### Question 23:
A Microsoft Windows file server farm uses Distributed File System Replication (DFSR) to synchronize data in an on-premises environment. The infrastructure is being migrated to the AWS Cloud.

Which service should the solutions architect use to replace the file server farm?
* Amazon EBS
* Amazon EFS
* Amazon FSx
* AWS Storage Gateway

### Question 24:
A web application allows users to upload photos and add graphical elements to them. The application offers two tiers of service: free and paid. Photos uploaded by paid users should be processed before those submitted using the free tier. The photos are uploaded to an Amazon S3 bucket which uses an event notification to send the job information to Amazon SQS.

How should a Solutions Architect configure the Amazon SQS deployment to meet these requirements?
* Use a separate SQS Standard queue for each tier. Configure Amazon EC2 instances to prioritize polling for the paid queue over the free queue.
* Use one SQS FIFO queue. Assign a higher priority to the paid photos so they are processed first.
* Use a separate SQS FIFO queue for each tier. Set the free queue to use short polling and the paid queue to use long polling.
* Use one SQS standard queue. Use batching for the paid photos and short polling for the free photos.

### Question 25:
A web application runs in public and private subnets. The application architecture consists of a web tier and database tier running on Amazon EC2 instances. Both tiers run in a single Availability Zone (AZ).

Which combination of steps should a solutions architect take to provide high availability for this architecture? (Select TWO.)
* Create an Amazon EC2 Auto Scaling group and Application Load Balancer (ALB) spanning multiple AZs
* Create new public and private subnets in a new AZ. Create a database using Amazon EC2 in one AZ
* Create new public and private subnets in the same AZ for high availability
* Add the existing web application instances to an Auto Scaling group behind an Application Load Balancer (ALB)
* Create new public and private subnets in the same VPC, each in a new AZ. Migrate the database to an Amazon RDS multi-AZ deployment

### Question 26:
A Solutions Architect has deployed an application on several Amazon EC2 instances across three private subnets. The application must be made accessible to internet-based clients with the least amount of administrative effort.

How can the Solutions Architect make the application available on the internet?
* Create an Application Load Balancer and associate three private subnets from the same Availability Zones as the private instances. Add the private instances to the ALB.
* Create an Application Load Balancer and associate three public subnets from the same Availability Zones as the private instances. Add the private instances to the ALB.
* Create a NAT gateway in a public subnet. Add a route to the NAT gateway to the route tables of the three private subnets.
* Create an Amazon Machine Image (AMI) of the instances in the private subnet and launch new instances from the AMI in public subnets. Create an Application Load Balancer and add the public instances to the ALB.

### Question 27:
A retail company with many stores and warehouses is implementing IoT sensors to gather monitoring data from devices in each location. The data will be sent to AWS in real time. A solutions architect must provide a solution for ensuring events are received in order for each device and ensure that data is saved for future processing.

Which solution would be MOST efficient?
* Use an Amazon SQS standard queue for real-time events with one queue for each device. Trigger an AWS Lambda function from the SQS queue to save data to Amazon S3
* Use Amazon Kinesis Data Streams for real-time events with a partition key for each device. Use Amazon Kinesis Data Firehose to save data to Amazon S3
* Use Amazon Kinesis Data Streams for real-time events with a shard for each device. Use Amazon Kinesis Data Firehose to save data to Amazon EBS
* Use an Amazon SQS FIFO queue for real-time events with one queue for each device. Trigger an AWS Lambda function for the SQS queue to save data to Amazon EFS

### Question 28:
A persistent database must be migrated from an on-premises server to an Amazon EC2 instances. The database requires 64,000 IOPS and, if possible, should be stored on a single Amazon EBS volume.

Which solution should a Solutions Architect recommend?
* Use an instance from the I3 I/O optimized family and leverage instance store storage to achieve the IOPS requirement.
* Create a Nitro-based Amazon EC2 instance with an Amazon EBS Provisioned IOPS SSD (i01) volume attached. Provision 64,000 IOPS for the volume.
* Create an Amazon EC2 instance with two Amazon EBS Provisioned IOPS SSD (i01) volumes attached. Provision 32,000 IOPS per volume and create a logical volume using the OS that aggregates the capacity.
* Create an Amazon EC2 instance with four Amazon EBS General Purpose SSD (gp2) volumes attached. Max out the IOPS on each volume and use a RAID 0 stripe set.

### Question 29:
A video production company is planning to move some of its workloads to the AWS Cloud. The company will require around 5 TB of storage for video processing with the maximum possible I/O performance. They also require over 400 TB of extremely durable storage for storing video files and 800 TB of storage for long-term archival.

Which combinations of services should a Solutions Architect use to meet these requirements?
* Amazon EC2 instance store for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage.
* Amazon EBS for maximum performance, Amazon EFS for durable data storage, and Amazon S3 Glacier for archival storage.
* Amazon EC2 instance store for maximum performance, Amazon EFS for durable data storage, and Amazon S3 for archival storage.
* Amazon EBS for maximum performance, Amazon S3 for durable data storage, and Amazon S3 Glacier for archival storage.

### Question 30:
A company is working with a strategic partner that has an application that must be able to send messages to one of the company’s Amazon SQS queues. The partner company has its own AWS account.

How can a Solutions Architect provide least privilege access to the partner?
* Update the permission policy on the SQS queue to grant all permissions to the partner’s AWS account.
* Create a cross-account role with access to all SQS queues and use the partner's AWS account in the trust document for the role.
* Create a user account that and grant the sqs:SendMessage permission for Amazon SQS. Share the credentials with the partner company.
* Update the permission policy on the SQS queue to grant the sqs:SendMessage permission to the partner’s AWS account.

### Question 31:
A company requires that all AWS IAM user accounts have specific complexity requirements and minimum password length.

How should a Solutions Architect accomplish this?
* Set a password policy for each IAM user in the AWS account.
* Create an IAM policy that enforces the requirements and apply it to all users.
* Set a password policy for the entire AWS account.
* Use an AWS Config rule to enforce the requirements when creating user accounts.

### Question 32:
A manufacturing company captures data from machines running at customer sites. Currently, thousands of machines send data every 5 minutes, and this is expected to grow to hundreds of thousands of machines in the near future. The data is logged with the intent to be analyzed in the future as needed.

What is the SIMPLEST method to store this streaming data at scale?
* Create an Amazon Kinesis Firehose delivery stream to store the data in Amazon S3
* Create an Amazon SQS queue, and have the machines write to the queue
* Create an Auto Scaling Group of Amazon EC2 instances behind ELBs to write data into Amazon RDS
* Create an Amazon EC2 instance farm behind an ELB to store the data in Amazon EBS Cold HDD volumes

### Question 33:
An organization want to share regular updates about their charitable work using static webpages. The pages are expected to generate a large amount of views from around the world. The files are stored in an Amazon S3 bucket. A solutions architect has been asked to design an efficient and effective solution.

Which action should the solutions architect take to accomplish this?
* Use the geoproximity feature of Amazon Route 53
* Use cross-Region replication to all Regions
* Use Amazon CloudFront with the S3 bucket as its origin
* Generate presigned URLs for the files

### Question 34:
An application running on Amazon EC2 needs to asynchronously invoke an AWS Lambda function to perform data processing. The services should be decoupled.

Which service can be used to decouple the compute services?
* AWS Step Functions
* Amazon SNS
* AWS Config
* Amazon MQ

### Question 35:
Amazon EC2 instances in a development environment run between 9am and 5pm Monday-Friday. Production instances run 24/7. Which pricing models should be used? (choose 2)
* Use Reserved instances for the development environment
* Use scheduled reserved instances for the development environment
* Use On-Demand instances for the production environment
* Use Spot instances for the development environment
* Use Reserved instances for the production environment

### Question 36:
A company runs an application that uses an Amazon RDS PostgreSQL database. The database is currently not encrypted. A Solutions Architect has been instructed that due to new compliance requirements all existing and new data in the database must be encrypted. The database experiences high volumes of changes and no data can be lost.

How can the Solutions Architect enable encryption for the database without incurring any data loss?
* Update the RDS DB to Multi-AZ mode and enable encryption for the standby replica. Perform a failover to the standby instance and then delete the unencrypted RDS DB instance.
* Create a snapshot of the existing RDS DB instance. Create an encrypted copy of the snapshot. Create a new RDS DB instance from the encrypted snapshot. Configure the application to use the new DB endpoint.
* Create a snapshot of the existing RDS DB instance. Create an encrypted copy of the snapshot. Create a new RDS DB instance from the encrypted snapshot and update the application. Use AWS DMS to synchronize data between the source and destination RDS DBs.
* Create an RDS read replica and specify an encryption key. Promote the encrypted read replica to primary. Update the application to point to the new RDS DB endpoint.

### Question 37:
A developer created an application that uses Amazon EC2 and an Amazon RDS MySQL database instance. The developer stored the database user name and password in a configuration file on the root EBS volume of the EC2 application instance. A Solutions Architect has been asked to design a more secure solution.

What should the Solutions Architect do to achieve this requirement?
* Move the configuration file to an Amazon S3 bucket. Create an IAM role with permission to the bucket and attach it to the EC2 instance.
* Install an Amazon-trusted root certificate on the application instance and use SSL/TLS encrypted connections to the database.
* Attach an additional volume to the EC2 instance with encryption enabled. Move the configuration file to the encrypted volume.
* Create an IAM role with permission to access the database. Attach this IAM role to the EC2 instance.

### Question 38:
A new application is to be published in multiple regions around the world. The Architect needs to ensure only 2 IP addresses need to be whitelisted. The solution should intelligently route traffic for lowest latency and provide fast regional failover.

How can this be achieved?
* Launch EC2 instances into multiple regions behind an ALB and use a Route 53 failover routing policy
* Launch EC2 instances into multiple regions behind an NLB and use AWS Global Accelerator
* Launch EC2 instances into multiple regions behind an NLB with a static IP address
* Launch EC2 instances into multiple regions behind an ALB and use Amazon CloudFront with a pair of static IP addresses

### Question 39:
A company wishes to restrict access to their Amazon DynamoDB table to specific, private source IP addresses from their VPC. What should be done to secure access to the table?
* Create an interface VPC endpoint in the VPC with an Elastic Network Interface (ENI)
* Create an AWS VPN connection to the Amazon DynamoDB endpoint
* Create the Amazon DynamoDB table in the VPC
* Create a gateway VPC endpoint and add an entry to the route table

### Question 40:
A company plans to make an Amazon EC2 Linux instance unavailable outside of business hours to save costs. The instance is backed by an Amazon EBS volume. There is a requirement that the contents of the instance’s memory must be preserved when it is made unavailable.

How can a solutions architect meet these requirements?
* Terminate the instance outside business hours. Recover the instance again when required.
* Hibernate the instance outside business hours. Start the instance again when required.
* Use Auto Scaling to scale down the instance outside of business hours. Scale up the instance when required.
* Stop the instance outside business hours. Start the instance again when required.

### Question 41:
A website runs on Amazon EC2 instances in an Auto Scaling group behind an Application Load Balancer (ALB) which serves as an origin for an Amazon CloudFront distribution. An AWS WAF is being used to protect against SQL injection attacks. A review of security logs revealed an external malicious IP that needs to be blocked from accessing the website.

What should a solutions architect do to protect the application?
* Modify the network ACL for the EC2 instances in the target groups behind the ALB to deny the malicious IP address
* Modify the network ACL on the CloudFront distribution to add a deny rule for the malicious IP address
* Modify the configuration of AWS WAF to add an IP match condition to block the malicious IP address
* Modify the security groups for the EC2 instances in the target groups behind the ALB to deny the malicious IP address.

### Question 42:
A company runs an application in a factory that has a small rack of physical compute resources. The application stores data on a network attached storage (NAS) device using the NFS protocol. The company requires a daily offsite backup of the application data.

Which solution can a Solutions Architect recommend to meet this requirement?
* Use an AWS Storage Gateway file gateway hardware appliance on premises to replicate the data to Amazon S3.
* Create an IPSec VPN to AWS and configure the application to mount the Amazon EFS file system. Run a copy job to backup the data to EFS.
* Use an AWS Storage Gateway volume gateway with cached volumes on premises to replicate the data to Amazon S3.
* Use an AWS Storage Gateway volume gateway with stored volumes on premises to replicate the data to Amazon S3.

### Question 43:
A company runs an application on six web application servers in an Amazon EC2 Auto Scaling group in a single Availability Zone. The application is fronted by an Application Load Balancer (ALB). A Solutions Architect needs to modify the infrastructure to be highly available without making any modifications to the application.

Which architecture should the Solutions Architect choose to enable high availability?
* Create an Auto Scaling group to launch three instances across each of two Regions.
* Create a launch template that can be used to quickly create more instances in another Region.
* Create an Amazon CloudFront distribution with a custom origin across multiple Regions.
* Modify the Auto Scaling group to use two instances across each of three Availability Zones.

### Question 44:
Your company shares some HR videos stored in an Amazon S3 bucket via CloudFront. You need to restrict access to the private content so users coming from specific IP addresses can access the videos and ensure direct access via the Amazon S3 bucket is not possible.

How can this be achieved?
* Configure CloudFront to require users to access the files using a signed URL, create an origin access identity (OAI) and restrict access to the files in the Amazon S3 bucket to the OAI
* Configure CloudFront to require users to access the files using signed cookies, and move the files to an encrypted EBS volume
* Configure CloudFront to require users to access the files using signed cookies, create an origin access identity (OAI) and instruct users to login with the OAI
* Configure CloudFront to require users to access the files using a signed URL, and configure the S3 bucket as a website endpoint

### Question 45:
A company runs a web application that serves weather updates. The application runs on a fleet of Amazon EC2 instances in a Multi-AZ Auto scaling group behind an Application Load Balancer (ALB). The instances store data in an Amazon Aurora database. A solutions architect needs to make the application more resilient to sporadic increases in request rates.

Which architecture should the solutions architect implement? (Select TWO.)
* Add Amazon Aurora Replicas
* Add an AWS Transit Gateway to the Availability Zones
* Add and AWS WAF in front of the ALB
* Add an Amazon CloudFront distribution in front of the ALB
* Add an AWS Global Accelerator endpoint

### Question 46:
A solutions architect is creating a system that will run analytics on financial data for 4 hours a night, 5 days a week. The analysis is expected to run for the same duration and cannot be interrupted once it is started. The system will be required for a minimum of 1 year.

Which type of Amazon EC2 instances should be used to reduce the cost of the system?
* Standard Reserved Instances
* Spot Instances
* Scheduled Reserved Instances
* On-Demand Instances

### Question 47:
A company provides a REST-based interface to an application that allows a partner company to send data in near-real time. The application then processes the data that is received and stores it for later analysis. The application runs on Amazon EC2 instances.

The partner company has received many 503 Service Unavailable Errors when sending data to the application and the compute capacity reaches its limits and is unable to process requests when spikes in data volume occur.

Which design should a Solutions Architect implement to improve scalability?
* Use Amazon Kinesis Data Streams to ingest the data. Process the data using AWS Lambda functions.
* Use Amazon SQS to ingest the data. Configure the EC2 instances to process messages from the SQS queue.
* Use Amazon API Gateway in front of the existing application. Create a usage plan with a quota limit for the partner company.
* Use Amazon SNS to ingest the data and trigger AWS Lambda functions to process the data in near-real time.

### Question 48:
A company offers an online product brochure that is delivered from a static website running on Amazon S3. The company’s customers are mainly in the United States, Canada, and Europe. The company is looking to cost-effectively reduce the latency for users in these regions.

What is the most cost-effective solution to these requirements?
* Create an Amazon CloudFront distribution and set the price class to use all Edge Locations for best performance.
* Create an Amazon CloudFront distribution and set the price class to use only U.S, Canada and Europe.
* Create an Amazon CloudFront distribution that uses origins in U.S, Canada and Europe.
* Create an Amazon CloudFront distribution and use Lambda@Edge to run the website's data processing closer to the users.

### Question 49:
A company has uploaded some highly critical data to an Amazon S3 bucket. Management are concerned about data availability and require that steps are taken to protect the data from accidental deletion. The data should still be accessible, and a user should be able to delete the data intentionally.

Which combination of steps should a solutions architect take to accomplish this? (Select TWO.)
* Create a bucket policy on the S3 bucket.
* Enable default encryption on the S3 bucket.
* Create a lifecycle policy for the objects in the S3 bucket.
* Enable versioning on the S3 bucket.
* Enable MFA Delete on the S3 bucket.

### Question 50:
An application running on an Amazon ECS container instance using the EC2 launch type needs permissions to write data to Amazon DynamoDB.

How can you assign these permissions only to the specific ECS task that is running the application?
* Create an IAM policy with permissions to DynamoDB and assign It to a task using the taskRoleArn parameter
* Create an IAM policy with permissions to DynamoDB and attach it to the container instance
* Use a security group to allow outbound connections to DynamoDB and assign it to the container instance
* Modify the AmazonECSTaskExecutionRolePolicy policy to add permissions for DynamoDB

### Question 51:
A company is investigating methods to reduce the expenses associated with on-premises backup infrastructure. The Solutions Architect wants to reduce costs by eliminating the use of physical backup tapes. It is a requirement that existing backup applications and workflows should continue to function.

What should the Solutions Architect recommend?
* Connect the backup applications to an AWS Storage Gateway using an iSCSI-virtual tape library (VTL).
* Create an Amazon EFS file system and connect the backup applications using the NFS protocol.
* Create an Amazon EFS file system and connect the backup applications using the iSCSI protocol.
* Connect the backup applications to an AWS Storage Gateway using the iSCSI protocol.

### Question 52:
A company runs a dynamic website that is hosted on an on-premises server in the United States. The company is expanding to Europe and is investigating how they can optimize the performance of the website for European users. The website’s backed must remain in the United States. The company requires a solution that can be implemented within a few days.

What should a Solutions Architect recommend?
* Use Amazon CloudFront with Lambda@Edge to direct traffic to an on-premises origin.
* Use Amazon CloudFront with a custom origin pointing to the on-premises servers.
* Migrate the website to Amazon S3. Use cross-Region replication between Regions and a latency-based Route 53 policy.
* Launch an Amazon EC2 instance in an AWS Region in the United States and migrate the website to it.

### Question 53:
An Amazon RDS Read Replica is being deployed in a separate region. The master database is not encrypted but all data in the new region must be encrypted. How can this be achieved?
* Enable encryption on the master DB instance, then create an encrypted cross-region Read Replica
* Enable encryption using Key Management Service (KMS) when creating the cross-region Read Replica
* Encrypt a snapshot from the master DB instance, create an encrypted cross-region Read Replica from the snapshot
* Encrypt a snapshot from the master DB instance, create a new encrypted master DB instance, and then create an encrypted cross-region Read Replica

### Question 54:
A company runs an application on an Amazon EC2 instance the requires 250 GB of storage space. The application is not used often and has small spikes in usage on weekday mornings and afternoons. The disk I/O can vary with peaks hitting a maximum of 3,000 IOPS. A Solutions Architect must recommend the most cost-effective storage solution that delivers the performance required.

Which configuration should the Solutions Architect recommend?

Which solution should the solutions architect recommend?
* Amazon EBS Provisioned IOPS SSD (i01)
* Amazon EBS Cold HDD (sc1)
* Amazon EBS Throughput Optimized HDD (st1)
* Amazon EBS General Purpose SSD (gp2)

### Question 55:
A company is migrating from an on-premises infrastructure to the AWS Cloud. One of the company's applications stores files on a Windows file server farm that uses Distributed File System Replication (DFSR) to keep data in sync. A solutions architect needs to replace the file server farm.

Which service should the solutions architect use?
* Amazon FSx
* Amazon EFS
* AWS Storage Gateway
* Amazon S3

### Question 56:
A company uses an Amazon RDS MySQL database instance to store customer order data. The security team have requested that SSL/TLS encryption in transit must be used for encrypting connections to the database from application servers. The data in the database is currently encrypted at rest using an AWS KMS key.

How can a Solutions Architect enable encryption in transit?
* Download the AWS-provided root certificates. Use the certificates when connecting to the RDS DB instance.
* Add a self-signed certificate to the RDS DB instance. Use the certificates in all connections to the RDS DB instance.
* Take a snapshot of the RDS instance. Restore the snapshot to a new instance with encryption in transit enabled.
* Enable encryption in transit using the RDS Management console and obtain a key using AWS KMS.

### Question 57:
An eCommerce application consists of three tiers. The web tier includes EC2 instances behind an Application Load balancer, the middle tier uses EC2 instances and an Amazon SQS queue to process orders, and the database tier consists of an Auto Scaling DynamoDB table. During busy periods customers have complained about delays in the processing of orders. A Solutions Architect has been tasked with reducing processing times.

Which action will be MOST effective in accomplishing this requirement?
* Replace the Amazon SQS queue with Amazon Kinesis Data Firehose.
* Use Amazon EC2 Auto Scaling to scale out the middle tier instances based on the SQS queue depth.
* Use Amazon DynamoDB Accelerator (DAX) in front of the DynamoDB backend tier.
* Add an Amazon CloudFront distribution with a custom origin to cache the responses for the web tier.

### Question 58:
An e-commerce application is hosted in AWS. The last time a new product was launched, the application experienced a performance issue due to an enormous spike in traffic. Management decided that capacity must be doubled this week after the product is launched.

What is the MOST efficient way for management to ensure that capacity requirements are met?
* Add Amazon EC2 Spot instances
* Add a Step Scaling policy
* Add a Simple Scaling policy
* Add a Scheduled Scaling action

### Question 59:
A company delivers content to subscribers distributed globally from an application running on AWS. The application uses a fleet of Amazon EC2 instance in a private subnet behind an Application Load Balancer (ALB). Due to an update in copyright restrictions, it is necessary to block access for specific countries.

What is the EASIEST method to meet this requirement?
* Use Amazon CloudFront to serve the application and deny access to blocked countries
* Modify the ALB security group to deny incoming traffic from blocked countries
* Modify the security group for EC2 instances to deny incoming traffic from blocked countries
* Use a network ACL to block the IP address ranges associated with the specific countries

### Question 60:
A solutions architect is designing a new service that will use an Amazon API Gateway API on the frontend. The service will need to persist data in a backend database using key-value requests. Initially, the data requirements will be around 1 GB and future growth is unknown. Requests can range from 0 to over 800 requests per second.

Which combination of AWS services would meet these requirements? (Select TWO.)
* Amazon EC2 Auto Scaling
* Amazon DynamoDB
* AWS Lambda
* AWS Fargate
* Amazon RDS

### Question 61:
A financial services company has a web application with an application tier running in the U.S and Europe. The database tier consists of a MySQL database running on Amazon EC2 in us-west-1. Users are directed to the closest application tier using Route 53 latency-based routing. The users in Europe have reported poor performance when running queries.

Which changes should a Solutions Architect make to the database tier to improve performance?
* Migrate the database to Amazon RedShift. Use AWS DMS to synchronize data. Configure applications to use the RedShift data warehouse for queries.
* Migrate the database to Amazon RDS for MySQL. Configure Multi-AZ in one of the European Regions.
* Create an Amazon RDS Read Replica in one of the European regions. Configure the application tier in Europe to use the read replica for queries.
* Migrate the database to an Amazon Aurora global database in MySQL compatibility mode. Configure the application tier in Europe to use the local reader endpoint.

### Question 62:
A Solutions Architect has been tasked with re-deploying an application running on AWS to enable high availability. The application processes messages that are received in an ActiveMQ queue running on a single Amazon EC2 instance. Messages are then processed by a consumer application running on Amazon EC2. After processing the messages the consumer application writes results to a MySQL database running on Amazon EC2.

Which architecture offers the highest availability and low operational complexity?
* Deploy a second Active MQ server to another Availability Zone. Launch an additional consumer EC2 instance in another Availability Zone. Use MySQL database replication to another Availability Zone.
* Deploy Amazon MQ with active/standby brokers configured across two Availability Zones. Launch an additional consumer EC2 instance in another Availability Zone. Use Amazon RDS for MySQL with Multi-AZ enabled.
* Deploy Amazon MQ with active/standby brokers configured across two Availability Zones. Create an Auto Scaling group for the consumer EC2 instances across two Availability Zones. Use an Amazon RDS MySQL database with Multi-AZ enabled.
* Deploy Amazon MQ with active/standby brokers configured across two Availability Zones. Launch an additional consumer EC2 instance in another Availability Zone. Use MySQL database replication to another Availability Zone.

### Question 63:
An eCommerce company runs an application on Amazon EC2 instances in public and private subnets. The web application runs in a public subnet and the database runs in a private subnet. Both the public and private subnets are in a single Availability Zone.

Which combination of steps should a solutions architect take to provide high availability for this architecture? (Select TWO.)
* Create an EC2 Auto Scaling group and Application Load Balancer that spans across multiple AZs.
* Create an EC2 Auto Scaling group in the public subnet and use an Application Load Balancer.
* Create new public and private subnets in a different AZ. Migrate the database to an Amazon RDS multi-AZ deployment.
* Create new public and private subnets in the same AZ but in a different Amazon VPC.
* Create new public and private subnets in a different AZ. Create a database using Amazon EC2 in one AZ.

### Question 64:
A solutions architect needs to backup some application log files from an online ecommerce store to Amazon S3. It is unknown how often the logs will be accessed or which logs will be accessed the most. The solutions architect must keep costs as low as possible by using the appropriate S3 storage class.

Which S3 storage class should be implemented to meet these requirements?
* S3 One Zone-Infrequent Access (S3 One Zone-IA)
* S3 Glacier
* S3 Intelligent-Tiering
* S3 Standard-Infrequent Access (S3 Standard-IA)

### Question 65:
A company is deploying a fleet of Amazon EC2 instances running Linux across multiple Availability Zones within an AWS Region. The application requires a data storage solution that can be accessed by all of the EC2 instances simultaneously. The solution must be highly scalable and easy to implement. The storage must be mounted using the NFS protocol.

Which solution meets these requirements?
* Create an Amazon RDS database and store the data in a BLOB format. Point the application instances to the RDS endpoint.
* Create an Amazon S3 bucket and create an S3 gateway endpoint to allow access to the file system using the NFS protocol.
* Create an Amazon EFS file system with mount targets in each Availability Zone. Configure the application instances to mount the file system.
* Create an Amazon EBS volume and use EBS Multi-Attach to mount the volume to all EC2 instances across each Availability Zone.

# Exam 2

### Question 1:
A company runs an application on Amazon EC2 instances which requires access to sensitive data in an Amazon S3 bucket. All traffic between the EC2 instances and the S3 bucket must not traverse the internet and must use private IP addresses. Additionally, the bucket must only allow access from services in the VPC.

Which combination of actions should a Solutions Architect take to meet these requirements? (Select TWO.)
* Apply an IAM policy to a VPC peering connection.
* Enable default encryption on the bucket.
* Apply a bucket policy to restrict access to the S3 endpoint.
* Create a VPC endpoint for Amazon S3.
* Create a peering connection to the S3 bucket VPC.

### Question 2:
A company has refactored a legacy application to run as two microservices using Amazon ECS. The application processes data in two parts and the second part of the process takes longer than the first.

How can a solutions architect integrate the microservices and allow them to scale independently?
* Implement code in microservice 1 to publish data to an Amazon SNS topic. Implement code in microservice 2 to subscribe to this topic
* Implement code in microservice 1 to send data to an Amazon SQS queue. Implement code in microservice 2 to process messages from the queue
* Implement code in microservice 1 to send data to Amazon Kinesis Data Firehose. Implement code in microservice 2 to read from Kinesis Data Firehose
* Implement code in microservice 1 to send data to an Amazon S3 bucket. Use S3 event notifications to invoke microservice 2

### Question 3:
A company's web application is using multiple Amazon EC2 Linux instances and storing data on Amazon EBS volumes. The company is looking for a solution to increase the resiliency of the application in case of a failure.

What should a solutions architect do to meet these requirements?
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Mount an instance store on each EC2 instance
* Launch the application on EC2 instances in each Availability Zone. Attach EBS volumes to each EC2 instance
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Store data on Amazon EFS and mount a target on each instance
* Create an Application Load Balancer with Auto Scaling groups across multiple Availability Zones. Store data using Amazon S3 One Zone-Infrequent Access (S3 One Zone-A)

### Question 4:
An application upgrade caused some issues with stability. The application owner enabled logging and has generated a 5 GB log file in an Amazon S3 bucket. The log file must be securely shared with the application vendor to troubleshoot the issues.

What is the MOST secure way to share the log file?
* Generate a presigned URL and ask the vendor to download the log file before the URL expires.
* Create access keys using an administrative account and share the access key ID and secret access key with the vendor.
* Enable default encryption for the bucket and public access. Provide the S3 URL of the file to the vendor.
* Create an IAM user for the vendor to provide access to the S3 bucket and the application. Enforce multi-factor authentication.

### Question 5:
A web application is deployed in multiple regions behind an ELB Application Load Balancer. You need deterministic routing to the closest region and automatic failover. Traffic should traverse the AWS global network for consistent performance.

How can this be achieved?
* Place an EC2 Proxy in front of the ALB and configure automatic failover
* Configure AWS Global Accelerator and configure the ALBs as targets
* Use a CloudFront distribution with multiple custom origins in each region and configure for high availability
* Create a Route 53 Alias record for each ALB and configure a latency-based routing policy

### Question 6:
A solutions architect has created a new AWS account and must secure AWS account root user access.

Which combination of actions will accomplish this? (Select TWO.)
* Add the root user to a group containing administrative permissions
* Delete the root user account
* Store root user access keys in an encrypted Amazon S3 bucket
* Ensure the root user uses a strong password
* Enable multi-factor authentication for the root user

### Question 7:
A Solutions Architect must design a storage solution for incoming billing reports in CSV format. The data will be analyzed infrequently and discarded after 30 days.

Which combination of services will be MOST cost-effective in meeting these requirements?
* Write the files to an S3 bucket and use Amazon Athena to query the data
* Import the logs into an RDS MySQL instance
* Import the logs to an Amazon Redshift cluster
* Use AWS Data Pipeline to import the logs into a DynamoDB table

### Question 8:
A company requires a solution to allow customers to customize images that are stored in an online catalog. The image customization parameters will be sent in requests to Amazon API Gateway. The customized image will then be generated on-demand and can be accessed online.

The solutions architect requires a highly available solution. Which solution will be MOST cost-effective?
* Use Amazon EC2 instances to manipulate the original images into the requested customization. Store the original images in Amazon S3 and the manipulated images in Amazon DynamoDB. Configure an Amazon CloudFront distribution with the S3 bucket as the origin
* Use AWS Lambda to manipulate the original images to the requested customization. Store the original and manipulated images in Amazon S3. Configure an Amazon CloudFront distribution with the S3 bucket as the origin
* Use Amazon EC2 instances to manipulate the original images into the requested customization. Store the original and manipulated images in Amazon S3. Configure an Elastic Load Balancer in front of the EC2 instances
* Use AWS Lambda to manipulate the original images to the requested customization. Store the original images in Amazon S3 and the manipulated images in Amazon DynamoDB. Configure an Elastic Load Balancer in front of the Amazon EC2 instances

### Question 9:
A website runs on Amazon EC2 instances behind an Application Load Balancer (ALB). The website has a mix of dynamic and static content. Customers around the world are reporting performance issues with the website.

Which set of actions will improve website performance for users worldwide?
* Create an Amazon CloudFront distribution and configure the ALB as an origin. Then update the Amazon Route 53 record to point to the CloudFront distribution
* Create a latency-based Amazon Route 53 record for the ALB. Then launch new EC2 instances with larger instance sizes and register the instances with the ALB
* Migrate the website to an Amazon S3 bucket in the Regions closest to the users. Then create an Amazon Route 53 geolocation record to point to the S3 buckets
* Launch new EC2 instances hosting the same web application in different Regions closer to the users. Use an AWS Transit Gateway to connect customers to the closest region

### Question 10:
An organization plans to deploy a higher performance computing (HPC) workload on AWS using Linux. The HPC workload will use many Amazon EC2 instances and will generate a large quantity of small output files that must be stored in persistent storage for future use.

A Solutions Architect must design a solution that will enable the EC2 instances to access data using native file system interfaces and to store output files in cost-effective long-term storage.

Which combination of AWS services meets these requirements?
* Amazon EBS volumes with Amazon S3 Glacier.
* Amazon FSx for Windows File Server with Amazon S3.
* Amazon FSx for Lustre with Amazon S3.
* AWS DataSync with Amazon S3 Intelligent tiering.

### Question 11:
A solutions architect is designing an application on AWS. The compute layer will run in parallel across EC2 instances. The compute layer should scale based on the number of jobs to be processed. The compute layer is stateless. The solutions architect must ensure that the application is loosely coupled and the job items are durably stored.

Which design should the solutions architect use?
* Create an Amazon SQS queue to hold the jobs that needs to be processed. Create an Amazon EC2 Auto Scaling group for the compute application. Set the scaling policy for the Auto Scaling group to add and remove nodes based on the number of items in the SQS queue
* Create an Amazon SNS topic to send the jobs that need to be processed. Create an Amazon EC2 Auto Scaling group for the compute application. Set the scaling policy for the Auto Scaling group to add and remove nodes based on the number of messages published to the SNS topic
* Create an Amazon SQS queue to hold the jobs that need to be processed. Create an Amazon EC2 Auto Scaling group for the compute application. Set the scaling policy for the Auto Scaling group to add and remove nodes based on network usage
* Create an Amazon SNS topic to send the jobs that need to be processed. Create an Amazon EC2 Auto Scaling group for the compute application. Set the scaling policy for the Auto Scaling group to add and remove nodes based on CPU usage

### Question 12:
A company is deploying a new web application that will run on Amazon EC2 instances in an Auto Scaling group across multiple Availability Zones. The application requires a shared storage solution that offers strong consistency as the content will be regularly updated.

Which solution requires the LEAST amount of effort?
* Create a shared Amazon Block Store (Amazon EBS) volume and mount it on the individual Amazon EC2 instances
* Create a volume gateway using AWS Storage Gateway to host the data and mount it to the Auto Scaling group
* Create an Amazon Elastic File System (Amazon EFS) file system and mount it on the individual Amazon EC2 instances
* Create an Amazon S3 bucket to store the web content and use Amazon CloudFront to deliver the content

### Question 13:
A group of business analysts perform read-only SQL queries on an Amazon RDS database. The queries have become quite numerous and the database has experienced some performance degradation. The queries must be run against the latest data. A Solutions Architect must solve the performance problems with minimal changes to the existing web application.

What should the Solutions Architect recommend?
* Load the data into Amazon ElastiCache and instruct the business analysts to run their queries against the ElastiCache endpoint.
* Create a read replica of the primary database and instruct the business analysts to direct queries to the replica.
* Load the data into an Amazon Redshift cluster and instruct the business analysts to run their queries against the cluster.
* Export the data to Amazon S3 and instruct the business analysts to run their queries using Amazon Athena.

### Question 14:
An IoT sensor is being rolled out to thousands of a company’s existing customers. The sensors will stream high volumes of data each second to a central location. A solution must be designed to ingest and store the data for analytics. The solution must provide near-real time performance and millisecond responsiveness.

Which solution should a Solutions Architect recommend?
* Ingest the data into an Amazon SQS queue. Process the data using an AWS Lambda function and then store the data in Amazon DynamoDB.
* Ingest the data into an Amazon SQS queue. Process the data using an AWS Lambda function and then store the data in Amazon RedShift.
* Ingest the data into an Amazon Kinesis Data Stream. Process the data with an AWS Lambda function and then store the data in Amazon DynamoDB.
* Ingest the data into an Amazon Kinesis Data Stream. Process the data with an AWS Lambda function and then store the data in Amazon RedShift.

### Question 15:
A company allows its developers to attach existing IAM policies to existing IAM roles to enable faster experimentation and agility. However, the security operations team is concerned that the developers could attach the existing administrator policy, which would allow the developers to circumvent any other security policies.

How should a solutions architect address this issue?
* Create an Amazon SNS topic to send an alert every time a developer creates a new policy
* Prevent the developers from attaching any policies and assign all IAM duties to the security operations team
* Set an IAM permissions boundary on the developer IAM role that explicitly denies attaching the administrator policy
* Use service control policies to disable IAM activity across all accounts in the organizational unit

### Question 16:
A solutions architect is designing a two-tier web application. The application consists of a public-facing web tier hosted on Amazon EC2 in public subnets. The database tier consists of Microsoft SQL Server running on Amazon EC2 in a private subnet. Security is a high priority for the company.

How should security groups be configured in this situation? (Select TWO.)
* Configure the security group for the web tier to allow inbound traffic on port 443 from 0.0.0.0/0
* Configure the security group for the database tier to allow inbound traffic on ports 443 and 1433 from the security group for the web tier
* Configure the security group for the web tier to allow outbound traffic on port 443 from 0.0.0.0/0
* Configure the security group for the database tier to allow outbound traffic on ports 443 and 1433 to the security group for the web tier
* Configure the security group for the database tier to allow inbound traffic on port 1433 from the security group for the web tier

### Question 17:
A company is storing a large quantity of small files in an Amazon S3 bucket. An application running on an Amazon EC2 instance needs permissions to access and process the files in the S3 bucket.

Which action will MOST securely grant the EC2 instance access to the S3 bucket?
* Create an IAM role with least privilege permissions and attach it to the EC2 instance profile.
* Create an IAM user for the application with specific permissions to the S3 bucket.
* Create a bucket ACL on the S3 bucket and configure the EC2 instance ID as a grantee.
* Generate access keys and store the credentials on the EC2 instance for use in making API calls.

### Question 18:
A DynamoDB database you manage is randomly experiencing heavy read requests that are causing latency. What is the simplest way to alleviate the performance issues?
* Enable DynamoDB DAX
* Create an ElastiCache cluster in front of DynamoDB
* Create DynamoDB read replicas
* Enable EC2 Auto Scaling for DynamoDB

### Question 19:
A company requires a solution for replicating data to AWS for disaster recovery. Currently, the company uses scripts to copy data from various sources to a Microsoft Windows file server in the on-premises data center. The company also requires that a small amount of recent files are accessible to administrators with low latency.

What should a Solutions Architect recommend to meet these requirements?
* Update the script to copy data to an Amazon EBS volume instead of the on-premises file server.
* Update the script to copy data to an Amazon EFS volume instead of the on-premises file server.
* Update the script to copy data to an Amazon S3 Glacier archive instead of the on-premises file server.
* Update the script to copy data to an AWS Storage Gateway for File Gateway virtual appliance instead of the on-premises file server.

### Question 20:
A web application is being deployed on an Amazon ECS cluster using the Fargate launch type. The application is expected to receive a large volume of traffic initially. The company wishes to ensure that performance is good for the launch and that costs reduce as demand decreases

What should a solutions architect recommend?
* Use an AWS Lambda function to scale Amazon ECS based on metric breaches that trigger an Amazon CloudWatch alarm.
* Use Amazon EC2 Auto Scaling with simple scaling policies to scale when an Amazon CloudWatch alarm is breached.
* Use Amazon EC2 Auto Scaling to scale out on a schedule and back in once the load decreases.
* Use Amazon ECS Service Auto Scaling with target tracking policies to scale when an Amazon CloudWatch alarm is breached.

### Question 21:
A company runs several NFS file servers in an on-premises data center. The NFS servers must run periodic backups to Amazon S3 using automatic synchronization for small volumes of data.

Which solution meets these requirements and is MOST cost-effective?
* Set up AWS Glue to extract the data from the NFS shares and load it into Amazon S3.
* Set up an SFTP sync using AWS Transfer for SFTP to sync data from on premises to Amazon S3.
* Set up an AWS DataSync agent on the on-premises servers and sync the data to Amazon S3.
* Set up an AWS Direct Connect connection between the on-premises data center and AWS and copy the data to Amazon S3.

### Question 22:
A company runs an eCommerce application that uses an Amazon Aurora database. The database performs well except for short periods when monthly sales reports are run. A Solutions Architect has reviewed metrics in Amazon CloudWatch and found that the Read Ops and CPUUtilization metrics are spiking during the periods when the sales reports are run.

What is the MOST cost-effective solution to solve this performance issue?
* Create an Amazon Redshift data warehouse and run the reporting there.
* Create an Aurora Replica and use the replica endpoint for reporting.
* Enable storage Auto Scaling for the Amazon Aurora database.
* Modify the Aurora database to use an instance class with more CPU.

### Question 23:
A solutions architect is optimizing a website for real-time streaming and on-demand videos. The website’s users are located around the world and the solutions architect needs to optimize the performance for both the real-time and on-demand streaming.

Which service should the solutions architect choose?
* Amazon Route 53
* Amazon CloudFront
* Amazon S3 Transfer Acceleration
* AWS Global Accelerator

### Question 24:
An application stores transactional data in an Amazon S3 bucket. The data is analyzed for the first week and then must remain immediately available for occasional analysis.

What is the MOST cost-effective storage solution that meets the requirements?
* Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 7 days.
* Configure a lifecycle policy to transition the objects to Amazon S3 One Zone-Infrequent Access (S3 One Zone-IA) after 30 days.
* Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 30 days.
* Configure a lifecycle policy to transition the objects to Amazon S3 Standard-Infrequent Access (S3 Standard-IA) after 7 days.

### Question 25:
A company is planning a migration for a high performance computing (HPC) application and associated data from an on-premises data center to the AWS Cloud. The company uses tiered storage on premises with hot high-performance parallel storage to support the application during periodic runs of the application, and more economical cold storage to hold the data when the application is not actively running.

Which combination of solutions should a solutions architect recommend to support the storage needs of the application? (Select TWO.)
* Amazon FSx for Lustre for high-performance parallel storage
* Amazon EFS for cold data storage
* Amazon S3 for high-performance parallel storage
* Amazon S3 for cold data storage
* Amazon FSx for Windows for high-performance parallel storage

### Question 26:
A High Performance Computing (HPC) application will be migrated to AWS. The application requires low network latency and high throughput between nodes and will be deployed in a single AZ.

How should the application be deployed for best inter-node performance?
* Behind a Network Load Balancer (NLB)
* In a cluster placement group
* In a spread placement group
* In a partition placement group

### Question 27:
A Solutions Architect must select the most appropriate database service for two use cases. A team of data scientists perform complex queries on a data warehouse that take several hours to complete. Another team of scientists need to run fast, repeat queries and update dashboards for customer support staff.

Which solution delivers these requirements MOST cost-effectively?
* RDS for both use cases
* RedShift for the analytics use case and ElastiCache in front of RedShift for the customer support dashboard
* RedShift for the analytics use case and RDS for the customer support dashboard
* RedShift for both use cases

### Question 28:
A company runs an internal browser-based application. The application runs on Amazon EC2 instances behind an Application Load Balancer. The instances run in an Amazon EC2 Auto Scaling group across multiple Availability Zones. The Auto Scaling group scales up to 20 instances during work hours, but scales down to 2 instances overnight. Staff are complaining that the application is very slow when the day begins, although it runs well by midmorning

How should the scaling be changed to address the staff complaints and keep costs to a minimum?
* Implement a step scaling action triggered at a lower CPU threshold, and decrease the cooldown period
* Implement a target tracking action triggered at a lower CPU threshold, and decrease the cooldown period
* Implement a scheduled action that sets the minimum and maximum capacity to 20 shortly before the office opens
* Implement a scheduled action that sets the desired capacity to 20 shortly before the office opens

### Question 29:
An application launched on Amazon EC2 instances needs to publish personally identifiable information (PII) about customers using Amazon SNS. The application is launched in private subnets within an Amazon VPC.

Which is the MOST secure way to allow the application to access service endpoints in the same region?
* Use an Internet Gateway
* Use a proxy instance
* Use AWS PrivateLink
* Use a NAT gateway

### Question 30:
A web application has recently been launched on AWS. The architecture includes two tier with a web layer and a database layer. It has been identified that the web server layer may be vulnerable to cross-site scripting (XSS) attacks.

What should a solutions architect do to remediate the vulnerability?
* Create a Network Load Balancer. Put the web layer behind the load balancer and enable AWS WAF
* Create an Application Load Balancer. Put the web layer behind the load balancer and enable AWS WAF
* Create a Classic Load Balancer. Put the web layer behind the load balancer and enable AWS WAF
* Create an Application Load Balancer. Put the web layer behind the load balancer and use AWS Shield Standard

### Question 31:
An application uses Amazon EC2 instances and an Amazon RDS MySQL database. The database is not currently encrypted. A solutions architect needs to apply encryption to the database for all new and existing data.

How should this be accomplished?
* Create an Amazon ElastiCache cluster and encrypt data using the cache nodes
* Enable encryption for the database using the API. Take a full snapshot of the database. Delete old snapshots
* Take a snapshot of the RDS instance. Create an encrypted copy of the snapshot. Restore the RDS instance from the encrypted snapshot
* Create an RDS read replica with encryption at rest enabled. Promote the read replica to master and switch the application over to the new master. Delete the old RDS instance

### Question 32:
An automotive company plans to implement IoT sensors in manufacturing equipment that will send data to AWS in real time. The solution must receive events in an ordered manner from each asset and ensure that the data is saved for future processing.

Which solution would be MOST efficient?
* Use an Amazon SQS standard queue for real-time events with one queue for each equipment asset. Trigger an AWS Lambda function from the SQS queue to save data to Amazon S3.
* Use Amazon Kinesis Data Streams for real-time events with a shard for each equipment asset. Use Amazon Kinesis Data Firehose to save data to Amazon EBS.
* Use Amazon Kinesis Data Streams for real-time events with a partition for each equipment asset. Use Amazon Kinesis Data Firehose to save data to Amazon S3.
* Use an Amazon SQS FIFO queue for real-time events with one queue for each equipment asset. Trigger an AWS Lambda function for the SQS queue to save data to Amazon EFS.

### Question 33:
A company runs a number of core enterprise applications in an on-premises data center. The data center is connected to an Amazon VPC using AWS Direct Connect. The company will be creating additional AWS accounts and these accounts will also need to be quickly, and cost-effectively connected to the on-premises data center in order to access the core applications.

What deployment changes should a Solutions Architect implement to meet these requirements with the LEAST operational overhead?
* Configure AWS Transit Gateway between the accounts. Assign Direct Connect to the transit gateway and route network traffic to the on-premises servers.
* Configure VPC endpoints in the Direct Connect VPC for all required services. Route the network traffic to the on-premises servers.
* Create a VPN connection between each new account and the Direct Connect VPC. Route the network traffic to the on-premises servers.
* Create a Direct Connect connection in each new account. Route the network traffic to the on-premises servers.

### Question 34:
A company wants to migrate a legacy web application from an on-premises data center to AWS. The web application consists of a web tier, an application tier, and a MySQL database. The company does not want to manage instances or clusters.

Which combination of services should a solutions architect include in the overall architecture? (Select TWO.)
* AWS Fargate
* Amazon DynamoDB
* Amazon Kinesis Data Streams
* Amazon RDS for MySQL
* Amazon EC2 Spot Instances

### Question 35:
A company is planning to upload a large quantity of sensitive data to Amazon S3. The company’s security department require that the data is encrypted before it is uploaded.

Which option meets these requirements?
* Use client-side encryption with Amazon S3 managed encryption keys.
* Use client-side encryption with a master key stored in AWS KMS.
* Use server-side encryption with keys stored in KMS.
* Use server-side encryption with customer-provided encryption keys.

### Question 36:
Some objects that are uploaded to Amazon S3 standard storage class are initially accessed frequently for a period of 30 days. Then, objects are infrequently accessed for up to 90 days. After that, the objects are no longer needed.

How should lifecycle management be configured?
* Transition to STANDARD_IA after 30 days. After 90 days transition to GLACIER
* Transition to STANDARD_IA after 30 days. After 90 days transition to ONEZONE_IA
* Transition to REDUCED_REDUNDANCY after 30 days. After 90 days expire the objects
* Transition to ONEZONE_IA after 30 days. After 90 days expire the objects

### Question 37:
A highly sensitive application runs on Amazon EC2 instances using EBS volumes. The application stores data temporarily on Amazon EBS volumes during processing before saving results to an Amazon RDS database. The company’s security team mandate that the sensitive data must be encrypted at rest.

Which solution should a Solutions Srchitect recommend to meet this requirement?
* Configure SSL/TLS encryption using AWS KMS customer master keys (CMKs) to encrypt database volumes.
* Use AWS Certificate Manager to generate certificates that can be used to encrypt the connections between the EC2 instances and RDS.
* Use Amazon Data Lifecycle Manager to encrypt all data as it is stored to the EBS volumes and RDS database.
* Configure encryption for the Amazon EBS volumes and Amazon RDS database with AWS KMS keys.

### Question 38:
A Solutions Architect is designing a web application that runs on Amazon EC2 instances behind an Elastic Load Balancer. All data in transit must be encrypted.

Which solution options meet the encryption requirement? (choose 2)
* Use a Network Load Balancer (NLB) with an HTTPS listener, then install SSL certificates on the NLB and EC2 instances
* Use an Application Load Balancer (ALB) with an HTTPS listener, then install SSL certificates on the ALB and EC2 instances
* Use a Network Load Balancer (NLB) with a TCP listener, then terminate SSL on EC2 instances
* Use an Application Load Balancer (ALB) in passthrough mode, then terminate SSL on EC2 instances
* Use an Application Load Balancer (ALB) with a TCP listener, then terminate SSL on EC2 instances

### Question 39:
A company has a file share on a Microsoft Windows Server in an on-premises data center. The server uses a local network attached storage (NAS) device to store several terabytes of files. The management team require a reduction in the data center footprint and to minimize storage costs by moving on-premises storage to AWS.

What should a Solutions Architect do to meet these requirements?
* Create an Amazon EFS volume and use an IPSec VPN.
* Configure an AWS Storage Gateway as a volume gateway.
* Create an Amazon S3 bucket and an S3 gateway endpoint.
* Configure an AWS Storage Gateway file gateway.

### Question 40:
A data-processing application runs on an i3.large EC2 instance with a single 100 GB EBS gp2 volume. The application stores temporary data in a small database (less than 30 GB) located on the EBS root volume. The application is struggling to process the data fast enough, and a Solutions Architect has determined that the I/O speed of the temporary database is the bottleneck.

What is the MOST cost-efficient way to improve the database response times?
* Move the temporary database onto instance storage
* Put the temporary database on a new 50-GB EBS gp2 volume
* Enable EBS optimization on the instance and keep the temporary files on the existing volume
* Put the temporary database on a new 50-GB EBS io1 volume with a 3000 IOPS allocation

### Question 41:
A web application that allows users to upload and share documents is running on a single Amazon EC2 instance with an Amazon EBS volume. To increase availability the architecture has been updated to use an Auto Scaling group of several instances across Availability Zones behind an Application Load Balancer. After the change users can only see a subset of the documents.

What is the BEST method for a solutions architect to modify the solution so users can see all documents?
* Run a script to synchronize the data between Amazon EBS volumes
* Copy the data from all EBS volumes to Amazon EFS. Modify the application to save new documents to Amazon EFS
* Use Sticky Sessions with the ALB to ensure users are directed to the same EC2 instance in a session
* Configure the Application Load Balancer to send the request to all servers. Return each document from the correct server

### Question 42:
A company have 500 TB of data in an on-premises file share that needs to be moved to Amazon S3 Glacier. The migration must not saturate the company’s low-bandwidth internet connection and the migration must be completed within a few weeks.

What is the MOST cost-effective solution?
* Use AWS Global Accelerator to accelerate upload and optimize usage of the available bandwidth
* Order 7 AWS Snowball appliances and select an S3 Glacier vault as the destination. Create a bucket policy to enforce a VPC endpoint
* Create an AWS Direct Connect connection and migrate the data straight into Amazon Glacier
* Order 7 AWS Snowball appliances and select an Amazon S3 bucket as the destination. Create a lifecycle policy to transition the S3 objects to Amazon S3 Glacier

### Question 43:
A company runs an application in an Amazon VPC that requires access to an Amazon Elastic Container Service (Amazon ECS) cluster that hosts an application in another VPC. The company’s security team requires that all traffic must not traverse the internet.

Which solution meets this requirement?
* Create a Network Load Balancer in one VPC and an AWS PrivateLink endpoint for Amazon ECS in another VPC.
* Configure a gateway endpoint for Amazon ECS. Update the route table to include an entry pointing to the ECS cluster.
* Configure an Amazon Route 53 private hosted zone for each VPC. Use private records to resolve internal IP addresses in each VPC.
* Create a Network Load Balancer and AWS PrivateLink endpoint for Amazon ECS in the VPC that hosts the ECS cluster.

### Question 44:
A company’s Amazon EC2 instances were terminated or stopped, resulting in a loss of important data that was stored on attached EC2 instance stores. They want to avoid this happening in the future and need a solution that can scale as data volumes increase with the LEAST amount of management and configuration.

Which storage is most appropriate?
* Amazon S3
* Amazon EBS
* Amazon RDS
* Amazon EFS

### Question 45:
A company has divested a single business unit and needs to move the AWS account owned by the business unit to another AWS Organization. How can this be achieved?
* Create a new account in the destination AWS Organization and migrate resources
* Migrate the account using AWS CloudFormation
* Create a new account in the destination AWS Organization and share the original resources using AWS Resource Access Manager
* Migrate the account using the AWS Organizations console

### Question 46:
A company has acquired another business and needs to migrate their 50TB of data into AWS within 1 month. They also require a secure, reliable and private connection to the AWS cloud.

How are these requirements best accomplished?
* Provision an AWS VPN CloudHub connection and migrate the data over redundant links
* Launch a Virtual Private Gateway (VPG) and migrate the data over the AWS VPN
* Provision an AWS Direct Connect connection and migrate the data over the link
* Migrate data using AWS Snowball. Provision an AWS VPN initially and order a Direct Connect link

### Question 47:
A multi-tier application runs with eight front-end web servers in an Amazon EC2 Auto Scaling group in a single Availability Zone behind an Application Load Balancer. A solutions architect needs to modify the infrastructure to be highly available without modifying the application.

Which architecture should the solutions architect choose that provides high availability?
* Create an Auto Scaling template that can be used to quickly create more instances in another Region
* Modify the Auto Scaling group to use four instances across each of two Availability Zones
* Create an Auto Scaling group that uses four instances across each of two subnets
* Create an Auto Scaling group that uses four instances across each of two Regions

### Question 48:
An application is hosted on the U.S west coast. Users there have no problems, but users on the east coast are experiencing performance issues. The users have reported slow response times with the search bar autocomplete and display of account listings.

How can you improve the performance for users on the east coast?
* Create an ElastiCache database in the U.S east region
* Create a DynamoDB Read Replica in the U.S east region
* Setup cross-region replication and use Route 53 geolocation routing
* Host the static content in an Amazon S3 bucket and distribute it using CloudFront

### Question 49:
An application running on Amazon ECS processes data and then writes objects to an Amazon S3 bucket. The application requires permissions to make the S3 API calls.

How can a Solutions Architect ensure the application has the required permissions?
* Create an IAM role that has read/write permissions to the bucket and update the task definition to specify the role as the taskRoleArn.
* Create a set of Access Keys with read/write permissions to the bucket and update the task credential ID.
* Update the S3 policy in IAM to allow read/write access from Amazon ECS, and then relaunch the container.
* Attach an IAM policy with read/write permissions to the bucket to an IAM group and add the container instances to the group.

### Question 50:
A Solutions Architect needs to design a solution that will allow Website Developers to deploy static web content without managing server infrastructure. All web content must be accessed over HTTPS with a custom domain name. The solution should be scalable as the company continues to grow.

Which of the following will provide the MOST cost-effective solution?
* Amazon S3 with a static website
* Amazon CloudFront with an Amazon S3 bucket origin
* Amazon EC2 instance with Amazon EBS
* AWS Lambda function with Amazon API Gateway

### Question 51:
A solutions architect has been tasked with designing a highly resilient hybrid cloud architecture connecting an on-premises data center and AWS. The network should include AWS Direct Connect (DX).

Which DX configuration offers the HIGHEST resiliency?
* Configure multiple public VIFs on top of a DX connection.
* Configure a DX connection with an encrypted VPN on top of it.
* Configure DX connections at multiple DX locations.
* Configure multiple private VIFs on top of a DX connection.

### Question 52:
An application has been deployed on Amazon EC2 instances behind an Application Load Balancer (ALB). A Solutions Architect must improve the security posture of the application and minimize the impact of a DDoS attack on resources.

Which of the following solutions is MOST effective?
* Create a custom AWS Lambda function that monitors for suspicious traffic and modifies a network ACL when a potential DDoS attack is identified.
* Configure an AWS WAF ACL with rate-based rules. Enable the WAF ACL on the Application Load Balancer.
* Enable access logs on the Application Load Balancer and configure Amazon CloudWatch to monitor the access logs and trigger a Lambda function when potential attacks are identified. Configure the Lambda function to modify the ALBs security group and block the attack.
* Enable VPC Flow Logs and store them in Amazon S3. Use Amazon Athena to parse the logs and identify and block potential DDoS attacks.

### Question 53:
A shared services VPC is being setup for use by several AWS accounts. An application needs to be securely shared from the shared services VPC. The solution should not allow consumers to connect to other instances in the VPC.

How can this be setup with the least administrative effort? (choose 2)
* Create a Network Load Balancer (NLB)
* Use AWS ClassicLink to expose the application as an endpoint service
* Configure security groups to restrict access
* Use AWS PrivateLink to expose the application as an endpoint service
* Setup VPC peering between each AWS VPC

### Question 54:
A website is running on Amazon EC2 instances and access is restricted to a limited set of IP ranges. A solutions architect is planning to migrate static content from the website to an Amazon S3 bucket configured as an origin for an Amazon CloudFront distribution. Access to the static content must be restricted to the same set of IP addresses.

Which combination of steps will meet these requirements? (Select TWO.)
* Create an origin access identity (OAI) and associate it with the distribution. Change the permissions in the bucket policy so that only the OAI can read the objects.
* Create an AWS WAF web ACL that includes the same IP restrictions that exist in the EC2 security group. Associate this new web ACL with the CloudFront distribution.
* Create an origin access identity (OAI) and associate it with the distribution. Generate presigned URLs that limit access to the OAI.
* Attach the existing security group that contains the IP restrictions to the Amazon CloudFront distribution.
* Create an AWS WAF web ACL that includes the same IP restrictions that exist in the EC2 security group. Associate this new web ACL with the Amazon S3 bucket.

### Question 55:
An application is running on Amazon EC2 behind an Elastic Load Balancer (ELB). Content is being published using Amazon CloudFront and you need to restrict the ability for users to circumvent CloudFront and access the content directly through the ELB.

How can you configure this solution?
* Use signed URLs or signed cookies to limit access to the content
* Create a VPC Security Group for the ELB and use AWS Lambda to automatically update the CloudFront internal service IP addresses when they change
* Create an Origin Access Identity (OAI) and associate it with the distribution
* Use a Network ACL to restrict access to the ELB

### Question 56:
You have created a file system using Amazon Elastic File System (EFS) which will hold home directories for users. What else needs to be done to enable users to save files to the EFS file system?
* Modify permissions on the root directory to grant read-write-execute permissions to the users. Then create a subdirectory and mount it to the users’ home directory
* Create a separate EFS file system for each user and grant read-write-execute permissions on the root directory to the respective user. Then mount the file system to the users’ home directory
* Instruct the users to create a subdirectory on the file system and mount the subdirectory to their home directory
* Create a subdirectory for each user and grant read-write-execute permissions to the users. Then mount the subdirectory to the users’ home directory

### Question 57:
An AWS workload in a VPC is running a legacy database on an Amazon EC2 instance. Data is stored on a 2000GB Amazon EBS (gp2) volume. At peak load times, logs show excessive wait time.

What should be implemented to improve database performance using persistent storage?
* Change the EC2 instance type to one with burstable performance
* Migrate the data on the EBS volume to provisioned IOPS SSD (io1)
* Change the EC2 instance type to one with EC2 instance store volumes
* Migrate the data on the Amazon EBS volume to an SSD-backed volume

### Question 58:
A website runs on a Microsoft Windows server in an on-premises data center. The web server is being migrated to Amazon EC2 Windows instances in multiple Availability Zones on AWS. The web server currently uses data stored in an on-premises network-attached storage (NAS) device.

Which replacement to the NAS file share is MOST resilient and durable?
* Migrate the file share to Amazon Elastic File System (Amazon EFS)
* Migrate the file share to Amazon EBS
* Migrate the file share to AWS Storage Gateway
* Migrate the file share to Amazon FSx for Windows File Server

### Question 59:
A solutions architect is finalizing the architecture for a distributed database that will run across multiple Amazon EC2 instances. Data will be replicated across all instances so the loss of an instance will not cause loss of data. The database requires block storage with low latency and throughput that supports up to several million transactions per second per server.

Which storage solution should the solutions architect use?
* Amazon EC2 instance store
* Amazon S3
* Amazon EBS
* Amazon EFS

### Question 60:
A large media site has multiple applications running on Amazon ECS. A Solutions Architect needs to use content metadata to route traffic to specific services.

What is the MOST efficient method to fulfil this requirement?
* Use Amazon CloudFront to manage and route traffic to the correct service
* Use an AWS Classic Load Balancer with a host-based routing rule to route traffic to the correct service
* Use an AWS Application Load Balancer with a path-based routing rule to route traffic to the correct service
* Use the AWS CLI to update an Amazon Route 53 hosted zone to route traffic as services get updated

### Question 61:
An application running video-editing software is using significant memory on an Amazon EC2 instance. How can a user track memory usage on the Amazon EC2 instance?
* Install the CloudWatch agent on the EC2 instance to push memory usage to an Amazon CloudWatch custom metric
* Use an instance type that supports memory usage reporting to a metric by default
* Call Amazon CloudWatch to retrieve the memory usage metric data that exists for the EC2 instance
* Assign an IAM role to the EC2 instance with an IAM policy granting access to the desired metric

### Question 62:
An organization is migrating data to the AWS cloud. An on-premises application uses Network File System shares and must access the data without code changes. The data is critical and is accessed frequently.

Which storage solution should a Solutions Architect recommend to maximize availability and durability?
* Amazon Elastic File System
* AWS Storage Gateway – File Gateway
* Amazon Elastic Block Store
* Amazon Simple Storage Service

### Question 63:
A company uses a Microsoft Windows file share for storing documents and media files. Users access the share using Microsoft Windows clients and are authenticated using the company’s Active Directory. The chief information officer wants to move the data to AWS as they are approaching capacity limits. The existing user authentication and access management system should be used.

How can a Solutions Architect meet these requirements?
* Move the documents and media files to an Amazon Simple Storage Service bucket and apply bucket ACLs.
* Move the documents and media files to an Amazon FSx for Windows File Server file system.
* Move the documents and media files to an Amazon Elastic File System and use POSIX permissions.
* Move the documents and media files to an Amazon FSx for Lustre file system.

### Question 64:
A Solutions Architect must design a solution that encrypts data in Amazon S3. Corporate policy mandates encryption keys be generated and managed on premises. Which solution should the Architect use to meet the security requirements?
* AWS CloudHSM
* SSE-KMS: Server-side encryption with AWS KMS managed keys
* SSE-S3: Server-side encryption with Amazon-managed master key
* SSE-C: Server-side encryption with customer-provided encryption keys

### Question 65:
An Amazon RDS PostgreSQL database is configured as Multi-AZ. A solutions architect needs to scale read performance and the solution must be configured for high availability. What is the most cost-effective solution?
* Deploy a read replica in the same AZ as the master DB instance
* Create a read replica as a Multi-AZ DB instance
* Deploy a read replica in a different AZ to the master DB instance
* Deploy a read replica using Amazon ElastiCache

# Exam 3

### Question 1:
A Solutions Architect is designing a mobile application that will capture receipt images to track expenses. The Architect wants to store the images on Amazon S3. However, uploading the images through the web server will create too much traffic.

What is the MOST efficient method to store images from a mobile application on Amazon S3?
* Upload directly to S3 using a pre-signed URL
* Upload to a separate Auto Scaling Group of server behind an ELB Classic Load Balancer, and have the server instances write to the Amazon S3 bucket
* Expand the web server fleet with Spot instances to provide the resources to handle the images
* Upload to a second bucket, and have a Lambda event copy the image to the primary bucket

### Question 2:
A company operates a production web application that uses an Amazon RDS MySQL database. The database has automated, non-encrypted daily backups. To increase the security of the data, it has been recommended that encryption should be enabled for backups. Unencrypted backups will be destroyed after the first encrypted backup has been completed.

What should be done to enable encryption for future backups?
* Create a snapshot of the database. Copy it to an encrypted snapshot. Restore the database from the encrypted snapshot
* Enable an encrypted read replica on RDS for MySQL. Promote the encrypted read replica to primary. Remove the original database instance
* Enable default encryption for the Amazon S3 bucket where backups are stored
* Modify the backup section of the database configuration to toggle the Enable encryption check box

### Question 3:
An application allows users to upload and download files. Files older than 2 years will be accessed less frequently. A solutions architect needs to ensure that the application can scale to any number of files while maintaining high availability and durability.

Which scalable solutions should the solutions architect recommend?
* Store the files in Amazon Elastic Block Store (EBS) volumes. Schedule snapshots of the volumes. Use the snapshots to archive data older than 2 years
* Store the files on Amazon S3 with a lifecycle policy that moves objects older than 2 years to S3 Standard Infrequent Access (S3 Standard-IA)
* Store the files in Amazon Elastic Block Store (EBS) volumes. Create a lifecycle policy to move files older than 2 years to Amazon S3 Glacier
* Store the files on Amazon Elastic File System (EFS) with a lifecycle policy that moves objects older than 2 years to EFS Infrequent Access (EFS IA)

### Question 4:
A High Performance Computing (HPC) application needs storage that can provide 135,000 IOPS. The storage layer is replicated across all instances in a cluster.

What is the optimal storage solution that provides the required performance and is cost-effective?
* Use Amazon EBS Provisioned IOPS volume with 135,000 IOPS
* Use Amazon Instance Store
* Use Amazon S3 with byte-range fetch
* Use Amazon EC2 Enhanced Networking with an EBS HDD Throughput Optimized volume

### Question 5:
A company has experienced malicious traffic from some suspicious IP addresses. The security team discovered the requests are from different IP addresses under the same CIDR range.

What should a solutions architect recommend to the team?
* Add a deny rule in the inbound table of the network ACL with a lower rule number than other rules
* Add a rule in the inbound table of the security group to deny the traffic from that CIDR range
* Add a deny rule in the outbound table of the network ACL with a lower rule number than other rules
* Add a rule in the outbound table of the security group to deny the traffic from that CIDR range

### Question 6:
A company runs a financial application using an Amazon EC2 Auto Scaling group behind an Application Load Balancer (ALB). When running month-end reports on a specific day and time each month the application becomes unacceptably slow. Amazon CloudWatch metrics show the CPU utilization hitting 100%.

What should a solutions architect recommend to ensure the application is able to handle the workload and avoid downtime?
* Configure an EC2 Auto Scaling scheduled scaling policy based on the monthly schedule
* Configure an EC2 Auto Scaling simple scaling policy based on CPU utilization
* Configure an Amazon CloudFront distribution in front of the ALB
* Configure Amazon ElastiCache to remove some of the workload from the EC2 instances

### Question 7:
A Solutions Architect is designing a static website that will use the zone apex of a DNS domain (e.g. example.com). The Architect wants to use the Amazon Route 53 service. Which steps should the Architect take to implement a scalable and cost-effective solution? (choose 2)   
* Create a Route 53 hosted zone, and set the NS records of the domain to use Route 53 name servers   
* Serve the website from an Amazon S3 bucket, and map a Route 53 Alias record to the website endpoint   
* Host the website on an Amazon EC2 instance, and map a Route 53 Alias record to the public IP address of the EC2 instance   
* Host the website using AWS Elastic Beanstalk, and map a Route 53 Alias record to the Beanstalk stack   
* Host the website on an Amazon EC2 instance with ELB and Auto Scaling, and map a Route 53 Alias record to the ELB endpoint   

### Question 8:
A Solutions Architect is migrating a small relational database into AWS. The database will run on an EC2 instance and the DB size is around 500 GB. The database is infrequently used with small amounts of requests spread across the day. The DB is a low priority and the Architect needs to lower the cost of the solution.

 What is the MOST cost-effective storage type for the data volume?
* Amazon EBS Throughput Optimized HDD   
* Amazon EBS Provisioned IOPS SSD   
* Amazon EFS   
* Amazon EBS General Purpose SSD   

### Question 9:
A Solutions Architect needs to monitor application logs and receive a notification whenever a specific number of occurrences of certain HTTP status code errors occur. Which tool should the Architect use?
* CloudWatch Events
* CloudWatch Logs
* CloudTrail Trails
* CloudWatch Metrics

### Question 10:
An EC2 status check on an EBS volume is showing as insufficient-data. What is the most likely explanation?   
* The checks have failed on the volume   
* The checks may still be in progress on the volume   
* The volume does not have enough data on it to check properly   
* The checks require more information to be manually entered   

### Question 11:
You have implemented API Gateway and enabled a cache for a specific stage. How can you control the cache to enhance performance and reduce load on back-end services?   
* Using time-to-live (TTL) settings   
* Using CloudFront controls   
* Configure the throttling feature   
* Enable bursting   

### Question 12:
A company has deployed an API in a VPC behind an internal Network Load Balancer (NLB). An application that consumes the API as a client is deployed in a second account in private subnets.

Which architectural configurations will allow the API to be consumed without using the public Internet? (Select TWO.)
* Configure a PrivateLink connection for the API into the client VPC. Access the API using the PrivateLink address
* Configure an AWS Resource Access Manager connection between the two accounts. Access the API using the private address
* Configure a ClassicLink connection for the API into the client VPC. Access the API using the ClassicLink address
* Configure a VPC peering connection between the two VPCs. Access the API using the private address
* Configure an AWS Direct Connect connection between the two VPCs. Access the API using the private address

### Question 13:
A company is generating large datasets with millions of rows that must be summarized by column. Existing business intelligence tools will be used to build daily reports.

 Which storage service meets the requirements?
* Amazon DynamoDB   
* Amazon RDS   
* Amazon ElastiCache   
* Amazon RedShift   

### Question 14:
A production application runs on an Amazon RDS MySQL DB instance. A solutions architect is building a new reporting tool that will access the same data. The reporting tool must be highly available and not impact the performance of the production application.

How can this be achieved?
* Create a Multi-AZ RDS Read Replica of the production RDS DB instance
* Create a cross-region Multi-AZ deployment and create a read replica in the second region
* Use Amazon Data Lifecycle Manager to automatically create and manage snapshots
* Create a Single-AZ RDS Read Replica of the production RDS DB instance. Create a second Single-AZ RDS Read Replica from the replica

### Question 15:
A Solutions Architect is designing a workload that requires a high performance object-based storage system that must be shared with multiple Amazon EC2 instances.

Which AWS service delivers these requirements?
* Amazon S3   
* Amazon EBS   
* Amazon EFS   
* Amazon ElastiCache   

### Question 16:
A web application in a three-tier architecture runs on a fleet of Amazon EC2 instances. Performance issues have been reported and investigations point to insufficient swap space. The operations team requires monitoring to determine if this is correct.

What should a solutions architect recommend?
* Use EC2 metadata to collect information, then publish it to Amazon CloudWatch custom metrics. Monitor SwapUsage metrics in CloudWatch
* Configure an Amazon CloudWatch SwapUsage metric dimension. Monitor the SwapUsage dimension in the EC2 metrics in CloudWatch
* Enable detailed monitoring in the EC2 console. Create an Amazon CloudWatch SwapUtilization custom metric. Monitor SwapUtilization metrics in CloudWatch
* Install an Amazon CloudWatch agent on the instances. Run an appropriate script on a set schedule. Monitor SwapUtilization metrics in CloudWatch

### Question 17:
An e-commerce web application needs a highly scalable key-value database. Which AWS database service should be used?
* Amazon ElastiCache
* Amazon RedShift
* Amazon RDS
* Amazon DynamoDB

### Question 18:
You have created an application in a VPC that uses a Network Load Balancer (NLB). The application will be offered in a service provider model for AWS principals in other accounts within the region to consume. Based on this model, what AWS service will be used to offer the service for consumption?   
* API Gateway   
* IAM Role Based Access Control   
* VPC Endpoint Services using AWS PrivateLink   
* Route 53

### Question 19:
An application currently stores all data on Amazon EBS volumes. All EBS volumes must be backed up durably across multiple Availability Zones.

 What is the MOST resilient way to back up volumes?
* Enable EBS volume encryption   
* Mirror data across two EBS volumes   
* Take regular EBS snapshots   
* Create a script to copy data to an EC2 instance store   

### Question 20:
An application is deployed on multiple AWS regions and accessed from around the world. The application exposes static public IP addresses. Some users are experiencing poor performance when accessing the application over the Internet.

What should a solutions architect recommend to reduce internet latency?
* Set up AWS Direct Connect locations in multiple Regions
* Set up an Amazon Route 53 geoproximity routing policy to route traffic
* Set up an Amazon CloudFront distribution to access an application
* Set up AWS Global Accelerator and add endpoints

### Question 21:
An Architect is designing a serverless application that will accept images uploaded by users from around the world. The application will make API calls to back-end services and save the session state data of the user to a database.

Which combination of services would provide a solution that is cost-effective while delivering the least latency?
* API Gateway, Amazon S3, AWS Lambda, DynamoDB   
* Amazon CloudFront, API Gateway, Amazon S3, AWS Lambda, DynamoDB   
* Amazon S3, API Gateway, AWS Lambda, Amazon RDS   
* Amazon CloudFront, API Gateway, Amazon S3, AWS Lambda, Amazon RDS   

### Question 22:
A Solutions Architect is designing a solution for a financial application that will receive trading data in large volumes. What is the best solution for ingesting and processing a very large number of data streams in near real time?   
* Kinesis Data Streams
* RedShift
* EMR   
* Kinesis Firehose   

### Question 23:
You need a service that can provide you with control over which traffic to allow or block to your web applications by defining customizable web security rules. You need to block common attack patterns, such as SQL injection and cross-site scripting, as well as creating custom rules for your own applications.

Which AWS service fits these requirements?
* Security Groups
* CloudFront
* AWS WAF
* Route 53   

### Question 24:
A company has created a duplicate of its environment in another AWS Region. The application is running in warm standby mode. There is an Application Load Balancer (ALB) in front of the application. Currently, failover is manual and requires updating a DNS alias record to point to the secondary ALB.

How can a solutions architect automate the failover process?
* Enable an Amazon Route 53 health check
* Create a latency based routing policy on Amazon Route 53
* Create a CNAME record on Amazon Route 53 pointing to the ALB endpoint
* Enable an ALB health check

### Question 25:
An application runs on Amazon EC2 Linux instances. The application generates log files which are written using standard API calls. A storage solution is required that can be used to store the files indefinitely and must allow concurrent access to all files.

Which storage service meets these requirements and is the MOST cost-effective?
* Amazon S3
* Amazon EC2 instance store
* Amazon EBS
* Amazon EFS

### Question 26:
A critical database runs in your VPC for which availability is a concern. Which RDS DB instance events may force the DB to be taken offline during a maintenance window?   
* Promoting a Read Replica   
* Selecting the Multi-AZ feature   
* Updating DB parameter groups   
* Security patching   

### Question 27:
A gaming company collects real-time data and stores it in an on-premises database system. The company are migrating to AWS and need better performance for the database. A solutions architect has been asked to recommend an in-memory database that supports data replication.

Which database should a solutions architect recommend?
* Amazon RDS for PostgreSQL
* Amazon RDS for MySQL
* Amazon ElastiCache for Memcached
* Amazon ElastiCache for Redis

### Question 28:
You have been asked to deploy a new High-Performance Computing (HPC) cluster. You need to create a design for the EC2 instances that ensures close proximity, low latency and high network throughput.

Which AWS features will help you to achieve this requirement whilst considering cost? (choose 2)
* Use Provisioned IOPS EBS volumes   
* Use dedicated hosts   
* Use EC2 instances with Enhanced Networking   
* Launch I/O Optimized EC2 instances in one private subnet in an AZ   
* Use Placement groups   

### Question 29:
An issue has been reported whereby Amazon EC2 instances are not being terminated from an Auto Scaling Group behind an ELB when traffic volumes are low. How can this be fixed?
* Modify the scaling settings on the ELB
* Modify the scale down increment
* Modify the lower threshold settings on the ASG
* Modify the upper threshold settings on the ASG

### Question 30:
The development team at your company has created a new mobile application that will be used by users to access confidential data. The developers have used Amazon Cognito for authentication, authorization, and user management. Due to the sensitivity of the data, there is a requirement to add another method of authentication in addition to a username and password.

You have been asked to recommend the best solution. What is your recommendation?
* Integrate IAM with a user pool in Cognito   
* Integrate a third-party identity provider (IdP)   
* Enable multi-factor authentication (MFA) in IAM   
* Use multi-factor authentication (MFA) with a Cognito user pool   

### Question 31:
A company is planning to use Amazon S3 to store documents uploaded by its customers. The images must be encrypted at rest in Amazon S3. The company does not want to spend time managing and rotating the keys, but it does want to control who can access those keys.

What should a solutions architect use to accomplish this?
* Server-Side Encryption with Customer-Provided Keys (SSE-C)
* Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3)
* Server-Side Encryption with AWS KMS-Managed Keys (SSE-KMS)
* Server-Side Encryption with keys stored in an S3 bucket

### Question 32:
A Solutions Architect is designing a solution to store and archive corporate documents, and has determined that Amazon Glacier is the right solution. Data must be delivered within 10 minutes of a retrieval request.

Which features in Amazon Glacier can help meet this requirement?
* Standard retrieval
* Bulk retrieval
* Expedited retrieval
* Vault Lock   

### Question 33:
You are developing an application that uses Lambda functions. You need to store some sensitive data that includes credentials for accessing the database tier. You are planning to store this data as environment variables within Lambda. How can you ensure this sensitive information is properly secured?   
* This cannot be done, only the environment variables that relate to the Lambda function itself can be encrypted   
* There is no need to make any changes as all environment variables are encrypted by default with AWS Lambda   
* Use encryption helpers that leverage AWS Key Management Service to store the sensitive information as Ciphertext   
* Store the environment variables in an encrypted DynamoDB table and configure Lambda to retrieve them as required   

### Question 34:
A company has some statistical data stored in an Amazon RDS database. The company wants to allow users to access this information using an API. A solutions architect must create a solution that allows sporadic access to the data, ranging from no requests to large bursts of traffic.

Which solution should the solutions architect suggest?
* Set up an Amazon API Gateway and use Amazon ECS
* Set up an Amazon API Gateway and use AWS Lambda functions
* Set up an Amazon API Gateway and use Amazon EC2 with Auto Scaling
* Set up an Amazon API Gateway and use AWS Elastic Beanstalk

### Question 35:
A solutions architect is designing a microservices architecture. AWS Lambda will store data in an Amazon DynamoDB table named Orders. The solutions architect needs to apply an IAM policy to the Lambda function’s execution role to allow it to put, update, and delete items in the Orders table. No other actions should be allowed.

Which of the following code snippets should be included in the IAM policy to fulfill this requirement whilst providing the LEAST privileged access?
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Deny",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Deny",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Deny",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": "dynamodb:* ",
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/*"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/*"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/*"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"
* "Sid": "PutUpdateDeleteOnOrders",
"Effect": "Allow",
"Action": [
"dynamodb:PutItem",
"dynamodb:UpdateItem",
"dynamodb:DeleteItem"
],
"Resource": "arn:aws:dynamodb:us-east-1:227392126428:table/Orders"

### Question 36:
A new application will be launched on an Amazon EC2 instance with an Elastic Block Store (EBS) volume. A solutions architect needs to determine the most cost-effective storage option. The application will have infrequent usage, with peaks of traffic for a couple of hours in the morning and evening. Disk I/O is variable with peaks of up to 3,000 IOPS.

Which solution should the solutions architect recommend?
* Amazon EBS Throughput Optimized HDD (st1)
* Amazon EBS General Purpose SSD (gp2)
* Amazon EBS Provisioned IOPS SSD (io1)
* Amazon EBS Cold HDD (sc1)

### Question 37:
You are deploying an application on Amazon EC2 that must call AWS APIs. Which method of securely passing credentials to the application should you use?
* Store API credentials as an object in Amazon S3   
* Assign IAM roles to the EC2 instances   
* Embed the API credentials into your application files   
* Store the API credentials on the instance using instance metadata

### Question 38:
Health related data in Amazon S3 needs to be frequently accessed for up to 90 days. After that time the data must be retained for compliance reasons for seven years and is rarely accessed.

Which storage classes should be used?
* Store data in STANDARD for 90 days then transition the data to DEEP_ARCHIVE
* Store data in STANDARD for 90 days then expire the data
* Store data in STANDARD for 90 days then transition to REDUCED_REDUNDANCY
* Store data in INTELLIGENT_TIERING for 90 days then transition to STANDARD_IA

### Question 39:
An online store uses an Amazon Aurora database. The database is deployed as a Multi-AZ deployment. Recently, metrics have shown that database read requests are high and causing performance issues which result in latency for write requests.

What should the solutions architect do to separate the read requests from the write requests?
* Create a read replica and modify the application to use the appropriate endpoint
* Enable read through caching on the Amazon Aurora database
* Create a second Amazon Aurora database and link it to the primary database as a read replica
* Update the application to read from the Multi-AZ standby instance

### Question 40:
An Architect needs to find a way to automatically and repeatably create many member accounts within an AWS Organization. The accounts also need to be moved into an OU and have VPCs and subnets created.

What is the best way to achieve this?
* Use CloudFormation with scripts
* Use the AWS Organizations API
* Use the AWS Management Console
* Use the AWS CLI

### Question 41:
You are designing a solution on AWS that requires a file storage layer that can be shared between multiple EC2 instances. The storage should be highly-available and should scale easily.

Which AWS service can be used for this design?
* Amazon S3
* Amazon EBS   
* Amazon EC2 instance store
* Amazon EFS

### Question 42:
A company is migrating an on-premises 10 TB MySQL database to AWS. The company expects the database to quadruple in size and the business requirement is that replicate lag must be kept under 100 milliseconds.

Which Amazon RDS engine meets these requirements?
* Oracle   
* Microsoft SQL Server   
* MySQL   
* Amazon Aurora   

### Question 43:
A company runs a service on AWS to provide offsite backups for images on laptops and phones. The solution must support millions of customers, with thousands of images per customer. Images will be retrieved infrequently, but must be available for retrieval immediately.

Which is the MOST cost-effective storage option that meets these requirements?
* Amazon S3 Standard   
* Amazon EFS   
* Amazon S3 Standard-Infrequent Access   
* Amazon Glacier with expedited retrievals   

### Question 44:
A security officer requires that access to company financial reports is logged. The reports are stored in an Amazon S3 bucket. Additionally, any modifications to the log files must be detected.

Which actions should a solutions architect take?
* Use S3 server access logging on the bucket that houses the reports with the read and write management events and log file validation options enabled
* Use S3 server access logging on the bucket that houses the reports with the read and write data events and the log file validation options enabled
* Use AWS CloudTrail to create a new trail. Configure the trail to log read and write data events on the S3 bucket that houses the reports. Log these events to a new bucket, and enable log file validation
* Use AWS CloudTrail to create a new trail. Configure the trail to log read and write management events on the S3 bucket that houses the reports. Log these events to a new bucket, and enable log file validation

### Question 45:
A high-performance file system is required for a financial modelling application. The data set will be stored on Amazon S3 and the storage solution must have seamless integration so objects can be accessed as files.

Which storage solution should be used?
* Amazon FSx for Lustre
* Amazon FSx for Windows File Server
* Amazon Elastic File System (EFS)
* Amazon Elastic Block Store (EBS)

### Question 46:
A Kinesis consumer application is reading at a slower rate than expected. It has been identified that multiple consumer applications have total reads exceeding the per-shard limits. How can this situation be resolved?
* Increase the number of read transactions per shard
* Implement read throttling for the Kinesis data stream
* Increase the number of shards in the Kinesis data stream
* Implement API throttling to restrict the number of requests per-shard

### Question 47:
There is expected to be a large increase in write intensive traffic to a website you manage that registers users onto an online learning program. You are concerned about writes to the database being dropped and need to come up with a solution to ensure this does not happen. Which of the solution options below would be the best approach to take?   
* Use CloudFront to cache the writes and configure the database as a custom origin   
* Update the application to write data to an SQS queue and provision additional EC2 instances to process the data and write it to the database   
* Update the application to write data to an S3 bucket and provision additional EC2 instances to process the data and write it to the database   
* Use RDS in a multi-AZ configuration to distribute writes across AZs   

### Question 48:
An organization is extending a secure development environment into AWS. They have already secured the VPC including removing the Internet Gateway and setting up a Direct Connect connection. What else needs to be done to add encryption?
* Setup a Virtual Private Gateway (VPG)
* Setup the Border Gateway Protocol (BGP) with encryption
* Enable IPSec encryption on the Direct Connect connection
* Configure an AWS Direct Connect Gateway

### Question 49:
You are planning to deploy a number of EC2 instances in your VPC. The EC2 instances will be deployed across several subnets and multiple AZs. What AWS feature can act as an instance-level firewall to control traffic between your EC2 instances?   
* AWS WAF
* Network ACL   
* Route table
* Security Group

### Question 50:
Your Business Intelligence team use SQL tools to analyze data. What would be the best solution for performing queries on structured data that is being received at a high velocity?   
* EMR using Hive   
* Kinesis Firehose with RDS   
* Kinesis Firehose with RedShift   
* EMR running Apache Spark   

### Question 51:
You need to scale read operations for your Amazon Aurora DB within a region. To increase availability you also need to be able to failover if the primary instance fails.

What should you implement?
* Aurora Global Database
* An Aurora Cluster Volume
* A DB cluster
* Aurora Replicas

### Question 52:
A Solutions Architect is determining the best method for provisioning Internet connectivity for a data-processing application that will pull large amounts of data from an object storage system via the Internet. The solution must be redundant and have no constraints on bandwidth.

Which option satisfies these requirements?
* Deploy NAT Instances in a public subnet   
* Use a NAT Gateway     
* Create a VPC endpoint   
* Attach an Internet Gateway   

### Question 53:
A company is planning to migrate a large quantity of important data to Amazon S3. The data will be uploaded to a versioning enabled bucket in the us-west-1 Region. The solution needs to include replication of the data to another Region for disaster recovery purposes.

How should a solutions architect configure the replication?
* Create an additional S3 bucket in another Region and configure cross-origin resource sharing (CORS)
* Create an additional S3 bucket with versioning in another Region and configure cross-origin resource sharing (CORS)
* Create an additional S3 bucket with versioning in another Region and configure cross-Region replication
* Create an additional S3 bucket in another Region and configure cross-Region replication

### Question 54:
A company is serving videos to their customers from us-east-1 from an Amazon S3 bucket. The company's customers are located around the world and there is high demand during peak hours. Customers in Asia complain about slow download speeds during peak hours and customers in all locations have reported experiencing HTTP 500 errors.

How can a Solutions Architect address the issues?
* Cache the web content using Amazon CloudFront and use all Edge locations for content delivery   
* Place an Amazon ElastiCache cluster in front of the S3 bucket   
* Replicate the bucket in us-east-1 and use Amazon Route 53 failover routing to determine which bucket to serve the content from   
* Use an Amazon Route 53 weighted routing policy for the CloudFront domain name to distribute GET requests between CloudFront and the S3 bucket   

### Question 55:
A new security mandate requires that all personnel data held in the cloud is encrypted at rest. Which two methods allow you to encrypt data stored in S3 buckets at rest cost-efficiently? (choose 2)
* Make use of AWS S3 bucket policies to control access to the data at rest   
* Use Multipart upload with SSL   
* Encrypt the data at the source using the client's CMK keys before transferring it to S3   
* Use AWS S3 server-side encryption with Key Management Service keys or Customer-provided keys   
* Use CloudHSM

### Question 56:
A solutions architect is designing a high performance computing (HPC) application using Amazon EC2 Linux instances. All EC2 instances need to communicate to each other with low latency and high throughput network performance.

Which EC2 solution BEST meets these requirements?
* Launch the EC2 instances in an Auto Scaling group in two Regions. Place a Network Load Balancer in front of the instances
* Launch the EC2 instances in a cluster placement group in one Availability Zone
* Launch the EC2 instances in a spread placement group in one Availability Zone
* Launch the EC2 instances in an Auto Scaling group spanning multiple Availability Zones

### Question 57:
An application requires a MySQL database which will only be used several times a week for short periods. The database needs to provide automatic instantiation and scaling. Which database service is most suitable?
* Amazon Aurora
* Amazon EC2 instance with MySQL database installed
* Amazon RDS MySQL
* Amazon Aurora Serverless

### Question 58:
You work for Digital Cloud Training and have just created a number of IAM users in your AWS account. You need to ensure that the users are able to make API calls to AWS services. What else needs to be done?   
* Create a group and add the users to it   
* Enable Multi-Factor Authentication for the users   
* Create a set of Access Keys for the users   
* Set a password for each user   

### Question 59:
An application on Amazon Elastic Container Service (ECS) performs data processing in two parts. The second part takes much longer to complete. How can an Architect decouple the data processing from the backend application component?
* Process each part using a separate ECS task. Create an Amazon SQS queue
* Process both parts using the same ECS task. Create an Amazon Kinesis Firehose stream
* Process each part using a separate ECS task. Create an Amazon SNS topic and send a notification when the processing completes
* Create an Amazon DynamoDB table and save the output of the first part to the table

### Question 60:
A web application is running on a fleet of Amazon EC2 instances using an Auto Scaling Group. It is desired that the CPU usage in the fleet is kept at 40%.

How should scaling be configured?
* Use a custom CloudWatch alarm to monitor CPU usage and notify the ASG using Amazon SNS
* Use a simple scaling policy that launches instances when the average CPU hits 40%
* Use a target tracking policy that keeps the average aggregate CPU utilization at 40%
* Use a step scaling policy that uses the PercentChangeInCapacity value to adjust the group size as required

### Question 61:
A Solutions Architect is designing a web page for event registrations, and needs a managed service to send a text message to users every time users sign up for an event.

Which AWS service should the Architect use to achieve this?
* Amazon SNS   
* AWS Lambda   
* Amazon SQS   
* Amazon STS   

### Question 62:
A security team wants to limit access to specific services or actions in all of the team's AWS accounts. All accounts belong to a large organization in AWS Organizations. The solution must be scalable and there must be a single point where permissions can be maintained.

What should a solutions architect do to accomplish this?
* Create a service control policy in the root organizational unit to deny access to the services or actions
* Create cross-account roles in each account to deny access to the services or actions
* Create a security group to allow accounts and attach it to user groups
* Create an ACL to provide access to the services or actions

### Question 63:
An application runs on Amazon EC2 instances across multiple Availability Zones. The instances run in an Amazon EC2 Auto Scaling group behind an Application Load Balancer. The application performs best when the CPU utilization of the EC2 instances is at or near 40%.

What should a solutions architect do to maintain the desired performance across all instances in the group?
* Use a target tracking policy to dynamically scale the Auto Scaling group
* Use scheduled scaling actions to scale up and scale down the Auto Scaling group
* Use an AWS Lambda function to update the desired Auto Scaling group capacity
* Use a simple scaling policy to dynamically scale the Auto Scaling group

### Question 64:
An application stack includes an Elastic Load Balancer in a public subnet, a fleet of Amazon EC2 instances in an Auto Scaling Group, and an Amazon RDS MySQL cluster. Users connect to the application from the Internet. The application servers and database must be secure.

What is the most appropriate architecture for the application stack?
* Create a private subnet for the Amazon EC2 instances and a public subnet for the Amazon RDS cluster
* Create a public subnet for the Amazon EC2 instances and a private subnet for the Amazon RDS cluster
* Create a private subnet for the Amazon EC2 instances and a private subnet for the Amazon RDS cluster
* Create a public subnet for the Amazon EC2 instances and a public subnet for the Amazon RDS cluster

### Question 65:
A web app allows users to upload images for viewing online. The compute layer that processes the images is behind an Auto Scaling group. The processing layer should be decoupled from the front end and the ASG needs to dynamically adjust based on the number of images being uploaded.

How can this be achieved?
* Create an Amazon SNS Topic to generate a notification each time a message is uploaded. Have the ASG scale based on the number of SNS messages
* Create a target tracking policy that keeps the ASG at 70% CPU utilization
* Create an Amazon SQS queue and custom CloudWatch metric to measure the number of messages in the queue. Configure the ASG to scale based on the number of messages in the queue
* Create a scheduled policy that scales the ASG at times of expected peak load

# Exam 4

### Question 1:
A manager is concerned that the default service limits my soon be reached for several AWS services. Which AWS tool can a Solutions Architect use to display current usage and limits?
* Amazon CloudWatch   
* AWS Trusted Advisor   
* AWS Dashboard   
* AWS Systems Manager   

### Question 2:
An application regularly uploads files from an Amazon EC2 instance to an Amazon S3 bucket. The files can be a couple of gigabytes in size and sometimes the uploads are slower than desired. What method can be used to increase throughput and reduce upload times?
* Use Amazon S3 multipart upload   
* Upload the files using the S3 Copy SDK or REST API   
* Turn off versioning on the destination bucket   
* Randomize the object names when uploading   

### Question 3:
A new financial platform has been re-architected to use Docker containers in a micro-services architecture. The new architecture will be implemented on AWS and a Solutions Architect must recommend the solution configuration. For operational reasons, it will be necessary to access the operating system of the instances on which the containers run.

Which solution delivery option should the Architect select?
* ECS with the EC2 launch type   
* ECS with a default cluster   
* EKS with Kubernetes managed infrastructure   
* ECS with the Fargate launch type   

### Question 4:
A Solutions Architect regularly deploys and manages infrastructure services for customers on AWS. The SysOps team are facing challenges in tracking changes that are made to the infrastructure services and rolling back when problems occur.

How can a Solutions Architect BEST assist the SysOps team?
* Use CodeDeploy to manage version control for the infrastructure services
* Use Trusted Advisor to record updates made to the infrastructure services
* Use CloudFormation templates to deploy and manage the infrastructure services
* Use AWS Systems Manager to manage all updates to the infrastructure services

### Question 5:
An operations team would like to be notified if an RDS database exceeds certain metric thresholds. How can a Solutions Architect automate this process for the operations team?
* Create a CloudWatch alarm and associate an SNS topic with it that sends an email notification   
* Setup an RDS alarm and associate an SNS topic with it that sends an email   
* Create a CloudWatch alarm and associate an SQS with it that delivers a message to SES   
* Create a CloudTrail alarm and configure a notification event to send an SMS   

### Question 6:
An existing Auto Scaling group is running with eight Amazon EC2 instances. A Solutions Architect has attached an Elastic Load Balancer (ELB) to the Auto Scaling group by connecting a Target Group. The ELB is in the same region and already has ten EC2 instances running in the Target Group.

When attempting to attach the ELB the request immediately fails, what is the MOST likely cause?
* You cannot attach running EC2 instances to an ASG   
* One or more of the instances are unhealthy
* Adding the 10 EC2 instances to the ASG would exceed the maximum capacity configured   
* ASGs cannot be edited once defined, you would need to recreate it   

### Question 7:
An application analyzes images of people that are uploaded to an Amazon S3 bucket. The application determines demographic data which is then saved to a .CSV file in another S3 bucket. The data must be encrypted at rest and then queried using SQL. The solution should be fully serverless.

Which actions should a Solutions Architect take to encrypt and query the data?
* Use AWS KMS encryption keys for the S3 bucket and use Amazon Kinesis Data Analytics to query the data
* Use Amazon S3 server-side encryption and Amazon QuickSight to query the data
* Use AWS KMS encryption keys for the S3 bucket and use Amazon Athena to query the data
* Use Amazon S3 server-side encryption and use Amazon RedShift Spectrum to query the data

### Question 8:
A Solutions Architect is creating a solution for an application that must be deployed on Amazon EC2 hosts that are dedicated to the client. Instance placement must be automatic and billing should be per instance.

Which type of EC2 deployment model should be used?
* Cluster Placement Group
* Reserved Instance
* Dedicated Host
* Dedicated Instance

### Question 9:
There has been an increase in traffic to an application that writes data to an Amazon DynamoDB database. Thousands of random tables reads occur per second and low-latency is required. What can a Solutions Architect do to improve performance for the reads without negatively impacting the rest of the application?
* Increase the number of Amazon DynamoDB write capacity units
* Use Amazon DynamoDB Accelerator to cache the reads
* Add an Amazon SQS queue to decouple the requests
* Use an Amazon Kinesis Data Stream to decouple requests

### Question 10:
A Solutions Architect is designing the compute layer of a serverless application. The compute layer will manage requests from external systems, orchestrate serverless workflows, and execute the business logic.

The Architect needs to select the most appropriate AWS services for these functions. Which services should be used for the compute layer? (choose 2)
* Use Amazon ECS for executing the business logic   
* Use AWS Elastic Beanstalk for executing the business logic   
* Use Amazon API Gateway with AWS Lambda for executing the business logic   
* Use AWS CloudFormation for orchestrating serverless workflows   
* Use AWS Step Functions for orchestrating serverless workflows   

### Question 11:
Encrypted Amazon Elastic Block Store (EBS) volumes are attached to some Amazon EC2 instances. Which statements are correct about using encryption with Amazon EBS volumes? (choose 2)
* Encryption is supported on all Amazon EBS volume types   
* Data in transit between an instance and an encrypted volume is also encrypted   
* Data is only encrypted at rest
* Volumes created from encrypted snapshots are unencrypted   
* You cannot mix encrypted with unencrypted volumes on an instance   

### Question 12:
A company runs an application on-premises that must consume a REST API running on Amazon API Gateway. The company has an AWS Direct Connect connection to their Amazon VPC. The solutions architect wants all API calls to use private addressing only and avoid the internet. How can this be achieved?
* Use a private virtual interface and create a VPC Endpoint for Amazon API Gateway
* Use a hosted virtual interface and create a VPC Endpoint for Amazon API Gateway
* Use a transit virtual interface and an AWS VPN to create a secure tunnel to Amazon API Gateway
* Use a public virtual interface and an AWS VPN to create a secure tunnel to Amazon API Gateway

### Question 13:
A new department will begin using AWS services an AWS account and a Solutions Architect needs to create an authentication and authorization strategy. Select the correct statements regarding IAM groups? (choose 2)
* IAM groups can be used to assign permissions to users   
* IAM groups can temporarily assume a role to take on permissions for a specific task   
* IAM groups can be used to group EC2 instances   
* An IAM group is not an identity and cannot be identified as a principal in an IAM policy   
* IAM groups can be nested up to 4 levels   

### Question 14:
A Solutions Architect is creating a design for a two-tier application with a MySQL RDS back-end. The performance requirements of the database tier are hard to quantify until the application is running and the Architect is concerned about right-sizing the database.

What methods of scaling are possible after the MySQL RDS database is deployed? (choose 2)
* Horizontal scaling for write capacity by enabling Multi-AZ   
* Horizontal scaling for read capacity by creating a read-replica   
* Horizontal scaling for read and write by enabling Multi-Master RDS DB
* Vertical scaling for read and write by choosing a larger instance size   
* Vertical scaling for read and write by using Transfer Acceleration   

### Question 15:
The AWS Acceptable Use Policy describes permitted and prohibited behavior on AWS and includes descriptions of prohibited security violations and network abuse. According to the policy, what is AWS’s position on penetration testing?
* AWS allow penetration for some resources without prior authorization
* AWS do not allow any form of penetration testing
* AWS allow penetration testing for all resources
* AWS allow penetration testing by customers on their own VPC resources

### Question 16:
An application that is being installed on an Amazon EC2 instance requires a persistent block storage volume. The data must be encrypted at rest and regular volume-level backups must be automated.

Which solution options should be used?
* Use an encrypted Amazon EBS volume and use Data Lifecycle Manager to automate snapshots
* Use an encrypted Amazon EFS filesystem and use an Amazon CloudWatch Events rule to start a backup copy of data using AWS Lambda
* Use an encrypted Amazon EC2 instance store and copy the data to another EC2 instance using a cron job and a batch script
* Use server-side encryption on an Amazon S3 bucket and use Cross-Region-Replication to backup on a schedule

### Question 17:
An Amazon ElastiCache for Redis cluster runs across multiple Availability Zones. A solutions architect is concerned about the security of sensitive data as it is replicated between nodes. How can the solutions architect protect the sensitive data?
* Enable at-rest encryption
* Issue a Redis AUTH command
* Enable in-transit encryption
* Set up MFA and API logging

### Question 18:
Amazon CloudWatch is being used to monitor the performance of AWS Lambda. Which metrics does Lambda track? (choose 2)
* Total number of requests   
* Total number of transactions   
* Latency per request   
* Number of users
* Total number of connections   

### Question 19:
A Solutions Architect is creating an application design with several components that will be publicly addressable. The Architect would like to use Alias records. Using Route 53 Alias records what targets can you specify? (choose 2)   
* CloudFront distribution   
* On-premise web server   
* Elastic BeanStalk environment   
* EFS filesystem
* ElastiCache cluster   

### Question 20:
A Solutions Architect is deploying a high performance computing (HPC) application on Amazon EC2 instances. The application requires extremely low inter-instance latency. How should the instances be deployed for BEST performance?
* Use an Elastic Fabric Adapter (EFA) and deploy instances in a cluster placement group
* Add multiple Elastic Network Adapters (ENAs) to each instance and create a NIC team
* Use an EBS-optimized instance with 10 Gigabit networking and deploy to a single subnet
* Use an instance with enhanced networking and deploy the instances in a partition placement group

### Question 21:
An event in CloudTrail is the record of an activity in an AWS account. What are the two types of events that can be logged in CloudTrail? (choose 2)   
* Data Events which are also known as data plane operations   
* System Events which are also known as instance level operations   
* Control Events which are also known as data plane operations
* Management Events which are also known as control plane operations   
* Platform Events which are also known as hardware level operations   

### Question 22:
A new application runs on Amazon EC2 instances and uses API Gateway and AWS Lambda. The company is planning on running an advertising campaign that will likely result in significant hits to the application after each ad is run.

A Solutions Architect is concerned about the impact this may have on the application and would like to put in place some controls to limit the number of requests per second that hit the application.

What controls should the Solutions Architect implement?
* API Gateway and Lambda scale automatically to handle any load so there’s no need to implement controls   
* Enable Lambda continuous scaling   
* Enable caching on the API Gateway and specify a size in gigabytes   
* Implement throttling rules on the API Gateway   

### Question 23:
A Solutions Architect is attempting to clean up unused EBS volumes and snapshots to save some space and cost. How many of the most recent snapshots of an EBS volume need to be maintained to guarantee that you can recreate the full EBS volume from the snapshot?
* You must retain all snapshots as the process is incremental and therefore data is required from each snapshot   
* Only the most recent snapshot. Snapshots are incremental, but the deletion process will ensure that no data is lost   
* Two snapshots, the oldest and most recent snapshots   
* The oldest snapshot, as this references data in all other snapshots   

### Question 24:
An application running in an on-premise data center writes data to a MySQL database. A Solutions Architect is re-architecting the application and plans to move the database layer into the AWS cloud on Amazon RDS. The application layer will run in the on-premise data center.

What must be done to connect the application to the RDS database via the Internet? (choose 2)
* Select a public IP within the DB subnet group to assign to the RDS instance   
* Create a DB subnet group that is publicly accessible   
* Choose to make the RDS instance publicly accessible and place it in a public subnet   
* Create a security group allowing access from the on-premise public IP to the RDS instance and assign to the RDS instance   
* Configure a NAT Gateway and attach the RDS database   

### Question 25:
A client has made some updates to their web application. The application uses an Auto Scaling Group to maintain a group of several EC2 instances. The application has been modified and a new AMI must be used for launching any new instances.

What does a Solutions Architect need to do to add the new AMI?
* Modify the existing launch configuration to add the new AMI   
* Suspend Auto Scaling and replace the existing AMI   
* Create a new launch configuration that uses the AMI and update the ASG to use the new launch configuration   
* Create a new target group that uses a new launch configuration with the new AMI   

### Question 26:
A large quantity of data is stored on a NAS device on-premises and accessed using the SMB protocol. The company require a managed service for hosting the filesystem and a tool to automate the migration.

Which actions should a Solutions Architect take?
* Migrate the data to Amazon S3 using and AWS Snowball Edge device
* Migrate the data to Amazon FSx for Windows File Server using AWS DataSync
* Migrate the data to Amazon EFS using the AWS Server Migration Service (SMS)
* Migrate the data to Amazon FSx for Lustre using AWS DataSync

### Question 27:
The database layer of an on-premises web application is being migrated to AWS. The database uses a multi-threaded, in-memory caching layer to improve performance for repeated queries. Which service would be the most suitable replacement for the database cache?
* Amazon RDS MySQL
* Amazon ElastiCache Memcached
* Amazon DynamoDB DAX
* Amazon ElastiCache Redis

### Question 28:
A Solutions Architect is designing a migration strategy for a company moving to the AWS Cloud. The company use a shared Microsoft filesystem that uses Distributed File System Namespaces (DFSN). What will be the MOST suitable migration strategy for the filesystem?
* Use the AWS Server Migration Service to migrate to an Amazon S3 bucket
* Use the AWS Server Migration Service to migrate to Amazon FSx for Lustre
* Use AWS DataSync to migrate to Amazon FSx for Windows File Server
* Use AWS DataSync to migrate to an Amazon EFS filesystem

### Question 29:
There is new requirement for a database that will store a large number of records for an online store. You are evaluating the use of DynamoDB. Which of the following are AWS best practices for DynamoDB? (choose 2)   
* Use large files
* Store objects larger than 400KB in S3 and use pointers in DynamoDB   
* Use for BLOB data use cases   
* Store more frequently and less frequently accessed data in separate tables   
* Use separate local secondary indexes for each item   

### Question 30:
A company has multiple AWS accounts for several environments (Prod, Dev, Test etc.). A Solutions Architect would like to copy an Amazon EBS snapshot from DEV to PROD. The snapshot is from an EBS volume that was encrypted with a custom key.

What steps must be performed to share the encrypted EBS snapshot with the Prod account? (choose 2)
* Create a snapshot of the unencrypted volume and share it with the Prod account   
* Use CloudHSM to distribute the encryption keys use to encrypt the volume   
* Share the custom key used to encrypt the volume   
* Modify the permissions on the encrypted snapshot to share it with the Prod account   
* Make a copy of the EBS volume and unencrypt the data in the process   

### Question 31:
A Solutions Architect has deployed a number of AWS resources using CloudFormation. Some changes must be made to a couple of resources within the stack. Due to recent failed updates, the Solutions Architect is a little concerned about the effects that implementing updates to the resources might have on other resources in the stack.

What is the easiest way to proceed cautiously?
* Deploy a new stack to test the changes   
* Use OpsWorks to manage the configuration changes   
* Create and execute a change set   
* Use a direct update   

### Question 32:
A company runs an API on a Linux server in their on-premises data center. The company are planning to migrate the API to the AWS cloud. The company require a highly available, scalable and cost-effective solution. What should a Solutions Architect recommend?
* Migrate the API server to Amazon EC2 instances in an Auto Scaling group and attach an Application Load Balancer
* Migrate the API to Amazon API Gateway and migrate the backend to Amazon EC2
* Migrate the API to Amazon CloudFront and use AWS Lambda as the origin
* Migrate the API to Amazon API Gateway and use AWS Lambda as the backend

### Question 33:
A company has over 2000 users and is planning to migrate data into the AWS Cloud. Some of the data is user’s home folders on an existing file share and the plan is to move this data to Amazon S3. Each user will have a folder in a shared bucket under the folder structure: bucket/home/%username%.

What steps should a Solutions Architect take to ensure that each user can access their own home folder and no one else’s? (choose 2)
* Create an IAM group and attach the IAM policy   
* Attach an S3 ACL sub-resource that grants access based on the %username% variable   
* Create a bucket policy that applies access permissions based on username   
* Create an IAM policy that applies folder-level permissions   
* Create an IAM policy that applies object-level S3 ACLs   

### Question 34:
The development team in a media organization is moving their SDLC processes into the AWS Cloud. Which AWS service can a Solutions Architect recommend that is primarily used for software version control?
* CodeCommit   
* CloudHSM   
* CodeStar   
* Step Functions   

### Question 35:
A Python application is currently running on Amazon ECS containers using the Fargate launch type. An ALB has been created with a Target Group that routes incoming connections to the ECS-based application. The application will be used by consumers who will authenticate using federated OIDC compliant Identity Providers such as Google and Facebook. The users must be securely authenticated on the front-end before they access the secured portions of the application.

How can this be configured using an ALB?
* This can be done on the ALB by creating an authentication action on a listener rule that configures an Amazon Cognito user pool with the social IdP   
* This cannot be done on an ALB; you’ll need to use another layer in front of the ALB   
* This cannot be done on an ALB; you’ll need to authenticate users on the back-end with AWS Single Sign-On (SSO) integration   
* The only option is to use SAML with Amazon Cognito on the ALB   

### Question 36:
An Amazon VPC contains a mixture of Amazon EC2 instances in production and non-production environments. A Solutions Architect needs to devise a way to segregate access permissions to different sets of users for instances in different environments.

How can this be achieved? (choose 2)
* Add a specific tag to the instances you want to grant the users or groups access to   
* Add an environment variable to the instances using user data   
* Attach an Identity Provider (IdP) and delegate access to the instances to the relevant groups
* Create an IAM policy with a conditional statement that matches the environment variables   
* Create an IAM policy that grants access to any instances with the specific tag   

### Question 37:
A Solutions Architect has deployed an API using Amazon API Gateway and created usage plans and API keys for several customers. Requests from one particular customer have been excessive and the solutions architect needs to limit the rate of requests. Other customers should not be affected. How should the solutions architect proceed?
* Configure a server-side throttling limit
* Configure the per-method throttling limits
* Configure per-client throttling limits
* Configure the account-level throttling limits

### Question 38:
A Solutions Architect is conducting an audit and needs to query several properties of EC2 instances in a VPC. What two methods are available for accessing and querying the properties of an EC2 instance such as instance ID, public keys and network interfaces? (choose 2)   
* Use the Batch command   
* Download and run the Instance Metadata Query Tool   
* Run the command “curl http://169.254.169.254/latest/meta-data/”   
* Use the EC2 Config service   
* Run the command “curl http://169.254.169.254/latest/dynamic/instance-identity/”   

### Question 39:
An application you manage runs a number of components using a micro-services architecture. Several ECS container instances in your ECS cluster are displaying as disconnected. The ECS instances were created from the Amazon ECS-Optimized AMI. What steps might you take to troubleshoot the issue? (choose 2)   
* Verify that the IAM instance profile has the necessary permissions   
* Verify that the instances have the correct IAM group applied   
* Verify that the container instances have the container agent installed   
* Verify that the container instances are using the Fargate launch type   
* Verify that the container agent is running on the container instances   

### Question 40:
An application running a private subnet of an Amazon VPC must have outbound internet access for downloading updates. The Solutions Architect does not want the application exposed to inbound connection attempts. Which steps should be taken?
* Create a NAT gateway and attach an internet gateway to the VPC
* Create a NAT gateway but do not create attach an internet gateway to the VPC
* Attach an internet gateway to the VPC but do not create a NAT gateway
* Attach an internet gateway to the private subnet and create a NAT gateway

### Question 41:
A Solutions Architect just completed the implementation of a 2-tier web application for a client. The application uses Amazon EC2 instances, Amazon ELB and Auto Scaling across two subnets. After deployment the Solutions Architect noticed that only one subnet has EC2 instances running in it. What might be the cause of this situation?
* The ELB is configured as an internal-only load balancer   
* The Auto Scaling Group has not been configured with multiple subnets   
* The AMI is missing from the ASG’s launch configuration   
* Cross-zone load balancing is not enabled on the ELB   

### Question 42:
A Solutions Architect needs to create a file system that can be concurrently accessed by multiple Amazon EC2 instances across multiple availability zones. The file system needs to support high throughput and the ability to burst. As the data that will be stored on the file system will be sensitive, it must be encrypted at rest and in transit.

Which storage solution should the Solutions Architect use for the shared file system?
* Use the Elastic Block Store (EBS) and mount the file system at the block level   
* Add EBS volumes to each EC2 instance and use an ELB to distribute data evenly between the volumes   
* Add EBS volumes to each EC2 instance and configure data replication   
* Use the Elastic File System (EFS) and mount the file system using NFS

### Question 43:
The application development team in a company have created a new application written in .NET. A Solutions Architect is looking for a way to easily deploy the application whilst maintaining full control of the underlying resources.

Which PaaS service provided by AWS would BEST suit this requirement?
* Elastic Beanstalk   
* CloudFront    
* EC2 Placement Groups   
* CloudFormation   

### Question 44:
A client has requested a design for a fault tolerant database that can failover between AZs. You have decided to use RDS in a multi-AZ configuration. What type of replication will the primary database use to replicate to the standby instance?   
* Asynchronous replication   
* Continuous replication   
* Scheduled replication   
* Synchronous replication   

### Question 45:
A Solutions Architect is designing an application for processing and extracting data from log files. The log files are generated by an application and the number and frequency of updates varies. The files are up to 1 GB in size and processing will take around 40 seconds for each file.

Which solution is the most cost-effective?
* Write the log files to an Amazon S3 bucket. Create an event notification to invoke an AWS Lambda function that will process the files
* Write the log files to an Amazon S3 bucket. Create an event notification to invoke an Amazon ECS task to process the files and save to an Amazon S3 bucket
* Write the log files to an Amazon EC2 instance with an attached EBS volume. After processing, save the files to an Amazon S3 bucket
* Write the log files to an Amazon SQS queue. Use AWS Lambda to process the files from the queue and save to an Amazon S3 bucket

### Question 46:
A Solutions Architect manages multiple Amazon RDS MySQL databases. To improve security, the Solutions Architect wants to enable secure user access with short-lived credentials. How can these requirements be met?
* Configure the MySQL databases to use AWS KMS data encryption keys
* Configure the MySQL databases to use the AWS Security Token Service (STS)
* Configure the application to use the AUTH command to send a unique password
* Create the MySQL user accounts to use the AWSAuthenticationPlugin with IAM

### Question 47:
A Solutions Architect is designing the messaging and streaming layers of a serverless application. The messaging layer will manage communications between components and the streaming layer will manage real-time analysis and processing of streaming data.

The Architect needs to select the most appropriate AWS services for these functions. Which services should be used for the messaging and streaming layers? (choose 2)
* Use Amazon EMR for collecting, processing and analyzing real-time streaming data   
* Use AWS CloudTrail for collecting, processing and analyzing real-time streaming data   
* Use Amazon SWF for providing a fully managed messaging service   
* Use Amazon Kinesis for collecting, processing and analyzing real-time streaming data
* Use Amazon SNS for providing a fully managed messaging service   

### Question 48:
A customer runs an application on-premise that stores large media files. The data is mounted to different servers using either the SMB or NFS protocols. The customer is having issues with scaling the storage infrastructure on-premise and is looking for a way to offload the data set into the cloud whilst retaining a local cache for frequently accessed content.

Which of the following is the best solution?
* Create a script that migrates infrequently used data to S3 using multi-part upload   
* Use the AWS Storage Gateway File Gateway   
* Establish a VPN and use the Elastic File System (EFS)   
* Use the AWS Storage Gateway Volume Gateway in cached volume mode   

### Question 49:
A Solutions Architect is creating a multi-tier application that includes loosely-coupled, distributed application components and needs to determine a method of sending notifications instantaneously. Using Amazon SNS which transport protocols are supported? (choose 2)
* HTTPS
* SWF
* Lambda
* FTP
* Email-JSON

### Question 50:
An application is running on EC2 instances in a private subnet of an Amazon VPC. A Solutions Architect would like to connect the application to Amazon API Gateway. For security reasons, it is necessary to ensure that no traffic traverses the Internet and to ensure all traffic uses private IP addresses only.

How can this be achieved?
* Create a NAT gateway   
* Add the API gateway to the subnet the EC2 instances are located in   
* Create a private API using an interface VPC endpoint   
* Create a public VIF on a Direct Connect connection   

### Question 51:
A company has deployed an API using Amazon API Gateway. There are many repeat requests and a solutions architect has been asked to implement measures to reduce request latency and the number of calls to the Amazon EC2 endpoint.

How can this be most easily achieved?
* Create a cache for a stage and configure a TTL
* Configure an edge-optimized endpoint with CloudFront
* Create a cache for a method and configure a TTL
* Configure a private endpoint place ElastiCache in front

### Question 52:
An organization is planning their disaster recovery solution. They plan to run a scaled down version of a fully functional environment. In a DR situation the recovery time must be minimized.

Which DR strategy should a Solutions Architect recommend?
* Multi-site
* Warm standby
* Pilot light
* Backup and restore

### Question 53:
A large multinational retail company has a presence in AWS in multiple regions. The company has established a new office and needs to implement a high-bandwidth, low-latency connection to multiple VPCs in multiple regions within the same account. The VPCs each have unique CIDR ranges.

What would be the optimum solution design using AWS technology? (choose 2)
* Provision an MPLS network   
* Implement Direct Connect connections to each AWS region   
* Implement a Direct Connect connection to the closest AWS region   
* Create a Direct Connect gateway, and create private VIFs to each region   
* Configure AWS VPN CloudHub   

### Question 54:
A Solutions Architect created a new subnet in an Amazon VPC and launched an Amazon EC2 instance into it. The Solutions Architect needs to directly access the EC2 instance from the Internet and cannot connect. Which steps should be undertaken to troubleshoot the issue? (choose 2)
* Check that you can ping the instance from another subnet   
* Check that there is a NAT Gateway configured for the subnet   
* Check that the instance has a public IP address   
* Check that Security Group has a rule for outbound traffic
* Check that the route table associated with the subnet has an entry for an Internet Gateway   

### Question 55:
A company has an eCommerce application that runs from multiple AWS Regions. Each region has a separate database running on Amazon EC2 instances. The company plans to consolidate the data to a columnar database and run analytics queries. Which approach should the company take?
* Use the COPY command to load data into an Amazon RedShift data warehouse and run the analytics queries there
* Launch Amazon Kinesis Data Streams producers to load data into a Kinesis Data stream. Use Kinesis Data Analytics to analyze the data
* Run an AWS Batch job to copy and process the data into a columnar Amazon RDS database. Use Amazon Athena to analyze the data
* Create an AWS Lambda function that copies the data onto Amazon S3. Use Amazon S3 Select to query the data

### Question 56:
A Solutions Architect needs a storage solution for a fleet of Linux web application servers. The solution should provide a file system interface and be able to support millions of files. Which AWS service should the Architect choose?
* Amazon EBS
* Amazon ElastiCache
* Amazon S3
* Amazon EFS

### Question 57:
An application stack is being created which needs a message bus to decouple the application components from each other. The application will generate up to 300 messages per second without using batching. A Solutions Architect needs to ensure that a message is delivered only once and duplicates are not introduced into the queue. It is not necessary to maintain the order of the messages.

Which SQS queue type should be used?
* Standard queues   
* Long polling queues   
* Auto Scaling queues   
* FIFO queues   

### Question 58:
An Amazon EC2 instance running a video on demand web application has been experiencing high CPU utilization. A Solutions Architect needs to take steps to reduce the impact on the EC2 instance and improve performance for consumers. Which of the steps below would help?
* Create a CloudFront RTMP distribution and point it at the EC2 instance   
* Use ElastiCache as the web front-end and forward connections to EC2 for cache misses   
* Create an ELB and place it in front of the EC2 instance   
* Create a CloudFront distribution and configure a custom origin pointing at the EC2 instance   

### Question 59:
A Solutions Architect must enable an application to download software updates from the internet. The application runs on a series of EC2 instances in an Auto Scaling group running in a private subnet. The solution must involve minimal ongoing systems management effort. How should the Solutions Architect proceed?
* Attach Elastic IP addresses
* Create a Virtual Private Gateway
* Implement a NAT gateway
* Launch a NAT instance

### Question 60:
A Solutions Architect is building a small web application running on Amazon EC2 that will be serving static content. The user base is spread out globally and speed is important. Which AWS service can deliver the best user experience cost-effectively and reduce the load on the web server?
* Amazon EBS volume   
* Amazon CloudFront   
* Amazon S3   
* Amazon RedShift   

### Question 61:
A company has several AWS accounts each with multiple Amazon VPCs. The company must establish routing between all private subnets. The architecture should be simple and allow transitive routing to occur.

How should the network connectivity be configured?
* Create a hub-and-spoke topology with AWS App Mesh and use AWS Resource Access Manager to share route tables
* Create a transitive VPC peering connection between each Amazon VPC and configure route tables
* Create an AWS Managed VPN between each Amazon VPC and configure route tables
* Create an AWS Transit Gateway and share it with each account using AWS Resource Access Manager

### Question 62:
A Solutions Architect needs to migrate an Oracle database running on RDS onto Amazon RedShift to improve performance and reduce cost. Which combination of tasks using AWS services should be used to execute the migration? (choose 2)   
* Migrate the database using the AWS Database Migration Service (DMS)
* Configure API Gateway to extract, transform and load the data into RedShift   
* Enable log shipping from the Oracle database to RedShift   
* Convert the schema using the AWS Schema Conversion Tool   
* Take a snapshot of the Oracle database and restore the snapshot onto RedShift   

### Question 63:
A Solutions Architect is writing some code that uses an AWS Lambda function and would like to enable the function to connect to an Amazon ElastiCache cluster within an Amazon VPC in the same AWS account. What VPC-specific information must be included in the function to enable this configuration? (choose 2)
* VPC Security Group IDs   
* VPC Subnet IDs   
* VPC Route Table IDs   
* VPC Logical IDs   
* VPC Peering IDs

### Question 64:
An application has been migrated from on-premises to an Amazon EC2 instance. The migration has failed due to an unknown dependency that the application must communicate with an on-premises server using private IP addresses.

Which action should a solutions architect take to quickly provision the necessary connectivity?
* Configure a Virtual Private Gateway
* Setup an AWS Direct Connect connection
* Create an Amazon CloudFront distribution
* Create an AWS Transit Gateway

### Question 65:
A three-tier web application that is deployed in an Amazon VPC has been experiencing heavy load on the database layer. The database layer uses an Amazon RDS MySQL instance in a multi-AZ configuration. Customers have been complaining about poor response times. During troubleshooting it has been noted that the database layer is experiencing high read contention during peak hours of the day.

What are two possible options that could be used to offload some of the read traffic from the database to resolve the performance issues? (choose 2)
* Use an ELB to distribute load between RDS instances   
* Migrate to DynamoDB   
* Add RDS read replicas in each AZ   
* Use a larger RDS instance size   
* Deploy ElastiCache in each AZ   

# Exam 6

### Question 1:
A customer is deploying services in a hybrid cloud model. The customer has mandated that data is transferred directly between cloud data centers, bypassing ISPs.

Which AWS service can be used to enable hybrid cloud connectivity?
* Amazon Route 53   
* AWS Direct Connect   
* Amazon VPC   
* IPSec VPN   

### Question 2:
A distribution method is required for some static files. The requests will mainly be GET requests and a high volume of GETs is expected, often exceeding 2000 per second. The files are currently stored in an S3 bucket. According to AWS best practices, how can performance be optimized?
* Integrate CloudFront with S3 to cache the content   
* Use ElastiCache to cache the content   
* Use S3 Transfer Acceleration   
* Use cross-region replication to spread the load across regions   

### Question 3:
An Amazon EC2 instance is generating very high packets-per-second and performance of the application stack is being impacted. A Solutions Architect needs to determine a resolution to the issue that results in improved performance.

Which action should the Architect take?
* Configure a RAID 1 array from multiple EBS volumes   
* Add multiple Elastic IP addresses to the instance   
* Use enhanced networking   
* Create a placement group and put the EC2 instance in it   

### Question 4:
A large multi-national client has requested a design for a multi-region database. The master database will be in the EU (Frankfurt) region and databases will be located in 4 other regions to service local read traffic. The database should be a managed service including the replication.

The solution should be cost-effective and secure. Which AWS service can deliver these requirements?
* ElastiCache with Redis and clustering mode enabled
* RDS with Multi-AZ   
* RDS with cross-region Read Replicas   
* EC2 instances with EBS replication   

### Question 5:
A government agency is using CloudFront for a web application that receives personally identifiable information (PII) from citizens.

What feature of CloudFront applies an extra level of encryption at CloudFront edge locations to ensure the PII data is secured end-to-end?   
* Origin access identity   
* Field-level encryption   
* Object invalidation   
* RTMP distribution   

### Question 6:
A Solutions Architect needs to capture information about the traffic that reaches an Amazon Elastic Load Balancer. The information should include the source, destination, and protocol.

What is the most secure and reliable method for gathering this data?
* Use Amazon CloudWatch Logs to review detailed logging information
* Enable Amazon CloudTrail logging and configure packet capturing
* Create a VPC flow log for the subnets in which the ELB is running
* Create a VPC flow log for each network interface associated with the ELB

### Question 7:
An Auto Scaling group of Amazon EC2 instances behind an Elastic Load Balancer (ELB) is running in an Amazon VPC. Health checks are configured on the ASG to use EC2 status checks. The ELB has determined that an EC2 instance is unhealthy and has removed it from service. A Solutions Architect noticed that the instance is still running and has not been terminated by EC2 Auto Scaling.

What would be an explanation for this behavior?
* Connection draining is enabled and the ASG is waiting for in-flight requests to complete   
* The ASG is waiting for the cooldown timer to expire before terminating the instance   
* The ELB health check type has not been selected for the ASG and so it is unaware that the instance has been determined to be unhealthy by the ELB and has been removed from service   
* The health check grace period has not yet expired   

### Question 8:
A company needs to capture detailed information about all HTTP requests that are processed by their Internet facing Application Load Balancer (ALB). The company requires information on the requester, IP address, and request type for analyzing traffic patterns to better understand their customer base.

Which actions should a Solutions Architect recommend?
* Enable Access Logs and store the data on S3   
* Enable EC2 detailed monitoring   
* Use CloudTrail to capture all API calls made to the ALB   
* Configure metrics in CloudWatch for the ALB   

### Question 9:
An application uses a MySQL database running on an Amazon EC2 instance. The application generates high I/O and constant writes to a single table on the database. Which Amazon EBS volume type will provide the MOST consistent performance and low latency?
* Throughput Optimized HDD (st1)
* General Purpose SSD (gp2)
* Provisioned IOPS SSD (io1)
* Cold HDD (sc1)

### Question 10:
A Solutions Architect needs to run a PowerShell script on a fleet of Amazon EC2 instances running Microsoft Windows. The instances have already been launched in an Amazon VPC. What tool can be run from the AWS Management Console that to execute the script on all target EC2 instances?
* Run Command   
* AWS OpsWorks   
* AWS CodeDeploy   
* AWS Config   

### Question 11:
The load on a MySQL database running on Amazon EC2 is increasing and performance has been impacted. Which of the options below would help to increase storage performance? (choose 2)
* Create a RAID 1 array from multiple EBS volumes   
* Use a larger instance size within the instance family   
* Use EBS optimized instances   
* Use Provisioned IOPS (I01) EBS volumes   
* Use HDD, Cold (SC1) EBS volumes   

### Question 12:
A financial services company regularly runs an analysis of the day’s transaction costs, execution reporting, and market performance. The company currently uses third-party commercial software for provisioning, managing, monitoring, and scaling the computing jobs which utilize a large fleet of EC2 instances.

The company is seeking to reduce costs and utilize AWS services. Which AWS service could be used in place of the third-party software?
* AWS Batch   
* AWS Systems Manager   
* Amazon Athena   
* Amazon Lex   

### Question 13:
A company has a fleet of Amazon EC2 instances behind an Elastic Load Balancer (ELB) that are a mixture of c4.2xlarge instance types and c5.large instances. The load on the CPUs on the c5.large instances has been very high, often hitting 100% utilization, whereas the c4.2xlarge instances have been performing well.

What should a Solutions Architect recommend to resolve the performance issues?
* Enable the weighted routing policy on the ELB and configure a higher weighting for the c4.2xlarge instances   
* Change the configuration to use only c4.2xlarge instance types   
* Add more c5.large instances to spread the load more evenly   
* Add all of the instances into a Placement Group   

### Question 14:
An Amazon Elastic File System (EFS) has been created to store data that will be accessed by a large number of Amazon EC2 instances. The data is sensitive and a Solutions Architect is creating a design for security measures to protect the data. It is required that network traffic is restricted correctly based on firewall rules and access from hosts is restricted by user or group.

How can this be achieved with Amazon EFS? (choose 2)
* Use POSIX permissions to control access from hosts by user or group   
* Use AWS Web Application Firewall (WAF) to protect EFS   
* Use Network ACLs to control the traffic   
* Use IAM groups to control access by user or group   
* Use EFS Security Groups to control network traffic   

### Question 15:
A Solutions Architect has created a new security group in an Amazon VPC. No rules have been created. Which of the statements below are correct regarding the default state of the security group? (choose 2)
* There is an outbound rule allowing traffic to the Internet Gateway   
* There are no inbound rules and traffic will be implicitly denied   
* There is an inbound rule allowing traffic from the Internet to port 22 for management   
* There are is an inbound rule that allows traffic from the Internet Gateway   
* There is an outbound rule that allows all traffic to all IP addresses   

### Question 16:
A Solutions Architect is designing the system monitoring and deployment layers of a serverless application. The system monitoring layer will manage system visibility through recording logs and metrics and the deployment layer will deploy the application stack and manage workload changes through a release management process.

 The Architect needs to select the most appropriate AWS services for these functions. Which services and frameworks should be used for the system monitoring and deployment layers? (choose 2)
* Use AWS Lambda to package, test, and deploy the serverless application stack   
* Use AWS SAM to package, test, and deploy the serverless application stack   
* Use AWS X-Ray to package, test, and deploy the serverless application stack   
* Use Amazon CloudWatch for consolidating system and application logs and monitoring custom metrics   
* Use AWS CloudTrail for consolidating system and application logs and monitoring custom metrics   

### Question 17:
A Solutions Architect has logged into an Amazon EC2 Linux instance using SSH and needs to determine a few pieces of information including what IAM role is assigned, the instance ID and the names of the security groups that are assigned to the instance.

From the options below, what would be the best source of this information?
* Metadata   
* Tags   
* User data   
* Parameters   

### Question 18:
A company is deploying a new two-tier web application that uses EC2 web servers and a DynamoDB database backend. An Internet facing ELB distributes connections between the web servers.

The Solutions Architect has created a security group for the web servers and needs to create a security group for the ELB. What rules should be added? (choose 2)
* Add an Outbound rule that allows HTTP/HTTPS, and specify the destination as the web server security group     
* Add an Inbound rule that allows HTTP/HTTPS, and specify the source as 0.0.0.0/0   
* Add an Outbound rule that allows ALL TCP, and specify the destination as the Internet Gateway   
* Add an Inbound rule that allows HTTP/HTTPS, and specify the source as 0.0.0.0/32   
* Add an Outbound rule that allows HTTP/HTTPS, and specify the destination as VPC CIDR   

### Question 19:
A Solutions Architect is deploying a production application that will use several Amazon EC2 instances and run constantly on an ongoing basis. The application cannot be interrupted or restarted. Which EC2 pricing model would be best for this workload?
* Reserved instances   
* On-demand instances   
* Flexible instances   
* Spot instances   

### Question 20:
A company is investigating ways to analyze and process large amounts of data in the cloud faster, without needing to load or transform the data in a data warehouse. The data resides in Amazon S3.

Which AWS services would allow the company to query the data in place? (choose 2)
* Amazon Elasticsearch   
* Amazon SWF   
* Amazon RedShift Spectrum   
* Amazon Kinesis Data Streams   
* Amazon S3 Select   

### Question 21:
A tool needs to analyze data stored in an Amazon S3 bucket. Processing the data takes a few seconds and results are then written to another S3 bucket. Less than 256 MB of memory is needed to run the process. What would be the MOST cost-effective compute solutions for this use case?
* Amazon Elastic Beanstalk
* AWS Fargate tasks
* Amazon EC2 spot instances
* AWS Lambda functions

### Question 22:
An application uses an Amazon RDS database and Amazon EC2 instances in a web tier. The web tier instances must not be directly accessible from the internet to improve security.

How can a Solutions Architect meet these requirements?
* Launch the EC2 instances in a private subnet with a NAT gateway and update the route table
* Launch the EC2 instances in a public subnet and use AWS WAF to protect the instances from internet-based attacks
* Launch the EC2 instances in a private subnet and create an Application Load Balancer in a public subnet
* Launch the EC2 instances in a public subnet and create an Application Load Balancer in a public subnet

### Question 23:
A web application receives order processing information from customers and places the messages on an Amazon SQS queue. A fleet of Amazon EC2 instances are configured to pick up the messages, process them, and store the results in a DynamoDB table. The current configuration has been resulting in a large number of empty responses to ReceiveMessage API requests.

A Solutions Architect needs to eliminate empty responses to reduce operational overhead. How can this be done? 
* Configure Long Polling to eliminate empty responses by allowing Amazon SQS to wait until a message is available in a queue before sending a response   
* Use a Standard queue to provide at-least-once delivery, which means that each message is delivered at least once   
* Configure Short Polling to eliminate empty responses by reducing the length of time a connection request remains open   
* Use a FIFO (first-in-first-out) queue to preserve the exact order in which messages are sent and received   

### Question 24:
A legacy application is being migrated into AWS. The application has a large amount of data that is rarely accessed. When files are accessed they are retrieved sequentially. The application will be migrated onto an Amazon EC2 instance.

What is the LEAST expensive EBS volume type for this use case?
* General Purpose SSD (gp2)
* Provisioned IOPS SSD (io1)
* Throughput Optimized HDD (st1)
* Cold HDD (sc1)

### Question 25:
An application receives a high traffic load between 7:30am and 9:30am daily. The application uses an Auto Scaling group to maintain three instances most of the time but during the peak period it requires six instances.

How can a Solutions Architect configure Auto Scaling to perform a daily scale-out event at 7:30am and a scale-in event at 9:30am to account for the peak load?
* Use a Simple scaling policy   
* Use a Step scaling policy   
* Use a Scheduled scaling policy   
* Use a Dynamic scaling policy   

### Question 26:
A fleet of Amazon EC2 instances running Linux will be launched in an Amazon VPC. An application development framework and some custom software must be installed on the instances. The installation will be initiated using some scripts. What feature enables a Solutions Architect to specify the scripts the software can be installed during the EC2 instance launch?
* User data
* AWS Config
* Metadata   
* Run command

### Question 27:
A Solutions Architect has created a VPC and is in the process of formulating the subnet design. The VPC will be used to host a two-tier application that will include Internet facing web servers, and internal-only DB servers. Zonal redundancy is required.

How many subnets are required to support this requirement?
* 2 subnets
* 4 subnets
* 6 subnets
* 1 subnet

### Question 28:
A web application runs on a series of Amazon EC2 instances behind an Application Load Balancer (ALB). A Solutions Architect is updating the configuration with a health check and needs to select the protocol to use. What options are available? (choose 2)
* SSL
* ICMP
* HTTPS
* TCP
* HTTP

### Question 29:
A Solutions Architect has created a new Network ACL in an Amazon VPC. No rules have been created. Which of the statements below are correct regarding the default state of the Network ACL? (choose 2)
* There is a default inbound rule allowing traffic from the VPC CIDR block   
* There is a default inbound rule denying all traffic   
* There is a default outbound rule allowing all traffic   
* There is a default outbound rule allowing traffic to the Internet Gateway   
* There is a default outbound rule denying all traffic   

### Question 30:
A Solutions Architect has created an AWS account and selected the Asia Pacific (Sydney) region. Within the default VPC there is a default security group. What settings are configured within this security group by default? (choose 2)
* There is an outbound rule that allows all traffic to all addresses   
* There is an outbound rule that allows traffic to the VPC router   
* There is an inbound rule that allows all traffic from any address   
* There is an inbound rule that allows all traffic from the security group itself   
* There is an outbound rule that allows all traffic to the security group itself   

### Question 31:
An Amazon EC2 instance has been launched into an Amazon VPC. A Solutions Architect needs to ensure that instances have both a private and public DNS hostnames. Assuming settings were not changed during creation of the VPC, how will DNS hostnames be assigned by default? (choose 2)
* In a default VPC instances will be assigned a public and private DNS hostname   
* In all VPCs instances no DNS hostnames will be assigned   
* In a non-default VPC instances will be assigned a public and private DNS hostname   
* In a default VPC instances will be assigned a private but not a public DNS hostname   
* In a non-default VPC instances will be assigned a private but not a public DNS hostname   

### Question 32:
A company is transitioning their web presence into the AWS cloud. As part of the migration the company will be running a web application both on-premises and in AWS for a period of time. During the period of co-existence the client would like 80% of the traffic to hit the AWS-based web servers and 20% to be directed to the on-premises web servers.

What method can a Solutions Architect use to distribute traffic as requested?
* Use Route 53 with a simple routing policy   
* Use an Application Load Balancer to distribute traffic based on IP address   
* Use Route 53 with a weighted routing policy and configure the respective weights   
* Use a Network Load Balancer to distribute traffic based on Instance ID   

### Question 33:
An Amazon EC2 instance behind an Elastic Load Balancer (ELB) is in the process of being de-registered. Which ELB feature is used to allow existing connections to close cleanly?
* Proxy Protocol   
* Connection Draining   
* Deletion Protection   
* Sticky Sessions   

### Question 34:
Several Amazon EC2 Spot instances are being used to process messages from an Amazon SQS queue and store results in an Amazon DynamoDB table. Shortly after picking up a message from the queue AWS terminated the Spot instance. The Spot instance had not finished processing the message. What will happen to the message?
* The message will remain in the queue and be immediately picked up by another instance   
* The results may be duplicated in DynamoDB as the message will likely be processed multiple times   
* The message will be lost as it would have been deleted from the queue when processed   
* The message will become available for processing again after the visibility timeout expires   

### Question 35:
A Solutions Architect is designing the disk configuration for an Amazon EC2 instance. The instance needs to support a MapReduce process that requires high throughput for a large dataset with large I/O sizes.

Which Amazon EBS volume is the MOST cost-effective solution for these requirements?
* EBS Throughput Optimized HDD   
* EBS General Purpose SSD   
* EBS Provisioned IOPS SSD   
* EBS General Purpose SSD in a RAID 1 configuration   

### Question 36:
The Solutions Architect in charge of a critical application must ensure the Amazon EC2 instances are able to be launched in another AWS Region in the event of a disaster.

What steps should the Solutions Architect take? (Select TWO.)
* Copy the snapshots using Amazon S3 cross-region replication
* Enable cross-region snapshots for the Amazon EC2 instances
* Create AMIs of the instances and copy them to another Region
* Launch instances in the second Region from the AMIs
* Launch instances in the second Region using the S3 API

### Question 37:
An Amazon EBS-backed EC2 instance has been launched. A requirement has come up for some high-performance ephemeral storage.

How can a Solutions Architect add a new instance store volume?
* You can use a block device mapping to specify additional instance store volumes when you launch your instance, or you can attach additional instance store volumes after your instance is running   
* You can specify the instance store volumes for your instance only when you launch an instance   
* You must use an Elastic Network Adapter (ENA) to add instance store volumes. First, attach an ENA, and then attach the instance store volume   
* You must shutdown the instance in order to be able to add the instance store volume   

### Question 38:
A security officer has requested that all data associated with a specific customer is encrypted. The data resides on Elastic Block Store (EBS) volumes. Which of the following statements about using EBS encryption are correct? (choose 2)     
* All instance types support encryption   
* Data in transit between an instance and an encrypted volume is also encrypted   
* There is no direct way to change the encryption state of a volume   
* All attached EBS volumes must share the same encryption state   
* Not all EBS types support encryption   

### Question 39:
The application development team in a company have developed a Java application and saved the source code in a .war file. They would like to run the application on AWS resources and are looking for a service that can handle the provisioning and management of the underlying resources it will run on.

Which AWS service should a Solutions Architect recommend the Developers use to upload the Java source code file?
* AWS CloudFormation   
* AWS CodeDeploy   
* AWS Elastic Beanstalk   
* AWS OpsWorks   

### Question 40:
A Solutions Architect created a new IAM user account for a temporary employee who recently joined the company. The user does not have permissions to perform any actions, which statement is true about newly created users in IAM?
* They are created with user privileges   
* They are created with full permissions   
* They are created with no permissions   
* They are created with limited permissions   

### Question 41:
A Solutions Architect needs to upload a large (2GB) file to an S3 bucket. What is the recommended way to upload a single large file to an S3 bucket?
* Use AWS Import/Export   
* Use Multipart Upload   
* Use a single PUT request to upload the large file   
* Use Amazon Snowball   

### Question 42:
An Amazon DynamoDB table has a variable load, ranging from sustained heavy usage some days, to only having small spikes on others. The load is 80% read and 20% write. The provisioned throughput capacity has been configured to account for the heavy load to ensure throttling does not occur.

What would be the most efficient solution to optimize cost?
* Create a DynamoDB Auto Scaling scaling policy   
* Create a CloudWatch alarm that notifies you of increased/decreased load, and manually adjust the provisioned throughput   
* Use DynamoDB DAX to increase the performance of the database   
* Create a CloudWatch alarm that triggers an AWS Lambda function that adjusts the provisioned throughput   

### Question 43:
A Solutions Architect enabled Access Logs on an Application Load Balancer (ALB) and needs to process the log files using a hosted Hadoop service. What configuration changes and services can be leveraged to deliver this requirement?
* Configure Access Logs to be delivered to EC2 and install Hadoop for processing the log files   
* Configure Access Logs to be delivered to S3 and use Kinesis for processing the log files   
* Configure Access Logs to be delivered to DynamoDB and use EMR for processing the log files   
* Configure Access Logs to be delivered to S3 and use EMR for processing the log files   

### Question 44:
A company has multiple Amazon VPCs that are peered with each other. The company would like to use a single Elastic Load Balancer (ELB) to route traffic to multiple EC2 instances in peered VPCs within the same region. How can this be achieved?
* This is not possible, the instances that an ELB routes traffic to must be in the same VPC   
* This is possible using the Classic Load Balancer (CLB) if using Instance IDs   
* This is possible using the Network Load Balancer (NLB) and Application Load Balancer (ALB) if using IP addresses as targets   
* This is not possible with ELB, you would need to use Route 53   

### Question 45:
A large quantity of data that is rarely accessed is being archived onto Amazon Glacier. Your CIO wants to understand the resilience of the service. Which of the statements below is correct about Amazon Glacier storage?  (choose 2) 
* Provides 99.9% availability of archives   
* Provides 99.999999999% durability of archives   
* Data is resilient in the event of one entire Availability Zone destruction   
* Data is resilient in the event of one entire region destruction   
* Data is replicated globally   

### Question 46:
An on-premise data center will be connected to an Amazon VPC by a hardware VPN that has public and VPN-only subnets. The security team has requested that traffic hitting public subnets on AWS that’s destined to on-premise applications must be directed over the VPN to the corporate firewall.

How can this be achieved?
* In the VPN-only subnet route table, add a route that directs all Internet traffic to the virtual private gateway   
* Configure a NAT Gateway and configure all traffic to be directed via the virtual private gateway   
* In the public subnet route table, add a route for your remote network and specify the virtual private gateway as the target   
* In the public subnet route table, add a route for your remote network and specify the customer gateway as the target

### Question 47:
One of the departments in a company has been generating a large amount of data on Amazon S3 and costs are increasing. Data older than 90 days is rarely accessed but must be retained for several years. If this data does need to be accessed at least 24 hours notice is provided.

How can a Solutions Architect optimize the costs associated with storage of this data whilst ensuring it is accessible if required?
* Use S3 lifecycle policies to move data to the STANDARD_IA storage class   
* Implement archival software that automatically moves the data to tape   
* Select the older data and manually migrate it to GLACIER   
* Use S3 lifecycle policies to move data to GLACIER after 90 days   

### Question 48:
The database layer of an on-premises web application is being migrated to AWS. The database currently uses an in-memory cache. A Solutions Architect must deliver a solution that supports high availability and replication for the caching layer.

Which service should the Solutions Architect recommend?
* Amazon RDS Multi-AZ
* Amazon DynamoDB
* Amazon ElastiCache Memcached
* Amazon ElastiCache Redis

### Question 49:
An organization in the agriculture sector is deploying sensors and smart devices around factory plants and fields. The devices will collect information and send it to cloud applications running on AWS.

Which AWS service will securely connect the devices to the cloud applications?
* AWS Glue   
* AWS IoT Core   
* AWS DMS   
* AWS Lambda   

### Question 50:
An on-premises server runs a MySQL database and will be migrated to the AWS Cloud. The company require a managed solution that supports high availability and automatic failover in the event of the outage of an Availability Zone (AZ).

Which solution is the BEST fit for these requirements?
* Use the AWS Database Migration Service (DMS) to directly migrate the database to an Amazon RDS MySQL Multi-AZ deployment
* Use the AWS Database Migration Service (DMS) to directly migrate the database to an Amazon EC2 MySQL Multi-AZ deployment
* Create a snapshot of the MySQL database server and use AWS DataSync to migrate the data Amazon S3. Launch a new Amazon RDS MySQL Multi-AZ deployment from the snapshot
* Use the AWS Database Migration Service (DMS) to directly migrate the database to Amazon RDS MySQL. Use the Schema Conversion Tool (SCT) to enable conversion from MySQL to Amazon RDS

### Question 51:
A Solutions Architect has created an AWS Organization with several AWS accounts. Security policy requires that use of specific API actions are limited across all accounts. The Solutions Architect requires a method of centrally controlling these actions.

What is the SIMPLEST method of achieving the requirements?
* Create an IAM policy in the root account and attach it to users and groups in each account
* Create cross-account roles in each account to limit access to the services and actions that are allowed
* Create a service control policy in the root organizational unit to deny access to the services or actions
* Create a Network ACL that limits access to the services or actions and attach it to all relevant subnets

### Question 52:
A company runs an application on premises that stores a large quantity of semi-structured data using key-value pairs. The application code will be migrated to AWS Lambda and a highly scalable solution is required for storing the data.

Which datastore will be the best fit for these requirements?
* Amazon EBS
* Amazon RDS MySQL
* Amazon DynamoDB
* Amazon EFS

### Question 53:
A company needs to ensure that they can failover between AWS Regions in the event of a disaster seamlessly with minimal downtime and data loss. The applications will run in an active-active configuration.

Which DR strategy should a Solutions Architect recommend?
* Pilot light
* Warm standby
* Multi-site
* Backup and restore

### Question 54:
Three AWS accounts are owned by the same company but in different regions. Account Z has two AWS Direct Connect connections to two separate company offices. Accounts A and B require the ability to route across account Z’s Direct Connect connections to each company office. A Solutions Architect has created an AWS Direct Connect gateway in account Z.

How can the required connectivity be configured?
* Create a VPC Endpoint to the Direct Connect gateway in account A and B
* Create a PrivateLink connection in Account Z and ENIs in accounts A and B
* Associate the Direct Connect gateway to a transit gateway in each region
* Associate the Direct Connect gateway to a virtual private gateway in account A and B

### Question 55:
A company has launched a multi-tier application architecture. The web tier and database tier run on Amazon EC2 instances in private subnets within the same Availability Zone.

Which combination of steps should a Solutions Architect take to add high availability to this architecture? (Select TWO.)
* Create new private subnets in the same VPC but in a different AZ. Create a database using Amazon EC2 in one AZ
* Create new public subnets in the same AZ for high availability and move the web tier to the public subnets
* Add the existing web application instances to an Auto Scaling group behind an Application Load Balancer (ALB)
* Create an Amazon EC2 Auto Scaling group and Application Load Balancer (ALB) spanning multiple AZs
* Create new private subnets in the same VPC but in a different AZ. Migrate the database to an Amazon RDS multi-AZ deployment

### Question 56:
A company runs a streaming media service and the content is stored on Amazon S3. The media catalog server pulls updated content from S3 and can issue over 1 million read operations per second for short periods. Latency must be kept under 5ms for these updates. Which solution will provide the BEST performance for the media catalog updates?
* Update the application code to use an Amazon ElastiCache for Redis cluster
* Implement an Instance store volume on the media catalog server
* Implement Amazon CloudFront and cache the content at Edge Locations
* Update the application code to use an Amazon DynamoDB Accelerator cluster

### Question 57:
A Solutions Architect is launching an Amazon EC2 instance with multiple attached volumes by modifying the block device mapping. Which block device can be specified in a block device mapping to be used with an EC2 instance? (choose 2)
* EBS volume   
* Instance store volume   
* EFS volume   
* S3 bucket   
* Snapshot   

### Question 58:
A company requires an Elastic Load Balancer (ELB) for an application they are planning to deploy on AWS. The application requires extremely high throughput and extremely low latencies. The connections will be made using the TCP protocol and the ELB must support load balancing to multiple ports on an instance. Which ELB would should the company use?
* Route 53   
* Classic Load Balancer   
* Application Load Balancer   
* Network Load Balancer   

### Question 59:
An application makes calls to a REST API running on Amazon EC2 instances behind an Application Load Balancer (ALB). Most API calls complete quickly. However, a single endpoint is making API calls that require much longer to complete and this is introducing overall latency into the system. What steps can a Solutions Architect take to minimize the effects of the long-running API calls?
* Create an Amazon SQS queue and decouple the long-running API calls
* Change the EC2 instance to one with enhanced networking to reduce latency
* Change the ALB to a Network Load Balancer (NLB) and use SSL/TLS termination
* Increase the ALB idle timeout to allow the long-running requests to complete

### Question 60:
An application runs on EC2 instances in a private subnet behind an Application Load Balancer in a public subnet. The application is highly available and distributed across multiple AZs. The EC2 instances must make API calls to an internet-based service. How can the Solutions Architect enable highly available internet connectivity?
* Create a NAT instance in the private subnet of each AZ. Update the route tables for each private subnet to direct internet-bound traffic to the NAT instance
* Configure an internet gateway. Add a route to the gateway to each private subnet route table
* Create a NAT gateway in the public subnet of each AZ. Update the route tables for each private subnet to direct internet-bound traffic to the NAT gateway
* Create a NAT gateway and attach it to the VPC. Add a route to the gateway to each private subnet route table

### Question 61:
A company runs a web-based application that uses Amazon EC2 instances for the web front-end and Amazon RDS for the database back-end. The web application writes transaction log files to an Amazon S3 bucket and the quantity of files is becoming quite large. It is acceptable to retain the most recent 60 days of log files and permanently delete the rest.

Which action can a Solutions Architect take to enable this to happen automatically?
* Use an S3 lifecycle policy to move the log files that are more than 60 days old to the GLACIER storage class   
* Use an S3 lifecycle policy with object expiration configured to automatically remove objects that are more than 60 days old   
* Use an S3 bucket policy that deletes objects that are more than 60 days old   
* Write a Ruby script that checks the age of objects and deletes any that are more than 60 days old   

### Question 62:
Some data has become corrupted in an Amazon RDS database. A Solutions Architect plans to use point-in-time restore to recover the data to the last known good configuration. Which of the following statements is correct about restoring an RDS database to a specific point-in-time? (choose 2)
* The default DB security group is applied to the new DB instance   
* Custom DB security groups are applied to the new DB instance   
* The database restore overwrites the existing database   
* You can restore up to the last 5 minutes   
* You can restore up to the last 1 minute   

### Question 63:
A development team needs to run up a few lab servers on a weekend for a new project. The servers will need to run uninterrupted for a few hours. Which EC2 pricing option would be most suitable?   
* Spot   
* Reserved
* On-Demand
* Dedicated instances

### Question 64:
An application is generating a large amount of clickstream events data that is being stored on S3. The business needs to understand customer behaviour and want to run complex analytics queries against the data.

Which AWS service can be used for this requirement?
* Amazon RDS   
* Amazon Neptune   
* Amazon Kinesis Firehose   
* Amazon RedShift   

### Question 65:
A customer has requested some advice on how to implement security measures in their Amazon VPC. The client has recently been the victim of some hacking attempts. The client wants to implement measures to mitigate further threats. The client has explained that the attacks always come from the same small block of IP addresses.

What would be a quick and easy measure to help prevent further attacks?
* Use a Security Group rule that denies connections from the block of IP addresses   
* Create a Bastion Host restrict all connections to the Bastion Host only   
* Use CloudFront’s DDoS prevention features   
* Use a Network ACL rule that denies connections from the block of IP addresses   
# AWS Certified SysOps Administrator Associate

# Exam 1

### Question 1:
A retail company wants to get out of the business of owning and maintaining its own IT infrastructure. As part of this digital transformation, the company wants to archive about 5PB of data in its on-premises data center to durable long term storage.
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data into AWS Glacier
* Setup AWS direct connect between the on-premises data center and AWS Cloud. Use this connection to transfer the data into AWS Glacier
* Transfer the on-premises data into multiple Snowball Edge Storage Optimized devices. Copy the Snowball Edge data into Amazon S3 and create a lifecycle policy to transition the data into AWS Glacier
* Setup Site-to-Site VPN connection between the on-premises data center and AWS Cloud. Use this connection to transfer the data into AWS Glacier

### Question 2:
A systems administrator has configured Amazon EC2 instances in an Auto Scaling Group (ASG) for two separate development teams. However, only one configuration has CloudWatch agent installed on the instances, whereas the other one does not have it. The administrator has not manually installed the agents on either group of instances.
* CloudWatch agent can be configured to be loaded on the EC2 instances while configuring the ASG. The developer could have unintentionally checked this flag on one of the ASGs he created
* The instance architecture might not have been compatible with the AMI chosen. The incompatibility results in various errors, one of which is, some of the AWS services will not be installed as expected
* If your AMI contains a CloudWatch agent, it’s automatically installed on EC2 instances when you create an EC2 Auto Scaling group. The developer needs to choose the AMI that has CloudWatch agent pre-configured on it
* The architecture of the InstanceType mentioned in your launch configuration does not match the image architecture. So, the ASG was created with errors, resulting in skipping CloudWatch agent. A thorough check is needed for such ASGs, more services could have been skipped

### Question 3:
An e-commerce company relies heavily on the AWS Systems Manager for automating various management tasks for the fleet of Amazon EC2 instances that host their applications.
* Automatic recovery of impaired instances is not possible currently
* Use the AWS-UpdateCloudFormationStackWithApproval document to update impaired instances
* Use the AWS-UpdateWindowsAmi document to recover impaired instances
* Use the AWSSupport-ExecuteEC2Rescue document to recover impaired instances

### Question 4:
A company initially used a manual process to create and manage different IAM roles needed for the organization. As the company expanded and lines of business grew, different AWS accounts were created to manage the AWS resources as well as the users. The manual process has resulted in errors with IAM roles getting created with insufficient permissions. The company is looking at automating the process of creating and managing the necessary IAM roles for multiple AWS accounts. The company already uses AWS Organizations to manage multiple AWS accounts.
* Use AWS Directory Service with AWS Organizations to automatically associate necessary IAM roles with the Microsoft Active Directory users
* Create CloudFormation templates and reuse them to create necessary IAM roles in each of the AWS accounts
* Use CloudFormation StackSets with AWS Organizations to deploy and manage IAM roles to multiple AWS accounts simultaneously
* Use AWS Resource Access Manager that integrates with AWS Organizations to deploy and manage shared resources across AWS accounts

### Question 5:
An hour after launching an important feature on its website, an analytics company has realized that an important page has issues that need to be addressed. The web application is hosted on an Amazon EC2 instance with CloudFront being used to reduce latency for the users. Few users have already accessed this page and the company wants to pull it down as soon as possible.
* Specify a default root object to show only this object and not the faulty web page
* By default, CloudFront caches files in edge locations for 24 hours. So, it's not possible to remove the file before this time
* Use CloudFront policies to control what the users can see
* Invalidate the file from CloudFront distribution so that the file is removed immediately

### Question 6:
A university has just registered for an AWS account to help provide the necessary cloud infrastructure for the students planning to implement a Big Data analytics workflow as part of their thesis. The university has hired you to set up this infrastructure and help their technology team understand the basics of the AWS Virtual Private Cloud (VPC).
* By default, all subnets can route between each other, whether they are private or public
* When you create a VPC, you must specify a range of IPv4 addresses for the VPC in the form of a Classless Inter-Domain Routing (CIDR) block
* Subnets, like VPCs, can span across Availability Zones, but will remain in a single AWS Region
* Regardless of the type of subnet, the internal IPv4 address range of the subnet is always private
* A private subnet, by default, does not have inbound data traffic from the internet. You create a route to the Internet Gateway in the subnet route table to allow access to the private subnet
* If a subnet has a route to an internet gateway, along with traffic that can be routed to a virtual private gateway for a Site-to-Site VPN connection, the subnet is known as a VPN-only subnet

### Question 7:
The technology team at a retail company has set the DisableApiTermination attribute for a business-critical Amazon EC2 Windows instance to prevent termination of the instance via an API. This instance is behind an Auto Scaling Group (ASG) and the InstanceInitiatedShutdownBehavior attribute is set for the instance. A developer has initiated shutdown from the instance using operating system commands.
* The instance will be terminated
* The operating system of the instance will send an Amazon SNS notification to the concerned person, that was configured when DisableApiTermination attribute was set. The operating system will hold the shutdown for few configured minutes and then progress with instance shutdown
* ASG cannot terminate an instance whose DisableApiTermination attribute is set
* The instance will not shutdown because DisableApiTermination attribute is set

### Question 8:
Multiple teams of an e-commerce company use the same AWS CloudFormation template to create stacks of resources needed by them. For the next deployment, the teams need to update the stacks and have been testing the changes through change sets. However, the teams suddenly realized that all their change sets have been lost. Unable to figure out the error they have approached you.
* An invalid change set was executed and this resulted in all stacks and change sets getting deleted
* CloudFormation had issued a rollback on the change sets while validating them and deleted all the invalid sets
* The change set while being validated, surpassed the account limit of some AWS resource. Since the stacks cannot be updated when the account limit is reached, the change sets have been deleted by CloudFormation
* A change set was successfully executed and this resulted in rest of the change sets being deleted by CloudFormation

### Question 9:
A data analytics company has its server infrastructure built on Amazon EC2 instances fronted with Elastic Load Balancers (ELBs). The ELBs are maintained in two AZs with each ELB having two EC2 instances registered with it. Both the instances in one AZ have been recorded as unhealthy.
* HTTP 503: Service unavailable will be received as response
* The Load Balancer routes requests to the unhealthy targets
* HTTP 403: Forbidden will be returned
* The Load Balancer will display an `unhealthy' status and will not accept any incoming requests

### Question 10:
As part of the ongoing system maintenance, a SysOps Administrator has decided to increase the storage capacity of an EBS volume that is attached to an Amazon EC2 instance. However, the increased size is not reflected in the file system.
* EBS volume needs to be detached and attached back again to the instance for the modifications to show
* After you increase the size of an EBS volume, you must extend the file system to a larger size
* Linux servers automatically pick the modifications done to EBS volumes, but Windows servers do not offer this feature. Use the Windows Disk Management utility to increase the disk size to the new modified volume size
* EBS volume might be encrypted. Encrypted EBS volumes will not show modifications done when still attached to the instance. Detach the EBS volume and attach it back

### Question 11:
A retail company has built its server infrastructure on Amazon EC2 instances that run on Windows OS. The development team has defined a few custom metrics that need to be collected by the unified CloudWatch agent.
* Configure the CloudWatch agent with StatsD protocol to collect the necessary system metrics
* CloudWatch agent can be configured with either StatsD protocol or collectd protocol to collect the necessary system metrics on windows servers
* Unified CloudWatch agent cannot be custom configured
* Configure the CloudWatch agent with collectd protocol to collect the necessary system metrics

### Question 12:
An e-commerce company uses AWS Elastic Beanstalk to create test environments comprising of an Amazon EC2 instance and an RDS instance whenever a new product or line-of-service is launched. The company is currently testing one such environment but wants to decouple the database from the environment to run some analysis and reports later in another environment. Since testing is in progress for a high-stakes product, the company wants to avoid downtime and database sync issues.
* Use an Elastic Beanstalk blue (environment A)/green (environment B) deployment to decouple the RDS DB instance from environment A. Create a new Elastic Beanstalk environment (environment B) with the necessary information to connect to the decoupled RDS DB instance
* Since it is a test environment, take a snapshot of the database and terminate the current environment. Create a new one without attaching an RDS instance directly to it (from the snapshot)
* Decoupling an RDS instance that is part of a running Elastic Beanstalk environment is not currently supported by AWS. You will need to terminate the current environment after taking the snapshot of the database and create a new one with RDS configured outside the environment
* Use an Elastic Beanstalk Immutable deployment to make the entire architecture completely reliable. You can terminate the first environment whenever you are confident of the second environment working correctly

### Question 13:
A developer has configured inbound traffic for the relevant ports in both the Security Group of the EC2 instance as well as the Network Access Control List (NACL) of the subnet for the EC2 instance. The developer is, however, unable to connect to the service running on the Amazon EC2 instance.
* Network ACLs are stateful, so allowing inbound traffic to the necessary ports enables the connection. Security Groups are stateless, so you must allow both inbound and outbound traffic
* Security Groups are stateful, so allowing inbound traffic to the necessary ports enables the connection. Network ACLs are stateless, so you must allow both inbound and outbound traffic
* IAM Role defined in the Security Group is different from the IAM Role that is given access in the Network ACLs
* Rules associated with Network ACLs should never be modified from command line. An attempt to modify rules from command line blocks the rule and results in an erratic behavior

### Question 14:
A small financial services startup uses Amazon EC2 instance for their server infrastructure and Amazon S3 for storage. The files stored on S3 are critical for the business and the company wants to track access to the buckets for audit and security purposes. The startup is looking at a cost-effective way of doing this without incurring extra costs.
* Use Amazon Inspector, a security assessment service that helps track the calls made to AWS services configured with it
* Use AWS CloudTrail to identify the requests made to the Amazon S3 buckets
* Enable Amazon S3 Server Access Logging for all the buckets that the company deems important and store these logs in another S3 bucket for analysis
* Use AWS X-Ray for tracing Amazon S3 requests from end-to-end

### Question 15:
A retail company stores its business-critical files on an Amazon S3 bucket that is also configured as a website endpoint. The company needs a robust configuration that will allow access only through CloudFront. No user or team member should be able to access the files directly from Amazon S3 URL.
* Setup the Amazon S3 bucket as a custom origin with CloudFront. Restrict the access to content by setting up custom headers
* Configure a Network Access Control List (ACL) with CloudFront to restrict access to users
* Create an Origin Access Identity (OAI) and configure S3 bucket permissions so that CloudFront can use the OAI to access the files in your bucket
* Configure a Security Group with CloudFront to restrict access to users

### Question 16:
An automobile company manages its AWS resource creation and maintenance process through AWS CloudFormation. The company has successfully used CloudFormation so far, and wishes to continue using the service. However, while moving to CloudFormation, the company only moved critical resources and left out the other resources to be managed manually. To leverage the ease of creation and maintenance that CloudFormation offers, the company wants to move rest of the resources to CloudFormation.
* Drift detection is the mechanism by which you add resources to the stack of Cloudformation resources already created
* Use Parameters section of CloudFormation template to input the required resources
* You can use Mappings part of CloudFormation template to input the needed resources
* You can bring an existing resource into AWS CloudFormation management using resource import

### Question 17:
A retail company is working on moving their technology infrastructure to AWS Cloud. The company has developed several custom scripts to monitor the instances hosting their applications and want to reuse these scripts on AWS Cloud. The development team is looking at a way to disable the pre-existing Amazon EC2 status checks.
* Status checks are built into Amazon EC2, so they cannot be disabled or deleted
* Amazon EC2 status checks are interwoven into CloudWatch metrics. You can disable EC2 instance status checks from the CloudWatch metrics console
* Amazon EC2 automated checks to identify hardware issues cannot be disabled. Automated checks for software issues can however be disabled
* Status checks are built into Amazon EC2, so they cannot be disabled, but can be deleted from active configuration

### Question 18:
A large IT company manages several projects on AWS Cloud and has decided to use AWS X-Ray to trace application workflows. The company uses a plethora of AWS services like API Gateway, Amazon EC2 instances, Amazon S3 storage service, Elastic Load Balancers and AWS Lambda functions.
* Application Load balancers do not send data to X-Ray
* You cannot use X-Ray to trace or analyze user requests to your Amazon API Gateway APIs
* AWS X-Ray does not integrate with Amazon S3 and you need to use CloudTrail for tracking requests on S3
* AWS X-Ray cannot be used to trace your AWS Lambda functions since they are not integrated

### Question 19:
A retail company has realized that their Amazon EBS volume backed EC2 instance is consistently over-utilized and needs an upgrade. A developer has connected with you to understand the key parameters to be considered when changing the instance type.
* The new instance retains its pubic, private IPv4 addresses, any Elastic IP addresses, and any IPv6 addresses that were associated with the old instance
* Resizing of an instance is possible if the root device is either EBS volume or an instance store volume. However, instance store volumes taking longer to start on the new instance, since cache data is lost on these instances
* You must stop your Amazon EBS–backed instance before you can change its instance type. AWS moves the instance to new hardware; however, the instance ID does not change
* There is no downtime on the instance if you choose an instance of a compatible type since AWS starts the new instance and shifts the applications from current instance
* If your instance is in an Auto Scaling group, the Amazon EC2 Auto Scaling service marks the stopped instance as unhealthy, and may terminate it and launch a replacement instance
* Resizing of an instance is only possible if the root device for your instance is an EBS volume

### Question 20:
A production-ready application has just been deployed to Amazon EC2 instance that uses MySQL RDS as the database. The team is looking at making the RDS deployment highly available and failure-proof.
* Scale up your DB instance when you are approaching storage capacity limits
* Configure your JVM with a TTL value of no more than 60 seconds, to help you re-establish the connection to your database, in case of failure
* Configure the RDS to be a multi Availability Zone (AZ) deployment
* Configure automated backups for the RDS instance, to retrieve data and instance status, if needed after a failure

### Question 21:
A multi-national company extensively uses AWS CloudFormation to model and provision its AWS resources. A human error had earlier deleted a critical service from the CloudFormation stack that resulted in business loss. The company is looking at a quick and effective solution to lock the critical resources from any updates or deletes.
* Use nested stacks that will retain the configuration in the parent configuration even if the child configuration is lost or cannot be used
* Use Stack policies to protect critical stack resources from unintentional updates
* Use parameter constraints to specify the Identities that can update the Stack
* Use revision controls to protect critical stack resources from unintentional updates

### Question 22:
A healthcare company aggregates the daily data via a nightly batch job that runs for two hours and then sends the output to downstream applications. Currently, this job is run on On-Demand instances. The company is looking at reducing costs for this job since it is not critical to business and the job can be re-initiated if it fails.
* Opt for Spot instances
* Purchase reserved instances that offer instances at high discounts
* Use a combination of On-Demand and Reserved instances to reduce cost while keeping a minimum capacity to run without interruption
* Opt for Spot block instances

### Question 23:
As a SysOps Administrator, you have been contacted by a team for troubleshooting a security issue they seem to be facing. A security check red flag is being raised for the security groups created by AWS Directory Services. The flag message says "Security Groups - Unrestricted Access."
* AWS Directory Service might have been initiated from an account that does not have proper permissions. Check the permissions on the IAM roles and IAM users used to initiate the service
* Ignore or suppress the red flag since it is safe to do so, in this scenario
* The security group configurations have to be checked and edited to cater to AWS security standards
* Use AWS Trusted Advisor to know the exact reason for this error and take action as recommended by the Trusted Advisor

### Question 24:
A company has recently moved its server infrastructure to Amazon EC2 instances. The company needs to use CloudWatch metrics to track the state of each of the instances.
* Configure CloudWatch from AWS Console for the instances that need to be monitored by CloudWatch. AWS automatically installs and configure the agent for the mentioned instances
* Install CloudWatch Agent on all the instances and attach an IAM role to the EC2 instances to be able to run the CloudWatch agent
* Install CloudWatch Agent on all the instances and attach an IAM user to the EC2 instances to be able to run the CloudWatch agent
* Install CloudWatch Agent on all the instances and attach necessary Security Groups to the EC2 instances to be able to run the CloudWatch agent

### Question 25:
A systems administration team is configuring Amazon EC2 metrics that are sent to Amazon CloudWatch for monitoring purposes. The team is looking for a metric that can help them identify the processing power required to run an application on the selected instance.
* CPUCreditUsage metric should be used to identify the processing power required
* CPUUtilization metric should be used to identify the processing power required
* ResourceCount is the correct metric to identify the processing power required
* CPUProcessPower metric should be used to identify the processing power required

### Question 26:
An e-commerce company runs its web application on Amazon EC2 instances backed by Amazon Elastic Block Store (Amazon EBS) volumes. An Amazon S3 bucket is used for storing sharable data. A developer has attached an Amazon EBS to an Amazon EC2 instance, but it’s still in the "attaching" state after 10-15 minutes.
* The attaching status indicates that the underlying hardware related to your EBS volume has failed. This issue cannot be fixed. Raise a service request on AWS and request for a new volume. You are not charged for volumes that are in error state
* The EBS volume could be encrypted and the custom KMS key used to encrypt the snapshot is missing. The custom KMS key needs to be added to the volume configuration
* Check that the device name you specified when you attempted to attach the EBS volume isn't already in use. Attempt to attach the volume to the instance, again, but use a different device name
* Each EBS volume receives an initial I/O credit balance, an error in accumulating the credit balance can stop the volume from attaching properly to the instance. Restart the instance to fix the error

### Question 27:
While checking different deployment options, a development team has realized that there is a significant increase in latency when data on a new EBS volume (created from a snapshot) is accessed for the first time. This seems to be the general behavior of all the EBS volumes used by Amazon EC2 instances for different applications.
* Initialize the EBS volume or pre-warm it before moving the volumes to production
* Use an Amazon EBS–optimized instance
* Use RAID 0 to maximize utilization of instance resources
* Increase read-ahead for high-throughput, read-heavy workloads on st1 and sc1

### Question 28:
A financial services company runs a flagship application that hosts critical data for several clients. The company uses AWS CloudTrail to track user activities on various AWS resources. An audit firm has raised several security-specific questions about the CloudTrail logs. The company is looking at ways to secure these logs from being tampered.
* Use Amazon S3 MFA Delete to know the delete operations performed by any user on the logs stored in S3 buckets
* Use Amazon S3 Versioning to keep all versions of the file created
* Use CloudTrail log file integrity to keep the logs tamper-proof
* Use KMS logfile security keys to keep the CloudTrail logs secure and tamper-proof

### Question 29:
A firm uses Amazon EC2 instances for running its flagship application. With new business expansion plans, the firm is looking at a bigger footprint for its AWS infrastructure. The development team needs to share Amazon Machine Images (AMIs) across AZs, AWS accounts and Regions.
* You do not need to share the Amazon EBS snapshots that an AMI references in order to share the AMI
* You can only share AMIs that have unencrypted volumes and volumes that are encrypted with an AWS-managed CMK
* You can only share AMIs that have unencrypted volumes and volumes that are encrypted with a customer-managed CMK
* AMIs are regional resources and can be shared across Regions
* You need to share any CMKs used to encrypt snapshots and any Amazon EBS snapshots that the AMI references

### Question 30:
A junior developer working on configuring CloudWatch alarms is unable to figure out why a particular CloudWatch Alarm is constantly in the ALARM state.
* Custom alarms once triggered remain in Alarm state till they are manually disabled from either the AWS Console or through application code
* CloudWatch alarm has been incorrectly configured and needs to be deleted and re-configured for fixing the persistent error
* Once an alarm is triggered and an action is performed, the application logic has to reset the alarm to its normal state. This code has to be included by the development team
* Alarms continue to evaluate metrics against the configured threshold, even after they have already triggered. You can adjust the alarm threshold if you do not want it to be in ALARM state

### Question 31:
A digital marketing company that manages customer data for its clients has seen a spike in traffic that seems to be malicious. The traffic is served via Amazon CloudFront service. The company wants to set up strong security to keep their server instances and databases secure and also be able to replicate the same security processes across multiple AWS accounts that the company holds.
* Configure Security Groups on CloudFront to deny access to IP addresses that seem to send the malicious traffic. The Security Group settings can be exported out to another AWS account for easy replication
* Configure AWS Web Application Firewall (WAF) on CloudFront to keep the AWS infrastructure safe from malicious attacks. Use AWS Firewall Manager to replicate and manage the WAF configurations across AWS accounts
* Configure AWS Firewall Manager to create a secure barrier on CloudFront. Settings can be replicated across accounts by manually exporting the Firewall Manager configuration
* Configure AWS Web Application Firewall (WAF) on Amazon EC2 instances to keep the instances as well as the databases safe. WAF configured on CloudFront increases latency for users accessing the application. WAF configuration can be replicated using CloudFormation templates

### Question 32:
A video streaming app uses Amazon Kinesis Data Streams for streaming data. The systems administration team needs to be informed of the shard capacity when it is reaching its limits.
* Configure Amazon CloudWatch Events to pick data from Amazon Inspector
* Use CloudWatch ServiceLens to monitor data on service limits of various AWS services
* Configure Amazon CloudTrail to generate logs for the service limits. CloudTrail and CloudWatch are integrated and hence alarm can be generated for customized service checks
* Monitor Trusted Advisor service check results with Amazon CloudWatch Events

### Question 33:
Your company has decided that certain users should have Multi-Factor Authentication (MFA) enabled for their sign-in credentials. A newly hired manager has a Gemalto MFA device that he used in his earlier company. He has approached you to configure it for his AWS account.
* AWS MFA relies on knowing a unique secret associated with your hardware MFA. This has to be generated again with AWS MFA for the Gemalto device to work with AWS
* AWS MFA does not support the use of your existing Gemalto device
* You can re-use an existing Gemalto device with AWS MFA, as Gemalto devices do not share any secrets between multiple parties
* Security constraints mandate that sharing of secrets between multiple parties can only happen in edge cases. Hence, formal approval is needed between AWS and the previous company to use the same Gemalto device

### Question 34:
A media company stores all their articles on Amazon S3 buckets. As a security measure, they have server access logging enabled for all the buckets. The company is looking at a solution that can regularly check if logging is enabled for all the existing buckets and for any new ones they create. If the solution can also automate the remedy, it will be a perfect fit for their requirement.
* Use AWS Config rules to check whether or not an S3 bucket has logging enabled, and carry out the necessary remediation if needed
* Enable AWS CloudTrail to track the logging information for all the S3 buckets. Currently, AWS does not provide an automatic remediation process, hence, use a Lambda function to rectify any aberrations found during the checks
* Create a Lambda function that will check the logging status of all the S3 buckets and raise an Amazon SNS notification, if a remedy is needed
* Amazon S3 server access logging is checked by AWS Trusted Advisor, as part of the best practices check it performs. Configure a remedy action with Trusted Advisor for all the resources that fails this best practice check

### Question 35:
A junior systems administrator has created read replicas for Amazon Aurora for MYSQL. The created read replicas are running into errors consistently.
* Statements containing non-deterministic functions like SYSDATE() should be predefined in the configuration to successfully create the read replica
* Though read replicas can work on both transactional and nontransactional storage engines, nontransactional engines are error-prone because of the way memory is managed on these engines
* Writing to tables on a read replica can break the replication
* To safely write to tables on a read replica, create indexes on the table after setting the read_only parameter to 0
* If the value for the max_allowed_packet parameter for a read replica is less than the max_allowed_packet parameter for the source DB instance, replica errors occur

### Question 36:
A developer has created rules for different events on Amazon EventBridge with AWS Lambda function as a target. The developer has also created an IAM Role with the necessary permissions and associated it with the rule. The rule however is failing, and on initial analysis, it is clear that the IAM Role associated with the rule is not being used when calling the Lambda function.
* AWS Command Line Interface (CLI) should not be used to add permissions to EventBridge targets
* The IAM Role is wrongly configured. Delete the existing Role and recreate with necessary permissions and associate the newly created Role with the EventBridge rule
* For Lambda functions configured as a target to EventBridge, you need to provide resource-based policy. IAM Roles will not work
* For Lambda, EventBridge relies on Access Control Lists (ACLs) to define permissions. IAM Roles will not work for Lambda when configured as a target for an EventBridge rule

### Question 37:
A development team has configured its AWS VPC with one public and one private subnet. The public subnet has an Amazon EC2 instance that hosts the application. The private subnet has the RDS database that the application needs to communicate with.
* Configure a VPC peering for enabling communication between the subnets
* Create a Security Group that allows connection from different subnets inside a VPC
* Subnets inside a VPC can communicate with each other without the need for any further configuration. Hence, no additional configurations are needed
* Elastic IP can be configured to initiate communication between private and public subnets

### Question 38:
The development team at a retail company manages the deployment and scaling of their web application through AWS Elastic Beanstalk. After configuring the Elastic Beanstalk environment, the team has realized that Beanstalk is not handling the scaling activities the way they expected. This has impacted the application's ability to respond to the variations in traffic.
* The Auto Scaling group in your Elastic Beanstalk environment uses the number of logged-in users, as the criteria to trigger auto-scaling action. These alarms must be configured based on the parameters appropriate for your application
* The IAM Role attached to the Auto Scaling group might not have enough permissions to scale instances on-demand
* By default, Auto Scaling group created from Beanstalk uses Elastic Load Balancing health checks. Configure the Beanstalk to use Amazon EC2 status checks
* The Auto Scaling group in your Elastic Beanstalk environment uses two default Amazon CloudWatch alarms to trigger scaling operations. These alarms must be configured based on the parameters appropriate for your application

### Question 39:
After configuring Amazon EC2 Auto Scaling, a systems administrator had tried to launch the Auto Scaling Group. But, the following launch failure message was displayed - Client.InternalError: Client error on launch.
* Your cluster placement group contains an invalid instance type
* The security group specified in your launch configuration might have been deleted
* This error can be caused when an Auto Scaling group attempts to launch an instance that has an encrypted EBS volume, but the service-linked role does not have access to the customer-managed CMK used to encrypt it
* The block device mappings in your launch configuration might contain block device names that are not available or currently not supported

### Question 40:
A startup has reserved On-Demand Capacity Reservations for the Amazon EC2 instances they use for running analytics. Once the billing report was generated, the company was surprised to see that the costs were much higher than expected. The startup has hired you as a SysOps Administrator to bridge this knowledge gap.
* Capacity Reservations do not offer any billing discounts
* Capacity Reservations can be used with Dedicated Hosts, however, they can't be used with placement groups
* On-Demand Capacity Reservations enable you to reserve capacity for your Amazon EC2 instances in a specific Availability Zone for any duration
* Capacity Reservations are transferable from one AWS account to another
* On-Demand Capacity Reservations require a fixed one-year or three-year commitment

### Question 41:
A junior developer created multiple stacks of resources in different AWS Regions per the CloudFormation template given to him. The development team soon started having issues with the created resources and their behavior. Initial checks have confirmed that some resources were created and some omitted, though the same template has been used. As a SysOps Administrator, you have been tasked to resolve these issues.
* Insufficient IAM permissions can lead to issues. When you work with an AWS CloudFormation stack, you not only need permissions to use AWS CloudFormation, you must also have permission to use the underlying services that are described in your template
* There might have been dependency errors, that resulted in the stack not being created completely
* The CloudFormation template was created using use-once only option and is not supposed to be reused for creating other stacks
* The CloudFormation template might have custom named IAM resources that are responsible for the unintended behavior

### Question 42:
An IT company runs its server infrastructure on Amazon EC2 instances configured in an Auto Scaling Group (ASG) fronted by an Elastic Load Balancer (ELB). For ease of deployment and flexibility in scaling, this AWS architecture is maintained via an Elastic Beanstalk environment. The Technology Lead of a project has requested to automate the replacement of unhealthy Amazon EC2 instances in the Elastic Beanstalk environment.
* To automate the replacement of unhealthy EC2 instances, you must change the health check type of your instance's Auto Scaling group from EC2 to ELB by using a configuration file of your Beanstalk environment
* Modify the Auto Scaling Group from Amazon EC2 console directly to change the health check type to ELB
* Modify the Auto Scaling Group from Amazon EC2 console directly to change the health check type to EC2
* To automate the replacement of unhealthy EC2 instances, you must change the health check type of your instance's Auto Scaling group from ELB to EC2 by using a configuration file of your Beanstalk environment

### Question 43:
A financial analytics company stores their confidential reports in an Amazon S3 bucket. These reports are no more valid or useful for the company after 5 years. Manual deletion is often delayed which results in higher storage costs for the company.
* Use S3 replication to replicate the latest data to another bucket and delete the entire bucket
* Disable versioning on the S3 bucket for which the retention period is being set, to avoid creating retention periods for all versions of the object. Then, configure the retention period in the object lock settings to 5 years
* Configure the "Retain Until Date" in the object lock settings to a date that is 5 years away from the current date
* Configure the Amazon S3 bucket default settings to specify the "Retain Until Date" for all the objects in the bucket

### Question 44:
The Chief Technology Officer (CTO) of a healthcare company realized that he does not have access to an Amazon S3 bucket present in the company's own AWS account. The CTO is the root user for the AWS account and has created other AWS users using the root user account.
* Root user always has access to all the resources of the account. The Amazon S3 bucket could be from another AWS account and the S3 bucket has been shared with the root user and hence appears in his list of S3 buckets
* An Amazon S3 bucket policy that specifies a wildcard (*) in the principal element, sometimes is declared void by AWS to avoid the risk of complete public exposure. Such S3 buckets policies are in invalid status and have random behavior
* If an IAM user, with full access to IAM and Amazon S3, assigns a bucket policy to an Amazon S3 bucket and doesn't specify the AWS account root user as a principal, the root user is denied access to that bucket
* Root user has access to all the resources in his AWS account. Contact AWS support to resolve the access issue

### Question 45:
An automobile company uses a hybrid environment to run its technology infrastructure using a mix of on-premises instances and AWS Cloud. The company has a few managed instances in Amazon VPC. The company wants to avoid using the internet for accessing AWS Systems Manager APIs from this VPC.
* You can privately access AWS Systems Manager APIs from Amazon VPC by creating Internet Gateway
* You can privately access AWS Systems Manager APIs from Amazon VPC by creating VPC Endpoint
* You can privately access AWS Systems Manager APIs from Amazon VPC by creating NAT gateway
* You can privately access AWS Systems Manager APIs from Amazon VPC by creating VPN connection

### Question 46:
AWS Shared Responsibility Model discusses the responsibilities that customers and AWS share for different services and resources.
* Managing the data present in S3 Buckets
* Defining rules to move data across different S3 storage classes
* Maintaining the operating systems and platforms for Amazon S3
* Choosing encryption options for data present in S3 buckets

### Question 47:
A highly critical financial services application is being moved to AWS Cloud from the on-premises data center. The application uses a fleet of Amazon EC2 instances provisioned in different geographical areas. The Chief Technology Officer (CTO) of the company needs to understand the communication network used between instances at various locations when they interact using public IP addresses.
* Traffic between two EC2 instances in the same AWS Region stays within the AWS network, even when it goes over public IP addresses
* Traffic between EC2 instances in different AWS Regions stays within the AWS network, if there is an Inter-Region VPC Peering connection between the VPCs where the two instances reside
* Direct Connect is the default way of communication where there is no Inter-Region VPC Peering connection between the VPCs. All traffic between instances will use Direct Connect and does not go over the internet
* Traffic between EC2 instances in different AWS Regions where there is no Inter-Region VPC Peering connection between the VPCs where these instances reside, will use edge locations to communicate without going over the internet
* Traffic between two EC2 instances always stays within the AWS network, even when it goes over public IP addresses by using AWS Global Infrastructure

### Question 48:
A personal care web application is hosted on Amazon EC2 instance in two different Availability Zones (AZs). The application uses Internet Protocol version 6 (IPv6) for communication. The EC2 instances are placed in private subnets. The instances need Internet access to download software updates twice a month.
* Configure a Carrier gateway, that allows outbound communication over IPv6 from instances in your VPC to the internet
* Configure an Internet Gateway to allow outbound communication on IPv6 for the instances in the private subnet for your VPC. Public subnets are by default connected to the internet and do not need any extra configuration
* Configure Egress-only Internet Gateway, that allows outbound communication over IPv6 from instances in your VPC to the internet
* Configure an Internet Gateway to allow outbound communication on IPv6. Associate the IPv6 address to an Elastic IP address to make it public

### Question 49:
As a SysOps Administrator, you maintain the development account of a large team that comprises of both developers and testers. The Development account has two IAM groups: Developers and Testers. Users in both groups have permission to work in the development account and access resources there. From time to time, a developer must update the live S3 Bucket in the production account.
* Use Inline policies to be sure that the permissions in a policy are not inadvertently assigned to an identity other than the one they're intended for
* Create a Role in Production account, that defines the Development account as a trusted entity and specify a permissions policy that allows trusted users to update the bucket. Developers can use the newly created role to access the live S3 buckets in production environment
* Create a Role in development account, that defines the production account as a trusted entity and specify a permissions policy that allows trusted users to update the bucket. Then, modify the IAM group policy in development account, so that testers are denied access to the newly created role. Developers can use the newly created role to access the live S3 buckets in production environment
* Create a Role in production account, that defines the development account as a trusted entity and specify a permissions policy that allows trusted users to update the bucket. Then, modify the IAM group policy in development account, so that testers are denied access to the newly created role. Developers can use the newly created role to access the live S3 buckets in production environment

### Question 50:
A SysOps Administrator has come across this CloudFormation template while doing the general maintenance work on the AWS resources used by his team.
* The output section takes the website URL and bucket URL for another stack, that is part of the nested stack configuration
* The S3 bucket created is configured to store objects from PublicRead API of Amazon RDS
* AWS CloudFormation will delete this bucket when it deletes the stack
* AWS CloudFormation will not delete this bucket when it deletes the stack
* This template creates a bucket as a website
* When run from AWS CLI, URL of the website hosted on S3 will be displayed as output

### Question 51:
An e-commerce web application is built on a fleet of Amazon EC2 instances with an Auto Scaling Group. The application performance remains consistent throughout the day. But, for a few weeks now, users have been complaining about lagging screens and failing orders between 5-6 PM almost every day. Server logs show a sharp spike in user activity for this one hour every day.
* Configure an Elastic Load Balancer, to replace the ASG, and move all the instances to ELB
* Modify the Auto Scaling Group launch configuration to include more number of instances
* You can choose to manually add few more instances to the ASG to deal with the sudden spike
* Create a scheduled scaling action to scale up before the traffic spike hits the servers

### Question 52:
A healthcare web application has been deployed on Amazon EC2 instances behind an Application Load Balancer (ALB). The application worked well in the development and test environments. In production, however, users are getting logged off and are being asked to log in several times in an hour.
* Enable Sticky Sessions on Application Load Balancer
* Enable logging on ALB and check the logs to see the error being generated
* Use Slow Start Mode when registering the targets to ALB. This assures that the instances get enough time to warm up and hence will not lose the cached data
* Routing configuration of a Load Balancer is used to route traffic to targets. Use this configuration to set the protocol and port number to the correct one

### Question 53:
A hospitality company runs their applications on its on-premises infrastructure but stores the critical customer data on AWS Cloud using AWS Storage Gateway. At a recent audit, the company has been asked if the customer data is secure while in-transit and at rest in the Cloud.
* AWS Storage Gateway uses IPsec to encrypt data that is transferred between your gateway appliance and AWS storage. All three Gateway types store data in encrypted form at-rest
* AWS Storage Gateway uses SSL/TLS (Secure Socket Layers/Transport Layer Security) to encrypt data that is transferred between your gateway appliance and AWS storage. File and Volume Gateway data stored on Amazon S3 is encrypted. Tape Gateway data cannot be encrypted at-rest
* AWS Storage Gateway uses SSL/TLS (Secure Socket Layers/Transport Layer Security) to encrypt data that is transferred between your gateway appliance and AWS storage. By default, Storage Gateway uses Amazon S3-Managed Encryption Keys to server-side encrypt all data it stores in Amazon S3
* AWS Storage Gateway uses IPsec to encrypt data that is transferred between your gateway appliance and AWS storage. File and Volume Gateway data stored on Amazon S3 is encrypted. Tape Gateway data cannot be encrypted at-rest

### Question 54:
An IT services company runs its technology infrastructure on AWS Cloud. The company runs audits for all the development and testing teams against the standards set by the organization. During a recent audit, the company realized that most of the patch compliance standards are not being followed by the teams. The teams have however tagged all their AWS resources as per the guidelines.
* Use Amazon Patch Manager to automate the process of patching instances
* Use AWS Systems Manager Automation to simplify the patch application process across all instances
* Use Amazon Inspector to automate the process of patching instances that helps improve the security and compliance of the instances
* Use AWS Systems Manager Patch Manager to automate the process of patching managed instances

### Question 55:
A high traffic web application is built on Amazon Aurora for MySQL. To cater to read-only traffic, the systems administrator has been tasked to create the read replicas for the primary database. After initializing replica creation, Amazon RDS starts the replication process.
* When the AuroraBinlogReplicaLag metric reaches 0, it implies that replica has caught up to the source DB instance
* When the AuroraReplicaLag metric reaches 0, it implies that replica has caught up to the source DB instance
* When the AuroraReplicaLag metric reaches -1, it implies that replica has caught up to the source DB instance
* When the AuroraBinlogReplicaLag metric reaches -1, it implies that replica has caught up to the source DB instance

### Question 56:
A media company uses Amazon EC2 instances with EBS volumes as the instance storage. The volumes have scheduled backups as part of the maintenance plans mandated by the company. One of the EBS volumes shows the status of error.
* The error status indicates that the communication channel between EBS volume and the instance has been disrupted. Restart the instance to fix the error
* You can restore the EBS volume from Amazon Data Lifecycle Manager, by shifting the volume to another EC2 instance configured with the Data Lifecycle Manager
* Restart the instance the EBS volume is connected to. In case the data doesn't show up, you can restore the data from the scheduled backups
* The error status indicates that the underlying hardware related to the EBS volume has failed. The given EBS volume cannot be recovered but the data can be restored from the backup to a new EBS volume

### Question 57:
The technology team at a startup is looking at moving their technology infrastructure to AWS Cloud. The team has hired you as a SysOps Administrator to help them understand the mechanics of the EC2 instance IP addressing in an Amazon Virtual Private Cloud (VPC).
* By default, AWS assigns a public IP address to instances launched in both- default and nondefault VPCs
* An instance can have both - a public IP address and an Elastic IP address with it
* AWS releases your instance's public IP address when it is stopped or terminated. However, the IP address is retained if the instance is hibernated
* You cannot manually associate or disassociate a public IP address from your instance
* By default, Amazon EC2 and Amazon VPC use the IPv4 addressing protocol; you can't disable this behavior
* If the public IP address of your instance in a VPC has been released, it will not receive a new one if there is more than one network interface attached to your instance

### Question 58:
As part of regular maintenance, a systems administrator was checking through the configured Auto Scaling groups (ASGs). An error was raised by an Auto Scaling group when attempting to launch an instance that has an encrypted EBS volume. The service-linked role did not have access to the customer-managed CMK used to encrypt the volume.
* Use a CMK in the same AWS account as the Auto Scaling group (ASG). Copy and re-encrypt the snapshot with another CMK that belongs to the same account as the Auto Scaling group. Allow the service-linked role to use the new CMK
* Export the CMK to the ASG account from the instance account. Then, define a role to access this CMK and attach the role to ASG
* Determine which service-linked role to use for this Auto Scaling group. Update the key policy on the CMK and allow the service-linked role to use the CMK. Update the Auto Scaling group to use the service-linked role
* It is not possible for ASGs to initiate EC2 instances that have encrypted volumes attached to them

### Question 59:
An organization has multiple AWS accounts to manage different lines of business. A user from the Finance account has to access reports stored in Amazon S3 buckets of two other AWS accounts (belonging to the HR and Audit departments) and copy these reports back to the S3 bucket in the Finance account. The user has requested the necessary permissions from the systems administrator to perform this task.
* Create resource-level permissions in the HR, Audit accounts to allow access to respective S3 buckets for the user in the Finance account
* Create identity-based IAM policy in the Finance account that allows the user to make a request to the S3 buckets in the HR and Audit accounts. Also, create resource-based IAM policies in the HR, Audit accounts that will allow the requester from the Finance account to access the respective S3 buckets
* Create IAM roles in the HR, Audit accounts, which can be assumed by the user from the Finance account when the user needs to access the S3 buckets of the accounts
* Create resource-based policies in the HR, Audit accounts that will allow the requester from the Finance account to access the respective S3 buckets

### Question 60:
A large IT project has multiple teams working on it. The teams share access across the resources - Amazon EC2 instances, Amazon S3 buckets and RDS database. A junior developer of a team ended up deleting data from a bucket that was used by various teams. This resulted in significant wastage of time and resources to mitigate the situation.
* Enable S3 Object Lock to locks all the objects that are used in the project
* Use Amazon S3 replication to replicate critical objects to avoid losing them from unintended deletes
* Enable S3 versioning on all the buckets used in the project
* Use Amazon S3 bucket owner condition to restrict access to unintended users

### Question 61:
A financial services company runs its server infrastructure on a fleet of Amazon EC2 instances running behind an Auto Scaling Group (ASG). The SysOps Administrator has configured the instances to be protected from termination during scale-in.
* The desired capacity of the ASG is decremented, but ASG will not be able to terminate any instance
* The desired capacity of the ASG is decremented and the instances are terminated based on the configuration
* The minimum capacity of the ASG is decremented, but ASG will not be able to terminate any instance
* When all instances are termination protected, scale-in event is not generated

### Question 62:
As a SysOps Administrator, you create and maintain various system configurations for the teams you work with. You have created a CloudFront distribution with origin as an Amazon S3 bucket. The configuration has worked fine so far. However, for a few hours now, an error similar to this has cropped up - The authorization header is malformed; the region '<AWS Region>' is wrong; expecting '<AWS Region>'.
* This error indicates that when CloudFront forwarded a request to the origin, the origin didn’t respond before the request expired. This could be an access issue caused by a firewall or a Security Group not allowing access to CloudFront to access S3 resources
* This error indicates the configured Amazon S3 bucket has been moved from one AWS Region to the other. That is, deleted from one AWS Region and created with the same name in another. To fix this error, update your CloudFront distribution so that it finds the S3 bucket in the bucket's current AWS Region
* This error indicates that the CloudFront distribution and Amazon S3 are not in the same AWS Region. Move one resource so that, both the CloudFront distribution and Amazon S3 are in the same AWS Region
* This error indicates that the API key used for authorization is from an AWS Region that is different from the Region that S3 bucket is created in

### Question 63:
A development team has written configurable scripts that need to be run every day to monitor the business endpoints and APIs. The team wants to integrate these scripts with Amazon CloudWatch service to help in overall monitoring and analysis.
* Use CloudWatch Synthetics to create canaries which create CloudWatch metrics to track and monitor the services
* Use CloudWatch ServiceLens to integrate the custom script into CloudWatch system for generating metrics and logs
* CloudWatch Dashboard settings can be used to integrate the user-written scripts into Alarms generated and managed by CloudWatch
* Configure a CloudWatch Composite Alarm and integrate the configurable script, written by the team, with the CloudWatch logs

### Question 64:
An application runs on a fleet of Amazon EC2 instances running behind an Application Load Balancer. An Auto Scaling Group (ASG) helps keep the application available and flexible to traffic changes. The EC2 instances need to connect to Amazon RDS instances for fetching data. EC2 Instances also need internet access to be able to download the patches needed for their software. To meet the security guidelines of the company - the Load Balancer, Auto Scaling Group with the EC2 instances and RDS - are all placed into different subnets of the VPC.
* Configure an Elastic network interface for all the instances that need to communicate with the internet. Attach this Elastic network interface to the public subnet of the VPC to route internet traffic
* Create and attach an Egress-only Internet Gateway to the VPC and then update the route table of the instance subnet to route internet traffic via the Egress-only Internet Gateway
* Create a carrier gateway and attach the carrier gateway to your VPC. You can then connect the subnets you wish to route to the carrier gateway
* Create and attach an Internet Gateway to the VPC. Update the route table of the subnet that hosts the EC2 instances, to route internet traffic via the Internet Gateway

### Question 65:
A large online business uses multiple Amazon EBS volumes for their storage requirements. According to the company guidelines, the EBS snapshots have to be taken every few minutes to retain the business-critical data in case of failure.
* Automated EBS snapshots is a configurable item from Amazon EC2 configuration screen on AWS console
* Use Amazon CloudWatch events to schedule automated EBS Snapshots
* Use Amazon SNS Notification service to trigger AWS Lambda function that can initiate the EBS snapshots
* Use AWS Lambda functions to initiate automatic EBS snapshots every few minutes

# Exam 2

### Question 1:
Your company has recently been attacked by a team of hackers, exploiting a vulnerability in your Windows OS. A new Windows patch has been released and it needs to be applied as soon as possible to all your instances.
* Use Artifact
* Deploy it using Amazon Inspector
* Deploy the patch using Systems Manager
* Patch the instances directly from the AWS Config interface

### Question 2:
VPC Peering has been enabled between VPC A and VPC B, and the route tables have been updated for VPC A. Still, your instances cannot communicate.
* Check if DNS Resolution is enabled
* Check the instance security groups
* Check the NACL
* Check the route tables in VPC B

### Question 3:
As part of the best practices for DevOps, all your infrastructure is deployed using CloudFormation. This includes EBS volumes. When the CloudFormation stacks are deleted, it is mandatory to keep a snapshot of the EBS volumes for backup and compliance purposes.
* Use cfn helper scripts and Wait Conditions upon stack deletion
* Enable termination protection
* Use DeletionPolicy=Snapshot
* Reference the EBS volume as a stack output

### Question 4:
In order to improve the read performance of the files stored in S3, you have decided to deploy it using CloudFront. As part of this deployment, you would like to ensure that only CloudFront is allowed to access the S3 bucket files.
* Attaching a security group to S3 and CloudFront and only allow incoming traffic from CloudFront using the security group rules
* Encrypt all your files using a KMS key that only CloudFront can access
* Attaching an IAM role to CloudFront and defining a bucket policy to only allow this role
* Using an Origin Access Identity and a bucket policy

### Question 5:
Some of your users' requests are completely being lost due to the metric SpilloverCount being greater than 0. This is now happening daily. Your application is running on EC2 instances managed by an ASG running behind a load balancer.
* Pre-warm your load balancer
* Enable ALB access logs and scale based on CloudWatch Logs
* Monitor for SurgeQueueLength and scale the ASG based on that metric
* Monitor for BackendConnectionErrors and scale the ASG based on that metric

### Question 6:
Your bank has an on-premise key store and wants to migrate it to the cloud. The bank needs to ensure that the keys were isolated on a self-managed encryption module for compliance reasons.
* KMS
* S3 SSE
* CloudHSM
* GuardDuty

### Question 7:
You have deployed a public and a private subnet. As such, you have also deployed an Internet Gateway, a NAT Gateway, an Egress Only Internet Gateway, and a Virtual Private Gateway. You would like your private subnet instances to get IPv4 access to the internet.
* Add a route with a target of 0.0.0.0/0 to the NAT Gateway
* Add a route with a target of 10.0.0.0/12 to the Virtual Private Gateway
* Add a route with a target of 0.0.0.0/0 to the Egress Only Internet Gateway
* Add a route with a target of 0.0.0.0/0 to the Internet Gateway

### Question 8:
When your baby products website started, it was running at low volume so your instances of type T2.micro were doing a fine job. After a while, your website exploded in popularity and now your ELB is seeing greater traffic. You had planned for the scaling events and your T2.micro instances are running in an auto scaling group. You also noticed that the EC2 instances are experiencing high CPU utilization because the CPU is being throttled and has very poor performance and your users are complaining. Hence the ASG is not scaling.
* You should enable T2 unlimited
* Your Load Balancer needs to be pre-warmed, and then your users will be happy
* You need to disable ELB stickiness
* Your T2.micro instances have run out of burst credit. Switch to a T2.large or m4.large instance type for greater stability
* Change the ELB from an Application Load Balancer type to a Network Load Balancer type

### Question 9:
Your RDS database sometimes can become unresponsive, failing health checks and you need your application to fail-over automatically and safely without losing any committed transactions.
* Setup a CloudWatch alarm for DB RAM going over 90% and reboot the database then
* Enable RDS Multi-AZ
* Create an RDS read replica in the same region and an AWS lambda function to promote that replica as the main database when the main RDS database is down
* Create an RDS read replica in a different region and an AWS lambda function to promote that replica as the main database when the main RDS database is down

### Question 10:
You are provisioning an internal full LAMP stack using CloudFormation, and the EC2 instance gets configured automatically using the cfn helper scripts, such as cfn-init and cfn-signal. The stack creation fails as CloudFormation fails to receive a signal from your EC2 instance.
* The cfn-init script failed
* AWS is experiencing an Insufficient Capacity for the instance type you requested
* The cfn-signal script does not get executed before the timeout of the wait condition
* The subnet where the application is deployed does not have a network route to the CloudFormation service through a NAT Gateway or Internet Gateway
* The EC2 instance does not have a proper IAM role allowing to signal the success to CloudFormation

### Question 11:
One of your web applications runs behind a load balancer and an auto scaling group, which has a scaling policy based on the backend Aurora database requests. On top of scaling the ASG, the CloudWatch alarms auto scale the Aurora database. After a few scale out and scale in events, your application has completely lost connectivity to the database. You check the database URL referenced in the SSM parameter store and it turns out that it does not correspond to any of the Aurora read replicas, although it used to.
* Create an AWS Lambda function CRON job that updates SSM with the latest connection string from all the alive Aurora Read Replicas
* Disable Aurora Auto Scaling
* Create a target group made up of the Aurora Read Replicas and set up a Network Load Balancer
* Use the Aurora Reader Endpoint

### Question 12:
As part of an internal IT audit, you must provide proof that AWS has the necessary ISO certifications.
* Use AWS GuardDuty
* Fill out an ISO Penetration Testing form
* Contact the AWS Support
* Use AWS Artifact

### Question 13:
When you launched as a short term rental company, you had 5 employees all working on the same AWS cloud account. These employees deployed their applications for various purposes, including billing, operations, finance, etc. Each of these employees has been operating in their own VPC. Now that you have grown to over 200 employees, some employees belonging to different teams have created VPC peering connections and interfered with each other's work. You would like to properly separate the environment your employees work in based on the department they belong to.
* AWS IAM Groups with restrictive policies
* AWS Organizations with OU
* AWS GuardDuty
* AWS IAM Roles with restrictive policies

### Question 14:
You have a production Postgres RDS database and a custom rule in AWS Config has been set up and shows that some connections established to your database are not encrypted.
* Review the DB parameter groups
* Edit the security group rules
* Enable SSL connections from the RDS Console
* Patch the database with the SSL/TLS Postgres Addon

### Question 15:
You are launching an EC2 instance and it fails with an InsufficientInstanceCapacity error. What should you do?
* Try to launch the instance in another AZ
* Request for a service limit increase in AWS support console
* Use AWS Trusted Advisor to understand the root cause of this issue
* Run Amazon Inspector on your EC2 instances to find out what's consuming the capacity

### Question 16:
Your consumer-facing website is a high-risk target for a DDoS attack and you would like to get 24/7 support in case they happen, as well as AWS bill reimbursement for the incurred costs during the attack.
* AWS WAF
* AWS Shield
* AWS Shield Advanced
* AWS DDoS OpsTeam

### Question 17:
You just released a new mobile game and users have the chance to interact with each other. In order to publish a profile picture, your company has made the architectural decision to have users directly upload their images into a designated S3 bucket.
* Federate the users with Cognito so they can assume a role to access S3
* Create one IAM user and publish the access keys as part of the mobile application
* Create an AWS Lambda function that will create an IAM User for each new user, and store their API keys in the mobile app database
* Federate the users with SAML so they can use Single Sign-On (SSO) to access S3

### Question 18:
A development team working for a gaming company has deployed an application on EC2 and needs CloudWatch monitoring for the relevant metrics with a resolution of 1 minute in order to set alarms that can rapidly react to changes.
* Use Systems Manager
* Use AWS Lambda to retrieve metrics often using the application /health route
* Enable EC2 detailed monitoring
* The development team should create and send a high-resolution custom metric

### Question 19:
You host a forum for law questions and per your country's law, you must store all the archives of conversations (about 1 TB) every week for 7 years. These archives must not be tampered with in any way, and you must prove you have set enough controls around your data protection.
* Store the archives in EBS and use Linux file system protection on the files
* Store the archives in Glacier and set up a Vault Lock Policy for WORM access
* Store the archives in S3 and set up a bucket policy, enable versioning and MFA-Delete
* Store the archives in AWS Artifact and enable compliance monitoring

### Question 20:
You are deploying an application and use the cfn-init and cfn-signal script to ensure the application is properly deployed before signaling to CloudFormation the success of your stack deployment. Right now, every time you deploy, CloudFormation completes successfully, even though the instance is still executing the cfn-init script.
* You forgot the Wait Condition
* You forgot to include the cfn-signal command in your user data
* You forgot to include a deletion policy
* You did not disable Rollbacks

### Question 21:
The Big Data team at an insurance company is performing a nightly ETL on top of your production RDS database to compute a view and then extract it into their data lake in Amazon S3. This query has been performing reasonably well in your website's infancy but now that it has grown in popularity, the query is running for a much longer period and affects the user experience while they browse your website.
* Use Athena to query RDS
* Create an RDS Read Replica for the ETL team
* Upgrade the RDS instance type
* Enable RDS Multi-AZ

### Question 22:
Your company is experiencing an unusually high cost of Elastic IPs (EIPs) as most of them sit unassigned. Management would like to see a report showing the allocation of costs for these EIPs by department.
* Use AWS Artifact to forbid people from leaving Elastic IPs unassigned for more than 20 minutes
* Define Cost Allocation Tags and generate a report using Cost Explorer
* Create an AWS Lambda function that checks on an hourly basis the status of the EIPs and tracks using CloudTrail who is the last person who accessed them
* Define an AWS Config Rule per department and track cost

### Question 23:
How should MFA-Delete be enabled on an S3 bucket?
* Using the root account and the AWS CLI
* Using an admin IAM user and the AWS Console
* Using an admin IAM user and the AWS CLI
* Using the root account and the AWS Console

### Question 24:
You want to improve the process to assign the accounting for your AWS bills to the different departments that the resources belong to. You currently have all your resources under one AWS account.
* Use AWS Organizations
* Use Tags
* Use Cost Allocation Tags
* Use EC2 Billing Report

### Question 25:
You would like to establish a software only private connection between your corporate data center and your AWS VPC.
* Virtual Private Gateway
* Customer Gateway
* Direct Connect
* Site-to-Site VPN

### Question 26:
As a service provider, you generate a daily report that you need to share with your dynamically changing list of over 10,000 customers. These reports sit in S3, and you would like to automate sharing the reports with them so they can have on-demand access upon their identity being proven.
* Provide each of your customers an AWS user and tell them to use the CLI
* Create a bucket policy so that the S3 files are only accessible from CloudFront and force SSL mutual authentication there
* Make the S3 bucket public and password protect each S3 file. Share the password with each customer
* Generate pre-signed URLs for your reports

### Question 27:
You would like to ensure that your instances in your private subnet for us-west-1b can talk to your public instances in us-west-1c using their private IP addresses.
* Use a NAT Gateway
* Create two VPCs with one subnet each, and peer them
* Create one VPC with two subnets
* Use a NAT instance

### Question 28:
Your e-commerce website has a few really popular items that constitute 10% of your portfolio items in your RDS database but represent 90% of your traffic. Your database is starting to struggle with the read demand and your CTO tasked you with designing a solution to improve the read scalability on the database side.
* Setup a DAX cluster
* Setup an API gateway with cache enabled in front of your database
* Setup Read Replicas
* Setup a Multi-AZ RDS database
* Setup an ElastiCache cluster

### Question 29:
You run a full e-commerce website on Elastic Beanstalk, which provisions an Application Load Balancer in a public subnet, an Auto Scaling Group that spans 3 private subnets, and an RDS database in Multi-AZ mode in two private subnets. The Load Balancer can access your application, and your application can access the database.
* Deploy a NAT Gateway in the public subnet and add entries to your route table
* Deploy the instances in the public subnet instead. Private subnets cannot access the internet
* Open up security groups on the EC2 instances
* Deploy an Internet Gateway in the public subnet and add entries to your route table

### Question 30:
You would like to replace your on-premise NFS v3 drive with something that will leverage the huge capacity of Amazon S3. You would like to ensure files that are commonly used are locally cached on-premises.
* Volume Gateway
* EBS Drives
* EFS
* File Gateway

### Question 31:
You are developing a new CloudFormation stack and writing some very complex cfn-init code. The code fails and you would like to debug why. When reading the documentation, you see all the logs are in the file /var/cfn/cfn-init-output.log and will give you more information as to why the instance provisioning is failing. But you realize that you can't gain access to this file as the CloudFormation stack always terminates the EC2 instance when the creation fails.
* Install the CloudWatch logs agent, create a new IAM role and assign it to the EC2 instance, and send the logs directly to CloudWatch Logs
* Increase the Wait Timeout to 2 hours
* Set OnFailure=DO_NOTHING
* Enable VPC Flow Logs and intercept the cfn-init log file

### Question 32:
Among the following actions, what action is the IAM policy allowing you to do?
* Allowing you to give any role to RDS instances
* Allowing you to give any role to EC2 instances
* Allowing you to give RDS full access to EC2 instances
* Allowing you to assign IAM Roles to EC2 if they start with "RDS-

### Question 33:
An AWS Lambda function written in Python shuts down all instances at night for cost savings purposes. Some of these instances should not be shut down, as the underlying applications transition to an unstable state afterward.
* Change the shutdown behavior of the EC2 instances and enable termination protection as well
* Store all the instance ids you should not shut down in SSM Parameter Store
* Tag your EC2 instances and make the AWS Lambda script skip the shutdown if the tag is found
* Use an environment variable for your AWS Lambda with a list of instances not to shut down

### Question 34:
Your gp2 drive of 8TB is reaching its peak performance of 10,000 IOPS while being almost fully utilized.
* Create two 4 TB gp2 drives and mount them in RAID 1 on the EC2 instance
* Convert the gp2 drive to io1 and increase the PIOPS
* Enable burst mode on the gp2 drive
* Create two 4 TB gp2 drives and mount them in RAID 0 on the EC2 instance

### Question 35:
You are setting up a distributed in-memory database and you would like to auto-scale your Auto Scaling Group based on the average RAM usage of your EC2 instances.
* Place the instances behind a load balancer, which will have the capability of monitoring the RAM of the EC2 instances with the smart balancing feature
* Enable EC2 detailed monitoring and use the CloudWatch metric RAMUtilization to setup scaling policies
* Auto Scale your ASG based on the CPUUtilization metric
* Push the RAMUtilization as a custom metric using custom scripts in EC2 and setup scaling policies using this metric

### Question 36:
Amazon DynamoDB is experiencing a high level of rejected requests and this outage is directly impacting your applications. Your CTO would like to know all the resources that are affected in your AWS Account and how to mitigate them.
* In AWS Personal Health Dashboard
* In AWS Organizations
* In AWS Service Health Dashboard
* In DynamoDB

### Question 37:
As part of monitoring your global e-learning website, you have decided to implement a CloudWatch dashboard. The most important metric to monitor is the number of users that are connected over time, in each region.
* Create one CloudWatch dashboard and add a graph per region using the CloudWatch metric "region" filter
* Create one CloudWatch dashboard of the metric, and tick the option "global metric". Use the CloudWatch Dashboard region dropdown to change the graph on demand
* Create one CloudWatch dashboard per region
* Create one CloudWatch dashboard and add a graph per region using the region selector in the top right corner of the AWS Console

### Question 38:
You distribute a monthly raw data extract of your public forum's discussions that is about 10TB each month. Currently, the archive is distributed through an EFS drive, that is mounted on all your EC2 instances. Customers retrieve the file through the load balancer you have. This solution is costing you a lot of money and forces you to tremendously scale on the 1st of each month as people all try to retrieve the file at the same time.
* Enable enhanced networking between EC2 and ALB
* Store the files in S3 and distribute them using a CloudFront distribution instead
* Enable static file caching on the ALB
* Store the files on instance stores instead, so you don't need to use EFS anymore

### Question 39:
You want a small website on EC2 instances under an ASG that has a target size varying between 2 and 10 instances. Your ASG has a policy to scale out when your target CPU Utilization is above 75%. It has been over 3 hours that the CPU Utilization of your ASG is 90% and still, no scaling out actions have taken place.
* Your ASG Launch process has been suspended
* Your ASG is at maximum capacity already
* Your ASG AZRebalance process has been suspended
* AWS does not have the capacity for more of the requested EC2 instance types
* The warmup period of the EC2 instances has not elapsed yet

### Question 40:
You work for a blockchain company and you have a ledger application that is memory intensive. It is exposed in an auto scaling group behind a load balancer. You would like to auto scale your application based on the number of users that you have.
* Auto Scale based on the number of connections CloudWatch metric for the Load Balancer
* Use the RAM usage CloudWatch metric directly from the Load Balancer and auto scale based on that
* Deploy a script on the Load Balancer to expose the number of users that are connected to your application as a custom CloudWatch metric
* Push the RAM usage as a custom metric for the Load Balancer and auto scale based on that

### Question 41:
You have designed an AMI in an account that is optimizing the legacy database technology your gambling company has developed. You wish to share that AMI with other AWS accounts that belong to the same organization.
* Edit the account list that can see the AMI from the AMI Console UI, and create an IAM role to be assumed by the other account using STS and the other accounts can start using it
* Edit the account list that can see the AMI from the AMI Console UI and the other accounts can start using it
* The AMI can be shared without doing anything special. Just provide the target account with your secret AMI id and they can start using it
* Create an IAM role to be assumed by the other account using STS and they can start accessing your AMI

### Question 42:
Your home-cooking website stores its recipes and comments from users in a Multi-AZ RDS database, which is located in a private subnet. As of yesterday, it seems that your users are unable to access the website and see an error message "512 - Cannot connect to the database".
* A read replica has been created recently
* The database DNS name has changed
* Network ACL inbound rules have changed
* Network ACL outbound rules have changed
* DB Security Group inbound rules have changed
* Security Group outbound rules have changed

### Question 43:
After enabling S3 MFA-Delete, for which actions do you need MFA? (Select two)
* Listing deleted versions
* Uploading a new object version
* Permanently delete an object version
* Suspending versioning
* Enabling Versioning

### Question 44:
How can you enforce SSE-S3 encryption on all the files uploaded into your example S3 bucket?
* Use an encrypted CloudFront distribution in front of your S3 bucket
* Use the following S3 bucket policy:
* Using the "Default Encryption" setting in AWS S3
* Use the following S3 bucket policy:

### Question 45:
Your data center generates tens of terabytes of data daily and has a cumulative historic data volume of 5PB. The data center is running short of storage as well as bandwidth infrastructure to store or transfer this data. Later you would like to analyze this data using Redshift or Athena, however, first you must clean it using a proprietary process running on EC2.
* Use S3 transfer acceleration
* Use AWS Data Migration
* Use Snowball Edge
* Use Volume Gateway

### Question 46:
Your application has complex runtime and OS dependencies and is taking a long time to be deployed on Elastic Beanstalk. You cannot sacrifice application availability.
* Create a Golden AMI with your application
* Create a new beanstalk environment for each application and apply blue/green deployment patterns
* Use rolling with additional batch
* Upgrade the EC2 instance type
* Use all at once deployment pattern

### Question 47:
You are in S3 and have deleted all the files in it. As you can see, the bucket is empty:
* An S3 bucket policy is set up and it prevents bucket deletion
* S3 is eventually consistent. Wait two minutes and retry, it will work then
* Some files are in Glacier
* S3 versioning is enabled and delete markers are still present in the bucket

### Question 48:
Which of the following services allows for an in-place switch from unencrypted to encrypted without impacting existing operations?
* RDS
* S3
* EBS
* EFS

### Question 49:
You operate a technology company that implements the Netflix chaos testing in production. This means that your EC2 instances in production can be terminated at any time, to test the resiliency of your applications. You have been experiencing a lot of 4XXs errors lately on your website that is exposed by a load balancer, and you realize you cannot SSH into the instances that were producing these errors as they have been terminated.
* Enable the ELB access logs and query them using Athena
* Use EC2 Rescue and bring back the log files from the wiped EBS volumes
* Contact AWS Support to recover the instances
* Look at the EC2 default logs in CloudWatch Logs

### Question 50:
Your website is hosted on S3 and exposed through a CloudFront distribution and some users are said to experience a lot of 501 errors.
* Enable S3 access logs and analyze using Inspector
* Analyze the CloudFront access logs using Athena
* Analyze the CloudFront access logs using Inspector
* Enable S3 access logs and analyze using Athena

### Question 51:
Your accounting application on an EC2 instance has the tendency to sometimes go into a panic and then the CPU Utilization of your EC2 instance runs at 100% for a long duration. When this happens, someone has to manually intervene and restart your application for it to work properly again.
* Put your instance in an ASG and behind an ELB and enable ELB health check, so that the instance gets terminated upon problems and a new one gets created
* Invoke an AWS Lambda function via a cron job that checks for the metric every minute and restarts the instance if a problem is found
* Create a CloudWatch Alarm when CPU Utilization reaches 100% for 3 periods of 5 minutes and trigger an EC2 reboot action
* Create a CloudWatch Event when CPU Utilization reaches 100% and trigger an EC2 reboot action

### Question 52:
Your company has decided to elect AWS champions that will train and drive the AWS cloud adoption internally. You would like to perform an analysis to see your most active AWS users.
* Use CloudTrail and Athena
* Use IAM usage report and Athena
* Use VPC Flow Logs and Athena
* Use GuardDuty and Athena

### Question 53:
As part of your yearly compliance report, it has been noted that many of your EC2 instances have been lagging with their OS patches updates. You have decided to use SSM to patch these instances regularly. To meet regulatory guidelines, you need to provide a report showing that no outstanding known vulnerabilities are left unpatched. This report must be generated weekly.
* AWS SSM
* AWS Inspector
* AWS Shield
* AWS GuardDuty

### Question 54:
Your company's main website is deployed on Amazon S3, and distributed by CloudFront. You have set up bucket policies on S3 to ensure only CloudFront can access your bucket. You would like your website URL to be https://johntrucks.com/ .
* A
* Alias
* AAAA
* CNAME

### Question 55:
You sell beauty products and have spent thousands of dollars on a new marketing campaign that declares that the 22nd of February is "national beauty day". The marketing campaign is showing very early signs of success and on the 22nd of February, you expect traffic to increase by 10x on your website. Your CEO wants to make sure your entire infrastructure is ready for the big day. Your website runs on Elastic Beanstalk, which deployed an ASG and an ELB.
* Enable Blue/Green Beanstalk Deployment
* Open a support request to increase the upper limit on the number of the EC2 instance types you're using
* Open a support request with AWS to request a penetration testing authorization
* Open a support request with AWS to pre-warm the load balancer
* Use a weighted policy record in Route 53

### Question 56:
A healthcare company has machines both on their own data center for HIPAA compliance reasons, as well as on the AWS cloud to perform their big data analysis. All the instances must be managed using the same Puppet modules, as per the CTO decision.
* Ansible
* OpsWorks
* Artifact
* GuardDuty

### Question 57:
You plan on creating a subnet and want it to have at least capacity for 28 EC2 instances.
* /28
* /26
* /25
* /27

### Question 58:
You have set up a security group for your bastion host that only allows SSH from your IP:
* The NACL rules are too open
* Someone is attacking your EC2 instance, use AWS Inspector to verify that
* The second rule allows EC2 instances from an entire security group to SSH into your bastion host
* The IP rule should be 109.190.217.138/0

### Question 59:
You have tape backup processes and you would like to start migrating to the cloud to leverage the S3 storage capacity while keeping the same processes and iSCSI-compatible backup software you purchased a 10-year license for.
* File Gateway
* Volume Gateway
* Snowball
* Tape Gateway

### Question 60:
You suspect some of your employees try to access files in S3 that they don't have access to.
* Use a bucket policy
* Enable S3 Access Logs and analyze them using Athena
* Use AWS Config to define compliance rules on these users
* Restrict their IAM policies and look at CloudTrail logs

### Question 61:
Your infrastructure runs a daily job to compute different metrics based on all the resources that are running in your account. The goal of this job is to provide you with metrics that will be pushed into a reporting Tableau dashboard and allow your SysOps Administrator to make good decisions to bring the cost down. That job is fault-tolerant and can be resumed at any time.
* EC2 On Demand
* EC2 Placement Groups - Cluster
* EC2 Reserved Instances
* EC2 Spot Instances

### Question 62:
You have developed a script that checks if all the instances that were launched in your AWS region are using an AMI ID that is authorized by your financial company standards. After creating and testing this script in your region, eu-west-1, you share it with your colleagues in New York and ask them to run the script. Upon running it, they come back to you and say it's not working, as all the instances are declared non-compliant. Auditors manually checked the instances and they are indeed compliant.
* The API call limit has been reached and the script did not handle that error case
* AMI IDs are region-specific and a different list of compliant AMI ID should be provided based on the region of where the script is executed
* Your colleagues did not run the script properly. You write detailed documentation on what they did wrong
* The script is missing IAM permissions. Edit the script to include the IAM policy from within and run it again

### Question 63:
The security team at your travel company has detected a series of malicious attacks on port 846. As such, it needs to ensure that all your security groups are compliant with having this port closed, at all times. In the event such a port is being opened, you need to receive a notification as soon as possible.
* AWS Shield
* AWS Config
* AWS GuardDuty
* AWS WAF

### Question 64:
You have an ASG in which the Terminate process is suspended. Your ASG goes into a rebalance, what will happen?
* The rebalance will start and the EC2 instances will fail to get launched
* The rebalance will start and the EC2 instances will launch, the ASG will grow up to 10% of its size. After a bit, the instances will get terminated as the ASG is at overcapacity
* The rebalance will start and the EC2 instances will launch, the ASG will grow up to 10% of its size. The instances will not get terminated
* The rebalance will not start, as the terminate process is suspended

### Question 65:
Under the shared responsibility model, what are you NOT responsible for in Amazon S3?
* S3 bucket policies
* S3 ACLs
* S3 Server Side encryption
* S3 versioning

# Exam 3

### Question 1:
A data analytics company uses AWS CloudFormation templates to provision their AWS infrastructure for Amazon EC2, Amazon VPC, and Amazon S3 resources. Using cross-stack referencing, a systems administrator creates a stack called NetworkStack which will export the subnetId that can be used when creating EC2 instances in another stack.
* !Sub
* !Ref
* !GetAtt
* !ImportValue

### Question 2:
The technology team at a retail company uses CloudFormation to manage its AWS infrastructure. The team has created a network stack containing a VPC with subnets and a web application stack with EC2 instances and an RDS instance. The team wants to reference the VPC created in the network stack into its web application stack.
* Create a cross-stack reference and use the Outputs output field to flag the value of VPC from the network stack. Then use Ref intrinsic function to reference the value of VPC into the web application stack
* Create a cross-stack reference and use the Export output field to flag the value of VPC from the network stack. Then use Fn::ImportValue intrinsic function to import the value of VPC into the web application stack
* Create a cross-stack reference and use the Export output field to flag the value of VPC from the network stack. Then use Ref intrinsic function to reference the value of VPC into the web application stack
* Create a cross-stack reference and use the Outputs output field to flag the value of VPC from the network stack. Then use Fn::ImportValue intrinsic function to import the value of VPC into the web application stack

### Question 3:
A data analytics company runs its technology operations on AWS Cloud using different VPC configurations for each of its applications. A systems administrator wants to configure the Network Access Control List (ACL) and Security Group (SG) of VPC1 to allow access for AWS resources in VPC2.
* Network ACLs and Security Groups share a parent-child relationship. If resources in VPC2 are given inbound and outbound permissions on Network ACLs of VPC1, the resources will get necessary permissions on the associated security groups too
* The Security Groups of instances on VPC1 should be configured to allow inbound traffic from resources in VPC2. By default, Network ACLs allow all inbound and outbound traffic. So, a default Network ACLs on VPC1 will not need any configuration changes
* Based on the inbound and outbound traffic configurations on Network ACL of VPC1, you can create a similar deny rules on Security Groups of the instances in VPC1 to deny all traffic, other than the one originating from resources in VPC2
* By default, Security Groups allow outbound traffic. Hence, only the inbound traffic configuration of the security groups have to be changed to allow requests from resources in VPC2 to access instances in VPC1. If the subnet is not associated with any Network ACL, you will not need any configuration changes

### Question 4:
A systems administrator has attached two policies to an IAM user. The first policy states that the user has explicitly been denied all access to EC2 instances. The second policy states that the user has been allowed permission for EC2:Describe action.
* The user will get access because it has an explicit allow
* The IAM user stands in an invalid state, because of conflicting policies
* The order of the policy matters. If policy 1 is before 2, then the user is denied access. If policy 2 is before 1, then the user is allowed access
* The user will be denied access because one of the policies has an explicit deny on it

### Question 5:
A developer is tasked with cleaning up obsolete resources. When he tried to delete an AWS CloudFormation stack, the stack deletion process returned without any error or a success message. The stack was not deleted either.
* Some resources must be empty before they can be deleted. Such resources will not be deleted if they are not empty and stack deletion fails without any error
* The AWS user who initiated the stack deletion does not have enough permissions
* Dependent resources should be deleted first, before deleting the rest of the resources in the stack. If this order is not followed, then stack deletion fails without an error
* If you attempt to delete a stack with termination protection enabled, the deletion fails and the stack - including its status - remains unchanged

### Question 6:
A multi-national retail company wants to explore a hybrid cloud environment with AWS so that it can start leveraging AWS services for some of its daily workflows. The development team at the company wants to establish a dedicated, encrypted, low latency, and high throughput connection between its data center and AWS Cloud. The team has set aside sufficient time to account for the operational overhead of establishing this connection.
* Use VPC transit gateway to establish a connection between the data center and AWS Cloud
* Use AWS Direct Connect to establish a connection between the data center and AWS Cloud
* Use site-to-site VPN to establish a connection between the data center and AWS Cloud
* Use AWS Direct Connect plus VPN to establish a connection between the data center and AWS Cloud

### Question 7:
A new systems administrator has joined a large healthcare services company recently. As part of his onboarding, the IT department is conducting a review of the checklist for tasks related to AWS Identity and Access Management.
* Configure AWS CloudTrail to log all IAM actions
* Enable MFA for privileged users
* Use user credentials to provide access specific permissions for Amazon EC2 instances
* Create a minimum number of accounts and share these account credentials among employees
* Grant maximum privileges to avoid assigning privileges again

### Question 8:
A Silicon Valley based startup uses Elastic Beanstalk to manage its IT infrastructure on AWS Cloud and it would like to deploy the new application version to the EC2 instances. When the deployment is executed, some instances should serve requests with the old application version, while other instances should serve requests using the new application version until the deployment is completed.
* Rolling with additional batches
* All at once
* Immutable
* Rolling

### Question 9:
A systems administrator at a company is working on a CloudFormation template to set up resources. Resources will be defined using code and provisioned based on certain conditions.
* Conditions
* Outputs
* Resources
* Parameters

### Question 10:
A startup is looking at moving their web application to AWS Cloud. The database will be on Amazon RDS and it should not be accessible to the public. The application needs to remain connected to the database for the application to work. Also, the RDS instance will need access to the internet to download patches every month.
* Host the application servers in the public subnet and database in the private subnet of the VPC. Configure Network Address Translation (NAT) gateway to provide access to the internet for both the subnets. The route table of both the subnets will have an entry to NAT gateway
* Host the application servers in the public subnet and database in the private subnet of the VPC. The public subnet will connect to the internet using an Internet Gateway configured with the VPC. The private subnet can connect to the internet if they are configured using IPv6 protocol
* Host the application servers in the public subnet and database in the private subnet of the VPC. The public subnet will connect to the internet using an Internet Gateway configured with the VPC. Use VPC-peering between the private and public subnets to open internet access for the database in private subnet
* Host the application servers in the public subnet of the VPC and database in the private subnet. The public subnet will connect to the internet using an Internet Gateway configured with the VPC. Database in the private subnet will use Network Address Translation (NAT) gateway, present in the public subnet, to connect to internet

### Question 11:
A company uses Amazon S3 bucket replication to copy data from one S3 bucket into the other, for compliance purposes. The Technical Lead of the development team wants to be notified if replication of an object across S3 buckets fails.
* Enable S3 Replication with Notification, which allows you to set up notifications for objects that failed replication
* Enable S3 Replication Time Control (S3 RTC), which allows you to set up notifications for eligible objects that failed replication
* Amazon S3 publishes object events to CloudWatch. Configure Amazon Simple Notification Service (Amazon SNS) to send notifications for replication failure of objects
* Use Amazon Simple Queue Service (Amazon SQS) queue to copy objects from one S3 bucket to the other. If replication fails, messages in the queue can be configured to send notification using SNS

### Question 12:
A media company uses S3 to aggregate the raw video footage from its reporting teams across the US. The company has recently expanded into new geographies in Europe and Australia. The technical teams at the overseas branch offices have reported huge delays in uploading large video files to the destination S3 bucket.
* Create multiple AWS direct connect connections between the AWS Cloud and branch offices in Europe and Australia. Use the direct connect connections for faster file uploads into S3
* Create multiple site-to-site VPN connections between the AWS Cloud and branch offices in Europe and Australia. Use these VPN connections for faster file uploads into S3
* Use multipart uploads for faster file uploads into the destination S3 bucket
* Use Amazon S3 Transfer Acceleration to enable faster file uploads into the destination S3 bucket
* Use AWS Global Accelerator for faster file uploads into the destination S3 bucket

### Question 13:
A media company runs its business on Amazon EC2 instances backed by Amazon S3 storage. The company is apprehensive about the consistent increase in costs incurred from S3 buckets. The company wants to make some decisions regarding data retention, storage, and deletion based on S3 usage and cost reports. As a SysOps Administrator, you have been hired to develop a solution to track the costs incurred by each S3 bucket in the AWS account.
* Use AWS Trusted Advisor's rich set of best practice checks to configure cost utilization for individual S3 buckets. Trusted Advisor also provides recommendations based on the findings derived from analyzing your AWS cloud architecture
* Configure AWS Budgets to see the cost against each S3 bucket in the AWS account
* Add a common tag to each bucket. Activate the tag as a cost allocation tag. Use the AWS Cost Explorer to create a cost report for the tag
* Use AWS Simple Monthly Calculator to check the cost against each S3 bucket in your AWS account

### Question 14:
You are working as an AWS Certified SysOps Administrator at an e-commerce company and you want to build a fleet of EBS-optimized EC2 instances to handle the load of your new application. To meet the compliance guidelines, your organization wants any secret strings used in the application to be encrypted to prevent exposing values as clear text.
* Audit using CloudTrail
* Encrypt first with KMS then store in SSM Parameter store
* Audit using SSM Audit Trail
* Store the secret as SecureString in SSM Parameter Store
* Store the secret as PlainText in SSM Parameter Store

### Question 15:
An e-commerce company runs their database workloads on Provisioned IOPS SSD (io1) volumes.
* 100 GiB size volume with 1000 IOPS
* 100 GiB size volume with 5000 IOPS
* 100 GiB size volume with 7500 IOPS
* 100 GiB size volume with 3000 IOPS

### Question 16:
The development team at an IT company is looking at moving its web applications to Amazon EC2 instances. The team is weighing its options for EBS volumes and instance store-backed instances for these applications with varied workloads.
* Use separate Amazon EBS volumes for the operating system and your data, even though root volume persistence feature is available
* Data stored in the instance store is preserved when you stop or terminate your instance. However, data is lost when you hibernate the instance. Configure EBS volumes or have a backup plan to avoid using critical data to this behavior
* EBS encryption does not support boot volumes
* By default, data on a non-root EBS volume is preserved even if the instance is shutdown or terminated
* Snapshots of EBS volumes, stored on Amazon S3, can be accessed using Amazon S3 APIs
* EBS snapshots only capture data that has been written to your Amazon EBS volume, which might exclude any data that has been locally cached by your application or operating system

### Question 17:
An e-commerce company manages its IT infrastructure on AWS Cloud via Elastic Beanstalk. The development team at the company is planning to deploy the next version with MINIMUM application downtime and the ability to rollback quickly in case the deployment goes wrong.
* Deploy the new version to a separate environment via Blue/Green Deployment, and then swap Route 53 records of the two environments to redirect traffic to the new version
* Deploy the new application version using 'Rolling with additional batch' deployment policy
* Deploy the new application version using 'Rolling' deployment policy
* Deploy the new application version using 'All at once' deployment policy

### Question 18:
A SysOps Administrator has been tasked with copying AMIs from one Region to another. While doing this task, the following error message popped up: Linux error message "This AMI was copied from an AMI with a kernel that is unavailable in the destination Region: {Image ID}"
* Linux hardware virtual machine (HVM) AMIs aren't supported in all AWS Regions and copying these across unsupported Regions results in this error
* The error is a general indication of AMI not being provisioned correctly
* Linux paravirtual (PV) AMIs aren't supported in all AWS Regions and copying these across unsupported Regions results in this error
* Linux AMIs do not support copy across Regions

### Question 19:
A retail company runs its server infrastructure on a fleet of Amazon EC2 instances with Amazon RDS as the database service. For the high availability of the entire architecture, multi-AZ deployments have been chosen for the RDS instance. A new version of the database engine has been released by the vendor and the company wants to test the release with production data and configurations before upgrading the production instance.
* Procure an instance which has the new version of the database engine. Take the snapshot of your existing database and restore the snapshot to this instance. Test on this instance
* Create a configuration similar to the one in production using CloudFormation templates. You can reuse these templates to create any number of instances whenever required
* Create a read replica of the RDS instance in production. Upgrade the read replica to the latest version and experiment with this instance
* Create a DB snapshot of your existing DB instance and create a new instance from the restored snapshot. Initiate a version upgrade on this new instance and safely experiment with the instance

### Question 20:
The development team at an e-commerce company uses Amazon MySQL RDS because it simplifies much of the time-consuming administrative tasks typically associated with databases. A new systems administrator has joined the team and wants to understand the replication capabilities for Multi-AZ as well as Read-replicas.
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans at least two Availability Zones within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows synchronous replication and spans at least two Availability Zones within a single region. Read replicas follow asynchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region
* Multi-AZ follows asynchronous replication and spans one Availability Zone within a single region. Read replicas follow synchronous replication and can be within an Availability Zone, Cross-AZ, or Cross-Region

### Question 21:
A junior administrator at a retail company is documenting the process flow to provision EC2 instances via the Amazon EC2 API. These instances are to be used for an internal application that processes HR payroll data. He wants to highlight those volume types that cannot be used as a boot volume.
* Throughput Optimized HDD (st1)
* General Purpose SSD (gp2)
* Cold HDD (sc1)
* Instance Store
* Provisioned IOPS SSD (io1)

### Question 22:
Owing to lapses in security, a development team has deleted a Secrets Manager secret. Now, when the team tried to create a new secret with the same name, they ended up with an error - You can't create this secret because a secret with this name is already scheduled for deletion. The secret has to be created with the same name to avoid issues in their application.
* Use AWS Command Line Interface (AWS CLI) to permanently delete a secret without any recovery window, run the DeleteSecret API call with the ForceDeleteWithoutRecovery parameter
* The secret key deletion is an asynchronous process. There might be a short delay before updates are received. Try after few minutes for successful completion
* Use AWS Management Console to delete the key permanently. You will be allowed to create a new key with the same name after the older one is successfully deleted
* When you delete a secret, the Secrets Manager deprecates it with a seven-day recovery window. It is not possible to create a new secret with the same name for this duration

### Question 23:
A social media company manages over 100 c4.large instances in the us-west-1 region. The EC2 instances run complex algorithms. The systems administrator would like to track CPU utilization of the EC2 instances as frequently as every 10 seconds.
* Simply get it from the CloudWatch Metrics
* Create a high-resolution custom metric and push the data using a script triggered every 10 seconds
* Open a support ticket with AWS
* Enable EC2 detailed monitoring

### Question 24:
An e-commerce company has used Aurora Serverless MySQL compatible DB clusters for deploying a new application to understand its capacity needs. Based on the scaling actions of Aurora, the company will decide on the database requirements for deploying the new application. In this context, the company wants to audit the database activity, collect and publish the logs generated by Aurora Serverless to Amazon CloudWatch.
* Aurora Serverless connects to a proxy fleet of DB instances and hence you cannot see the log files. You can connect with your AWS support contact to get help on this requirement
* For MySQL-compatible DB clusters, you can enable the slow query log, general log, or audit logs to get a view of the database activity
* Aurora Serverless cluster is integrated with Amazon CloudWatch and logs are sent automatically
* You can view the logs directly from the Amazon Relational Database Service (Amazon RDS) console

### Question 25:
A streaming services company has created an audio streaming application and it would like their Australian users to be served by the company's Australian servers. Other users around the globe should not be able to access the servers through DNS queries.
* Geolocation
* Failover
* Weighted
* Latency

### Question 26:
A large IT company uses several AWS accounts for the different lines of business. Quite often, the systems administrator is faced with the problem of sharing Customer Master Keys (CMKs) across multiple AWS accounts for accessing AWS resources spread across these accounts.
* AWS Owned CMK can be used across AWS accounts. Configure an AWS Owned CMK and use it across accounts that need to share the key material
* The key policy for the CMK must give the external account (or users and roles in the external account) permission to use the CMK. IAM policies in the external account must delegate the key policy permissions to its users and roles
* Use AWS KMS service-linked roles to share access across AWS accounts
* Declare a key policy for the CMK to give the external account permission to use the CMK. This key policy should be embedded with the first request of every transaction

### Question 27:
A healthcare company has developed its flagship application on AWS Cloud with data security requirements such that the encryption key must be stored in a custom application running on-premises. The company wants to offload the data storage as well as the encryption process to Amazon S3 but continue to use the existing encryption keys.
* Client-Side Encryption with data encryption is done on the client-side before sending it to Amazon S3
* Server-Side Encryption with Customer Master Keys (CMKs) Stored in AWS Key Management Service (SSE-KMS)
* Server-Side Encryption with Amazon S3-Managed Keys (SSE-S3)
* Server-Side Encryption with Customer-Provided Keys (SSE-C)

### Question 28:
A company is moving their on-premises technology infrastructure to AWS Cloud. Compliance rules and regulatory guidelines mandate the company to use its own software that needs socket level configurations. As the company is new to AWS Cloud, they have reached out to you for guidance on this requirement.
* Opt for Amazon EC2 Dedicated Host
* Opt for Reserved Instances that allow you to plan and help install the necessary software
* Opt for Amazon EC2 Dedicated Instance
* Opt for On-Demand instances that are highly available and require no prior planning

### Question 29:
Two AWS CloudFormation stack policies are shared below.
* Policy-2 denies updates on MyDatabase, whereas, Policy-1 allows updates on MyDatabase
* Policy-1 denies updates on MyDatabase, whereas, Policy-2 allows updates on MyDatabase
* Both the policies deny all update actions on the database with the MyDatabase logical ID. And they allow all update actions on all other stack resources
* Both the policies allow updates on all resources

### Question 30:
A developer is trying to access an Amazon S3 bucket for storing the images used by the web application. The S3 bucket has public read access enabled on it. However, when the developer tries to access the bucket, an error pops up - 403 Access Denied. The confused developer has connected with you to know why he has no access to the public S3 bucket.
* Run the AWSSupport-TroubleshootS3PublicRead automation document on AWS Systems Manager to help diagnose issues with accessing objects from a public S3 bucket
* Explicit deny statement in the bucket policy can cause forbidden-access errors. Check the bucket policy of the S3 bucket
* AWS Organizations service control policy doesn't allow access to Amazon S3 bucket that the developer is trying to access. Service policy needs to be changed using AWS Organizations
* The resource owner which is the AWS account that created the S3 bucket, has access to the bucket. This is an error in creation, delete the S3 bucket and re-create it again

### Question 31:
A healthcare company stores confidential data on an Amazon Simple Storage Service (S3) bucket. New security compliance guidelines require that files be stored with server-side encryption. The encryption used must be Advanced Encryption Standard (AES-256) and the company does not want to manage S3 encryption keys.
* SSE-C
* SSE-KMS
* Client Side Encryption
* SSE-S3

### Question 32:
The development team at your company wants to upload files to S3 buckets using the SSE-KMS encryption mechanism. However, the team is receiving permission errors while trying to push the objects over HTTP.
* 'x-amz-server-side-encryption': 'SSE-S3'
* 'x-amz-server-side-encryption': 'aws:kms'
* 'x-amz-server-side-encryption': 'AES256'
* 'x-amz-server-side-encryption': 'SSE-KMS'

### Question 33:
As part of the systems administration work, an AWS Certified SysOps Administrator is creating policies and attaching them to IAM identities. After creating necessary Identity-based policies, he is now creating Resource-based policies.
* Permissions boundary
* AWS Organizations Service Control Policies (SCP)
* Trust policy
* Access control list (ACL)

### Question 34:
A data analytics company wants to seamlessly integrate its on-premises data center with AWS cloud-based IT systems which would be critical to manage as well as scale-up the complex planning and execution of every stage of its analytics workflows. As part of a pilot program, the company wants to integrate data files from its on-premises servers into AWS via an NFS interface.
* AWS Storage Gateway - Volume Gateway
* AWS Storage Gateway - Tape Gateway
* AWS Storage Gateway - File Gateway
* AWS Site-to-Site VPN

### Question 35:
Security and Compliance is a Shared Responsibility between AWS and the customer. As part of this Shared Responsibility, the customer is also responsible for securing the resources that he has procured under his AWS account.
* AWS is responsible for training their customers and their employees as part of Customer Specific training
* AWS is responsible for patching and fixing flaws within the infrastructure, for patching the guest Operating Systems and applications of the customers
* For Amazon EC2 service, managing guest operating system (including updates and security patches), application software and Security Groups is the responsibility of the customer
* For Amazon S3 service, managing the operating system and platform is customer responsibility

### Question 36:
A multi-national retail company uses AWS Organizations to manage its users across different divisions. Even though CloudTrail is enabled on the member AWS accounts, managers have noticed that access issues for CloudTrail logs across different divisions and AWS Regions are becoming a bottleneck in troubleshooting issues. They have decided to use the organization trail to keep things simple.
* There is nothing called Organization Trail. The master account can, however, enable CloudTrail logging, to keep track of all activities across AWS accounts
* By default, CloudTrail tracks only bucket-level actions. To track object-level actions, you need to enable Amazon S3 data events
* By default, CloudTrail event log files are not encrypted
* Member accounts do not have access to organization trail, neither do they have access to the Amazon S3 bucket that logs the files
* Member accounts will be able to see the Organization trail, but cannot modify or delete it

### Question 37:
A multi-national company runs its technology infrastructure on a fleet of Amazon EC2 instances, Elastic Load Balancers, Amazon RDS and Amazon S3 storage. The company already uses AWS Config to track and maintain configuration changes. The company also uses AWS Systems Manager for maintaining its AWS infrastructure.
* Use AWS Systems Manager Patch Manager that automates the process of patching managed instances with both security-related and other types of updates
* Use AWS Systems Manager Inventory that provides visibility into your Amazon EC2 and on-premises computing environment
* Use AWS Systems Manager Maintenance Windows to help you define a schedule to check configurations and track any needed changes
* Use Systems Manager Automation that simplifies common maintenance and configuration tasks

### Question 38:
A social media company uses Amazon S3 to store the images uploaded by the users. These images are kept encrypted in S3 by using AWS-KMS and the company manages its own Customer Master Key (CMK) for encryption. A systems administrator accidentally deleted the CMK a day ago, thereby rendering the user's photo data unrecoverable. You have been contacted by the company to consult them on possible solutions to this issue.
* The CMK can be recovered by the AWS root account user
* Contact AWS support to retrieve the CMK from their backup
* The company should issue a notification on its web application informing the users about the loss of their data
* As the CMK was deleted a day ago, it must be in the 'pending deletion' status and hence you can just cancel the CMK deletion and recover the key

### Question 39:
A social media company is using AWS CloudFormation to manage its technology infrastructure. It has created a template to provision a stack with a VPC and a subnet. The output value of this subnet has to be used in another stack.
* Use Fn::ImportValue
* Use Fn::Transform
* Use 'Export' field in the Output section of the stack's template
* Use 'Expose' field in the Output section of the stack's template

### Question 40:
A systems administration intern is trying to configure what an Amazon EC2 should do when it interrupts a Spot Instance.
* Hibernate the Spot Instance
* Stop the Spot Instance
* Terminate the Spot Instance
* Reboot the Spot Instance

### Question 41:
A retail company has complex AWS VPC architecture that is getting difficult to maintain. The company has decided to configure VPC flow logs to track the network traffic to analyze various traffic flow scenarios. The systems administration team has configured VPC flow logs for one of the VPCs, but it's not able to see any logs. After initial analysis, the team has been able to track the error. It says Access error and the administrator of the team wants to change the IAM Role defined in the flow log definition.
* The flow log is still in the process of being created. It sometimes takes almost 10 minutes to start the logs
* The error indicates that the IAM role does not have a trust relationship with the flow logs service. Change the trust relationship from flow log configuration
* The error indicates an internal error has occurred in the flow logs service. Raise a service request with AWS
* The error indicates IAM role is not correctly configured. After you've created a flow log, you cannot change its configuration. Instead, you need to delete the flow log and create a new one with the required configuration

### Question 42:
A bug in an application code has resulted in an EC2 instance's CPU utilization touching almost 100 percent thereby freezing the instance. The instance needs a restart to work normally once it hits this point. It will take a few weeks for the team to fix the issue. Till the bug fix is deployed, you have been tasked to automate the instance restart at the first sign of the instance becoming unresponsive.
* Create a CloudWatch alarm for CPU Utilization of the Amazon EC2 instance, with detailed monitoring enabled. Configure an action to restart the instance when the alarm is triggered
* Create a CloudWatch alarm for CPU Utilization of the Amazon EC2 instance, with basic monitoring enabled. Configure an AWS Lambda function against the alarm action. The Lambda function will restart the instance, automating the process
* CPU utilization parameter of an Amazon EC2 instance is a pre-defined metric in CloudWatch and is available in basic monitoring of an instance. Configure the restart action against this metric to automate the instance restart process
* Create a custom code to send CPU utilization of the instance to CloudWatch metrics. Configure an action to restart the instance when the alarm is triggered

### Question 43:
An IT company extensively uses Amazon S3 buckets for storage, hosting, backup and compliance specific replication. A Team Lead has reached out to you for creating a report that lists all the objects that have failed replication in the S3 buckets that the project manages. This process needs to be automated as the Team Lead needs this list daily.
* Use Amazon S3 Inventory reports to list the objects that have failed replication in the S3 buckets
* Use Amazon S3 Storage Lens to report all the objects that failed replication process in the S3 buckets
* Use Amazon S3 Select to list the objects that have failed replication in the S3 buckets
* Configure Amazon Simple Queue Service (Amazon SQS) queue against the CloudWatch metrics for S3 replication. You can use custom code to aggregate these messages to get the final list of objects that failed replication

### Question 44:
An e-commerce company is running its server infrastructure on Amazon EC2 instance store-backed instances. For better performance, the company has decided to move their applications to another Amazon EC2 instance store-backed instance with a different instance type.
* You can't resize an instance store-backed instance. Instead, you choose a new compatible instance and move your application to the new instance
* Create an image of your instance, and then launch a new instance from this image with the instance type that you need. Any public IP address associated with the instance can be moved with the instance for uninterrupted access of services
* You can't resize an instance store-backed instance. Instead, configure an EBS volume to be the root device for the instance and migrate using the EBS volume
* Create an image of your instance, and then launch a new instance from this image with the instance type that you need. Take any Elastic IP address that you've associated with your original instance and associate it with the new instance for uninterrupted service to your application

### Question 45:
A video streaming solutions provider is migrating to AWS Cloud infrastructure for delivering its content to users across the world. The company wants to make sure that the solution supports at least a million requests per second for its EC2 server farm.
* Application Load Balancer
* Classic Load Balancer
* Network Load Balancer
* Infrastructure Load Balancer

### Question 46:
A financial services firm wants to run its applications on single-tenant hardware to meet security guidelines.
* Dedicated Hosts
* Spot Instances
* Dedicated Instances
* On-Demand Instances

### Question 47:
An analytics company generates reports for various client applications, some of which have critical data. As per the company's compliance guidelines, data has to be encrypted during data exchange, for all channels of communication. An Amazon S3 bucket is configured as a website endpoint and this is now being added as a custom origin for CloudFront.
* CloudFront always forwards requests to S3 by using the protocol that viewers used to submit the requests. So, we only need to configure CloudFront to mandate the use of HTTPS for users
* Communication between CloudFront and Amazon S3 is always on HTTP protocol since the network used for communication is internal to AWS and is inherently secure
* Configure CloudFront that mandates viewers to use HTTPS to request objects from S3. Configure S3 bucket to support HTTPS communication only. This will force CloudFront to use HTTPS for communication between CloudFront and S3
* Configure CloudFront to mandate viewers to use HTTPS to request objects from S3. However, CloudFront and S3 will use HTTP to communicate with each other

### Question 48:
A healthcare solutions company is undergoing a compliance audit by the regulator. The company has hundreds of IAM users that make API calls but specifically it needs to be determined who is making KMS API calls.
* CloudTrail
* X-Ray
* CloudWatch Metrics
* Config

### Question 49:
After a developer had mistakenly shutdown a test instance, the Team Lead has decided to configure termination protection on all the instances. As a systems administrator, you have been tasked to review the termination policy and check its viability for the given requirements.
* To prevent instances that are part of an Auto Scaling group from terminating on scale in, use instance protection
* The DisableApiTermination attribute prevents Amazon EC2 Auto Scaling from terminating an instance
* The DisableApiTermination attribute does not prevent you from terminating an instance by initiating shutdown from Amazon EC2 console
* The DisableApiTermination attribute prevents you from terminating an instance by initiating shutdown from the instance
* You can't enable termination protection for Spot Instances

### Question 50:
An e-commerce company has established a Direct Connect connection between AWS Cloud and their on-premises infrastructure. The development team needs to access the Amazon S3 bucket present in their AWS account to pull the customer data for an application hosted on the on-premises infrastructure.
* Create a VPC gateway endpoint for the S3 bucket you need to access. Then use the private virtual interface (VIF) using Direct Connect to access the bucket
* Create a VPC interface endpoint for the S3 bucket you need to access. Then use the private virtual interface (VIF) using Direct Connect to access the bucket
* Directly access the S3 bucket through a private virtual interface (VIF) using Direct Connect
* Create a dedicated or hosted connection. Establish a cross-network connection and then create a public virtual interface for your connection. Configure an end router for use with the public virtual interface

### Question 51:
As a SysOps Administrator, you manage a large team of IAM user accounts that are part of multiple AWS accounts. With the growing team size, you have decided to divide IAM users into IAM groups to be able to manage the permissions and policies better.
* An IAM user can belong to multiple IAM groups and an IAM group can be part of another IAM group
* Groups can be given security credentials to be able to access web services directly
* Groups cannot be given security credentials directly, however, these can take up an IAM Role to access web services directly
* Groups can be granted permissions using access control policies
* An IAM user can belong to multiple IAM groups. But, Groups cannot belong to other groups

### Question 52:
A financial services startup is building an interactive tool for personal finance needs. The users would be required to capture their financial data via this tool. As this is sensitive information, the backup of the user data must be kept encrypted in S3. The startup does not want to provide its own encryption keys but still wants to maintain an audit trail of when an encryption key was used and by whom.
* Use SSE-C to encrypt the user data on S3
* Use SSE-S3 to encrypt the user data on S3
* Use client-side encryption with client provided keys and then upload the encrypted user data to S3
* Use SSE-KMS to encrypt the user data on S3

### Question 53:
A banking service uses Amazon EC2 instances and Amazon RDS databases to run its core business functionalities. The Chief Technology Officer (CTO) of the company has requested granular OS level metrics from the database service for benchmarking.
* Enable Performance Insights to expand on the existing Amazon RDS monitoring features to illustrate your database's performance
* Enable Enhanced Monitoring for your RDS DB instance
* Subscribe to CloudWatch metrics that track CPU utilization of the instances the RDS is hosted on
* Subscribe to Amazon RDS events to be notified when changes occur with a DB instance and its connected resources

### Question 54:
Which of the following security credentials can only be generated by the AWS Account root user?
* IAM User passwords
* CloudFront Key Pairs
* IAM User Access Keys
* EC2 Instance Key Pairs

### Question 55:
Your application is hosted by a provider on yourapp.freehosting.com. You would like to have your users access your application using www.yourdomain.com, which you own and manage under Route 53.
* Create a PTR record
* Create an A record
* Create an Alias Record
* Create a CNAME record

### Question 56:
A video streaming solutions company wants to use AWS Cloudfront to distribute its content only to its service subscribers.
* Require HTTPS for communication between CloudFront and your custom origin
* Use CloudFront signed URLs
* Require HTTPS for communication between CloudFront and your S3 origin
* Use CloudFront signed cookies
* Forward HTTPS requests to the origin server by using the ECDSA or RSA ciphers

### Question 57:
A telecommunications company runs its business on AWS Cloud with Amazon EC2 instances and Amazon S3 buckets. Of late, users are complaining of intermittently receiving 500 Internal Error response when accessing the S3 bucket. The team is looking at a way to track the frequency of the error and fix the issue.
* Objects encrypted by AWS KMS are not accessible to users unless permission for KMS key access is provided. Include logic to provide access to KMS keys
* The users accessing the bucket do not have proper permissions to access the objects present in S3. Check the application logic for the IAM Role being assigned when accessing the S3 bucket
* Enable Amazon CloudWatch metrics that include a metric for 5xx server errors. Retrying generally fixes this error
* Check if the S3 bucket has all the objects users are trying to access

### Question 58:
A junior developer is tasked with creating necessary configurations for AWS CloudFormation that is extensively used in a project. After declaring the necessary stack policy, the developer realized that the users still do not have access to stack resources. The stack policy created by the developer looks like so:
* The stack policy is invalid and hence the users are not granted any permissions. The developer needs to fix the syntactical errors in the policy
* A stack policy applies only during stack updates, it doesn't provide access controls. The developer needs to provide access through IAM policies
* Stack policies are associated with a particular IAM role or an IAM user. Hence, they only work for the users you have explicitly attached the policy to
* Stack policies do not allow wildcard character value (*) for the Principal element of the policy

### Question 59:
A web application runs on multiple Amazon EC2 instances that are configured behind an Auto Scaling Group (ASG). The company wants the scaling action to begin as soon as CPU utilization crosses 50% for the instances.
* Configure ASG to scale based on demand
* Configure ASG to scale based on events
* Configure ASG to scale based on a schedule
* Configure ASG to use predictive scaling

### Question 60:
A retail company has a web application that is deployed on 10 EC2 instances running behind an Application Load Balancer. You have configured your web application to capture the IP address of the client making requests. When viewing the data captured you notice that every IP address being captured is the same, which also happens to be the IP address of the Application Load Balancer.
* Look at the X-Forwarded-For header
* Modify the front-end of the website so that the users send their IP in the requests
* Look at the client's cookie
* Look at the X-Forwarded-Proto header

### Question 61:
A startup uses Amazon S3 buckets for storing their customer data. The company has defined different retention periods for different objects present in their Amazon S3 buckets, based on the compliance requirements. But, the retention rules do not seem to work as expected.
* You cannot place a retention period on an object version through a bucket default setting
* Different versions of a single object can have different retention modes and periods
* When you apply a retention period to an object version explicitly, you specify a Retain Until Date for the object version
* When you use bucket default settings, you specify a Retain Until Date for the object version
* The bucket default settings will override any explicit retention mode or period you request on an object version

### Question 62:
An organization that started as a single AWS account, gradually moved to a multi-account setup. The organization also has multiple AWS environments in each account, that were being managed at the account level. Backups are a big part of this management task. The organization is looking at moving to a centralized backup management process that consolidates and automates Cross-Region backup tasks across AWS accounts.
* Use Amazon Data Lifecycle Manager to manage creation, deletion, and managing of all the AWS resources under an account. Tag all the resources that need to be backed up and use lifecycle policies to customize the backup management to cater to the needs of the organization
* Use Amazon EventBridge to create a workflow for scheduled backup of all AWS resources under an account. Amazon S3 lifecycle policies, Amazon EC2 instance backups, and Amazon RDS backups can be used to create the events for the EventBridge. The same workflow can be scheduled to work on production and non-production environments, based on the tags created
* Configure AWS Systems Manager Maintenance Windows to schedule backup tasks as per company's policies. Tag the resources to help identify them by the AWS environment they run in. Amazon CloudWatch dashboards hosted by Systems Manager to get an overall view of the status of all resources under the AWS account
* Create a backup plan in AWS Backup. Assign tags to resources based on the environment ( Production, Development, Testing). Create one backup policy for production environments and one backup policy for non-production environments. Schedule the backup plan based on the organization's backup policies

### Question 63:
An application hosted on Amazon EC2 instances polls messages from Amazon SQS queue for downstream processing. The team is now looking at configuring an Auto Scaling group to scale using the CloudWatch metrics for Amazon SQS queue to process messages without delays.
* A composite key Queue Name - Queue ID is used to fetch SQS queue data from CloudWatch metrics
* A key-value pair of name:<queue name> and value:<value> needs to be considered for fetching SQS queue data from CloudWatch metrics
* Queue ID should be used to fetch the SQS queue data from the CloudWatch metrics
* Queue name of the SQS queue should be used to fetch the necessary data from CloudWatch metrics

### Question 64:
A retail company has branch offices in multiple locations and the development team has configured an Application Load Balancer across targets in multiple Availability Zones. The team wants to analyze the incoming requests for latencies and the client's IP address patterns.
* CloudTrail logs
* CloudWatch metrics
* ALB request tracing
* ALB access logs

### Question 65:
A systems administrator at a company is trying to create a digital signature for SSH'ing into the Amazon EC2 instances.
* Root user credentials
* Access keys
* Key pairs
* Multi-Factor Authentication (MFA)


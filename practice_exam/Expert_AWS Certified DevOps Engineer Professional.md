# AWS Certified DevOps Engineer Professional

# Exam 1

### Question 1:
The DevOps team at your company is using CodeDeploy to deploy new versions of a Lambda function after it has passed a CodeBuild check via your CodePipeline. Before deploying, the CodePipeline has a step in which it optionally kickstarts a restructuring of files on an S3 bucket that is forward compatible. That restructuring is done using a Step Function execution which invokes a Fargate task. The new Lambda function cannot work until the restructuring task has fully completed.
* In your appspec.yml file, include an AfterAllowTraffic hook that checks on the completion of the Step Function execution
* Enable Canary Deployment in CodeDeploy so that only a fraction of the service is served by the new Lambda function while the restructuring is happening
* In your appspec.yml file, include a BeforeAllowTraffic hook that checks on the completion of the Step Function execution
* Include an extra step in the Step Function to signal to CodeDeploy the completion of the restructuring and serve new traffic to the new Lambda function

### Question 2:
As a DevOps Engineer at a data analytics company, you're deploying a web application on EC2 using an Auto Scaling group. The data is stored in RDS MySQL Multi-AZ, and a caching layer using ElastiCache. The application configuration takes time and currently needs over 20 minutes to warm up. 10 of those minutes are spent installing and configuring the web application, and another 10 minutes are spent warming up the local instance data cache.
* Migrate from ElastiCache to DynamoDB. Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script
* Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script. Use AWS Lambda to configure the instance local cache at boot time
* Create an AMI that contains the web application and a copy of the local data cache. Configure the dynamic part at runtime an EC2 User Data script
* Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script

### Question 3:
A retail company is finishing its migration to AWS and realizes that while some employees have passed the AWS Certified DevOps Engineer Professional certification and know AWS very well, other ones are still beginning and haven't passed their Associate-level certifications yet. The company has established architectural and tagging specific internal rules and would like to minimize the risk of the AWS-beginner employees launching uncompliant resources.
* Define commonly used architectures as CloudFormation templates. Create Service Catalog stacks from these templates, and ensure the tagging is done properly. Place the IAM users into a beginner group and allow the users to only launch stacks from Service Catalog, while restricting any write access to other services
* Place the beginner IAM users into a group and create an IAM policy that requires conditional approvals from senior DevOps engineers upon resource creation. Hook an SNS topic into the IAM approval channel
* Define commonly used architectures as CloudFormation templates. Place the IAM users into a beginner group and allow the users to only launch stacks from these CloudFormation stacks, while restricting any write access to other services
* Create AWS Config custom rules that will check for the compliance of your company's resources thanks to a Lambda Function. Update the Lambda Function over time while your company improves its architectural and tagging rules. Provide IAM users full access to AWS

### Question 4:
As a DevOps Engineer at an e-commerce company, you have deployed a web application in an Auto Scaling group (ASG) that is being distributed by an Application Load Balancer (ALB). The web application is using RDS Multi-AZ as a back-end and has been experiencing some issues to connect to the database. The health check implemented in the application currently returns an un-healthy status if the application cannot connect to the database. The ALB / ASG health check integration has been enabled, and therefore the ASG keeps on terminating instances right after they're done booting up.
* Set an instance in Standby right after it has launched
* Enable termination protection for EC2
* Create an autoscaling hook for instance termination. Troubleshoot the instance while it is in the Terminating:Wait state
* Suspend the Launch process

### Question 5:
A mobility company connects people with taxi drivers and the DevOps team at the company uses CodeCommit as a backup and disaster recovery service for several of its DevOps processes. The team is creating a CICD pipeline so that your code in the CodeCommit master branch automatically gets packaged as a Docker container and published to ECR. The team would then like that image to be automatically deployed to an ECS cluster using a Blue/Green strategy.
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY environment variables passed in through CodeBuild configuration, the values being those from your user. Upon the success of that CodeBuild stage, create a new task definition automatically using CodePipeline and apply that task definition to the ECS service using a CloudFormation action
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Upon the success of that CodeBuild stage, create a new task definition automatically using CodePipeline and apply that task definition to the ECS service using a CloudFormation action
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Upon the success of that CodeBuild stage, start a CodeDeploy stage with a target being your ECS service
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Create a CloudWatch Event Rule that will react to pushes to ECR and invoke CodeDeploy, the target of which should be the ECS cluster

### Question 6:
A global financial services company manages over 100 accounts using AWS Organizations and it has recently come to light that several accounts and regions did not have AWS CloudTrail enabled. It also wants to be able to track the compliance of the CloudTrail enablement as a dashboard, and automatically be alerted in case of issues. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy it in all your accounts and regions under the AWS organization. Create another StackSet to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create an SNS topic to get notifications when compliance is breached, and subscribe a Lambda function to it, that will send out these notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create one CloudFormation template in a centralized account to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create a CloudWatch Event to generate events when compliance is breached, and subscribe a Lambda function to it, that will send out notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create another CloudFormation StackSet to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance. Create a CloudWatch Event to generate events when compliance is breached, and subscribe a Lambda function to it, that will send out notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create one CloudFormation template in a centralized account to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create an SNS topic to get notifications when compliance is breached, and subscribe a Lambda function to it, that will send out these notifications

### Question 7:
The DevOps team at a leading bitcoin wallet and exchange services company is trying to deploy a CloudFormation template that contains a Lambda Function, an S3 bucket, an IAM role, and a DynamoDB table from CodePipeline but the team is getting an InsufficientCapabilitiesException.
* Enable the IAM Capability on the CodePipeline configuration for the Deploy CloudFormation stage action
* Update the CodePipeline IAM Role so it has permissions to create all the resources mentioned in the CloudFormation template
* Increase the service limits for your S3 bucket limits as you've reached it
* Fix the CloudFormation template as there is circular dependency and CloudFormation does not have that capability

### Question 8:
The DevOps team at a social media company has created a CodePipeline pipeline and the final step is to use CodeDeploy to update an AWS Lambda function. As a DevOps Engineering Lead at the company, you have decided that for every deployment, the new Lambda function must sustain a small amount of traffic for 10 minutes and then shift all the traffic to the new function. It has also been decided that safety must be put in place to automatically roll-back if the Lambda function experiences too many crashes.
* Choose a deployment configuration of LambdaAllAtOnce
* Create a CloudWatch Alarm on the Lambda CloudWatch metrics and associate it with the CodeDeploy deployment
* Create a CloudWatch Event for the Lambda Deployment Monitoring and associate it with the CodeDeploy deployment
* Choose a deployment configuration of LambdaCanary10Percent10Minutes
* Choose a deployment configuration of LambdaLinear10PercentEvery10Minutes

### Question 9:
As a DevOps Engineer at an IT company, you have deployed a web application with a health check that currently checks if the application is running actively. The application is running in an ASG and the ALB health check integration is turned on. Recently your application has had issues with connecting to a backend database and as such the users of your website were experiencing issues accessing your website through the faulty instances.
* Enhance the health check so that the return status code corresponds to the connectivity to the database
* Enhance the Health Check to report a JSON document that contains the health status of the connectivity to the database. Tune the ALB health check to look for a specific string in the health check result using a RegEx
* Include the health check in a Route 53 record so that users going through the ALB are not routed to the unhealthy instances
* Migrate the application to Elastic Beanstalk and enable advanced health monitoring

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 10:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

# Exam 2

### Question 1:
The development team at a social media company is using AWS CodeCommit to store code. As a Lead DevOps Engineer at the company, you have defined a company-wide rule so that the team should not be able to push to the master branch. You have added all the developers in an IAM group developers and attached the AWS managed IAM policy arn:aws:iam::aws:policy/AWSCodeCommitPowerUser to the group. This policy provides full access to AWS CodeCommit repositories but does not allow repository deletion, however, your developers can still push to the master branch.
* Include a CodeCommit repository policy on each repository with an explicit Deny for codecommit:GitPush
* Include a git commit pre-hook that invokes a Lambda function and checks if the push is done to master
* Add a new IAM policy attached to the group to Deny codecommit:GitPush with a condition on the master branch
* Modify the AWS managed IAM policy attached to the group to Deny codecommit:GitPush with a condition on the master branch

### Question 2:
An e-commerce company is managing its entire application stack and infrastructure using AWS OpsWorks Stacks. The DevOps team at the company has noticed that a lot of instances have been automatically replaced in the stack and the team would henceforth like to be notified via Slack notifications when these events happen.
* Create a CloudWatch Events rule for aws.opsworks and set the initiated_by field to auto-scaling. Target a Lambda function that will send notifications out to the Slack channel
* Subscribe your OpsWorks auto-healing notifications to an SNS topic. Subscribe a Lambda function that will send notifications out to the Slack channel
* Create a CloudWatch Events rule for aws.opsworks and set the initiated_by field to auto-scaling. Enable the CloudWatch Event Slack integration for sending out the notifications
* Create a CloudWatch Events rule for aws.opsworks and set the initiated_by field to auto-healing. Target a Lambda function that will send notifications out to the Slack channel

### Question 3:
You are working as a DevOps Engineer at an e-commerce company and have a deployed a Node.js application on Elastic Beanstalk. You would like to track error rates and specifically, you need to ensure by looking at the application log, that you do not have more than 100 errors in a 5 minutes interval. In case you are getting too many errors, you would like to be alerted via email.
* Create a CloudWatch Logs Metric Filter and assign a CloudWatch Metric. Create a CloudWatch Alarm linked to the metric and use SNS as a target. Create an email subscription on SNS
* Use the Elastic Beanstalk Health Metrics to monitor the application health and track the error rates. Create a CloudWatch alarm on top of the metric and use SNS as a target. Create an email subscription on SNS
* Create a CloudWatch Logs Metric Filter with a target being a CloudWatch Alarm. Make the CloudWatch Alarm use SNS as a target. Create an email subscription on SNS
* Implement custom logic in your Node.js application to track the number of errors it has received in the last 5 minutes. In case the number exceeds the threshold, use the SetAlarmState API to trigger a CloudWatch alarm. Make the CloudWatch Alarm use SNS as a target. Create an email subscription on SNS

### Question 4:
The DevOps team at an auditing firm has deployed its flagship application on Elastic Beanstalk that processes invoices uploaded by customers in CSV form. The invoices can be quite big, with up to 10MB and 1,000,000 records total. Processing is CPU intensive which results in slowing down the application. Customers are sent an email when the processing is done, through the use of a cron job. The auditing firm has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a separate Beanstalk environment that's a worker environment and processes invoices through an SQS queue. The invoices are uploaded into S3 and a reference to it is sent to the SQS by the web tier. The worker tier processes these files. A cron job defined using the cron.yml file will send out the emails
* Create a separate Beanstalk environment that's a worker environment and processes invoices through an SQS queue. The invoices are uploaded into S3 and a reference to it is sent to the SQS by the web tier. The worker tier processes these files. A cron job defined using the cron.yml file on the web tier will send out the emails
* Create a separate Beanstalk tier within the same environment that's a worker configuration and processes invoices through an SQS queue. The invoices are directly sent into SQS after being gzipped by the web tier. The workers process these files. A cron job defined using the cron.yml file on the web tier will send out the emails
* Create a separate Beanstalk tier within the same environment that's a worker configuration and processes invoices through an SQS queue. The invoices are directly sent into SQS after being gzipped by the web tier. The workers process these files. A cron job defined using the cron.yml file will send out the emails

### Question 5:
An analytics company is capturing metrics for its AWS services and applications using CloudWatch metrics. It needs to be able to go back up to 7 years in time for visualizing these metrics due to regulatory requirements. As a DevOps Engineer at the company, you have been tasked with designing a solution that will help the company comply with the regulations.
* Create a Kinesis Firehose subscription to your CloudWatch metrics stream. Send all the data into S3 using Firehose, and create a QuickSight dashboard to visualize the metrics. Use Athena to query for specific time ranges
* Create a CloudWatch dashboard on top of CloudWatch metrics. Enable 'Extended Retention' on CloudWatch metrics, and implement an AWS Config rule that checks for this setting. If the AWS Config rule is non-compliant, use an Auto Remediation to turn it back on
* Create a CloudWatch event rule to trigger every 15 minutes. The target of the rule should be a Lambda Function that will run an API call to export the metrics and put them in S3. Create a CloudWatch dashboard on top of the metrics in S3
* Create a CloudWatch event rule to trigger every 15 minutes. The target of the rule should be a Lambda Function that will run an API call to export the metrics and put them in Amazon ES. Create a Kibana dashboard on top to visualize the metrics

### Question 6:
A data analytics company would like to create an automated solution to be alerted in case of EC2 instances being under-utilized for over 24 hours in order to save some costs. The solution should require a manual intervention of an operator validating the assessment before proceeding for instance termination.
* Enable Trusted Advisor and ensure the check for low-utilized EC2 instances are on. Create a CloudWatch Event that tracks the events created by Trusted Advisor and use a Lambda Function as a target for that event. The Lambda function should trigger an SSM Automation document with a manual approval step. Upon approval, the SSM document proceeds with the instance termination
* Create a CloudWatch Alarm tracking the minimal CPU utilization across all your EC2 instances. Connect the CloudWatch Alarm to an SNS topic and use the Lambda Function as a subscriber to the SNS topic. The Lambda function should trigger an SSM Automation document with a manual approval step. Upon approval, the SSM document proceeds with the instance termination
* Enable Trusted Advisor and ensure the check for low-utilized EC2 instances are on. Connect Trusted Advisor to an SNS topic for that check and use a Lambda Function as a subscriber to the SNS topic. The Lambda function should trigger an SSM Automation document with a manual approval step. Upon approval, the SSM document proceeds with the instance termination
* Create a CloudWatch Event rule that triggers every 5 minutes and use a Lambda function as a target. The Lambda function should issue API calls to AWS CloudWatch Metrics and store the information in DynamoDB. Use a DynamoDB Stream to detect a stream of the low-utilized event for a period of 24 hours and trigger a Lambda function. The Lambda function should trigger an SSM Automation document with a manual approval step. Upon approval, the SSM document proceeds with the instance termination

### Question 7:
An online coding platform wants to fully customize the build tasks and automatically run builds concurrently to take the pain out of managing the build environments. The DevOps team at the company wants to use CodeBuild for all build-tasks and would like the artifacts created by CodeBuild to be named based on the branch being tested. The team wants this solution to be scalable to newer branches with a minimal amount of rework.
* Create a buildspec.yml file that will look for the environment variable CODEBUILD_SOURCE_VERSION at runtime. Use the variable in the artifacts section of your buildspec.yml file
* Create a buildspec.yml file that will look for the environment variable BRANCH_NAME at runtime. For each existing branch and new branch, create a separate CodeBuild and set the BRANCH_NAME variable accordingly. Use the variable in the artifacts section of your buildspec.yml file
* Create a unique buildspec.yml file that will be the same for each branch and will name the artifacts the same way. When the artifact is uploaded into S3, create an S3 Event that will trigger a Lambda function that will issue an API call against CodeBuild, extract the branch name from it and rename the file on S3
* Create a buildspec.yml file that will be different for every single branch. Create a new CodeBuild for each branch. Upon adding a new branch, ensure to edit the buildspec.yml file

### Question 8:
As a DevOps Engineer at an IT company, you are looking to create a daily EBS backup workflow. That workflow must take an EBS volume, and create a snapshot from it. When the snapshot is created, it must be copied to another region. In case the other region is unavailable because of a disaster, then that backup should be copied to a third region. An email address must be notified of the final result. There's a requirement to keep an audit trail of all executions as well.
* Create an AWS Step Function. Implement each step as a Lambda function and add failure logic between the steps to deal with conditional cases
* Create an SSM Automation that will perform each action. Add failure logic between steps to deal with conditional cases
* Create an EC2 instance in the region where the EBS volume is. Create a CRON script that will invoke a Python script that performs all the steps and logic outlined above. For each step completion, write metadata to a DynamoDB table
* Create a CloudWatch Event rule that gets triggered every day. It triggers a Lambda function written in Python that performs all the steps and logic outlined above. Analyze the history of execution using AWS Config

### Question 9:
An e-commerce company has deployed its flagship application in two Auto Scaling groups (ASGs) and two Application Load Balancers (ALBs). You have a Route 53 record that points to the ALB+ASG group where the application has been the most recently deployed. Deployments are alternating between the two groups, and every time a deployment happens it is done on the non-active ALB+ASG group. Finally, the Route53 record is updated. It turns out that some of your clients are not behaving correctly towards the DNS record and thus making requests to the inactive ALB+ASG group.
* Deploy a set of NGINX proxy onto each application instance so that if requests are made through the inactive ALB, they are proxied onto the correct ALB
* Deploy the application to Elastic Beanstalk under two environments. To do a deployment, deploy to the older environment, then perform a CNAME swap
* Remove one ALB and keep the two ASG. When new deployments happen, deploy to the older ASG, and then swap the target group in the ALB rule. Keep the Route53 record pointing to the ALB
* Change the TTL of the Route53 to 1 minute before doing a deployment. Do the deployment and then increase the TTL back to the old value

### Question 10:
A multi-national retail company is planning for disaster recovery and needs the data to be stored in Amazon S3 in two different regions that are in different continents. The data is written at a high rate of 10000 objects per second. For regulatory reasons, the data also needs to be encrypted in transit and at rest. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a bucket policy to create a condition for Denying any request that is "aws:SecureTransport": "false". Encrypt the objects at rest using SSE-S3. Setup Cross-Region Replication
* Create a bucket policy to create a condition for Denying any request that is "aws:SecureTransport": "false". Encrypt the objects at rest using SSE-KMS. Setup Cross-Region Replication
* Create a bucket policy to create a condition for Denying any request that is "aws:SecureTransport": "true". Encrypt the objects at rest using SSE-S3. Setup Cross-Region Replication
* Create a bucket policy to create a condition for Denying any request that is "aws:SecureTransport": "true". Encrypt the objects at rest using SSE-KMS. Setup Cross-Region Replication

### Question 11:
As a DevOps Engineer at an e-commerce company, you have deployed a web application in an Auto Scaling group (ASG) that is being distributed by an Application Load Balancer (ALB). The web application is using RDS Multi-AZ as a back-end and has been experiencing some issues to connect to the database. The health check implemented in the application currently returns an un-healthy status if the application cannot connect to the database. The ALB / ASG health check integration has been enabled, and therefore the ASG keeps on terminating instances right after they're done booting up.
* Create an autoscaling hook for instance termination. Troubleshoot the instance while it is in the Terminating:Wait state
* Enable termination protection for EC2
* Suspend the Launch process
* Set an instance in Standby right after it has launched

### Question 12:
A 3D modeling company would like to deploy applications on Elastic Beanstalk with support for various programming languages with predictable and standardized deployment strategies. Some of these languages are supported (such as Node.js, Java, Golang) but others such as Rust are not supported. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a custom platform for each language that is not supported. Package each application in S3 before deploying to Elastic Beanstalk
* Package each application as a standalone AMI that contains the OS, the application runtime and the application itself. To update a Beanstalk environment, provide a new AMI
* Run Opsworks on top of Elastic Beanstalk to bring the missing compatibility layer
* Deploy to Elastic Beanstalk using a Multi-Docker container configuration. Package each application as a Docker container in ECR

### Question 13:
A data intelligence and analytics company enables publishers to measure, analyze, and improve the impact of the advertising across their range of online deliverables. The DevOps team at the company wants to use CodePipeline to deploy code from CodeCommit with CodeDeploy. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create an EC2 instance with an IAM role giving access to the CodeCommit repository where CodeDeploy is deploying from. CodeDeploy will install the agent on the EC2 instance
* Create an EC2 instance with an IAM user access credentials giving access to the CodeCommit repository where CodeDeploy is deploying from. Ensure that the EC2 instance also has the CodeDeploy agent installed. Tag the instance to have it part of a deployment group
* Create an EC2 instance with an IAM role giving access to the S3 bucket where CodeDeploy is deploying from. Ensure that the EC2 instance also has the CodeDeploy agent installed. Tag the instance to have it part of a deployment group
* Create an EC2 instance with an IAM user access credentials giving access to the S3 bucket where CodeDeploy is deploying from. Ensure that the EC2 instance also has the CodeDeploy agent installed. Tag the instance to have it part of a deployment group

### Question 14:
The DevOps team at a financial services company is deploying the flagship application in highly available mode using Elastic Beanstalk which has created an ASG and an ALB. The team has also specified a .ebextensions file to create an associated DynamoDB table. As a DevOps Engineer in the team, you would like to perform an update to the application but you need to make sure the DNS name won't change and that no new resources will be created. The application needs to remain available during the update.
* Use a rolling update with 20% at a time
* Use immutable
* Use a blue/green deployment and swap CNAMEs
* Use in-place

### Question 15:
A multi-national retail company is operating a multi-account strategy using AWS Organizations. Each account produces logs to CloudWatch Logs and the company would like to aggregate these logs under a single centralized account for archiving purposes. It needs the solution to be secure and centralized. The target destination for the logs should have little to no provisioning on the storage side.
* Create a log destination in the centralized account, and create a log subscription on that destination. Create a Kinesis Streams and subscribe it to the destination. Create a Kinesis Firehose delivery stream and subscribe it to the Kinesis Stream. The target of the Kinesis Firehose should be Amazon ES
* Create a log destination in the centralized account, and create a log subscription on that destination. Create a Lambda function on that log subscription, and implement a script to send the data to Amazon ES
* Create a log destination in the centralized account, and create a log subscription on that destination. Create a Kinesis Streams and subscribe it to the destination. Create a Kinesis Firehose delivery stream and subscribe it to the Kinesis Stream. The target of the Kinesis Firehose should be Amazon S3
* Create a log destination in the centralized account, and create a log subscription on that destination. Create a Kinesis Firehose delivery stream and subscribe it to the log destination. The target of Kinesis Firehose should be Amazon S3

### Question 16:
The DevOps team at a presentation software company is deploying their flagship application using Elastic Beanstalk. The application is deployed using a Deploy stage in a CodePipeline pipeline. The technical requirements mandate changing the configuration of the Application Load Balancer tied to Elastic Beanstalk by adding an HTTP to HTTPS redirection rule.
* Using the EB CLI, create a .elasticbeanstalk/saved_configs/config.yml, and specify the rules for the key aws:elbv2:listener:default. Run a deploy using the EB CLI from your computer onto the Elastic Beanstalk Environment
* Create a file named .ebextensions/alb.config in your code repository and add a container_commands block for which you will specify a container command that will run in leader_only mode. The EC2 instance will issue an API call to the Load Balancer to add the redirection rule
* Using the EB CLI, create a .elasticbeanstalk/saved_configs/config.yml, and specify the rules for the key aws:elbv2:listener:default. Configure CodePipeline to deploy to Elastic Beanstalk using the EB CLI and push the code
* Create a file named .ebextensions/alb.config in your code repository and add an option_settings block for which you will specify the Rules for the key aws:elbv2:listener:default. Push your code and let the CodePipeline run

### Question 17:
The compliance department at a Wall Street trading firm has hired you as an AWS Certified DevOps Engineer Professional to help with several strategic DevOps initiatives. The department has asked you to regularly generate the list of all the software packages installed on the EC2 instances. The solution needs to be able to extend to future instances in the AWS account and send notifications if the instances are not set up correctly to track their software.
* Create a CloudWatch Event rule to trigger a Lambda function on an hourly basis. Do a comparison of the instances that are running in EC2 and those tracked by SSM
* Install the SSM agent on the instances. Run an SSM Inventory to collect the metadata and send them to Amazon S3
* Use an SSM Run Command to have the SSM service find which instances are not currently tracked by SSM
* Install the SSM agent on the instances. Run an SSM Automation during maintenance windows to get the list of all the packages using yum list installed. Write the output to Amazon S3
* Use AWS Inspector to track the installed package list on your EC2 instances. Visualize the metadata directly in the AWS Inspector Insights console

### Question 18:
A health-care services company has strong regulatory requirements and it has come to light recently that some of the EBS volumes have not been encrypted. It is necessary for the company to monitor and audit compliance over time and alert the corresponding teams if unencrypted EBS volumes are detected.
* Create an AWS Config custom rule checking for the EC2 instances, and their EBS attachments. Connect the rule to an SNS topic to provide alerting
* Create an AWS Lambda Function that is triggered by a CloudWatch Event rule. The rule is monitoring for new EBS volumes being created. The Lambda function should send a notification to SNS in case of a compliance check
* Create an AWS Config managed rule checking for EBS volume encryption. Connect the rule to an SNS topic to provide alerting
* Create an AWS Config managed rule checking for EBS volume encryption. Use a CloudWatch Event rule to provide alerting

### Question 19:
The DevOps team at your company is using CodeDeploy to deploy new versions of a Lambda function after it has passed a CodeBuild check via your CodePipeline. Before deploying, the CodePipeline has a step in which it optionally kickstarts a restructuring of files on an S3 bucket that is forward compatible. That restructuring is done using a Step Function execution which invokes a Fargate task. The new Lambda function cannot work until the restructuring task has fully completed.
* In your appspec.yml file, include a BeforeAllowTraffic hook that checks on the completion of the Step Function execution
* Enable Canary Deployment in CodeDeploy so that only a fraction of the service is served by the new Lambda function while the restructuring is happening
* In your appspec.yml file, include an AfterAllowTraffic hook that checks on the completion of the Step Function execution
* Include an extra step in the Step Function to signal to CodeDeploy the completion of the restructuring and serve new traffic to the new Lambda function

### Question 20:
A cyber-security company has had a dubious distinction of their own AWS account credentials being put in public GitHub repositories. The company wants to implement a workflow to be alerted in case credentials are leaked, generate a report of API calls made recently using the credentials, and de-activate the credentials. All executions of the workflow must be auditable.
* Create a CloudWatch Event checking for AWS_RISK_CREDENTIALS_EXPOSED in the CloudTrail Service. Trigger a Step Function workflow that will issue API calls to IAM, CloudTrail, and SNS to achieve the desired requirements
* Create a CloudWatch Event checking for AWS_RISK_CREDENTIALS_EXPOSED in the Health Service. Trigger a Lambda Function that will issue API calls to IAM, CloudTrail, and SNS to achieve the desired requirements
* Create a CloudWatch Event checking for AWS_RISK_CREDENTIALS_EXPOSED in the CloudTrail Service. Trigger a Lambda Function workflow that will issue API calls to IAM, CloudTrail, and SNS to achieve the desired requirements
* Create a CloudWatch Event checking for AWS_RISK_CREDENTIALS_EXPOSED in the Health Service. Trigger a Step Function workflow that will issue API calls to IAM, CloudTrail, and SNS to achieve the desired requirements

### Question 21:
As part of the CICD pipeline, a DevOps Engineer is performing a functional test using a CloudFormation template that will later get deployed to production. That CloudFormation template creates an S3 bucket and a Lambda function which transforms images uploaded into S3 into thumbnails. To test the Lambda function, a few images are automatically uploaded and the thumbnail output is expected from the Lambda function on the S3 bucket. As part of the clean-up of these functional tests, the CloudFormation stack is deleted, but right now the delete fails.
* A StackPolicy prevents the CloudFormation template to be deleted. Clear the Stack Policy and try again
* The S3 bucket contains files and therefore cannot be deleted by CloudFormation. Create an additional Custom Resource backed by a Lambda function that performs a clean-up of the bucket
* The S3 bucket contains files and therefore cannot be deleted by CloudFormation. Add the property Delete: Force to your CloudFormation template so that the S3 bucket is emptied before being deleted
* The Lambda function is still using the S3 bucket and CloudFormation cannot, therefore, delete the S3 bucket. Place a WaitCondition on the Lambda function to fix the issue

### Question 22:
As the Lead DevOps Engineer at a retail company, you have a Spring boot web application running in an Auto Scaling group and behind an Application Load Balancer. You must collect the logs before an instance is terminated to perform log analytics later on. It's also necessary to collect all the access logs. The analysis of these logs should be performed at a minimal cost, and only need to be run from time to time.
* Analyze the logs using an EMR cluster
* Enable Access Logs at the Target Group level
* Create an Auto Scaling Group Lifecycle Hook for the terminate action. Create a CloudWatch Event rule for that lifecycle hook and invoke a Lambda function. The Lambda function should use an SSM Run Command to extract the application logs and store them in S3
* Analyze the logs using AWS Athena
* Enable Access Logs at the Application Load Balancer level
* Create an Auto Scaling Group Lifecycle Hook for the terminate action. Create a CloudWatch Event rule for that lifecycle hook and invoke a Lambda function. The Lambda function should use an SSM Run Command to install the CloudWatch Logs Agent and push the applications logs in S3

### Question 23:
As a DevOps Engineer at an IT company, you have deployed a web application with a health check that currently checks if the application is running actively. The application is running in an ASG and the ALB health check integration is turned on. Recently your application has had issues with connecting to a backend database and as such the users of your website were experiencing issues accessing your website through the faulty instances.
* Enhance the health check so that the return status code corresponds to the connectivity to the database
* Migrate the application to Elastic Beanstalk and enable advanced health monitoring
* Include the health check in a Route 53 record so that users going through the ALB are not routed to the unhealthy instances
* Enhance the Health Check to report a JSON document that contains the health status of the connectivity to the database. Tune the ALB health check to look for a specific string in the health check result using a RegEx

### Question 24:
A graphics design company is experimenting with a new feature for an API and the objective is to pass the field "color" in the JSON payload to enable this feature. The new Lambda function should treat "color": "none" as a request from an older client. The company would like to only have to manage one Lambda function in the back-end while being able to support both old and new clients. The API Gateway API is currently deployed on the v1 stage. Old clients include Android applications which may take time to be updated. The technical requirements mandate that the solution should support the old clients for years to come.
* Create a new Lambda function version and release it. Use API Gateway mapping documents to add a default value "color": "none" to the JSON request being passed on your API Gateway stage
* Create a new Lambda function version and release it. Create a new API Gateway Stage and deploy it to the v2 stage. Both use the same Lambda function as a backing route for the v1 and v2 stages. Add a static mapping on the v1 route to add "color": "none" on requests
* Enable API Gateway v1 API caching and delete the v1 AWS Lambda function. Deploy a v2 API Gateway backed by a newly released v2 AWS Lambda function. Add an API Gateway stage variable to enable the "color": "none" default value
* Create a new Lambda function version and release it as a separate v2 function. Create a new API Gateway Stage and deploy it to the v2 stage. The v1 API gateway stage points to the v1 Lambda function and the v2 API Gateway stage to the v2 Lambda function. Implement redirection from the Lambda v1 function to the Lambda v2 function when the request is missing the "color" field

### Question 25:
An industrial appliances company would like to take advantage of AWS Systems Manager to manage their on-premise instances and their EC2 instances. This will allow them to run some SSM RunCommand across their hybrid fleet. The company would also like to effectively manage the size of the fleet. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution to address this requirement.
* Create an IAM Service Role for each instance to be able to call the AssumeRole operation on the SSM service. Generate a unique activation code and activation ID for each on-premise servers. Use these credentials to register your on-premise servers. They will appear with the prefix 'i-' in your SSM console
* Create an IAM User for each on-premise server to be able to call the AssumeRole operation on the SSM service. Using the Access Key ID and the Secret Access Key ID, use the AWS CLI to register your on-premise servers. They will appear with the prefix 'mi-' in your SSM console
* Create an IAM Service Role for instances to be able to call the AssumeRole operation on the SSM service. Generate an activation code and activation ID for your on-premise servers. Use these credentials to register your on-premise servers. They will appear with the prefix 'mi-' in your SSM console
* Create an IAM User for all on-premise servers to be able to call the AssumeRole operation on the SSM service. Using the Access Key ID and the Secret Access Key ID, use the AWS CLI to register your on-premise servers. They will appear with the prefix 'i-' in your SSM console

### Question 26:
A social media company has multiple EC2 instances that are behind an Auto Scaling group (ASG) and you would like to retrieve all the log files within the instances before they are terminated. You would like to also build a metadata index of all the log files so you can efficiently find them by instance id and date range.
* Create a DynamoDB table with a primary key of instance-id and a sort key of datetime
* Create a termination hook for your ASG and create a CloudWatch Events rule to trigger an AWS Lambda function. The Lambda function should invoke an SSM Run Command to send the log files from the EC2 instance to CloudWatch Logs. Create a log subscription to send it to Firehose and then S3
* Create a termination hook for your ASG and create a CloudWatch Events rule to trigger an AWS Lambda function. The Lambda function should invoke an SSM Run Command to send the log files from the EC2 instance to S3
* Create a Lambda function that is triggered by CloudWatch Events for PUT. Write to the DynamoDB table
* Create a DynamoDB table with a primary key of datetime and a sort key of instance-id
* Create a Lambda function that is triggered by S3 events for PUT. Write to the DynamoDB table

### Question 27:
A retail company uses the open-source tool Jenkins on its on-premise infrastructure to perform CICD. It has decided to move to AWS and take advantage of the elasticity properties of the cloud provider to have more efficient workloads. It needs to ensure the Jenkins setup is highly available, fault-tolerant and also elastic to perform builds. The company has hired you as an AWS Certified DevOps Engineer Professional to build the most cost-effective solution for this requirement.
* Deploy Jenkins as a multi-master setup across multiple AZ. Create an Auto Scaling Group made of EC2 instances that are Jenkins slave. Configure Jenkins to launch build on these slaves
* Deploy Jenkins as a multi-master setup across one AZ, managed by an Auto Scaling Group. Configure Jenkins to launch build on these slaves
* Deploy Jenkins as a multi-master setup across multiple AZ. Enable the CodeBuild Plugin for Jenkins so that builds are launched as CodeBuild builds
* Deploy Jenkins as a multi-master setup across one AZ, managed by an Auto Scaling Group. Enable the CodeBuild Plugin for Jenkins so that builds are launched as CodeBuild builds

### Question 28:
An e-commerce company has deployed a Spring application on Elastic Beanstalk running the Java platform. As a DevOps Engineer at the company, you are referencing an RDS PostgreSQL database through an environment variable so that your application can use it for storing its data. You are using a library to perform a database migration in case the schema changes. Upon deploying updates to Beanstalk, you have seen the migration fail because all the EC2 instances running the new version try to run the migration on the RDS database.
* Create an .ebextensions/db-migration.config file in your code repository and set a container_commands block. Set your migration command there and use the leader_only: true attribute
* Create an .ebextensions/db-migration.config file in your code repository and set a commands block. Set your migration command there and use the lock_mode: true attribute
* Create an .ebextensions/db-migration.config file in your code repository and set a commands block. Set your migration command there and use the leader_only: true attribute
* Create an .ebextensions/db-migration.config file in your code repository and set a container_commands block. Set your migration command there and use the lock_mode: true attribute

### Question 29:
A cyber forensics company would like to ensure that CloudTrail is always enabled in its AWS account. It also needs to have an audit trail of the status for CloudTrail. In the case of compliance breaches, the company would like to automatically resolve them.
* Place all your AWS IAM users under an IAM group named 'everyone'. Create an IAM deny policy on that group to prevent users from using the DeleteTrail API. Create a CloudWatch Event rule that will trigger a Lambda function every 5 minutes. That Lambda function will check if CloudTrail is enabled using an API call and enable it back if necessary
* Create a CloudWatch Event rule that will trigger a Lambda function every 5 minutes. That Lambda function will check if CloudTrail is enabled using an API call and enable it back if necessary
* Place all your AWS IAM users under an IAM group named 'everyone'. Create an IAM deny policy on that group to prevent users from using the DeleteTrail API. Create an AWS Config rule that tracks if every user is in that IAM group. Create a CloudWatch Event rule to get alerted in case of breaches, and trigger a Lambda function that will add users to the 'everyone' group automatically
* Create an AWS Config rule to track if CloudTrail is enabled. Create a CloudWatch Event rule to get alerted in case of breaches, and trigger a Lambda function that will re-enable CloudTrail

### Question 30:
An ed-tech company has created a paid-per-use API using API Gateway. This API is available at http://edtech.com/api/v1. The website's static files have been uploaded in S3 and now support a new API route http://edtech.com/api/v1/new-feature if available. Your team has decided it is safer to send a small amount of traffic to that route first and test if the metrics look okay. Your API gateway routes are backed by AWS Lambda.
* Create a new Lambda function alias. Enable Canary deployments on the Lambda alias. Deploy the new API to the Lambda alias and assign a small amount of traffic to the canary Lambda version. Enable new route redirection for AWS Lambda and track metrics data using Amazon ES
* Create a new Lambda function alias. Enable Canary deployments on the Lambda alias. Deploy the new API to the Lambda alias and assign a small amount of traffic to the canary Lambda version. Enable new route redirection for AWS Lambda and track metrics data using CloudWatch
* Create a new API Gateway Stage. Enable Canary deployments on the v1 stage. Deploy the new stage to the v1 stage and assign a small amount of traffic to the canary stage. Track metrics data using Amazon ES
* Create a new API Gateway Stage. Enable Canary deployments on the v1 stage. Deploy the new stage to the v1 stage and assign a small amount of traffic to the canary stage. Track metrics data using CloudWatch

### Question 31:
A financial services company has a solution in place to track all the API calls made by users, applications, and SDK within the AWS account. Recently, it has experienced a hack and could find a user amongst the logs that did some compromising API calls. The company wants to know with 100% certainty that the log files represent the correct sequence of events and have not been altered. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Turn on API calls logging using AWS CloudTrail. Deliver the logs in an S3 bucket and choose a lifecycle policy that archives file right away in Glacier. Implement a Glacier Vault Lock policy
* Turn on AWS account configuration tracking using AWS Config. Deliver the logs in an S3 bucket and choose a lifecycle policy that archives the files right away in Glacier. Implement a Glacier Vault Lock policy
* Turn on API calls logging using AWS CloudTrail. Deliver the logs in an S3 bucket, and use the log verification integrity API call to verify the log file
* Turn on AWS account configuration tracking using AWS Config. Deliver the configuration logs into S3 and use the log verification integrity API to verify the log files

### Question 32:
As a DevOps Engineer at a social media company, you have implemented a CICD pipeline that takes code from a CodeCommit repository, builds it using CodeBuild thanks to the instructions in the local Dockerfile, and then pushes to ECR at 123456789.dkr.ecr.region.amazonaws.com/my-web-app. The last step of your CICD pipeline is to deploy to the application to your ECS cluster. It seems that while you do so, the application is only partly updated on some ECS instances which are running an older version of your image. You have found that terminating the instance or clearing the local Docker cache fixes the issue, but would like to implement something more robust.
* When creating a new task definition for your ECS service, ensure to add the latest tag in the full image name so that ECS pulls the correct image every time
* After the deploy step in CodePipeline is done, include a Custom Step using a Lambda function that triggers an AWS Lambda function. That function will SSH onto your ECS instances and clear the local Docker cache and stop the task
* After the deploy step in CodePipeline is done, include a Custom Step using a Lambda function that triggers an SSM Run Command. That command will clear the local Docker cache and stop the task
* When creating a new task definition for your ECS service, ensure to add the sha256 hash in the full image name so that ECS pulls the correct image every time

### Question 33:
A multi-national retail company is in the process of capturing all of its infrastructure as code using CloudFormation. The infrastructure inventory is huge and will contain a networking stack, an application stack, a data stack, and so on. Some teams are ready to move ahead with the process while others are lagging, and there is a desire to keep all the infrastructure version controlled.
* Create one template per logical element of your infrastructure. Create a master stack that contains all the other stacks as a nested template. Deploy the master template once using CloudFormation and then update the nested stacks individually as new CloudFormation code is created
* Create one template per logical element of your infrastructure. Deploy them using CloudFormation as they are ready. Use outputs and exports to reference values in the stacks. Keep each file separately in a version-controlled repository
* Create one template per logical element of your infrastructure. Create a master stack that contains all the other stacks as a nested template. Deploy the master template using CloudFormation every-time a nested stack template is updated in version control
* Create one master template that contains all the stacks in your infrastructure. Collaborate on that template using pull requests and merges to the master branch in your code repository. Deploy the master template every-time it is updated

### Question 34:
A multi-national retail company has defined tagging guidelines and standard for all its resources in AWS and would like to create a dashboard to visualize the compliance of all the resources with the ability to find out the non-compliant resources. The company has hired you as an AWS Certified DevOps Engineer Professional to develop a solution for this requirement.
* Use AWS Service Catalog to get an inventory of all the resources in your account. Use the integrated dashboard feature to track compliance
* Track all your resources with AWS CloudTrail. Output the data in S3 and create a Quicksight dashboard
* Use SSM to track resource groups without tags. Export that data using SSM inventory into S3, and build a QuickSight dashboard
* Use AWS Config to track resources in your account. Use SNS to stream changes to a Lambda function that writes to S3. Create a QuickSight dashboard on top of it

### Question 35:
A global financial services company manages over 100 accounts using AWS Organizations and it has recently come to light that several accounts and regions did not have AWS CloudTrail enabled. It also wants to be able to track the compliance of the CloudTrail enablement as a dashboard, and automatically be alerted in case of issues. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create one CloudFormation template in a centralized account to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create an SNS topic to get notifications when compliance is breached, and subscribe a Lambda function to it, that will send out these notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create one CloudFormation template in a centralized account to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create a CloudWatch Event to generate events when compliance is breached, and subscribe a Lambda function to it, that will send out notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy it in all your accounts and regions under the AWS organization. Create another StackSet to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance across all the other accounts. Create an SNS topic to get notifications when compliance is breached, and subscribe a Lambda function to it, that will send out these notifications
* Create a CloudFormation template to enable CloudTrail. Create a StackSet and deploy that StackSet in all your accounts and regions under the AWS organization. Create another CloudFormation StackSet to enable AWS Config, and create a Config rule to track if CloudTrail is enabled. Create an AWS Config aggregator for a centralized account to track compliance. Create a CloudWatch Event to generate events when compliance is breached, and subscribe a Lambda function to it, that will send out notifications

### Question 36:
As a DevOps Engineer at a social media company, you have deployed your application in an Auto Scaling group (ASG) using CloudFormation. You would like to update the Auto Scaling Group to have all the instances reference the newly created launch configuration, which upgrades the instance type. Your ASG currently contains 6 instances and you need at least 4 instances to be up at all times.
* AutoScalingReplacingUpdate
* AutoScalingLaunchTemplateUpdate
* AutoScalingLaunchConfigurationUpdate
* AutoScalingRollingUpdate

### Question 37:
As part of your CodePipeline, you are running multiple test suites. Two are bundled as Docker containers and run directly on CodeBuild, while another one runs as a Lambda function executing Python code. All these test suites are based on HTTP requests and upon analyzing, these are found to be network bound, not CPU bound. Right now, the CodePipeline takes a long time to execute as these actions happen one after the other. They prevent the company from adding further tests. The whole pipeline is managed by CloudFormation.
* Increase the number of vCPU assigned to the CodeBuild builds and the RAM assigned to your Lambda function
* Enable CloudFormation StackSets to run the actions in parallel
* Change the runOrder of your actions so that they have the same value
* Migrate all the test suites to Jenkins and use the ECS plugin

### Question 38:
Your application is deployed on Elastic Beanstalk and you manage the configuration of the stack using a CloudFormation template. A new golden AMI is created every week and contains a hardened AMI that has all the necessary recent security patches. You have deployed over 100 applications using CloudFormation & Beanstalk this way and you would like to ensure the newer AMI used for EC2 instances is updated every week. There are no standardization or naming conventions made across all the CloudFormation templates.
* Store the Golden AMI id in an S3 object. Create a CloudFormation parameter that points to the S3 object, and is passed on to the configuration of the Elastic Beanstalk environment. Create a CloudWatch Event rule that is triggered every week that will launch a Lambda function. That Lambda function should trigger a refresh of all the CloudFormation templates using the UpdateStack API
* Store the Golden AMI id in an SSM Parameter Store parameter. Create a CloudFormation parameter that points to the SSM Parameter Store, and is passed on to the configuration of the Elastic Beanstalk environment. Create a CloudWatch Event rule that is triggered every week that will launch a Lambda function. That Lambda function should trigger a refresh of all the CloudFormation templates using the UpdateStack API
* Store the Golden AMI id in an SSM Parameter Store parameter. Create a CloudFormation parameter of type String, and is passed on to the configuration of the Elastic Beanstalk environment. Create a CloudWatch Event rule that is triggered every week that will launch a Lambda function. That Lambda function should fetch the parameter from the SSM Parameter Store and trigger a refresh of all the CloudFormation templates using the UpdateStack API while passing the new parameter
* Store the Golden AMI id in an S3 object. Create a CloudFormation mapping to contain the last value of the Golden AMI id. That mapping is passed on to the configuration of the Elastic Beanstalk environment. Create a CloudWatch Event rule that is triggered every week that will launch a Lambda function. That Lambda function should update the mapping section of every CloudFormation template using a YAML parser, upload the new templates to S3 and trigger a refresh of all the CloudFormation templates using the UpdateStack API while passing the new parameter

### Question 39:
The DevOps team at a leading bitcoin wallet and exchange services company is trying to deploy a CloudFormation template that contains a Lambda Function, an S3 bucket, an IAM role, and a DynamoDB table from CodePipeline but the team is getting an InsufficientCapabilitiesException.
* Enable the IAM Capability on the CodePipeline configuration for the Deploy CloudFormation stage action
* Update the CodePipeline IAM Role so it has permissions to create all the resources mentioned in the CloudFormation template
* Fix the CloudFormation template as there is circular dependency and CloudFormation does not have that capability
* Increase the service limits for your S3 bucket limits as you've reached it

### Question 40:
An IT company is creating an online booking system for hotels. The booking workflow that the company has implemented can take over 3 hours to complete as a manual verification step is required by a 3rd party provider to ensure big transactions are not fraudulent.
* Create the booking workflow in AWS Lambda. Enable public invocations of the Lambda functions so that clients can start the booking process. The Lambda function will wait for the service provider's response and then issue the status back to the client. Secure the calls using IAM
* Create the booking workflow in Step Functions. Create an API Gateway stage using a service integration with Step Functions. Secure your API using Cognito
* Create the booking workflow in Step Functions. Create an API Gateway stage using a service integration with AWS Lambda, which will, in turn, invoke the Step Function workflow. Secure your API using Cognito
* Create the booking workflow in AWS Lambda. Create an API Gateway stage using a service integration with AWS Lambda. The Lambda function will wait for the service provider response and then issue the status back to API Gateway. Secure your API using Cognito

### Question 41:
The DevOps team at a multi-national financial services company manages hundreds of accounts through AWS Organizations. As part of the security compliance requirements, the team must enforce the use of a security-hardened AMI in each AWS account. When a new AMI is created, the team wants to make sure new EC2 instances cannot be instantiated from the old AMI. Additionally, the team also wants to track and audit compliance of AMI usage across all the accounts.
* Create an AWS Lambda function in all the accounts using CloudFormation StackSets, which will check the AMI id of all the EC2 instances in the account. Give it an IAM role that allows it to publish messages to an SNS topic in the master account
* Create an AWS Config Custom Rule in all the accounts using CloudFormation StackSets. Report the rule's result using an AWS Config aggregation
* Create an AWS Automation document to create that AMI in a master account and share the AMI with the other accounts. When a new AMI is created, un-share the previous AMI and share the new one
* Create an AWS Automation document to create that AMI and deploy it to all the accounts using AWS CloudFormation StackSets. Run the Automation in all the accounts to have the AMI created locally
* Create an AWS Automation document to create that AMI in a master account and copy the AMI into the other accounts. When a new AMI is created, copy it as well

### Question 42:
An IT company is deploying a Python Flask based application and would like to ensure that it has a base AMI that contains the necessary Python runtime, as well as OS patches. That AMI must be used able to be referenced programmatically from across all regions in your account in a scalable way. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution to address this requirement.
* Create an SSM Automation document to create the AMI in a repeatable manner
* Use AWS Inspector to create a patched AMI using the latest working AMI
* Store the AMI ID in the SSM parameter store in one region, and create a Step Function that copies the value of that AMI ID across all the other regions. Use the same parameter store name so it can be re-used across regions
* Store the AMI ID in the SSM parameter store in one region, and have a Lambda function that copies the AMI across all the other regions, and stores the corresponding AMI ID in SSM. Use the same parameter store name so it can be re-used across regions
* Use AWS Lambda to create a patched AMI using the latest working AMI

### Question 43:
An e-commerce company would like to automate the patching of their hybrid fleet and distribute some patches through their internal patch repositories every week. As a DevOps Engineer at the company, you have been tasked to implement this most efficiently.
* Using SSM, implement a Custom Patch Baseline. Define a Maintenance window and include the Run Command RunPatchBaseline. Schedule the maintenance window with a weekly recurrence
* Using SSM, do a RunCommand to install the custom repositories in the OS' internal configuration files. Use the Default Patch Baseline. Define a Maintenance window and include the Run Command RunPatchBaseline. Schedule the maintenance window with a weekly recurrence
* Manage your instances with AWS OpsWorks. Define a maintenance window and define custom chef cookbooks for the 'configure' lifecycle hook that will patch the instances from the internal patch repositories. Schedule the window with a weekly recurrence
* Using SSM Parameter Store, configure the custom repositories in the OS' internal configuration files. Use the Default Patch Baseline. Define a Maintenance window and include the Run Command RunPatchBaseline. Schedule the maintenance window with a weekly recurrence

### Question 44:
As part of the CICD pipeline, the DevOps team at a retail company wants to deploy the latest application code to a staging environment and the team also wants to ensure it can execute an automated functional test suite before deploying to production. The code is managed via CodeCommit. Usually, the functional test suite runs for over two hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a CodePipeline pointing to the master branch of your CodeCommit repository and automatically deploy to a staging environment using CodeDeploy. After that stage, invoke a custom stage using a Lambda function that will invoke a Step Function execution. The Step Function will run the test suite. Create a CloudWatch Event Rule on the execution termination of your Step Function to invoke a Lambda function and signal CodePipeline the success or failure. If the stage doesn't fail, the last stage will deploy the application to production
* Create a CodePipeline pointing to the master branch of your CodeCommit repository and automatically deploy to a staging environment using CodeDeploy. After that stage, invoke a custom stage using a Lambda function that will run the test suite. If the stage doesn't fail, the last stage will deploy the application to production
* Create a CodePipeline pointing to the master branch of your CodeCommit repository and as a first stage run a CodeBuild build that will run the test suite against the staging environment. Upon passing, deploy to staging using CodeDeploy and if it succeeds, deploy to production
* Create a CodePipeline pointing to the master branch of your CodeCommit repository and automatically deploy to a staging environment using CodeDeploy. After that stage, invoke a CodeBuild build that will run the test suite. If the stage doesn't fail, the last stage will deploy the application to production

### Question 45:
A Big Data analytics company has deployed a stream processing application using KCL to read records from a Kinesis Stream. The application is running on one EC2 instance. It seems that the consuming application is lagging under a large load and therefore records are not processed in time and eventually dropped from the stream.
* Migrate the application to AWS Lambda
* Increase the number of shards in Kinesis to increase throughput
* Run the application in an Auto Scaling Group and scale based on the CloudWatch Metric MillisBehindLatest
* Increase the stream data retention period
* Decrease the numbers of shards in Kinesis to decrease the load

### Question 46:
Your company has adopted CodeCommit and forces developers to create new branches and create pull requests before merging the code to master. The development team lead reviewing the pull request needs high confidence in the quality of the code and therefore would like the CICD system to automatically build a Pull Request to provide a testing badge with a pass/fail status.
* Create a CloudWatch Event Rule that reacts to the creation and updates done to Pull Requests in the source repository. The target of that rule should be CodeBuild. Create a second CloudWatch Event rule to watch for CodeBuild build success or failure event and as a target invoke a Lambda function that will update the pull request with the Build outcome
* Create a CloudWatch Event Rule with a scheduled rate of 5 minutes that invokes a Lambda function. This function checks for the creation and updates done to Pull Requests in the source repository, and invokes CodeBuild when needed. The function waits for CodeBuild to be done and then updates the Pull Request with a message with the build outcome
* Create a CloudWatch Event Rule with a scheduled rate of 5 minutes that invokes a Lambda function. This function checks for the creation and updates done to Pull Requests in the source repository, and invokes CodeBuild when needed. Create a CloudWatch Event rule to watch for CodeBuild build success or failure event and as a target invoke a Lambda function that will update the pull request with the Build outcome
* Create a CloudWatch Event Rule that reacts to the creation and updates done to Pull Requests in the source repository. The target of that rule should be AWS Lambda. This function invokes CodeBuild and waits for CodeBuild to be done and then updates the Pull Request with a message with the build outcome

### Question 47:
Your company has adopted a git repository technology to store and have version control on the application code. Your company would like to make sure the production branch of the code is deployed to the production environment, but also would like to enable other versions of the code to be deployed to the development and staging environments for performing various kinds of user acceptance testing.
* Create a CodeCommit repository for the development code and create a CodePipeline pipeline that will deploy any changes to the master branch to the development and staging environment. Create a second CodeCommit repository and CodePipeline pipeline that will deploy changes from the production branch to the production environment after the code is merged through a pull request
* Create a CodeCommit repository for the development code and create a CodePipeline pipeline that will deploy any changes to the master branch to the development and staging environment. Create a second CodeCommit repository and CodePipeline pipeline that will deploy changes from the production branch to the production environment after a manual approval step has happened in the first CodePipeline
* Create a CodeCommit repository and create a CodePipeline pipeline that will deploy any changes to the master branch to the development and staging environment. Create a manual approval step after the deployment to staging to ensure the application is reviewed before being deployed to production in the last pipeline stage
* Create a CodeCommit repository and create a CodePipeline pipeline that will deploy any changes to the master branch to the development and staging environment. Create a second CodePipeline pipeline that will deploy changes to the production branch to the production environment after the code is merged through a pull request

### Question 48:
A retail company is storing the users' information along with their purchase history in a DynamoDB table and it has also enabled the DynamoDB Streams. Three use cases are implemented for this table: a Lambda function reads the stream to send emails for new users subscriptions, another Lambda function which sends an email after a user has done their first purchase and finally the last Lambda function which awards discounts to users every 10 purchase. When there is a high volume of data on your DynamoDB table, the Lambda functions are experiencing a throttling issue. As you plan on adding future Lambda functions to read from that stream, you need to update the existing solution.
* Create a DynamoDB DAX cluster to cache the reads
* Increase the RCUs on your DynamoDB table to avoid throttling issues
* Create a new Lambda function that will read from the stream and pass on the payload to SNS. Have the other three and upcoming Lambda functions directly read from the SNS topic
* Increase the memory on the Lambda function so that they have an increased vCPU allocation and process the data faster while making fewer requests to DynamoDB

### Question 49:
A gaming company would like to be able to receive near real-time notifications when the API call DeleteTable is invoked in DynamoDB.
* Enable DynamoDB Streams, and have a Lambda function consuming that stream. Send alerts to SNS whenever a record is being deleted
* Create a CloudTrail event filter and hook it up to a Lambda function. Use the Lambda function to send an SNS notification
* Enable CloudTrail. Create a CloudWatch Event rule to track an AWS API call via CloudTrail and use SNS as a target
* Send CloudTrail Logs to CloudWatch Logs and use an AWS Lambda function to be triggered on a CloudWatch Logs metrics filter. Use the Lambda function to send an SNS notification

### Question 50:
As the Lead DevOps Engineer at an e-commerce company, you would like to upgrade the major version of your MySQL database, which is managed by CloudFormation with AWS::RDS::DBInstance and setup using Multi-AZ.
* Create an RDS Read Replica in a CloudFormation template by specifying SourceDBInstanceIdentifier and wait for it to be created. Afterward, upgrade the RDS Read Replica EngineVersion to the next major version. Then promote the Read Replica and use it as your new master database
* Upgrade the RDS database by updating the EngineVersion to the next major version, then run an UpdateStack Operation
* Create an RDS Read Replica in a CloudFormation template by specifying SourceDBInstanceIdentifier and wait for it to be created. Afterward, upgrade the RDS Read Replica DBEngineVersion to the next major version. Then promote the Read Replica and use it as your new master database
* Upgrade the RDS database by updating the DBEngineVersion to the next major version, then run an UpdateStack Operation

### Question 51:
The DevOps team at a leading travel-booking services company is using a CloudFormation template to deploy a Lambda function. The Lambda function code is uploaded into S3 into a file named s3://my-bucket/my-lambda-code.zip by CodePipeline after having passed all the required build checks. CodePipeline then invokes the CloudFormation template to deploy the new code. The team has found that although the CloudFormation template successfully runs, the Lambda function is not updated.
* Enable S3 versioning and provide an S3ObjectVersion key
* Upload the code every time to a new S3 bucket
* Add a pause of 3 seconds before starting the CloudFormation job. This is an eventual consistency issue due to overwriting PUT
* Clear the Lambda cache with a Custom Job in CodePipeline before the CloudFormation step
* Enable the SAM Framework option
* Upload the code every time with a new filename in the same bucket

### Question 52:
The DevOps team at a retail company has deployed its flagship application on EC2 instances using CodeDeploy and uses an RDS PostgreSQL database to store the data, while it uses DynamoDB to store the user sessions. As the Lead DevOps Engineer at the company, you would like the application to securely access RDS & DynamoDB.
* Store the RDS credentials in Secrets Manager and create an IAM instance role for EC2 to access Secrets Manager and DynamoDB
* Store the RDS credentials & DynamoDB credentials in Secrets Manager and create an IAM instance role for EC2 to access Secrets Manager
* Store the RDS credentials in a DynamoDB table and create an IAM instance role for EC2 to access DynamoDB
* Store IAM user credentials & RDS credentials in Secrets Manager and create an IAM instance role for EC2 to access Secrets Manager

### Question 53:
A media streaming solutions company has deployed an application that allows its customers to view movies in real-time. The application connects to an Amazon Aurora database, and the entire stack is currently deployed in the United States. The company has plans to expand to Europe and Asia for its operations. It needs the movies table to be accessible globally but needs the users and movies_watched table to be regional only.
* Use an Amazon Aurora Global Database for the movies table and use DynamoDB for the users and movies_watched tables
* Use a DynamoDB Global Table for the movies table and use DynamoDB for the users and movies_watched tables
* Use an Amazon Aurora Global Database for the movies table and use Amazon Aurora for the users and movies_watched tables
* Use a DynamoDB Global Table for the movies table and use Amazon Aurora for the users and movies_watched tables

### Question 54:
A Silicon Valley based startup runs a news discovery web application and it uses CodeDeploy to deploy the web application on a set of 20 EC2 instances behind an Application Load Balancer. The ALB is integrated with CodeDeploy. The DevOps teams at the startup would like the deployment to be gradual and to automatically rollback in case of unusually high maximum CPU utilization for the EC2 instances while traffic is being served.
* Create a CloudWatch metric for the maximum CPU utilization of your EC2 instances. Create a CloudWatch Alarm on top of that metric. Create a deployment in CodeDeploy that has rollback enabled, integrated with the CloudWatch alarm
* Create a CloudWatch metric for the maximum CPU utilization of your EC2 instances. Create a deployment in CodeDeploy that has rollback enabled, integrated with the CloudWatch metric
* In the ValidateService hook in appspec.yml, measure the CPU utilization for 5 minutes. Configure CodeDeploy to rollback on deployment failures. In case the hook fails, then CodeDeploy will rollback
* Create a CloudWatch metric for the maximum CPU utilization of your Application Load Balancer. Create a deployment in CodeDeploy that has rollback enabled, integrated with the CloudWatch metric

### Question 55:
The DevOps team at a business travel solutions company wants to use CodeDeploy to ensure zero downtime during deployments through rolling updates. The team wants to deploy the company's flagship web application on a set of 5 EC2 instances running behind an Application Load Balancer. The team would like the deployment to be gradual and to automatically rollback in case of a failed deployment, which is determined by the application not being able to pass health checks.
* Integrate CodeDeploy with the Application Load Balancer. In case the Application Load Balancers fails the health checks on the instances where the new version has been deployed, it will notify CodeDeploy. Configure CodeDeploy to rollback on deployment failures
* In the AfterInstall hook in appspec.yml, verify the service is properly running. Configure CodeDeploy to rollback on deployment failures. In case the hook fails, then CodeDeploy will rollback
* Create a CloudWatch Event rule on CodeDeploy to invoke a Lambda function upon deployment on every instance. The Lambda function tests the health check, and if it fails, stops the CodeDeploy deployment using the StopDeployment API, and then start a new deployment of the old version using the CreateDeployment API
* In the ValidateService hook in appspec.yml, verify the service is properly running. Configure CodeDeploy to rollback on deployment failures. In case the hook fails, then CodeDeploy will rollback

### Question 56:
As a DevOps Engineer at a data analytics company, you're deploying a web application on EC2 using an Auto Scaling group. The data is stored in RDS MySQL Multi-AZ, and a caching layer using ElastiCache. The application configuration takes time and currently needs over 20 minutes to warm up. 10 of those minutes are spent installing and configuring the web application, and another 10 minutes are spent warming up the local instance data cache.
* Migrate from ElastiCache to DynamoDB. Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script
* Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script
* Create an AMI that contains the web application. Configure the dynamic part at runtime using an EC2 User Data script. Use AWS Lambda to configure the instance local cache at boot time
* Create an AMI that contains the web application and a copy of the local data cache. Configure the dynamic part at runtime an EC2 User Data script

### Question 57:
A mobility company connects people with taxi drivers and the DevOps team at the company uses CodeCommit as a backup and disaster recovery service for several of its DevOps processes. The team is creating a CICD pipeline so that your code in the CodeCommit master branch automatically gets packaged as a Docker container and published to ECR. The team would then like that image to be automatically deployed to an ECS cluster using a Blue/Green strategy.
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Create a CloudWatch Event Rule that will react to pushes to ECR and invoke CodeDeploy, the target of which should be the ECS cluster
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Upon the success of that CodeBuild stage, start a CodeDeploy stage with a target being your ECS service
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the AWS_ACCESS_KEY_ID and AWS_SECRET_ACCESS_KEY environment variables passed in through CodeBuild configuration, the values being those from your user. Upon the success of that CodeBuild stage, create a new task definition automatically using CodePipeline and apply that task definition to the ECS service using a CloudFormation action
* Create a CodePipeline that will invoke a CodeBuild stage. The CodeBuild stage should acquire ECR credentials using the CLI helpers, build the image, and then push it to ECR. Upon the success of that CodeBuild stage, create a new task definition automatically using CodePipeline and apply that task definition to the ECS service using a CloudFormation action

### Question 58:
The DevOps team at a geological hazard monitoring agency maintains an application that provides near real-time notifications to Android and iOS devices during tremors, volcanic eruptions and tsunamis. The team has created a CodePipeline pipeline, which consists of CodeCommit and CodeBuild, and the application is deployed on Elastic Beanstalk. The team would like to enable Blue/Green deployments for Beanstalk through CodePipeline.
* Make CodePipeline deploy to a new Beanstalk environment. After that stage action, create another stage action to invoke a Custom Job using AWS Lambda, which will perform the API call to swap the CNAME of the environments
* Make CodePipeline deploy to the current Beanstalk environment using a rolling with additional batch strategy. Add a CodeDeploy stage action afterward to enable Blue / Green
* Make CodePipeline deploy to a new Beanstalk environment. After that stage action, create another stage action to invoke a CloudFormation template that will perform a CNAME swap
* Make CodePipeline deploy to the current Beanstalk environment using an immutable strategy. Add a CodeStar stage action afterward to enable Blue / Green configured through the template.yml file

### Question 59:
A financial planning company runs a tax optimization application that allows people to enter their personal financial information and get recommendations. The company is committed to the maximum security for the Personally identifiable information (PII) data in S3 buckets, and as part of compliance requirements, it needs to implement a solution to be alerted in case of new PII and its access in S3.
* Create an Amazon Lambda function that is integrated with Amazon Sagemaker to detect PII data. Integrate the Lambda function with S3 events for PUT requests
* Set up an S3 bucket policy that filters requests containing PII data using a conditional statement
* Enable Amazon Macie on the selected S3 buckets. Setup alerting using CloudWatch Events
* Enable Amazon GuardDuty on the select S3 buckets. Setup alerting using CloudWatch Alarms

### Question 60:
A social media company is running its flagship application via an Auto-Scaling group (ASG) which has 15 EC2 instances spanning across 3 Availability Zones (AZs). The current average CPU utilization of the group sits at 15% off-peak time. During peak time, it goes all the way to 45%, and these peak times happen predictably during business hours. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that invokes a Lambda function which will terminate 9 instances after peak times
* Use a CloudFormation UpdatePolicy to define how the Auto Scaling Group should behave off and on peaks. Ensure the ASG invokes the CloudFormation using SNS notifications relay
* Create a Lambda function that terminates 9 instances at the end of business hours. Create a second Lambda function that creates instances when peak time starts. Schedule the functions using CloudWatch Events
* Create a scaling policy that tracks the CPU utilization with a target of 75%. Create a scheduled action that increases the number of minimum instances to 6 during peak times and a second scheduled action that reduces the number of minimum instances to 3 off-peak times

### Question 61:
The technology team at a leading bank is using software that has a license type that gets billed based on the number of CPU sockets that are being used. The team would like to ensure that they are using the most appropriate EC2 launch mode and create a compliance dashboard that highlights any violation of that decision. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution for this requirement.
* Launch the EC2 instances on Dedicated Hosts and create a tag for the application. Deploy an AWS Service Catalog rule backed by a Lambda function to track that the application is always launched on an EC2 instance with the correct mode
* Launch the EC2 instances on Reserved Instance and create a tag for the application. Deploy an AWS Service Catalog rule backed by a Lambda function to track that the application is always launched on an EC2 instance with the correct mode
* Launch the EC2 instances on Reserved Instances and create a tag for the application. Deploy an AWS Config custom rule backed by a Lambda function that will check the application tag and ensure the instance is launched on the correct launch mode
* Launch the EC2 instances on Dedicated Hosts and create a tag for the application. Deploy an AWS Config custom rule backed by a Lambda function that will check the application tag and ensure the instance is launched on the correct launch mode

### Question 62:
The DevOps team at an e-commerce company is working with the in-house security team to improve the security workflow of the code release process. The DevOps team would like to initiate a 3rd party code vulnerability analysis tool for every push done to code in your CodeCommit repository. The code has to be sent via an external API.
* Create a CloudWatch Event rule on your CodeCommit repository that reacts to pushes. As a target, choose an AWS Lambda function that will request the code from CodeCommit, zip it and send it to the 3rd party API
* Create a CodeCommit hook on an EC2 instance that streams changes from CodeCommit into the local filesystem. A cron job on the EC2 instance will zip the code and send it to the 3rd party API upon changes being detected
* Create a CloudWatch Event rule on your CodeCommit repository that reacts to pushes. As a target, choose an S3 bucket so that the code will be automatically zipped into S3. Create an S3 Event rule to trigger a Lambda function that will retrieve the zipped code from S3 and send it to the 3rd party API
* Create a CloudWatch Event rule on a schedule of 5 minutes that triggers a Lambda function that will check for new commits done on your CodeCommit repository. If new commits are detected, download and zip the code and then send it to the 3rd party API

### Question 63:
The technology team at a health-care solutions company has developed a REST API which is deployed in an Auto Scaling Group behind an Application Load Balancer. The API stores the data payload in DynamoDB and the static content is served through S3. Upon doing some analytics, it's found that 85% of the read requests are shared across all users.
* Enable DynamoDB Accelerator (DAX) for DynamoDB and CloudFront for S3
* Enable ElastiCache Redis for DynamoDB and ElastiCache Memcached for S3
* Enable DAX for DynamoDB and ElastiCache Memcached for S3
* Enable ElastiCache Redis for DynamoDB and CloudFront for S3

### Question 64:
An Internet-of-Things (IoT) solutions company has decided to release every single application as a Docker container and to use ECS classic (on EC2) as the container orchestration system and ECR as the Docker registry. Part of implementing a monitoring pipeline is to ensure all application logs can be stored in CloudWatch logs.
* Create ECS task definitions for your applications, with a mapping of the /var/log directory onto the local filesystem of the EC2 instance. Install the CloudWatch Agent on the EC2 instance using user-data and track the /var/log/containers directory. Create an EC2 instance role with the necessary permissions to write to CloudWatch logs
* Create ECS task definitions that include the awslogs driver. Set an IAM instance role on the EC2 instance with the necessary permissions to write to CloudWatch logs
* Create ECS task definitions that include the awslogs driver. Set an IAM task role in the task definition with the necessary permissions to write to CloudWatch logs
* Create ECS task definitions for your applications, with a sidecar container which contains the CloudWatch Agent tracking the /var/log/containers directory. Map the application's /var/log directory onto the sidecar filesystem. Set an IAM task role in the task definition with the necessary permissions to write to CloudWatch logs

### Question 65:
A healthcare technology company provides a Software as a Service (SaaS) solution to hospitals throughout the United States to use the company’s proprietary system to integrate their clinical documentation and coding workflows. The DevOps team at the company would like to enable a CICD pipeline that enables safe deployments to production and the ability to work on new features of the product roadmap.
* Create the main CodeCommit repository and set the CICD pipeline to deploy the master branch. For each new feature being implemented, create a new CodeCommit repository and create pull requests to merge into the main repository. Set an IAM policy on your developer group to prevent direct pushes to the main repository
* Create a CodeCommit repository and create a branch for each feature. Create a CICD pipeline for each branch, and the last step of the CICD pipeline should be to merge into master. Set an IAM policy on your developer group to prevent direct pushes to master
* Create a CodeCommit repository and set the CICD pipeline to deploy the master branch. For each new feature being implemented, create a new branch and create pull requests to merge into master. Set a repository access policy on your repository to prevent direct pushes to master
* Create a CodeCommit repository and set the CICD pipeline to deploy the master branch. For each new feature being implemented, create a new branch and create pull requests to merge into master. Set an IAM policy on your developer group to prevent direct pushes to master

### Question 66:
A global health-care company has an EFS filesystem being used in eu-west-1. The company would like to plan for a disaster recovery strategy and backup that EFS file system in ap-southeast-2. It needs to have a hot copy of the data so that the applications can be re-deployed in ap-southeast-2 with a minimum RPO and RTO. The VPCs in each region are not peered with each other.
* Create a replication cluster managed by EC2 with Auto Scaling in eu-west-1. Scale according to a Custom Metric you would publish with the application representing the lag in file reads. Replicate the data into Amazon S3 in ap-southeast-2. Create another replication cluster in ap-southeast-2 that reads from Amazon S3 and copies the files into a standby EFS cluster
* Create a CloudWatch Event hourly rule that triggers an AWS Batch cluster in eu-west-1 to perform an incremental replication. Replicate the data into Amazon S3 in another region. Create an EC2 replication cluster in ap-southeast-2 that reads from Amazon S3 and copies the files into a standby EFS cluster
* Create a CloudWatch Event hourly rule that triggers an AWS Batch cluster in eu-west-1 to perform an incremental replication. Replicate the data into Amazon S3 in another region. Create a Lambda Function in ap-southeast-2 for PUT on Amazon S3 and triggers an SSM Run Command to copy the files from S3 into EFS
* Create a replication cluster managed by EC2 with Auto Scaling in eu-west-1. Scale according to a Custom Metric you would publish with the application representing the lag in file reads. Create a standby EFS cluster in ap-southeast-2 and mount it on the same EC2 cluster. Let the replication software perform EFS to EFS replication

### Question 67:
As the Lead DevOps Engineer at an analytics company, you are deploying a global application using a CICD pipeline comprising of AWS CodeCommit, CodeBuild, CodeDeploy and orchestrated by AWS CodePipeline. Your pipeline is currently setup in eu-west-1 and you would like to extend the pipeline to deploy your application in us-east-2. This will require a multi-step CodePipeline to be created there and invoked.
* At the end of the pipeline in eu-west-1, include a CodeDeploy step to deploy the application to the CodePipeline in us-east-2
* At the end of the pipeline in eu-west-1, include a CodeCommit step to push the changes to the code into the master branch of another CodeCommit repository in us-east-2. Make the CodePipeline in us-east-2 source files from CodeCommit
* At the end of the pipeline in eu-west-1, include a CodePipeline step to invoke the CodePipeline in us-east-2. Ensure the CodePipeline in us-east-2 has the necessary IAM permission to read the artifacts in S3 in eu-west-1
* At the end of the pipeline in eu-west-1, include an S3 step to copy the artifacts being used by CodeDeploy to an S3 bucket in us-east-2. Make the CodePipeline in us-east-2 source files from S3

### Question 68:
The engineering team at a multi-national retail company is deploying its flagship web application onto an Auto Scaling Group using CodeDeploy. The team has chosen a strategy of a rolling update so that instances are updated in small batches in the ASG. The ASG has five instances running. At the end of the deployment, it seems that three instances are running the new version of the application, while the other two are running the old version. CodeDeploy is reporting a successful deployment.
* A CloudWatch alarm has been triggered during the deployment
* Two new instances were created during the deployment
* The auto-scaling group launch configuration has not been updated
* Two instances are having an IAM permissions issue and cannot download the new code revision from S3

### Question 69:
A Big Data analytics company is operating a distributed Cassandra cluster on EC2. Each instance in the cluster must have a list of all the other instance's IP to function correctly, store in a configuration file. As a Devops Engineer at the company, you would like this solution to adapt automatically when newer EC2 instances join the cluster, or when some EC2 instances are terminated.
* Manage the EC2 instances using an Auto Scaling Group. Include a lifecycle hook for the instance pending and termination that will trigger an EC2 user-data script on the EC2 instances. The script issues an EC2 DescribeInstances API call and update the configuration file locally
* Manage the EC2 instances using OpsWorks. Include a chef cookbook on the setup lifecycle event that will update the configuration file accordingly
* Manage the EC2 instances using OpsWorks. Include a chef cookbook on the configure lifecycle event that will update the configuration file accordingly
* Manage the EC2 instances using an Auto Scaling Group. Include a lifecycle hook for the instance pending and termination that will trigger an AWS Lambda function. The Lambda function will issue an EC2 DescribeInstances API call and update the configuration file through SSH

### Question 70:
The DevOps team at a yoga-inspired apparel company wants to stand up development environments for testing new features. The team would like to receive all CodePipeline pipeline failures to be sent to the company's #devops Slack channel. The company has hired you as an AWS Certified DevOps Engineer Professional to build a solution to address this use-case.
* Create a CloudWatch Event Rule with the source corresponding to
* The target of the rule should be a Lambda function that will invoke a 3rd party Slack webhook
* Create a CloudWatch Event Rule with the source corresponding to
* The target of the rule should be a 'Slack send'. Provide the channel name and webhook URL
* Create a CloudWatch Event rule with the source corresponding to

### Question 71:
A retail company is finishing its migration to AWS and realizes that while some employees have passed the AWS Certified DevOps Engineer Professional certification and know AWS very well, other ones are still beginning and haven't passed their Associate-level certifications yet. The company has established architectural and tagging specific internal rules and would like to minimize the risk of the AWS-beginner employees launching uncompliant resources.
* Place the beginner IAM users into a group and create an IAM policy that requires conditional approvals from senior DevOps engineers upon resource creation. Hook an SNS topic into the IAM approval channel
* Define commonly used architectures as CloudFormation templates. Place the IAM users into a beginner group and allow the users to only launch stacks from these CloudFormation stacks, while restricting any write access to other services
* Create AWS Config custom rules that will check for the compliance of your company's resources thanks to a Lambda Function. Update the Lambda Function over time while your company improves its architectural and tagging rules. Provide IAM users full access to AWS
* Define commonly used architectures as CloudFormation templates. Create Service Catalog stacks from these templates, and ensure the tagging is done properly. Place the IAM users into a beginner group and allow the users to only launch stacks from Service Catalog, while restricting any write access to other services

### Question 72:
The DevOps team at a social media company has created a CodePipeline pipeline and the final step is to use CodeDeploy to update an AWS Lambda function. As a DevOps Engineering Lead at the company, you have decided that for every deployment, the new Lambda function must sustain a small amount of traffic for 10 minutes and then shift all the traffic to the new function. It has also been decided that safety must be put in place to automatically roll-back if the Lambda function experiences too many crashes.
* Choose a deployment configuration of LambdaCanary10Percent10Minutes
* Create a CloudWatch Alarm on the Lambda CloudWatch metrics and associate it with the CodeDeploy deployment
* Choose a deployment configuration of LambdaLinear10PercentEvery10Minutes
* Choose a deployment configuration of LambdaAllAtOnce
* Create a CloudWatch Event for the Lambda Deployment Monitoring and associate it with the CodeDeploy deployment

### Question 73:
A retail company is implementing a CodePipeline pipeline in which every push to the CodeCommit master branch gets deployed to development, staging, and production environment consisting of EC2 instances. When deploying to production, traffic should be deployed on a few instances so that metrics can be gathered before a manual approval step is done to deploy to all the instances.
* In CodeDeploy, create four deployment groups - one for development, one for staging, one for the canary testing instances in production and one for the entire production instances. Create one CodePipeline and chain up these stages together, introducing a manual approval step after the deployment to the canary instances
* In CodeDeploy, create four deployment groups - one for development, one for staging, one for the canary testing instances in production and one for the entire production instances. Create one CodePipeline for each deployment group all having the same source being your code repository. Introducing a manual approval step in the pipeline that deploys to production
* In CodeDeploy, create three deployment groups - one for development, one for staging, and one for the entire production instances. Create three separate CodePipeline for each deployment group having all the same sources being your code repository. For the deployment to production, enable the Canary deployment setting for CodeDeploy, and introduce a manual step after the canary deployment that will pause the rest of the deployment. Upon approval, the rest of the instances in production will have a deployment made to them
* In CodeDeploy, create three deployment groups - one for development, one for staging, and one for the entire production instances. Create one CodePipeline and chain up these together. For the deployment to production, enable the Canary deployment setting for CodeDeploy, and introduce a manual step after the canary deployment that will pause the rest of the deployment. Upon approval, the rest of the instances in production will have a deployment made to them

### Question 74:
The DevOps team at an analytics company is deploying an Apache Kafka cluster that contains 6 instances and is distributed across 3 Availability Zones (AZs). Apache Kafka is a stateful service and needs to store its data in an EBS volume. Therefore each instance must have the auto-healing capability and always attach the correct EBS volumes.
* Create 6 EC2 instances using CloudFormation with EBS volumes. Define the attachments in the CloudFormation template. If the EC2 instance is terminated, it will be automatically re-created by CloudFormation with the correct EBS attachment
* Create an Auto Scaling Group in CloudFormation with a min/max desired capacity of 6 instances spread across 3 AZs, and 6 EBS volumes also across the 3 AZs. Create a user data script so that instances launching from the ASG automatically acquire an available EBS volume in the corresponding AZ
* Create a CloudFormation template with an ASG of min/max capacity of 1, and an EBS volume. Tag the ASG and EBS volume. Create a User Data script that will acquire the EBS volume at boot time. Use a master CloudFormation template and reference the nested template 6 times
* Create 6 EC2 instances using CloudFormation with EBS volumes. Define the attachments in the CloudFormation template. If the EC2 instance is terminated, launch a drift detection in CloudFormation and then use CloudFormation remediation

### Question 75:
A financial services company is using security-hardened AMI due to strong regulatory compliance requirements. The company must be able to check every day for AMI vulnerabilities based on the newly disclosed ones through the common vulnerabilities and exposures (CVEs) program. Currently, all the instances are launched through an Auto Scaling group (ASG) leveraging the latest security-hardened AMI.
* Create a CloudWatch Event with a daily schedule, the target being a Lambda Function. Tag all the instances in your ASG with CheckVulnerabilities: True. The Lambda function should start an assessment in AWS Inspector targeting all instances having the tag
* Create a CloudWatch Event with a daily schedule, the target being a Step Function. The Step Function should launch an EC2 instance from the AMI and tag it with CheckVulnerabilities: True. The Step Function then starts an AMI assessment template using AWS Inspector and the above tag. Terminate the instance afterward
* Create a CloudWatch Event with a daily schedule. Invoke a Lambda Function that will start an AWS Inspector Run directly from the AMI reference in the API call. AWS Inspector will automatically launch an instance and terminate it upon assessment completion
* Create a CloudWatch Event with a daily schedule. Make the target of the rule being AWS Inspector and pass some extra data in the rule using the AMI ID to inspect. AWS Inspector will automatically launch an instance and terminate it upon assessment completion
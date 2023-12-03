#### Question: Explain Availability zones.
**Answer:** Availability zones are like different neighborhoods within a city. Each zone is in a separate area, making it less likely for a single event, like a power outage or a storm, to affect all the zones. So, if something happens in one zone, your services in other zones remain unaffected.
In context with cloud environment, these are distinct locations within a region, designed to be isolated from failures in other zones. They provide high availability and redundancy.


#### Question: Explain subnets and regions to management body.
**Answer:** Subnets are like different sections within your office building (VPC). Each section is for different departments or teams. Regions, on the other hand, are like different cities where you can have your office. Each city can have its own set of office buildings (VPCs).
Subnets are partitions within a VPC and are associated with a specific Availability Zone. Regions are separate geographic areas where AWS data centers are located.


#### Question: What is an ec2 instance ?
**Answer:** An EC2 instance is like a computer that lives in your virtual office (VPC). It's where you can run programs, websites, or anything you'd usually do on your computer, but it's located in the cloud.


#### Question: Can you tell me bunch of ec2 instance types ?
**Answer:** EC2 instances come in various sizes and capabilities, just like different cars have different features. There are types for general tasks, memory-intensive work, or high-performance computing, each suited for specific jobs. Some of these would be t2, t3, m4, m5, c5 etc.


#### Question: What is an AMI in context with Ec2 instance ?
**Answer:** Think of an AMI as a pre-set computer setup you can use to create new computers (EC2 instances). It's like a special recipe for a computer, including the operating system, software, and settings. It can be referred as an Image ISO of the operating system to be installed, It's a pre-configured template used to create EC2 instances. It includes the operating system, application server, and applications.


#### Question: If security groups are there then why do we need NACLs or vice versa.
**Answer:** Security groups are like bouncers at the entrance of your office building, deciding who gets in or out of the entire building. NACLs are more like security guards stationed in different sections of the building (subnets), controlling movement within. Thus Security Groups act at the instance level, while NACLs act at the subnet level, offering an additional layer of security.


#### Question: Explain different types of volumes in AWS.
**Answer:** In a cloud office, different types of volumes are like different storage spaces. EBS is like a hard drive, S3 is like a file cabinet, and Glacier is like a secure storage room for long-term archives. Some of them are EBS (Elastic Block Store), S3 (Object Storage), EFS (Elastic File System).


#### Question: What are different frameworks of Lambda, why do we even require them ?
**Answer:** Lambda is like a team of workers you can hire to do specific jobs whenever you need. Frameworks give these workers different skills for various tasks, allowing them to handle different types of jobs efficiently. Examples include Serverless Framework, SAM (Serverless Application Model), and Chalice. They streamline Lambda deployments.


#### Question: what are launch configuration and launch template and how do they differ from each other.
**Answer:** Both are like instructions for creating computers (EC2 instances), but a launch configuration is an older set of rules, while a launch template is a newer, more flexible, and organized way of doing the same job but Launch Templates offer more features and flexibility compared to Launch Configurations.


#### Question: What is trust relationship in context with IAM ?
**Answer:** Trust relationship is like a handshake between different identities (services or users) in your office. It defines which accounts or services are allowed to assume a particular IAM role.


#### Question: How does assume role works ?
**Answer:** Assume role is when one identity temporarily wears another identity’s hat to access specific resources, with permission. It's used to temporarily grant permissions to an IAM user, role, or AWS service.


#### Question: How can I switch an RDS intance from public to private or vice versa ?
**Answer:**  It's like changing the access to an office room. Making it public means anyone with permission can come in, while making it private limits access to a select few. 


#### Question: Why cloudformation when Terraform is already there.
**Answer:** Both are like different languages for giving instructions to set up your office building. CloudFormation is AWS’s language, while Terraform is like a multi-language translator that works across different cloud providers. CloudFormation is AWS’s native service, while Terraform is a third-party, multi-cloud infrastructure provisioning tool.


#### Question: what all algorithms are supported by Route53 ?
**Answer:** Route 53 is like a guide giving directions. It supports different methods of directing traffic to the right places, ensuring the quickest and most efficient routes for your services. It supports a variety of DNS routing algorithms like Simple, Weighted, Latency-based, and Geolocation routing.


#### Question: what is AWS inspector ? How does it work ?
**Answer:** Inspector is like a security guard that checks for any weaknesses or problems in your office building's security system. It looks for possible entry points for intruders and suggests ways to strengthen security. Over here It's a service that identifies security vulnerabilities within AWS resources.


#### Question: What is securityHub ? How does it work ?
**Answer:** SecurityHub is like a supervisor overlooking security measures across your office buildings (AWS accounts). It collects and prioritizes security findings to help you manage and improve security. It provides a comprehensive view of the security state of AWS resources. Majorly when you enable AWS inspector, it sends data to securityHub automatically.


#### Question: what is AWS control tower ?
**Answer:** Think of Control Tower as the manager of all your office buildings (AWS accounts). It helps set up and govern multiple accounts following security best practices and compliance requirements. It's a service that sets up and governs a secure, multi-account AWS environment.


#### Question: What is AWS SSM ?
**Answer:** SSM acts like a control panel to manage and automate office tasks (AWS resources). It helps in organizing and maintaining systems, automating tasks, and ensuring everything runs smoothly. It's a service used to manage AWS resources, automate tasks, and manage infrastructure.


#### Question: Explain the difference between EC2 and Lambda in AWS.
Expected **Answer:** EC2 provides virtual servers that you manage, while Lambda allows serverless execution of code without server provisioning.


#### Question: What is an EC2 instance and how does it differ from an AMI?
**Answer:**
EC2 Instance: It's a virtual server in the cloud where you can run applications. Think of it as a computer system hosted in AWS.
AMI (Amazon Machine Image): It's a template that provides the information needed to launch an EC2 instance. An AMI includes the operating system, application server, and applications. While an EC2 instance is like a running computer, an AMI is like a blueprint or image of that computer.


#### Question: Explain the significance of Security Groups and NACLs in AWS.
**Answer:**
Security Groups: Act as virtual firewalls for EC2 instances to control inbound and outbound traffic. They're stateful and evaluate traffic rules at the instance level.
Network Access Control Lists (NACLs): They're an additional layer of security, acting as a firewall for controlling traffic in and out of subnets. NACLs are stateless and work at the subnet level.


#### Question: What's the difference between EBS and S3 in AWS?
**Answer:**
Amazon S3 (Simple Storage Service): It's object storage for files, images, videos, and backups with virtually unlimited storage capacity and internet accessibility.
Amazon EBS (Elastic Block Store): It's block storage used for EC2 instances, behaving like a hard drive. It's more suitable for database storage and allows for snapshots and encryption.


#### Question: Describe AWS Lambda and its use cases.
**Answer:**
AWS Lambda: It's a serverless computing service that runs code in response to events and automatically manages resources. It's ideal for executing small, event-driven functions, making it perfect for tasks like data processing, file handling, and automation.


#### Question: What are Auto Scaling Groups and how do they work in AWS?
**Answer:**
Auto Scaling Groups: They automatically adjust the number of instances in response to changing demand. They maintain the desired number of instances even if one fails and can dynamically scale based on rules or policies.


#### Question: Explain the different storage classes in Amazon S3 and their use cases.
**Answer:**
* Standard: General-purpose storage for frequently accessed data.
* Infrequent Access (IA): For less frequently accessed data but requires rapid access when needed.
* Glacier: For long-term archival storage with retrieval times of minutes to hours.


#### Question: What is AWS IAM? Explain IAM Roles and Policies.
**Answer:**
* IAM (Identity and Access Management): It's used to control access to AWS services and resources.<br>
* IAM Roles: Define a set of permissions for making AWS service requests. They're used to grant specific permissions to entities that you trust.<br>
* IAM Policies: These are documents that define permissions. They specify what actions are allowed or denied and on what resources.


#### Question: Describe AWS RDS and its benefits.
**Answer:**
* Amazon RDS (Relational Database Service): It's a managed database service that makes it easy to set up, operate, and scale a relational database in the cloud. It supports various engines like MySQL, PostgreSQL, Oracle, and SQL Server.
* Benefits: Automated backups, scaling, patches, and high availability are some advantages of RDS.


#### Question: Explain the concept of VPC (Virtual Private Cloud) in AWS.
**Answer:**<br>
**VPC:** Imagine a VPC as your own virtual space in the cloud. It's like your personal office building in a city full of skyscrapers. Your VPC is where you control your network, your own space with its own address and security. You decide who can come in, what rooms they can access, and how they move around. It's a virtual network dedicated to your AWS account. It allows you to select your IP address range, create subnets, and configure route tables and network gateways. VPC provides isolation and control over your network environment.


#### Question: What is CloudFormation in AWS?
**Answer:** <br>
AWS CloudFormation: It's a service that helps model and set up your AWS resources using templates. It allows you to describe and provision all the infrastructure resources in your cloud environment.


#### Question: Explain the difference between AWS ECS and AWS EKS.
**Answer:**
* ECS (Elastic Container Service): It's a container management service for Docker containers, offering simplicity and native integration with other AWS services.<br>
* EKS (Elastic Kubernetes Service): It's a managed Kubernetes service offering open-source flexibility and scalability with less AWS-specific functionality.


#### Question: What is AWS Lambda Layers?
**Answer:**<br>
Lambda Layers: These allow you to centrally manage common code and data shared across multiple Lambda functions. Layers are useful for shared libraries, custom runtimes, and dependencies.


#### Question: How does AWS KMS (Key Management Service) work?
**Answer:**<br>
AWS KMS: It's a service for managing cryptographic keys. It uses Hardware Security Modules (HSM) to protect your keys and offers secure key creation, storage, and management.


#### Question: Explain AWS Redshift and its use cases.
**Answer:**<br>
AWS Redshift: It's a fully managed, petabyte-scale data warehouse service. It's optimized for querying large datasets and is suitable for analytics, reporting, and business intelligence.


#### Question: Describe AWS Direct Connect and its benefits.
**Answer:**<br>
AWS Direct Connect: It's a dedicated network connection from on-premises networks to AWS. It's used to reduce network costs, increase bandwidth throughput, and provide a consistent network experience.


#### Question: What is CloudWatch in AWS and how is it utilized?
**Answer:**
CloudWatch: It's a monitoring and observability service in AWS used for collecting and tracking metrics, monitoring logs, and setting alarms. It's pivotal for resource optimization and troubleshooting.


#### Question: Explain the differences between AWS RDS and DynamoDB.
**Answer:**
* RDS: It's a relational database service supporting SQL-type databases like MySQL, PostgreSQL, SQL Server, etc.<br>
* DynamoDB: It's a NoSQL database service designed for fast and predictable performance with seamless scalability.


#### Question: What is AWS SNS and how is it different from SQS?
**Answer:**
* SNS (Simple Notification Service): It's a publish-subscribe service allowing message broadcasting to various recipients.<br>
* SQS (Simple Queue Service): It's a message queue service for decoupling services and handling asynchronous communication between distributed systems.


#### Question: What is the AWS Well-Architected Framework and its importance?
**Answer:**
Well-Architected Framework: The AWS Well-Architected Framework is a set of best practices and guidelines designed to help cloud architects build secure, high-performing, resilient, and efficient infrastructure for their applications. Developed by Amazon Web Services (AWS), the Well-Architected Framework provides a consistent approach for customers and partners to evaluate their architectures and implement designs that will scale over time.<br>
Importance: Following these best practices ensures that AWS environments are well-structured and aligned with industry standards.
Operational Excellence: Focuses on operational aspects, such as incident response, monitoring, and automation.<br>
Aims to deliver business value by continually improving processes and procedures.
Security: Emphasizes the implementation of robust security measures to protect data, systems, and assets.<br>
Includes identity and access management, data protection, and incident response.
Reliability: Ensures that a system can recover from failures and meet customer expectations during normal and peak operation.<br>
Addresses areas like fault tolerance, disaster recovery, and scaling.
Performance Efficiency: Focuses on optimizing the use of computing resources to meet system requirements and to maintain efficiency.<br>
Covers areas like selecting the right types and sizes of resources and monitoring performance.
Cost Optimization: Aims to avoid unnecessary costs and optimize spending by understanding and controlling where the money is going.<br>
Includes strategies for monitoring usage, optimizing resource allocation, and managing costs over time.


#### Question: Explain the concept of AWS Lambda Triggers.
**Answer:**<br>
Lambda Triggers: They're events that invoke Lambda functions automatically when a particular event occurs in other AWS services. For instance, S3 upload triggers a Lambda function.


#### Question: Describe AWS Route 53 and its key features.
**Answer:**<br>
Route 53: It's a scalable domain name system (DNS) web service providing domain registration and routing internet traffic to resources.<br>
Key Features: Health checks, traffic flow, domain registration, and global data propagation are significant functionalities.


#### Question: What are the benefits of using AWS EFS (Elastic File System)?
**Answer:**<br>
EFS: It's a file storage service providing scalable storage for use with Amazon EC2 instances. Benefits include high availability, durability, and compatibility with multiple EC2 instances.


#### Question: Explain AWS CloudTrail and its role in AWS security.
**Answer:**<br>
CloudTrail: It's a service for logging and monitoring AWS API calls for auditing and security analysis.<br>
Role in Security: CloudTrail provides a record of actions taken by a user, role, or an AWS service for security and compliance needs.


#### Question: What is the AWS Storage Gateway and its use cases?
**Answer:**<br>
Storage Gateway: It's a service connecting an on-premises software appliance with cloud-based storage to provide seamless integration.<br>
Use Cases: Backup, disaster recovery, and hybrid cloud storage are common scenarios.


#### Question: Explain the benefits of using AWS Elastic Beanstalk.
**Answer:**<br>
Elastic Beanstalk: It's a service that simplifies deployment and management of applications in the AWS cloud.<br>
Benefits: It streamlines infrastructure management, eases deployment, and allows developers to focus on coding.


#### Question: How does AWS CloudFront work and what are its features?
**Answer:**<br>
CloudFront: It's a content delivery network (CDN) service, distributing content globally with low latency and high data transfer speeds.<br>
Features: Edge locations, caching, and origin fetch optimization are key functionalities.


#### Question: Describe AWS Data Pipeline and its functionalities.
**Answer:**<br>
Data Pipeline: It's a web service for processing and moving data between different AWS services and on-premises data sources.<br>
Functionalities: ETL (Extract, Transform, Load), scheduling, and data transformation are significant capabilities.


#### Question: What is AWS OpsWorks and its use cases in infrastructure management?
**Answer:**<br>
OpsWorks: It's a configuration management service that provides managed instances of Chef and Puppet for infrastructure management.<br>
Use Cases: Application and infrastructure management, automation, and security patching are primary scenarios.


#### Question: How does AWS X-Ray assist in application performance monitoring?
**Answer:**<br>
AWS X-Ray: It's a service that helps developers analyze and debug production, distributed applications.<br>
Role in Performance Monitoring: X-Ray provides insights into how an application is performing and where issues might occur in a distributed environment.


#### Question: Explain the AWS Secrets Manager and its role in security.
**Answer:**<br>
Secrets Manager: It's a service for managing sensitive information such as passwords, API keys, and other secrets.<br>
Security Role: It helps protect sensitive data by controlling access and enabling rotation of secrets for enhanced security.


#### Question: What type of autoscaling policies are there in AWS ?
**Answer:** 
* *Target Tracking*: Scales based on predefined metrics to maintain a target value.
* *Step Scaling*: Scales based on configured steps with different scaling adjustments.
* *Simple/Manual Scaling*: Allows fixed scaling actions manually.


#### Question: What is Warmup and Cool down period ?
**Answer:** 
* *Warm Up Time*: Duration for newly launched instances to stabilize before they receive full traffic.
* *Cool Down Period*: Time during which Auto Scaling waits before another scaling activity.


#### Question: What are components of IAM ?
**Answer:** 
* Users: Individuals needing access to AWS.
* Groups: Collections of users with the same permissions.
* Roles: Define a set of permissions for making AWS service requests.
* Policies: Define permissions and attach them to users, groups, or roles.


#### Question: What if I have lost the Pem file for ubuntu user of an ec2-instance ?
**Answer:**<br>
It's advisable to create a new key pair and associate it with the instance. Otherwise, if an EBS-backed instance, stopping it, detaching the root volume, attaching it to another instance, modifying the authorized_keys file, then reattaching it to the original instance might help recover access.


#### Question: What is VPC Peering ?
**Answer:** Connects VPCs via a direct network route using private IP addresses, allowing instances to communicate.


#### Question: What is Transit VPC ?
**Answer:** A method to interconnect multiple VPCs, enabling connectivity between them.


#### Question: What is a VPC analyzer ?
**Answer:** A tool for monitoring and identifying risks and threats in VPC flow logs.


#### Question: What is AWS Private Link ?
**Answer:** Allows secure connectivity between VPCs and supported AWS services without traversing the internet.


#### Question: What can you tell me about warm pool ?
**Answer:** A feature in EC2 Auto Scaling Groups that allows pre-provisioning instances to respond to sudden traffic spikes.


#### Question: How to recover an ec2-instance if it crashes ?
**Answer:** Depends on the type of instance and its stored data. For EBS-backed instances, the data persists on the EBS volume and can be attached to another instance. For instance store-backed instances, recovery would involve relaunching the instance, losing any non-persistent data.


#### Question: What's the difference between Restart and Start/Stop of an ec2-instance ?
**Answer:** 
Restart: Quickly halts and restarts the instance.
Start/Stop: Completely halts the instance, which persists even after a start command. The VM is launched on a different host machine.


#### Question: How to host static website in AWS ?
**Answer:** Host a static website on AWS using Amazon S3. Upload your files to an S3 bucket and enable static website hosting in the bucket properties.

#### **S3 Intelligent-Tiering** 

In the S3 Intelligent-Tiering storage class, Amazon S3 monitors objects’ access patterns. If you haven’t accessed an object for 30 consecutive days, Amazon S3 automatically moves it to the infrequent access tier, S3 Standard-IA. If you access an object in the infrequent access tier, Amazon S3 automatically moves it to the frequent access tier, S3 Standard.

 

**The other response options are incorrect because:**

S3 Glacier is a low-cost storage class that is ideal for data archiving. You can retrieve objects stored in the S3 Glacier storage class within a few minutes to a few hours.

The S3 Standard-IA storage class is ideal for data that is infrequently accessed but requires high availability when needed. **Both S3 Standard and S3 Standard-IA store data in a minimum of three Availability Zones.** S3 Standard-IA provides the same level of availability as S3 Standard but at a lower storage price. 

S3 One Zone-IA is ideal for infrequently accessed data that does not require high availability.

#### **AWS Lambda**

The correct response option is You pay only for compute time while your code is running.

 

AWS Lambda is a service that lets you run code without needing to provision or manage servers. 



While using AWS Lambda, you pay only for the compute time that you consume. You are charged only when your code is running. With AWS Lambda, you can run code for virtually any type of application or backend service, all with zero administration. 

**Amazon Augmented AI**

Amazon Augmented AI (Amazon A2I) provides built-in human review workflows for common machine learning use cases, such as content moderation and text extraction from documents. With Amazon A2I, you can also create your own workflows for machine learning models built on Amazon SageMaker or any other tools.

 

The other response options are incorrect because:

- Amazon Textract is a machine learning service that automatically extracts text and data from scanned documents.
- Amazon Lex is a service that enables you to build conversational interfaces using voice and text.
- Amazon Aurora is an enterprise-class relational database.

#### **AWS Cost Explorer**

With AWS Cost Explorer, you can quickly create custom reports to analyze your AWS cost and usage data.

 

The other response options are incorrect because:

- AWS Budgets lets you set custom alerts that will notify you when your service usage exceeds (or is forecasted to exceed) the amount that you have budgeted.
- AWS Pricing Calculator lets you explore AWS services and create an estimate for the cost of your use cases on AWS. In the AWS Pricing 
- Calculator, you can enter details for your cloud computing requirements and then receive a detailed estimate that can be exported and shared. 
- AWS Artifact is a service that enables you to access AWS security and compliance reports and special online agreements.


#### **Instance store**



Instance stores are ideal for temporary data that does not need to be kept long term. 



When an Amazon EC2 instance is stopped or terminated, all the data that has been written to the attached instance store is deleted.

 

***The other response options are incorrect because:***

- Amazon EBS volumes are ideal for data that needs to be retained. When an - Amazon EC2 instance is stopped or terminated, all of the data on the attached EBS volume is still available.
- Amazon S3 buckets cannot be attached to Amazon EC2 instances.
- A subnet is a section of a virtual private cloud (VPC) in which you can group resources based on security or operational needs.


####  **Security Group**

A security group is a virtual firewall that controls inbound and outbound traffic for an Amazon EC2 instance. 

By default, a security group denies all inbound traffic and allows all outbound traffic. You can add custom rules to configure which traffic should be allowed or denied.

 

***The other response options are incorrect because:***

- A subnet is a section of a VPC in which you can group resources based on security or operational needs.
- A network access control list (ACL) is a virtual firewall that controls inbound and outbound traffic at the subnet level.
- An internet gateway is a connection between a VPC and the internet. It allows public traffic from the internet to access a VPC.

####  **AWS Elastic Beanstalk**

You upload your application, and Elastic Beanstalk automatically handles the deployment details of capacity provisioning, load balancing, auto-scaling, and application health monitoring.

 

***The other response options are incorrect because:***

- AWS Outposts is a service that enables you to run infrastructure in a hybrid cloud approach.
- Amazon CloudFront is a content delivery service. 
- AWS Snowball is a device that enables you to transfer large amounts of data into and out of AWS.


#### **Operations Perspective**

The Operations Perspective of the AWS Cloud Adoption Framework also includes principles for operating in the cloud by using agile best practices.

 

***The other response options are incorrect because: ***

- The Business Perspective helps you to move from a model that separates business and IT strategies into a business model that integrates IT strategy.
- The People Perspective helps Human Resources (HR) employees prepare their teams for cloud adoption by updating organizational processes and staff skills to include cloud-based competencies.
- The Governance Perspective helps you understand how to update the staff skills and organizational processes that are necessary to ensure business governance in the cloud.





#### **AWS GuardDuty** 

AWS GuardDuty identifies threats by continually monitoring the network activity and account behavior within your AWS environment.

 

***The other response options are incorrect because:***

- A service that helps protect your applications against distributed denial-of-service (DDoS) attacks - This response option describes AWS Shield.
- A service that checks applications for security vulnerabilities and deviations from security best practices - This response option describes Amazon Inspector.
- A service that lets you monitor network requests that come into your web applications - This response option describes AWS WAF.


#### **Amazon Route 53**


Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications that are hosted in AWS. 

 

Additionally, you can transfer DNS records for existing domain names that are currently managed by other domain registrars, or register new domain names directly within Amazon Route 53.

 

The other response options are incorrect because:

- Monitor your applications and respond to system-wide performance changes - These actions can be performed in Amazon CloudWatch.
- Access AWS security and compliance reports and special online agreements - This action can be performed in AWS Artifact.
- Automate the deployment of workloads into your AWS environment - This action can be performed with AWS Quick Starts.



#### **Elastic Load Balancing**


A load balancer acts as a single point of contact for all incoming web traffic to your Auto Scaling group. This means that as Amazon EC2 instances are added or removed in response to the amount of incoming traffic, these requests are routed to the load balancer first and then spread across multiple resources that will handle them.

 

***The other response options are incorrect because:***

- A service that monitors your applications and automatically adds or removes capacity from your resource groups in response to changing demand - This response option describes AWS Auto Scaling.
- A service that provides data that you can use to monitor your applications, optimize resource utilization, and respond to system-wide performance changes - This response option describes Amazon CloudWatch. Although Elastic Load Balancing does optimize resource utilization by distributing incoming traffic across available resources, this would not be the best response option because Elastic Load Balancing does not provide all the other listed features.
- A service that enables you to set up, manage, and scale a distributed in-memory or cache environment in the cloud - This response option describes Amazon ElastiCache.



#### **Performance Eficiency**

The Performance Efficiency pillar focuses on using computing resources efficiently to meet system requirements, and to maintain that efficiency as demand changes and technologies evolve.

 

***The other responses are incorrect because:***

- The Operational Excellence pillar includes the ability to run workloads effectively, gain insights into their operations, and continuously improve supporting processes to deliver business value. 
- The Security pillar focuses on protecting data, systems, and assets. It also focuses on using cloud technologies to improve the security of your workloads.
- The Reliability pillar focuses on the ability of a workload to consistently and correctly perform its intended functions.

#### **AWS Snowmobile**

AWS Snowmobile is a service that is used for transferring up to 80 PB of data to AWS. Each Snowmobile is a 45-foot long shipping container that is pulled by a semi-trailer truck. It can transfer up to 80 PB of data.

 

***The other response options are incorrect because:***

- Amazon Neptune is a graph database service. You can use Amazon Neptune to build and run applications that work with highly connected datasets, such as recommendation engines, fraud detection, and knowledge graphs.
- Amazon CloudFront is a content delivery service.
- AWS DeepRacer is an autonomous 1/18 scale race car that you can use to test reinforcement learning models.

#### **AWS Direct Connect**


AWS Direct Connect is a service that enables you to establish a dedicated private connection between your data center and VPC. 



The private connection that AWS Direct Connect provides helps you to reduce network costs and increase the amount of bandwidth that can travel through your network.

 

The other response options are incorrect because:

- Amazon CloudFront is a content delivery service. It uses a network of edge locations to cache content and deliver content to customers all over the world.
- A virtual private gateway enables you to establish a virtual private network (VPN) connection between your VPC and a private network, such as an on-premises data center or internal corporate network. A virtual private gateway only allows traffic into the VPC only if it is coming from an approved network.
- An internet gateway is a connection between a VPC and the internet. It allows public traffic from the internet to access a VPC.


#### **Saving Plans**

Amazon EC2 Savings Plans enable you to reduce your compute costs by committing to a consistent amount of compute usage for a 1-year or 3-year term. This results in savings of up to 72% over On-Demand Instance costs. Any usage up to the commitment is charged at the discounted Savings Plan rate (for example, $10 an hour). Any usage beyond the commitment is charged at regular On-Demand Instance rates.

 

***The other response options are incorrect because:***

- Reserved Instances are a billing discount that is applied to the use of On-Demand Instances in your account. You can purchase Standard Reserved and Convertible Reserved Instances for a one-year or three-year term, and - Scheduled Reserved Instances for a one-year term. Unlike Savings Plans, Reserved Instances do not require you to commit to a consistent amount of compute usage over the duration of the contract.
Spot Instances are ideal for workloads with flexible start and end times or that can withstand interruptions. Spot Instances leverage unused EC2 computing capacity and offer you cost savings at up to 90% of On-Demand Instance prices.
- Dedicated Hosts are physical servers with EC2 instance capacity that is fully dedicated to your use. 
You can use your existing per-socket, per-core, or per-VM software licenses to help maintain license compliance. You can purchase On-Demand Dedicated Hosts or Reserved Dedicated Hosts. Of all the Amazon EC2 options that were covered in this course, Dedicated Hosts are the most expensive.


#### **Refactoring**

The other response options are incorrect because:

- Repurchasing involves replacing an existing application with a cloud-based version, such as software found in AWS Marketplace.
- Rehosting involves moving an application to the cloud with little to no modifications to the application itself. It is also known as “lift and shift.”
- Replatforming involves selectively optimizing aspects of an application to achieve benefits in the cloud without changing the core architecture of the application. It is also known as “lift, tinker, and shift.”


#### **Amazon EKS**

Amazon EKS is a fully managed service that you can use to run Kubernetes on AWS. Kubernetes is open-source software that enables you to deploy and manage containerized applications at scale.

 

Containers provide you with a standard way to package your application's code and dependencies into a single object. Containers are frequently used for processes and workflows in which there are essential requirements for security, reliability, and scalability.

 

***The other response options are incorrect because:***

- Amazon SageMaker is a service that enables you to quickly build, train, and deploy machine learning models.
- Amazon Aurora is an enterprise-class relational database. 
- Amazon Redshift is a data warehousing service that you can use for big data analytics.


#### **Availability Zone**

 

An Availability Zone is a single data center or a group of data centers within a Region. 

Availability Zones are located tens of miles apart from each other. This helps them to provide interconnectivity to support the services and applications that run within a Region.

 

The other response options are incorrect because:

- A separate geographical location with multiple locations that are isolated from each other - This response option describes a Region.
- The server from which Amazon CloudFront gets your files - This response option describes an origin.
- A site that Amazon CloudFront uses to cache copies of content for faster delivery to users at any location - This response option describes an Edge location.


#### **Amazon DynamoDB**

Amazon DynamoDB is a key-value database service. A key-value database might include data pairs such as “Name: John Doe,” “Address: 123 Any Street,” and “City: Anytown”.

 

In a key-value database, you can add or remove attributes from items in the table at any time. Additionally, not every item in the table has to have the same attributes.  

 

***The other response options are incorrect because:***

- Amazon Relational Database Service (Amazon RDS) and Amazon Aurora use structured query language (SQL) to store and query data. They are not key-value databases.
- Amazon DocumentDB is a document database service that supports MongoDB workloads.

#### **Amazon SQS**

Amazon SQS is a message queuing service. Using Amazon SQS, you can send, store, and receive messages between software components at any volume size, without losing messages or requiring other services to be available. 



In Amazon SQS, an application sends messages into a queue. A user or service retrieves a message from the queue, processes it, and then deletes it from the queue.

 

***The other response options are incorrect because: ***

- AWS Snowball is a device that enables you to transfer large amounts of data into and out of AWS.
- Amazon ElastiCache is a service that adds caching layers on top of your databases to help improve the read times of common requests.
- Amazon Route 53 is a DNS web service. It gives developers and businesses a reliable way to route end users to internet applications that are hosted in AWS. Additionally, you can transfer DNS records for existing domain names that are currently managed by other domain registrars or register new domain names directly in Amazon Route 53.
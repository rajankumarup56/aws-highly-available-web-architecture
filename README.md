# AWS Highly Available Web Architecture

## Project Overview

This project demonstrates how to design and deploy a highly available, scalable, and self-healing web architecture on Amazon Web Services (AWS).

The infrastructure automatically scales based on traffic, distributes incoming requests using a load balancer, and provides monitoring and logging capabilities for security and performance analysis.

---

## Architecture

![Architecture Diagram](architecture-diagram.png)

---

## AWS Services Used

- Amazon EC2
- Application Load Balancer
- Auto Scaling Group
- Amazon S3
- Amazon RDS (MySQL)
- Amazon CloudWatch
- AWS CloudTrail
- Amazon Athena
- IAM

---

## Key Features

- Highly Available Web Infrastructure
- Automatic scaling based on CPU utilization
- Load balancing across multiple EC2 instances
- Centralized logging and monitoring
- Database integration using Amazon RDS
- Security auditing using CloudTrail
- Log analysis using Amazon Athena

---

## Architecture Flow

User Request  
↓  
Application Load Balancer  
↓  
Target Group  
↓  
Auto Scaling Group  
↓  
EC2 Instances (Web Servers)  
↓  
Application Code from S3  

Monitoring and Logging:

CloudWatch → Performance Monitoring  
CloudTrail → API Activity Logging  
Athena → Log Analysis  

Database Layer:

Amazon RDS MySQL

---

## Implementation Steps

### 1 Create S3 Bucket

Upload application code and static assets to Amazon S3.

### 2 Launch EC2 Instance

Configure base server with required runtime environment.

### 3 Create Launch Template

Define EC2 configuration and startup script for automatic deployment.

### 4 Create Target Group

Register EC2 instances that will receive traffic from the load balancer.

### 5 Create Application Load Balancer

Distribute incoming traffic across EC2 instances.

### 6 Configure Auto Scaling Group

Ensure infrastructure automatically scales based on demand.

### 7 Configure CloudWatch Monitoring

Track CPU utilization, network traffic, and application health.

### 8 Enable CloudTrail Logging

Monitor and record AWS API activity for auditing and security.

### 9 Analyze Logs with Athena

Query CloudTrail logs using Amazon Athena.

### 10 Configure Amazon RDS

Deploy MySQL database for application data storage.

---

## Screenshots

### Load Balancer

![Load Balancer](screenshots/load-balancer.png)

### Target Group

![Target Group](screenshots/target-group.png)

### Auto Scaling Group

![Auto Scaling](screenshots/auto-scaling-group.png)

### EC2 Instances

![EC2](screenshots/ec2-instances.png)

### S3 Bucket

![S3](screenshots/s3-bucket.png)

### RDS Database

![RDS](screenshots/rds-database.png)

### CloudWatch Monitoring

![CloudWatch](screenshots/cloudwatch-monitoring.png)

### CloudTrail Logs

![CloudTrail](screenshots/cloudtrail-logs.png)

### Athena Query

![Athena](screenshots/athena-query.png)

---

## Learning Outcomes

- Designing highly available cloud architecture
- Implementing auto scaling infrastructure
- Load balancing web applications
- Monitoring AWS resources with CloudWatch
- Security auditing using CloudTrail
- Log analysis with Amazon Athena

---

## Author

Ranjan Kumar Upadhyay

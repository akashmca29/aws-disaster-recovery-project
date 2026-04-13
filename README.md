# AWS Disaster Recovery Architecture Project

## Project Overview

This project demonstrates a Disaster Recovery (DR) architecture using AWS services.

The system ensures data backup, failover capability, and high availability across regions.

---

## Architecture Diagram

![Architecture Diagram](architecture-diagram.png)

---

## Project Flow

1. Application runs in primary region (EC2 + RDS)
2. Data is backed up using AWS Backup
3. Backups stored in S3
4. Data replicated to secondary region
5. Route 53 handles failover routing
6. CloudWatch monitors system health
7. SNS sends alert notifications

---

## AWS Services Used

- Amazon EC2
- Amazon RDS
- Amazon S3
- AWS Backup
- Route 53
- CloudWatch
- SNS

---

## Features

- Automated Backup
- Cross Region Replication
- Failover Architecture
- Monitoring and Alerts
- High Availability

---
## Folder Structure
aws-disaster-recovery-project/
│
├── README.md
├── architecture-diagram.png
├── screenshots/
│   ├── ec2.png
│   ├── rds.png
│   ├── s3-backup.png
│   ├── aws-backup.png
│   ├── route53-failover.png
│   ├── cloudwatch.png
│   └── sns.png
├── backup-policy/
│   └── backup-plan.md
├── failover-steps.md
├── deployment-steps.md
├── interview-questions.md
├── resume-points.md
└── cost-estimation.md
---
## Disaster Recovery Strategy

- Backup Frequency: Daily
- Retention: 7–30 days
- Failover Type: Manual / DNS Failover
- RTO: < 15 minutes
- RPO: < 5 minutes

---

## Resume Points

- Designed disaster recovery architecture using AWS Backup and S3 replication
- Implemented cross-region failover using Route 53
- Configured CloudWatch alarms and SNS alerts
- Ensured high availability and data protection strategy

---

## Interview Questions

1. What is Disaster Recovery?
2. Difference between Backup and Replication?
3. What is RTO and RPO?
4. How does Route 53 failover work?
5. Why use S3 for backup?
6. What is AWS Backup?

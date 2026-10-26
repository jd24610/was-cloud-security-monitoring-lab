# was-cloud-security-monitoring-lab
Hands on AWS Security Lab Using S3, Cloudtrail,GuardDuty,and AwsBudgets.
# AWS Cloud Security Monitoring Lab

## Overview
This project is a hands-on lab built using the AWS Management Console to practice cloud security, storage protection, activity auditing, and threat detection.

## Objectives
- Secure cloud storage against public access.
- Configure encryption and file versioning.
- Audit AWS management activity using CloudTrail.
- Explore threat detection using Amazon GuardDuty.
- Monitor AWS spending during lab development.

## AWS Services Used
- Amazon S3: Cloud storage.
- AWS CloudTrail: Records and reviews AWS management events.
- Amazon GuardDuty: Threat detection.
- AWS Budgets: Spending alerts.
- Amazon CloudWatch: Explored metrics; S3 metrics were not located during this lab.

## Security Controls Implemented

### Amazon S3
- Created an S3 bucket.
- Enabled all four S3 Block Public Access settings.
- Verified default server-side encryption using SSE-S3.
- Enabled bucket versioning.
- Uploaded a file and verified that two versions were retained.

### AWS CloudTrail
Reviewed Event history and located these management events:
- CreateBucket
- PutBucketVersioning
- PutBucketEncryption

These events helped me understand how CloudTrail records AWS resource creation and configuration changes.

### Amazon GuardDuty
- Enabled GuardDuty.
- Checked the Findings page.
- No findings were displayed during the check.

An empty Findings page does not guarantee that an AWS account is free of threats.

### Cost Awareness
- Configured an AWS monthly budget with an alert threshold.
- Checked the AWS Billing console, which displayed $0.00 at the time of review.
- Recognized that budget alerts notify users but do not automatically stop spending.

## Skills Practiced
- AWS Management Console navigation
- Cloud storage security
- Public access prevention
- Server-side encryption
- S3 versioning and recovery concepts
- CloudTrail event investigation
- Cloud threat detection fundamentals
- Cloud cost awareness

## Lessons Learned
This lab provided practical experience configuring S3 security controls, reviewing AWS management events, exploring GuardDuty findings, and checking billing information.

It also reinforced the importance of verifying security settings and monitoring service costs.

## Future Improvements
- Add sanitized screenshots documenting the configuration.
- Explore IAM permissions and least-privilege access.
- Investigate CloudWatch metrics and monitoring options.
- Review GuardDuty findings as the lab progresses.
- Continue monitoring AWS spending and clean up unused resources.

## Disclaimer
This project was created for educational purposes in a personal AWS environment. No real-world security incident was investigated.

# AWS Video Streaming Pipeline: End-to-End Distributed Media System

[![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazon-aws)](https://aws.amazon.com)
[![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## 🎯 Project Overview

A production-grade, scalable video streaming pipeline built on AWS infrastructure, demonstrating distributed systems design, event-driven architecture, and cloud-native best practices.

### Key Features
- **Event-Driven Architecture**: Automated video processing triggered by S3 uploads
- **Asynchronous Processing**: SQS-based job queue for reliable task management
- **Scalable Transcoding**: EC2 Auto Scaling with FFmpeg for adaptive bitrate encoding
- **Global CDN Delivery**: CloudFront integration for low-latency streaming
- **Metadata Management**: RDS PostgreSQL for job tracking and video metadata
- **Comprehensive Monitoring**: CloudWatch dashboards with custom metrics and alarms

---

## 🏗️ Architecture

> Architecture diagram will be added in Phase 4

### AWS Services Used
- **Storage**: S3 (Standard, Intelligent-Tiering)
- **Compute**: Lambda (orchestration), EC2 (transcoding)
- **Messaging**: SQS (job queue)
- **Database**: RDS PostgreSQL
- **Content Delivery**: CloudFront
- **Monitoring**: CloudWatch, CloudTrail
- **Security**: IAM, VPC, Security Groups

---

## 📋 Prerequisites

- AWS Account with billing alerts configured
- AWS CLI v2.x configured
- Python 3.9+
- Git
- Basic understanding of AWS services and distributed systems

---

## 🚀 Quick Start

Setup instructions will be added as phases complete.

---

## 📁 Project Structure

aws-video-streaming-pipeline/
├── infrastructure/ # IaC configurations
│ ├── terraform/ # Terraform modules (future)
│ └── cloudformation/ # CloudFormation templates (future)
├── src/
│ ├── lambda/ # Lambda function code
│ ├── processing/ # Video transcoding scripts
│ └── utils/ # Shared utilities
├── scripts/ # Deployment and helper scripts
├── docs/ # Documentation
│ ├── architecture/ # Architecture diagrams
│ ├── setup/ # Setup guides
│ ├── operations/ # Operations runbooks
│ └── screenshots/ # Phase screenshots
├── tests/ # Unit and integration tests
└── sample-videos/ # Sample media files (not committed)

---

## 📚 Documentation

- [Phase 1: Environment Setup](docs/setup/phase-1-environment.md) *(In Progress)*
- [Phase 2: Core Infrastructure](docs/setup/phase-2-infrastructure.md) *(Coming Soon)*
- [Phase 3: Processing Logic](docs/setup/phase-3-processing.md) *(Coming Soon)*
- [Phase 4: Monitoring & Operations](docs/operations/phase-4-monitoring.md) *(Coming Soon)*
- [Portfolio Showcase](docs/PORTFOLIO.md) *(In Progress)*

---

## 🔒 Security Considerations

- All AWS credentials stored in AWS Secrets Manager (not in code)
- IAM roles with least-privilege permissions
- VPC isolation for compute resources
- S3 bucket encryption at rest
- CloudFront signed URLs for content protection

---

## 💰 Cost Estimation

Estimated monthly cost for moderate usage: **$15-30 USD**
- S3: ~$5 (100GB storage + requests)
- EC2: ~$10 (t3.medium spot instances)
- RDS: ~$15 (db.t3.micro)
- Lambda: <$1 (within free tier)
- CloudFront: ~$5 (10GB transfer)

*Costs vary based on usage. Monitor via AWS Cost Explorer.*

---

## 🎓 Learning Outcomes

By completing this project, you will demonstrate:
- Cloud infrastructure design and implementation
- Event-driven and asynchronous architecture patterns
- Video processing and media workflows
- Infrastructure as Code principles
- Monitoring and observability practices
- DevOps and CI/CD concepts

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👤 Author

**Chiranjibi Dewangan**
- Portfolio : https://chiranjibidewangan.com/
- LinkedIn  : https://www.linkedin.com/in/chiranjibi-dewangan 
- GitHub    : https://github.com/Chiranjibi-Dewangan

---

## 🙏 Acknowledgments

- AWS Documentation and Well-Architected Framework
- FFmpeg open-source community


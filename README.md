# 🏥 MediHelp - Automated AWS Healthcare Infrastructure

A production-ready infrastructure project using **Terraform** to deploy a secure, scalable, and serverless medical portal on **Amazon Web Services (AWS)**.

## 🏗️ Architecture Overview
The system is designed with high availability and security best practices:
- **Networking**: Custom VPC with Multi-AZ deployment (2 Public subnets, 2 Private subnets).
- **Security**: Granular Security Groups for Lambda, RDS, and API Gateway.
- **Compute**: AWS Lambda (Node.js/Python) handling backend logic.
- **Database**: Amazon RDS (MySQL/PostgreSQL) isolated in private subnets.
- **API Management**: AWS API Gateway (HTTP API) as the entry point.
- **State Management**: Remote Backend using S3 with DynamoDB for State Locking.



## 🛠️ Infrastructure Modules
- `/modules/networking`: Sets up VPC, IGW, Route Tables, and Subnets.
- `/modules/database`: Provisions the RDS instance and Subnet Groups.
- `/modules/compute`: Deploys Lambda functions and IAM Execution Roles.
- `/modules/api-gateway`: Maps the Lambda to a public-facing API endpoint.

## ⚙️ Prerequisites
- Terraform v1.0+
- AWS CLI configured with appropriate IAM permissions.
  `
2. Initialize Terraform: `terraform init`
3. Review execution plan: `terraform plan`
4. Deploy resources: `terraform apply -auto-approve`# -Automated-AWS-Healthcare-Infrastructure
  
## Screenshorts
https://github.com/cit-24-01-0532-cyber/-Automated-AWS-Healthcare-Infrastructure/blob/main/Screenshot%202026-05-28%20175043.png
https://github.com/cit-24-01-0532-cyber/-Automated-AWS-Healthcare-Infrastructure/blob/main/Screenshot%202026-05-28%20163552.png
https://github.com/cit-24-01-0532-cyber/-Automated-AWS-Healthcare-Infrastructure/blob/main/Screenshot%202026-05-28%20180847.png
https://github.com/cit-24-01-0532-cyber/-Automated-AWS-Healthcare-Infrastructure/blob/main/screenshort.png

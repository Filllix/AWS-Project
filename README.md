# AWS Cloud Engineering Portfolio

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?logo=amazon-aws&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-IaC-623CE4?logo=terraform&logoColor=white)
![DevOps](https://img.shields.io/badge/Focus-DevOps%20%26%20Cloud-blue)

This repository documents hands-on AWS projects built as part of a Cloud Engineer and DevOps learning journey. It focuses on practical infrastructure tasks: deploying compute resources, configuring networking components, enabling monitoring, and introducing Infrastructure as Code with Terraform.

The goal is to make each project easy to review for recruiters, collaborators, and freelance clients by showing clear documentation, repeatable steps, and project outcomes.

## Project Highlights

| Area | Project | Skills Demonstrated |
| --- | --- | --- |
| EC2 | [Deploy a simple website on AWS EC2](docs/ec2/simple-web-deployment-on-aws-ec2.pdf) | EC2, Linux, Nginx, security groups |
| Load Balancing | [Create an Application Load Balancer](docs/ec2/create-application-load-balancer.pdf) | ALB, target groups, HTTP routing |
| Scalability | [Create an Auto Scaling Group](docs/ec2/create-auto-scaling-group.pdf) | ASG, launch templates, scaling strategy |
| Monitoring | [Create CloudWatch monitoring](docs/ec2/create-cloudwatch-monitoring.pdf) | Metrics, alarms, observability |
| Identity | [Create an IAM user](docs/ec2/create-iam-user.pdf) | IAM users, permissions, access control |
| Terraform | [Deploy an EC2 server using Terraform](docs/terraform/deploy-ec2-server-using-terraform.pdf) | Terraform workflow, AWS provider, IaC |
| Terraform | [Create a Terraform module](docs/terraform/create-terraform-module.pdf) | Modules, reusability, infrastructure structure |

## Repository Structure

```text
.
|-- EC2-PROJECT/
|   `-- README.md
|-- TERRAFORM-PROJECT/
|   `-- README.md
|-- docs/
|   |-- ec2/
|   `-- terraform/
|-- .gitignore
`-- README.md
```

## Documentation

- [EC2 project documentation](EC2-PROJECT/README.md)
- [Terraform project documentation](TERRAFORM-PROJECT/README.md)
- [All project PDFs](docs/README.md)

## Skills Covered

- AWS EC2 server provisioning
- Linux server setup and Nginx deployment
- Security group and access configuration
- Application Load Balancer setup
- Auto Scaling Group configuration
- CloudWatch monitoring basics
- IAM user and permission management
- Terraform-based infrastructure provisioning
- Terraform module creation for reusable infrastructure

## Next Improvements

- Add Terraform source code examples for each infrastructure scenario.
- Add architecture diagrams for EC2, ALB, ASG, and monitoring flows.
- Add a CI workflow for Terraform formatting and validation.
- Add cost estimation notes and AWS cleanup steps for each project.
- Convert PDF walkthroughs into Markdown guides for easier review.

## Author

Created by [Filllix](https://github.com/Filllix) as a Cloud Engineer and DevOps portfolio project.

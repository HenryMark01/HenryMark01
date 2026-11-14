Hi there, I'm Henry!
=============================================================================================================================

Cloud Engineer based in Malaysia, building and running AWS infrastructure for enterprise customers. I started in system administration, managing on-premises and virtualized environments, then moved into AWS and automation.

Day to day I work on multi-account landing zones, hybrid networking (Transit Gateway, FortiGate, site-to-site VPN), Active Directory on AWS, centralized monitoring and security, and everything delivered as code with AWS CDK and Terraform through CI/CD pipelines.

I'm always learning. If you want to talk cloud architecture, networking or automation, feel free to reach out on [LinkedIn](https://linkedin.com/in/henrytharan).

## ⭐ Featured: Production Work

Real systems I designed and delivered, sanitized for public sharing.

### [AWS Multi-Account Landing Zone](https://github.com/HenryMark01/aws-multi-account-landing-zone)
Hub-and-spoke landing zone for 9 business units across 20 AWS accounts, built with AWS CDK (Python).
- Transit Gateway shared through RAM, FortiGate HA cluster terminating IPSec VPN from branch offices
- CloudFront + Global and Regional WAF in front of centralized public ALBs
- Shared services: Active Directory, private DNS, SIEM gateway
- Cross-account monitoring hub with CloudWatch OAM, auto-discovery Lambda and dynamic alarms
- Review-gated pipelines per account: synth, diff, drift check, manual approval

<a href="https://github.com/HenryMark01/aws-multi-account-landing-zone"><img src="https://raw.githubusercontent.com/HenryMark01/aws-multi-account-landing-zone/main/docs/images/architecture.png" width="800" alt="Multi-account landing zone architecture"></a>

### [Secure Edge-to-Cloud File Ingestion](https://github.com/HenryMark01/secure-edge-to-cloud-ingest)
Moves files from remote Windows sites into AWS **without any AWS credentials on the site PCs**.
- Windows agent uploads through short-lived S3 presigned URLs from API Gateway + Lambda
- Every file is malware scanned with ClamAV, then delivered to a private server through SSM (no SSH)
- Cross-region CI/CD builds, configures and signs the Windows installer automatically
- Replaced a v1 design that shipped long-lived IAM keys on every PC

<a href="https://github.com/HenryMark01/secure-edge-to-cloud-ingest"><img src="https://raw.githubusercontent.com/HenryMark01/secure-edge-to-cloud-ingest/main/docs/images/architecture.png" width="800" alt="Secure file ingestion architecture"></a>

### [LiteLLM AI Gateway on AWS](https://github.com/HenryMark01/litellm-ai-gateway-aws)
Self-hosted AI gateway giving teams one OpenAI-compatible endpoint for Amazon Bedrock, OpenAI and Anthropic, built with Terraform.
- ECS Fargate (gateway, backend, admin UI) with PostgreSQL and Redis, behind an ALB
- Cross-account Bedrock access through an assumed IAM role, no provider keys needed
- Model routing, retries and prompt caching from an S3-hosted config, secrets in Secrets Manager
- Bootstrap stage for state and least-privilege deploy policies, plus Checkov, smoke and integration test scripts

<a href="https://github.com/HenryMark01/litellm-ai-gateway-aws"><img src="https://raw.githubusercontent.com/HenryMark01/litellm-ai-gateway-aws/main/docs/images/architecture.png" width="800" alt="LiteLLM AI gateway architecture"></a>

## Other Projects

### Cloud Projects
- AWS Architecture Deployment with Terraform. [Link](https://github.com/HenryMark01/terraform-architecture-aws)
- Building a Serverless Web Application. [Link](https://github.com/HenryMark01/AWS-Projects/tree/main/Cloud%20Based%20e-book%20Delivery%20Solution)
- Distributed Load Testing on AWS. [Link](https://github.com/HenryMark01/distributed-load-testing-aws)
- Server Migration from GCP to AWS. [Link](https://github.com/HenryMark01/gcp-to-aws-cloud-migration)
- Creating your own VPC and 3 Tier Application. [Link](https://github.com/HenryMark01/Three-Tier-Application-on-AWS)
- Serverless Email Marketing App. [Link](https://github.com/HenryMark01/AWS-Projects/tree/main/Serverless%20Email%20Marketing%20App)
### DevOps Projects
- Kubernetes manifests to deploy architecture on AWS EKS. [Link](https://github.com/HenryMark01/kubernetes-aws-eks)
- Cloud-Native CICD Pipeline Automation: BoardGame Web Hosting. [Link](https://github.com/HenryMark01/Boardgame)
- Automated CI/CD Pipeline with Ansible and Kubernetes (Containerization). [Link](https://github.com/HenryMark01/kubernetes_project)
### AI Projects
- Blog Generator using GenAI (Amazon Bedrock). [Link](https://github.com/HenryMark01/lambda-bedrock/tree/main)

## Knowledgeable in:
- ☁️ Cloud Platform: AWS (multi-account with AWS Organizations)
- 🌐 Networking: VPC, Transit Gateway, RAM, VPC Endpoints, Route 53, FortiGate HA, Site-to-Site VPN
- 🏗 Infrastructure as Code: AWS CDK (Python), Terraform, CloudFormation, Ansible
- 🤖 AI Platform: LiteLLM, Amazon Bedrock, OpenAI and Anthropic APIs
- ∞ CI/CD: AWS CodePipeline / CodeBuild, GitHub Actions, Jenkins
- 🔐 Security: AWS WAF, IAM cross-account roles, Secrets Manager, ClamAV, Checkov, OWASP Dependency Check, Trivy, SonarQube
- 📊 Monitoring: CloudWatch (OAM, alarms, dashboards), SNS, EventBridge
- 🪟 Identity: Active Directory on AWS, Entra Connect
- 🐳 Containers: Docker, Kubernetes, Amazon EKS, ECS Fargate
- 🛠️ Build & Artifacts: Maven, Nexus3
- 🦊 Source Code Management: Git
- 🐧 Operating Systems: Windows Server, Linux
- 🐍 Languages: Python, PowerShell, Bash

## I also enjoy life. In my spare time, you can find me:
- 🎸 Playing Guitar & Singing (Performed in Concerts)
- 🧗🏻‍♀️ Hiking (Nature's Best Friend)
- 🏊 Swimming (Junior Aquaman)

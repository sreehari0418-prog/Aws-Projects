# Blood Fit - AI-Powered Medical Report Analysis System

An enterprise-grade serverless application designed to automate the extraction and analysis of clinical blood markers from medical reports using AWS AI services.

## 🚀 Key Features
- **AI-Driven Extraction**: Uses Amazon Textract for high-accuracy OCR and Amazon Comprehend for clinical data parsing.
- **Massive Medical Library**: Recognizes 50+ key blood markers across CBC, Metabolic, Lipid, and Endocrine panels.
- **DevSecOps Pipeline**: Fully automated CI/CD using GitHub Actions and containerization via Docker.
- **GitOps Deployment**: Automated cluster synchronization using Argo CD on AWS EKS.

## 🏗️ Architecture
```mermaid
graph TD
    A[User Upload] --> B[S3 Bucket]
    B --> C[AWS Textract]
    C --> D[Lambda Processor]
    D --> E[AWS Comprehend]
    E --> F[DynamoDB Table]
    F --> G[API Gateway]
    G --> H[Frontend UI]
    
    subgraph "CI/CD & GitOps"
    I[GitHub Repo] --> J[GitHub Actions]
    J --> K[Docker Hub]
    L[Argo CD] --> I
    L --> M[AWS EKS]
    end
```

## 🛠️ Tech Stack
- **AI/ML**: AWS Textract, AWS Comprehend
- **Compute**: AWS Lambda, AWS EKS
- **Database**: Amazon DynamoDB, Amazon S3
- **DevOps**: GitHub Actions, Docker, ArgoCD, Terraform

## 📺 Demo
Click the `demo-recording.mov` file in this folder to see the full pipeline in action!

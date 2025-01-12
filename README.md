# 30-Day DevOps Project: Multi-Cloud Deployment Across AWS, Azure, and GCP

## **Overview**
This project is a 30-day challenge designed to build and deploy a robust DevOps workflow leveraging the three major cloud providers: AWS, Azure, and GCP. The goal is to create scalable, secure, and automated infrastructure solutions while learning cloud-agnostic practices for modern DevOps.

---

## **Project Structure**
The repository is organized into separate directories for each cloud provider:

```
DEVOPS/
├── .venv/                 # Python virtual environment (ignored by Git)
├── aws/                   # AWS-specific configurations and resources
│   ├── weather-dashboard-demo/ # Example AWS application
│   ├── terraform/         # Infrastructure as Code (IaC) for AWS
│   └── scripts/           # Automation scripts for AWS
├── azure/                 # Azure-specific configurations and resources
│   ├── terraform/         # Infrastructure as Code (IaC) for Azure
│   └── scripts/           # Automation scripts for Azure
├── gcp/                   # GCP-specific configurations and resources
│   ├── terraform/         # Infrastructure as Code (IaC) for GCP
│   └── scripts/           # Automation scripts for GCP
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (ignored by Git)
├── .gitignore             # Ignored files and folders
└── README.md              # Project documentation (this file)
```

---

## **Project Goals**
1. Learn and apply DevOps principles for multi-cloud environments.
2. Deploy infrastructure using Infrastructure as Code (IaC) with Terraform.
3. Automate CI/CD pipelines for applications across AWS, Azure, and GCP.
4. Explore cloud-specific services and their equivalents across providers.
5. Monitor and optimize deployments with cloud-native monitoring tools.

---

## **Day-by-Day Plan**

### **Week 1: Setup and Foundation**
- **Day 1-2**: Configure environments for AWS, Azure, and GCP.
  - Install necessary CLI tools (AWS CLI, Azure CLI, gcloud CLI).
  - Authenticate with each cloud provider.
- **Day 3**: Set up Terraform workspaces for each cloud.
- **Day 4-5**: Design architecture diagrams for each environment.
- **Day 6-7**: Create S3, Blob, and Cloud Storage buckets for static hosting.

### **Week 2: Infrastructure as Code**
- **Day 8-9**: Write Terraform code to provision resources:
  - AWS: EC2, RDS, and S3.
  - Azure: Virtual Machines, SQL Databases, and Blob Storage.
  - GCP: Compute Engine, Cloud SQL, and Cloud Storage.
- **Day 10**: Test infrastructure deployment.
- **Day 11**: Automate deployments with GitHub Actions.
- **Day 12-14**: Add security layers (IAM roles, policies, VPCs, etc.).

### **Week 3: Application Deployment**
- **Day 15-16**: Deploy a sample application (Weather Dashboard) to each cloud:
  - AWS: Elastic Beanstalk or ECS.
  - Azure: App Service.
  - GCP: App Engine or Cloud Run.
- **Day 17**: Configure load balancers and auto-scaling.
- **Day 18-19**: Set up CI/CD pipelines for continuous delivery.
- **Day 20-21**: Implement logging and monitoring (e.g., CloudWatch, Azure Monitor, GCP Operations Suite).

### **Week 4: Optimization and Documentation**
- **Day 22-23**: Optimize cost and performance across all clouds.
- **Day 24-25**: Implement disaster recovery strategies (e.g., backups, multi-region).
- **Day 26**: Conduct security audits.
- **Day 27**: Write comprehensive documentation.
- **Day 28-29**: Present findings and compare cloud-specific features.
- **Day 30**: Submit project and reflect on the learning journey.

---

## **Technologies and Tools**

### **Languages**
- Python: Scripting and automation
- YAML: CI/CD configuration

### **Tools**
- Terraform: Infrastructure as Code (IaC)
- Docker: Containerization
- GitHub Actions: CI/CD pipelines
- AWS CLI, Azure CLI, gcloud CLI: Cloud interaction

### **Cloud Services**
- **AWS**: S3, EC2, RDS, CloudWatch, IAM
- **Azure**: Blob Storage, Virtual Machines, SQL Databases, Azure Monitor
- **GCP**: Cloud Storage, Compute Engine, Cloud SQL, Operations Suite

---

## **Setup Instructions**

### **1. Clone the Repository**
```bash
git clone <REPO_URL>
cd DEVOPS
```

### **2. Set Up Python Environment**
```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

### **3. Configure Environment Variables**
- Create a `.env` file at the root level with the following:
  ```env
  # AWS Config
  AWS_ACCESS_KEY_ID=your_aws_key
  AWS_SECRET_ACCESS_KEY=your_aws_secret
  AWS_DEFAULT_REGION=us-east-1

  # Azure Config
  AZURE_SUBSCRIPTION_ID=your_subscription_id
  AZURE_CLIENT_ID=your_client_id
  AZURE_SECRET=your_secret
  AZURE_TENANT_ID=your_tenant_id

  # GCP Config
  GOOGLE_APPLICATION_CREDENTIALS=path/to/your/credentials.json
  ```

### **4. Deploy Infrastructure**
- Navigate to each cloud-specific folder and apply Terraform configurations:
  ```bash
  cd aws/terraform
  terraform init
  terraform apply
  ```

---

## **Contributing**
1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push the branch:
   ```bash
   git push origin feature-name
   ```
5. Open a Pull Request.

---

## **License**
This project is licensed under the MIT License. See the LICENSE file for details.

---

## **Acknowledgments**
Special thanks to the open-source community and cloud providers for their tools and resources.


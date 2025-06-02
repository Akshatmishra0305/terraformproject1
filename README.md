# 🌐 Terraform AWS Infrastructure Project

This project provisions a complete AWS infrastructure using **Terraform**, designed for scalability, availability, and automation. It includes a custom VPC, public subnets, EC2 instances, a load balancer, and an S3 bucket.

## 🚀 What This Project Does

- Creates a **custom VPC** with CIDR `10.0.0.0/16`
- Provisions **2 public subnets** in `us-east-1a` and `us-east-1b`
- Attaches an **Internet Gateway** and sets up route tables
- Launches **2 EC2 instances** in different availability zones
- Deploys an **Application Load Balancer (ALB)** with a Target Group and Listener
- Attaches the EC2 instances to the ALB
- Creates a **public S3 bucket**
- Configures **Security Groups** for HTTP and SSH access
- Uses **user data scripts** (`userdata.sh`, `userdata1.sh`) for EC2 initialization
- Outputs the **ALB DNS name** on successful deployment

## 📁 Project Structure

terraformproject1/
├── main.tf # Main Terraform configuration
├── userdata.sh # User data script for EC2 instance 1
├── userdata1.sh # User data script for EC2 instance 2
└── README.md # Project documentation


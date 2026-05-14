CI/CD Pipeline for Attendance Application-11

📌 Project Overview

This project demonstrates how to automate deployment of an Attendance Management Application using AWS CodePipeline, EC2, and Amazon S3.

The main objective of this project is to automatically deploy the attendance system whenever code changes are made. The CI/CD pipeline improves deployment speed, reduces manual effort, and ensures continuous integration and deployment.

This project helps in understanding DevOps automation and cloud-based deployment workflows using AWS services.

---
🎯 Objective
Automate application deployment
Implement Continuous Integration
Implement Continuous Deployment
Reduce manual deployment tasks
Improve deployment efficiency
Build cloud-based DevOps workflow

---
🧰 AWS Services Used
1. AWS CodePipeline

Used to automate the complete CI/CD workflow.

2. Amazon EC2

Used to host the Attendance Management Application.

3. Amazon S3

Used to store deployment artifacts and source files.

4. IAM Roles

Used to securely manage AWS permissions.

5. Security Groups

Used to securely manage inbound and outbound traffic.

---

🏗️ Project Architecture

The project architecture includes:

Uploading Source Code
Creating S3 Artifact Bucket
Creating EC2 Deployment Server
Creating CodePipeline Workflow
Connecting Deployment Stages
Deploying Attendance Application
Automating Deployment Process
Testing CI/CD Pipeline

---
⚙️ Project Folder Structure
11. CICD Pipeline for Attendance Application/
│
├── app/
│   ├── templates/
│   ├── static/
│   ├── app.py
│   └── requirements.txt
│
├── pipeline/
│   ├── buildspec.yml
│   ├── appspec.yml
│   └── deploy.sh
│
├── scripts/
│   ├── install_dependencies.sh
│   └── start_server.sh
│
├── images/
│
└── README.md

---
⚙️ Step-by-Step Implementation
Step 1: Launch EC2 Instance
Open AWS Console
Go to EC2 Dashboard
Launch EC2 Instance
Select Ubuntu or Amazon Linux AMI
Configure Security Group
Allow:
HTTP (Port 80)
SSH (Port 22)
---

Step 2: Connect to EC2 Instance

Use SSH to connect:

ssh -i key.pem ec2-user@your-public-ip
---

Step 3: Install Application Dependencies

Install required packages:

sudo yum update -y
sudo yum install python3 -y
pip3 install -r requirements.txt
---

Step 4: Create S3 Bucket
Create Amazon S3 bucket
Store deployment artifacts
Configure bucket permissions

---

Step 5: Create CodePipeline
Configure source stage
Configure deployment stage
Connect EC2 deployment server
Enable automatic deployment workflow

---

Step 6: Deploy Attendance Application

Run application server:

python3 app.py

Verify deployment using browser.

---
Step 7: Test CI/CD Pipeline
Push code changes
Trigger pipeline automatically
Verify deployment success
Verify Attendance Application functionality

---

📸 Project Screenshots

<img width="1909" height="803" alt="Screenshot 2026-04-23 195955" src="https://github.com/user-attachments/assets/aff9f0cd-41d2-4bfb-b93c-e64c7a21b56b" />


🔹 Attendance Application Output
<img width="1141" height="587" alt="image" src="https://github.com/user-attachments/assets/f41690c8-687c-4639-aa0a-db354b139bc2" />



---
✅ Features
Automated CI/CD Workflow
Continuous Integration
Continuous Deployment
Automatic Deployment Trigger
Scalable Deployment Process
Cloud-based DevOps Automation
Secure AWS Infrastructure

---
📚 Learning Outcomes

Through this project, I learned:

How CI/CD pipelines work
How AWS CodePipeline automates deployment
How to deploy applications on EC2
Artifact management using S3
DevOps automation workflow
AWS service integration
Cloud deployment process
🚀 Future Improvements
Add Load Balancer
Configure Auto Scaling
Add CloudWatch Monitoring
Add HTTPS Support
Implement Docker Containerization
Add Notification System using SNS

---
🏁 Conclusion

This project successfully demonstrates automated CI/CD pipeline deployment for an Attendance Management Application using AWS CodePipeline, EC2, and Amazon S3. The infrastructure automates deployment workflows, improves software delivery efficiency, and reduces manual deployment tasks.

---
👩‍💻 Author

Akshata Naik
---

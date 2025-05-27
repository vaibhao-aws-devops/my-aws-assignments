# Apache2 Web Server Setup on AWS EC2

## Objective
To launch an Apache2 Web Server manually and using a shell script on an Ubuntu EC2 instance.

## Steps Performed

### 1. Launch EC2 Instance
- Logged into AWS Console
- Navigated to EC2 Dashboard and launched a new instance
- Selected Ubuntu AMI (Free Tier eligible)
- Chose instance type `t2.micro`
- Created key pair for SSH access
- Enabled auto-assign public IP
- Used default VPC settings
- Added EBS volume
- Launched the instance successfully

### 2. Manual Apache2 Installation
- Connected to EC2 via Git Bash using SSH
- Ran the following commands:
  ```bash
  sudo apt update
  sudo apt install apache2 -y
  sudo systemctl start apache2
  sudo systemctl enable apache2

Apache2 service verified via browser using Public IP

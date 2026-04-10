# aws-s3-rds-secure-data-storage
Secure data storage using AWS S3 and RDS

# AWS S3 + RDS Secure Data Storage 🚀

This project demonstrates a secure cloud architecture using AWS services including EC2, S3, and RDS to store and manage data efficiently.

---

# Project Overview

In this project:

* EC2 instance is used as an application server
* RDS (MySQL) is used as a database
* S3 bucket is used for storing files
* Secure communication is established between services

---

## 🏗️ Architecture

Client → EC2 Instance → (S3 + RDS)

* EC2 handles requests
* Files are stored in S3
* Structured data is stored in RDS
* All services are configured securely

---

## ⚙️ Services Used

* Amazon EC2 (t2.micro)
* Amazon RDS (MySQL)
* Amazon S3
* IAM (for secure access)
* VPC (default)

---

# EC2 Instance

* Instance Name: ec2-for-rds
* Instance Type: t2.micro
* Status: Running
* Region: ap-south-1

EC2 is used to connect with both S3 and RDS securely.

---

## 🗄️ RDS Database

* DB Name: database-1
* Engine: MySQL
* Status: Available
* Port: 3306

RDS is used to store structured data and is not publicly exposed.

---

## 📦 S3 Bucket

* File Uploaded: test.txt
* Region: ap-south-1

S3 is used for object storage like files and backups.

---

## 🔐 Security Features

* EC2 connects to RDS using private access
* IAM roles used for S3 access (no hardcoded credentials)
* RDS public access disabled
* Secure ports and access control

---

## 📸 Project Screenshots

### EC2 Instance Running

![EC2](ec2-instance-running.png)

### RDS Database Available

![RDS](rds-database-available.png)

### S3 Bucket Object

![S3](s3-bucket-object.png)

---

# How It Works

1. User sends request to EC2
2. EC2 processes the request
3. Files are stored/retrieved from S3
4. Data is stored/retrieved from RDS

---


---





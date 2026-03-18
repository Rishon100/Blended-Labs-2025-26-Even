# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: V RISHON ANAND
* **Register Number**: 212224240135
* **Date of Submission**: 18/03/2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

Step 1: Create DB Security Group (allow MySQL 3306 from Web Security Group)
Step 2: Create DB Subnet Group (2 AZ subnets)
Step 3: Create RDS MySQL DB (Multi-AZ, lab-db)
Step 4: Connect web app to database using endpoint
---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

(Insert Screenshot Here)
<img width="1919" height="1032" alt="Screenshot 2026-03-14 201817" src="https://github.com/user-attachments/assets/56e291bc-4c27-4771-9988-9ae38fdbb187" />

---

### Screenshot 2: Database Service Running

(Insert Screenshot Here)
<img width="1919" height="1030" alt="Screenshot 2026-03-14 201946" src="https://github.com/user-attachments/assets/f6dee63e-edac-478d-b280-e7b0a1520b60" />

---

### Screenshot 3: Sample Database and Table

(Insert Screenshot Here)
<img width="1919" height="1043" alt="Screenshot 2026-03-14 202313" src="https://github.com/user-attachments/assets/385dcf31-fdbd-465e-bd41-9c8fd7dcb325" />

---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst

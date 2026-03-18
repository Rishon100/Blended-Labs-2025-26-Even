# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: V Rishon Anand
* **Register Number**: 212224240135
* **Date of Submission**: 15/03/2026

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. Open AWS Management Console → EC2 → Launch Instance and name the instance Web Server in the N. Virginia region.
2. Select Amazon Linux 2023 AMI, choose t2.micro instance type, and select the vockey key pair.
3. Configure Network Settings by selecting Lab VPC, PublicSubnet1, and create a Web Server security group.
4. Enable termination protection and add a User Data script to install and start the Apache web server.
5. Launch the instance and monitor it using Status Checks, CloudWatch monitoring, system logs, and instance screenshot.

---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List


<img width="1919" height="1030" alt="lab3 1" src="https://github.com/user-attachments/assets/133f0c34-2e8e-4dbb-98c2-1e82ac988036" />

---

### Screenshot 2: SSH Connection to Instance

(Insert Screenshot Here)
<img width="1919" height="1032" alt="Screenshot 2026-02-27 102019" src="https://github.com/user-attachments/assets/19e02140-7db6-4444-b130-b97d8e276b91" />

---

### Screenshot 3: Instance Monitoring / Status

(Insert Screenshot Here)
<img width="1919" height="1024" alt="Screenshot 2026-02-27 111814" src="https://github.com/user-attachments/assets/547e2c3f-f143-4372-90a5-3ae489e70950" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

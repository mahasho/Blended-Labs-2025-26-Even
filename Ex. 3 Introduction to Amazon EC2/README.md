# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: RITHISH RAM M
* **Register Number**: 212225040345
* **Date of Submission**: 17.11.2026

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

First, I logged in to the AWS Management Console using my AWS account.

I searched for EC2 in the services section and opened the EC2 Dashboard.

I explored different sections like Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs to understand their functions.

I clicked on the “Launch Instance” button to create a new EC2 instance.

I selected Amazon Linux 2 AMI as the operating system.

I chose the t2.micro instance type because it is eligible for the AWS Free Tier.

I entered a name for my instance to identify it easily.

I created a new key pair, selected the PEM format, and downloaded it to my system.

I configured the security group settings.

I allowed SSH access on Port 22 only from my IP address.

I allowed HTTP access on Port 80 from anywhere (0.0.0.0/0).

I reviewed all the configurations and clicked on “Launch Instance.”

After launching, I waited until the instance state changed to “Running.”

I copied the public IP address of the instance from the EC2 dashboard.

I opened the terminal and navigated to the folder where the key pair file was saved.

I connected to the instance using the SSH command:
ssh -i "keyname.pem" ec2-user@<Public-IP>

I successfully logged in to the Amazon Linux server.

I went back to the EC2 console and selected the instance.

I clicked on “Stop” and observed the instance state changing to “Stopped.”

I clicked on “Start” and observed the state changing back to “Running.”

I also performed the “Reboot” operation and noticed that the instance restarted.

I opened the “Monitoring” tab to check CPU utilization and network metrics.

I observed the status checks to ensure the instance was running properly.

After completing the experiment, I selected the instance and clicked on “Terminate.”

I confirmed the termination and observed that the instance state changed to “Terminated.”

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1261" height="763" alt="image" src="https://github.com/user-attachments/assets/fb5335b4-40e8-48cc-8e95-aea2e1a8a830" />


---

### Screenshot 2: SSH Connection to Instance

<img width="1269" height="834" alt="image" src="https://github.com/user-attachments/assets/fb10691d-9f39-478c-8424-11c1c9cd418f" />
<img width="1258" height="719" alt="image" src="https://github.com/user-attachments/assets/c1a51b4b-40d2-4178-8f70-cb53ccb658fa" />

---

### Screenshot 3: Instance Monitoring / Status

<img width="1262" height="828" alt="image" src="https://github.com/user-attachments/assets/e405980c-352a-4b2b-b200-69f4a76662eb" />


---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

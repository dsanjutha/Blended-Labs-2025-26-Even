# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: Sanjutha D
* **Register Number**:212225240136


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

```
1.Logged in to the AWS Management Console and opened the EC2 Dashboard.
2.Explored Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.
3.Clicked Launch Instance and selected Amazon Linux 2 AMI.
4.Selected the t2.micro instance type and entered a name for the instance.
5.Created and downloaded a PEM key pair for secure SSH access.
6.Configured the Security Group by allowing SSH (Port 22) from my IP and HTTP (Port 80) from anywhere.
7.Reviewed the settings and launched the EC2 instance, then waited until it reached the Running state.
8.Copied the public IP and connected to the server using SSH through the terminal.
9.Tested Stop, Start, Reboot, and checked Monitoring and Status Checks.
10.After completing the experiment, terminated the EC2 instance and confirmed its state changed to Terminated.
```


---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="851" height="462" alt="image" src="https://github.com/user-attachments/assets/9a475902-1a1a-4591-a24b-ee65eff622cb" />



<img width="835" height="857" alt="image" src="https://github.com/user-attachments/assets/bc7a4c24-49d6-46c8-8bb8-e3f4e5401642" />


---

### Screenshot 2: SSH Connection to Instance

<img width="852" height="442" alt="image" src="https://github.com/user-attachments/assets/3beb5c48-faaf-4e07-aedb-ce149c56a6b0" />

<img width="851" height="435" alt="image" src="https://github.com/user-attachments/assets/088180d6-9926-49ad-b468-5cfe6057aba8" />


<img width="381" height="120" alt="image" src="https://github.com/user-attachments/assets/bf89cb44-4157-4f45-8885-0a193109b95e" />




---

### Screenshot 3: Instance Monitoring / Status
<img width="847" height="432" alt="image" src="https://github.com/user-attachments/assets/b97e8ca2-77c2-4511-815b-d270bbc08b67" />

<img width="852" height="441" alt="image" src="https://github.com/user-attachments/assets/a0123589-34f4-4d9f-ab55-8d193b05de62" />

---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.

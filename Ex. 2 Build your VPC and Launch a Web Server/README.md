# Build Your VPC and Launch a Web Server (AWS) 

## Author

* **Name**: Sanjutha D
* **Register Number**: 212225240136


---

## Objective

The objective of this experiment is to understand how to design and configure a basic network infrastructure in AWS using a Virtual Private Cloud (VPC). This lab focuses on creating a VPC with a public subnet, configuring an Internet Gateway and route table, launching an EC2 instance, and hosting a simple web server that can be accessed over the internet.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity

---

## Tools Used

* AWS Management Console
* Amazon VPC
* Amazon EC2
* Internet Gateway
* Route Table
* Security Groups

---

## Tasks Performed

### Task 1: Create a VPC

Create a new Virtual Private Cloud (VPC) with a private IP address range. The VPC acts as a logically isolated network in AWS where all other resources will be deployed.

Students should create a VPC with an appropriate CIDR block (for example, 10.0.0.0/16) and assign a meaningful name.

### Task 2: Create a Public Subnet

Create a subnet inside the VPC to host public resources. Enable auto-assign public IPv4 so that instances launched in this subnet receive a public IP address.

The subnet should use a smaller CIDR range (for example, 10.0.1.0/24).


### Task 3: Create and Attach Internet Gateway

Create an Internet Gateway (IGW) and attach it to the VPC. This allows communication between resources in the VPC and the internet.


### Task 4: Configure Route Table

Create a route table and add a default route (0.0.0.0/0) pointing to the Internet Gateway. Associate this route table with the public subnet.

This step ensures that traffic from the subnet can reach the internet.


### Task 5: Create Security Group

Create a security group to act as a virtual firewall for the EC2 instance. Configure inbound rules to allow:

SSH on port 22

HTTP on port 80


### Task 6: Launch EC2 Instance

Launch an EC2 instance inside the public subnet using Amazon Linux 2 AMI and a suitable instance type (t2.micro).

Attach the previously created security group and key pair.


### Task 7: Configure Web Server

Install and start a web server (Apache HTTPD) on the EC2 instance using user data or manual commands.

Create a simple HTML page and verify that it can be accessed from a web browser using the public IP address of the instance.---

## Workflow (Student Explanation)

```
1.Create a VPC with a suitable IPv4 CIDR block, such as 10.0.0.0/16.

2.Create a public subnet inside the VPC, such as 10.0.1.0/24.

3.Create and attach an Internet Gateway (IGW) to the VPC to provide internet connectivity.

4.Create a route table and add a route 0.0.0.0/0 through the Internet Gateway.

5.Associate the route table with the public subnet.

6.Launch an EC2 instance in the public subnet and enable a public IPv4 address.

7.Configure the security group to allow SSH (port 22) and HTTP (port 80) traffic.

8.Connect to the EC2 instance using SSH or EC2 Instance Connect.

9.Install and start the Apache HTTP web server on the EC2 instance.

10.Create a simple HTML webpage and place it in the Apache web server's document directory.

11.Access the webpage using the EC2 instance's public IPv4 address in a web browser.
```

---


12.Verify the output and capture screenshots of the VPC/subnet, running EC2 instance, and web server webpage.

## Output Screenshots (Attach 3)

### Screenshot 1: VPC and Subnet Details


<img width="855" height="433" alt="image" src="https://github.com/user-attachments/assets/de5e85d5-7512-4dd5-81b6-a781c5cfeb49" />


<img width="847" height="445" alt="image" src="https://github.com/user-attachments/assets/2e734771-b167-4ccb-a8c6-9cd7920eb710" />



<img width="850" height="437" alt="image" src="https://github.com/user-attachments/assets/2ccd52a1-315e-4f66-b453-a81a372b4a3d" />

---

### Screenshot 2: EC2 Instance Running
<img width="847" height="437" alt="image" src="https://github.com/user-attachments/assets/12ea3d21-84e1-4eed-9381-83e5a2a528a6" />


<img width="851" height="440" alt="image" src="https://github.com/user-attachments/assets/b186d3ae-dae3-4f3c-886e-2501a0148bc1" />

<img width="842" height="443" alt="image" src="https://github.com/user-attachments/assets/0e0c5a5c-3b91-49a0-9c1a-f050668c199c" />

<img width="850" height="441" alt="image" src="https://github.com/user-attachments/assets/9149b887-fffa-4f0c-8e4e-7874cc966cf6" />





---

### Screenshot 3: Web Server Output in Browser
<img width="746" height="313" alt="image" src="https://github.com/user-attachments/assets/6ec6d391-e01e-4a6d-a16e-58e353bb1e59" />

<img width="746" height="242" alt="image" src="https://github.com/user-attachments/assets/86fa67d5-1853-40fb-a0d2-297c9c90e475" />


---

## Result 

This experiment successfully demonstrated the creation of a custom VPC and deployment of a public-facing web server in AWS. By configuring networking components such as subnets, route tables, and security groups, and by launching an EC2 instance with a web server, the basic architecture of a cloud-hosted application was understood.

# Lab 6 – Scale and Load Balance Your Architecture


## Title

Scale and Load Balance Your Architecture




##Author 



 name : Sanjutha D   
 Reg no : 212225240136

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. First, I logged in to the **AWS Management Console** using my AWS account.

2. I opened the **EC2 Dashboard** and checked the running instances.

3. I created or selected the required **EC2 instances** for the application.

4. I created an **Application Load Balancer (ALB)** to distribute incoming traffic.

5. I configured the **Target Group** and added the EC2 instances as targets.

6. I configured the **Listeners and Security Groups** for the Load Balancer.

7. I checked the health status of the registered EC2 instances.

8. I created an **Auto Scaling Group** to automatically manage the number of EC2 instances.

9. I configured the **minimum, desired, and maximum capacity** for the Auto Scaling Group.

10. I configured scaling policies so that instances can be added or removed based on application demand.

11. I tested the application through the **Load Balancer DNS name** to verify that traffic was distributed across the instances.

12. Finally, I verified that the architecture could **scale automatically and balance traffic** between healthy EC2 instances.




---

## Output Screenshots 

<img width="856" height="442" alt="image" src="https://github.com/user-attachments/assets/1d6184d5-0dc5-4432-8ddc-db97c54296f8" />


<img width="841" height="438" alt="image" src="https://github.com/user-attachments/assets/f7c54b34-3568-4f58-a3b3-e31b1383d429" />


## Cretated Lab config

<img width="850" height="436" alt="image" src="https://github.com/user-attachments/assets/f6da55c6-9387-4cd7-9769-94f35f7a3429" />

<img width="846" height="423" alt="image" src="https://github.com/user-attachments/assets/03b2aa1e-6f57-4d2c-a0f9-36f30b98376e" />


## Dynamic Scaling Policy Created


<img width="847" height="432" alt="image" src="https://github.com/user-attachments/assets/ae61104c-0042-429e-9b0f-8c10da02f731" />



<img width="722" height="297" alt="image" src="https://github.com/user-attachments/assets/99c6f84c-fdd2-4b13-92b1-8cc6a525c5f8" />




<img width="542" height="252" alt="image" src="https://github.com/user-attachments/assets/2719d837-8bfc-487a-90d3-3e5d3b828d4a" />













---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.

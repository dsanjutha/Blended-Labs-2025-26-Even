# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: Sanjutha D
* **Register Number**: 212225240136

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
1. First, I logged in to the **AWS Management Console** using my AWS account.

2. I searched for **Amazon RDS (Relational Database Service)** in the AWS Services section and opened the RDS Dashboard.

3. I clicked on **Create Database** to start creating a new database server.

4. I selected **Standard Create** to configure the database settings manually.

5. I selected **MySQL** as the database engine.

6. I selected a suitable **database instance size** based on the requirements.

7. I entered a **DB instance identifier**, username, and password for the database.

8. I configured the **storage settings** such as storage type and allocated storage.

9. I configured the **connectivity settings**, including the VPC and security group.

10. I reviewed all the database settings and clicked **Create Database**.

11. AWS started creating the database server, and I waited until the database status changed to **Available**.

12. I checked the database details and obtained the **endpoint** used to connect to the database.

13. Finally, I verified that the database server was successfully created and ready to use.




---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server
 <img width="840" height="437" alt="image" src="https://github.com/user-attachments/assets/9c61bd41-90f6-4be4-aa5a-2e374de0d0a0" />


---

### Screenshot 2: Database Service Running

<img width="837" height="436" alt="image" src="https://github.com/user-attachments/assets/c997eb6d-aa07-4f9b-b1fe-dfd180246a50" />


---

### Screenshot 3: Sample Database and Table
<img width="668" height="275" alt="Screenshot 2026-08-15 221036" src="https://github.com/user-attachments/assets/539649c3-61d1-4b4a-ab9f-21f0f004afc8" />

---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst

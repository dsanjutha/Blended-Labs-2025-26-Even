# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: Sanjutha D
* **Register Number**: 212225240136


---

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)

---

## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

---

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

---

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

---

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

---

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

---

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.

---

### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.

---

## Working with Amazon Elastic Block Store (EBS) – Workflow

1. First, I logged in to the AWS Management Console using my AWS account.

2. I opened the EC2 Dashboard and selected Elastic Block Store (EBS).

3. I explored the Volumes section to understand EBS storage management.

4. I clicked on Create Volume to create a new EBS volume.

5. I selected the required volume type, such as General Purpose SSD (gp3).

6. I specified the required storage size and selected the appropriate Availability Zone.

7. I created the EBS volume and checked its status.

8. I selected the created volume and chose Attach Volume.

9. I selected an existing EC2 instance in the same Availability Zone.

10. I verified that the EBS volume was successfully attached to the EC2 instance.

11. I explored options such as Detach Volume, Delete Volume, and Create Snapshot.

12. Finally, I created a snapshot to understand how EBS data can be backed up.




---

## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="955" height="495" alt="image" src="https://github.com/user-attachments/assets/497da88b-46e1-478a-a04c-3e9e6b29f51f" />

---

### Screenshot 2: EBS Volume Attached to EC2

<img width="847" height="433" alt="image" src="https://github.com/user-attachments/assets/a25c4257-91f3-43fc-8b27-8f8c93192631" />
<img width="856" height="432" alt="image" src="https://github.com/user-attachments/assets/27e66242-4de0-4f39-8797-48912cc9f5d5" />

<img width="777" height="362" alt="image" src="https://github.com/user-attachments/assets/a631bc39-5ea8-4936-b850-ed2a0ca99673" />



---

### Screenshot 3: Mounted Volume with Data

<img width="846" height="433" alt="image" src="https://github.com/user-attachments/assets/40f28ac9-1893-4d7e-9aab-5d68b524802f" />


<img width="847" height="442" alt="image" src="https://github.com/user-attachments/assets/dd6e8c32-1aa5-4646-9877-43e28e4c5bd2" />



---

## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.

# Day 3 of My 30-Day Deep Dive into AWS Cloud

On Day 3 of my AWS journey, I focused on **Amazon EC2 (Elastic Compute Cloud)**, which is a fundamental service in AWS that provides resizable compute capacity in the cloud. Here’s a brief overview of EC2 and its key components:

## Amazon EC2 Overview
Amazon EC2 allows users to launch virtual servers, known as instances, which can be scaled up or down based on demand. This flexibility helps in building and deploying applications efficiently and cost-effectively.

## Key Components of EC2

### 1. Instances
Instances are virtual servers that run applications on the AWS infrastructure. They come in various types, optimized for different use cases, such as compute-optimized, memory-optimized, and storage-optimized instances.

### 2. Amazon Machine Images (AMIs)
AMIs are pre-configured templates that contain the information required to launch an instance, including the operating system, application server, and applications. Users can choose from a variety of AMIs or create their own customized AMIs.

### 3. Instance Types
Instance types determine the hardware of the host computer used for the instance. Each instance type offers different compute, memory, and storage capabilities. Common instance families include General Purpose (e.g., t2.micro), Compute Optimized (e.g., c5.large), and Memory Optimized (e.g., r5.large).

### 4. Key Pairs
Key pairs are used for secure login to EC2 instances. AWS stores the public key, while the user holds the private key. This method ensures that only authorized users can access the instances.

### 5. Elastic Block Store (EBS)
EBS provides block storage volumes for use with EC2 instances. These volumes persist independently from the life of the instance, allowing data to be retained even after the instance is terminated.

### 6. Security Groups
Security groups act as virtual firewalls for EC2 instances, controlling inbound and outbound traffic. They allow users to specify which IP ranges and protocols can access the instances.

### 7. Elastic IP Addresses
Elastic IP addresses are static IP addresses designed for dynamic cloud computing. They allow for the replacement of failed instances by remapping the IP address to another instance.

### 8. Auto Scaling
Auto Scaling automatically adjusts the number of EC2 instances in response to changing demand, ensuring consistent performance at the lowest possible cost.

### 9. Elastic Load Balancing (ELB)
ELB distributes incoming traffic across multiple EC2 instances, enhancing the fault tolerance and availability of applications.

Understanding these components is crucial for efficiently managing and utilizing EC2 resources. I’m looking forward to diving deeper into AWS services and sharing more insights. Stay tuned!

#AWS #CloudComputing #30DaysOfAWS #Day3 #EC2 #ElasticComputeCloud #TechLearning #CloudJourney

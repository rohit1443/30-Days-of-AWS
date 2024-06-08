# Day 7: Deep Dive into AWS Cloud - Different Port Numbers for Different Applications on EC2

## Understanding Ports and Their Importance
In networking, a port is a communication endpoint used by applications or services to exchange data. Each application running on an EC2 instance can be assigned a unique port number, enabling multiple applications to operate simultaneously without conflicts.

## Commonly Used Port Numbers
Here are some standard ports for different applications:

- **HTTP (Web Traffic):** Port 80
- **HTTPS (Secure Web Traffic):** Port 443
- **SSH (Secure Shell):** Port 22
- **FTP (File Transfer Protocol):** Port 21
- **SMTP (Email):** Port 25
- **MySQL (Database):** Port 3306
- **PostgreSQL (Database):** Port 5432

## Configuring Security Groups
Security groups in AWS act as virtual firewalls for your EC2 instances, controlling inbound and outbound traffic. To run applications on specific ports, you need to allow traffic on these ports in your security group settings.

### Steps to Configure Security Groups:
1. **Open the EC2 Dashboard:**
   - Navigate to the "Instances" section.
   - Select your instance and note the associated security group.

2. **Modify Security Group Rules:**
   - Go to the "Security Groups" section.
   - Select the security group and click on the "Inbound rules" tab.
   - Click "Edit inbound rules" and add rules for the required ports. For example:
     - HTTP: Port 80, Protocol: TCP, Source: 0.0.0.0/0
     - SSH: Port 22, Protocol: TCP, Source: Your IP

## Practical Application
### Running Multiple Applications on an EC2 Instance:
- **Web Server (HTTP/HTTPS):** Configure your web server to listen on ports 80 and 443.
- **Database Server (MySQL):** Set up your database server to listen on port 3306.
- **SSH Access:** Ensure port 22 is open for secure remote access.

### Example Scenario:
You have an EC2 instance running:
- An Apache web server on port 80 for HTTP traffic.
- A secure application on port 443 for HTTPS traffic.
- A MySQL database on port 3306.

### Sample Security Group Configuration:
| Type  | Protocol | Port Range | Source      |
|-------|----------|------------|-------------|
| HTTP  | TCP      | 80         | 0.0.0.0/0   |
| HTTPS | TCP      | 443        | 0.0.0.0/0   |
| SSH   | TCP      | 22         | Your IP     |
| MySQL | TCP      | 3306       | 0.0.0.0/0   |

## Summary
Managing different port numbers for applications on EC2 is crucial for network traffic management and security. By configuring security groups correctly, you can ensure that your applications run smoothly and securely.

For more details, visit the [AWS EC2 Security Groups Documentation](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html).

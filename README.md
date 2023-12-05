# Aws-Capstone-Project-Secure_VPC
## **Introduction**

This project was created to showcase how VPC security works also how we can use VPC for security and load balancer and autoscalaing for high availability in real time scenarios. Also, we can integrate multiple services with VPC such as EC2, Load balancer, and Autoscaling, and create a secure and scalable application.




 ## **Architecture of the project**

   
   ![arc](https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/255737f5-c911-4dd5-a0b8-663282f531b9)

## **Steps to execute the project**

  
* Design and configure a VPC: Create a VPC with custom IP ranges. Set up public and private subnets. Configure route 
 tables and associate subnets.

<img width="907" alt="VPC2" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/66a1476e-5120-4859-b431-83810db2a3fb">

    
* Implement network security: Set up network access control lists (ACLs) to control inbound and outbound traffic. 
Configure security groups for EC2 instances to allow specific ports and protocols.
    
* Provision of EC2 instances: Launch EC2 instances in both the public and private subnets. Configure security groups for 
    the instances to allow necessary traffic.
  
  <img width="956" alt="ec2" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/cdcc2c72-f367-4caf-8323-870065fe77e9">

* Setting up and running Ec2 : Setting up and running EC2 and created one host in public subnet access private ec2 using host and run and host sample server
  on port 8000
  <img width="959" alt="private1" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/12ee0525-b33f-48d4-baf9-c67d4eec0306">


    
* Networking and routing: Set up an internet gateway to allow internet access for instances in the public subnet.Configure 
    NAT gateway or NAT instance to enable outbound internet access for instances in the private subnet. Create appropriate 
    route tables and associate them with the subnets.

* Load balancer and autoscaling: Create a load balancer and attach it to an autoscaling group to make the application highly available
  in the same VPC that is created for the project.
  <img width="957" alt="autoscaling" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/1af83aa8-671c-4be7-8d5d-847679cc66ef">

  <img width="959" alt="load balancer" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/d2713c06-4eeb-4f50-9f2a-6896d278796f">




* SSH key pair and access control: Generate an SSH key pair and securely store the private key. Configure the instances to 
    allow SSH access only with the generated key pair. Also, give port 8000 access in the security group so that the application will be
  able to load in it.
  <img width="958" alt="port enabled1" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/48cae47c-2820-4c9b-89b3-0f5fb5c9f02d">


    
* Test and validate the setup: Test and run the link given by the load balancer and test the output on the browser
  also we can check the health of servers and if the server load increases the autoscaling group will increase the number of servers.
  
  <img width="960" alt="desired output" src="https://github.com/Malhar-Raste/Aws-Capstone-Project-Secure_VPC/assets/148332545/9c3e94e2-7013-41ad-a29c-c8c40eb8f354">


## Advantages of the setup 
* Getting high availability for the application hosting because of the load balancer and autoscaling group.
* Getting high security because of the VPC configuration.
  


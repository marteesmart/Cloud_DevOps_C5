# Welcome to the Virtual Private Cloud Lab

This task will get you acquainted on how to deploy VPC 


# Task 1: Deploy VPC using Management console
1. Launch the AWS Management Console
2. Launch a VPC with one public and one private subnets.
3. Create two route table and associate  each one to each subnets
4. Attach an internet gateway to the VPC and a NAT gateway to the private subnet.
5. Lauch a Linux instance into the public subnet of this VPC.
6. Ensure adequate security rules are followed.
7. Test the network connectivity
8. Perform clean up actions


# Submission
Attach a screenshot of every completed stages in a folder in your repository.




## For guide, you can check the links below:

https://docs.aws.amazon.com/cli/latest/reference/ec2/

https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-vpcs.html


https://docs.aws.amazon.com/vpc/latest/userguide/vpc-example-dev-test.html



## Solution

1. Launch the AWS Management Console

2. Launch a VPC with one public and one private subnets.  
![Launch VPC](screenshots/5.1.1.PNG)  


![private subnet](screenshots/5.1.2.1.PNG)  


![public subnet](screenshots/5.1.2.2.PNG)    


3. Create two route table and associate  each one to each subnets  
![Route table 1](screenshots/5.1.3.1.PNG)  
![Route table 2](screenshots/5.1.3.2.PNG)  



4. Attach an internet gateway to the VPC and a NAT gateway to the private subnet.
![IGW](screenshots/5.1.4.1.PNG)  
![NAT](screenshots/5.1.4.2.PNG)  


5. Lauch a Linux instance into the public subnet of this VPC.
![launch ec2](screenshots/5.1.5.PNG)
  
6. Ensure adequate security rules are followed.  
![network](screenshots/5.1.6.PNG)  
  

7. Test the network connectivity  
![ssh](screenshots/5.1.7.PNG)  
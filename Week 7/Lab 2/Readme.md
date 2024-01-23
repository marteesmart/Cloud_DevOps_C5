# Working with EFS

## Aim and Objective
Familiarity with installing a network file system to an EC2 instance

## Tasks

1. Create your Amazon EC2 resources and launch two EC2 instances.
2. Create your Amazon EFS file system with One Zone storage.
3. Connect to each of your Amazon EC2 instances, and mount the Amazon EFS file system using the same mount target for each instance
4. Confirm that the EFS was successfully installed.
5. Perform clean-up operations



## Guide:
To aid in achieving tasks 1-5, kindly follow the steps describe in the link along with lessons from class videos
https://docs.aws.amazon.com/efs/latest/ug/gs-step-two-create-efs-resources.html


## Submission

Attach a screenshot of completion of each task mentioned above. 


## Solution
1. Create VPC
![Create VPC](<screenshots/1. CREATE VPC.png>)  

2. Create security group for EC2 instances
![sg](<screenshots/2. CREATE EFS CLIENT SG.png>)    

3. Add NFS inbound rule to EFS security group
![NFS](<screenshots/3. NFS INBOUND RULE.png>)   

4. Create / Add EFS to EFS security group
![EFS1](<screenshots/4. ADD EFS TO SG.png>) 
![EFS2](<screenshots/5. REVIEW EFS SELECTION.png>)  
![EFS3](<screenshots/6. CREATE EFS.png>)    

5. Create EC2 instances 
![EC2_1](<screenshots/7. CREATE EC2 INSTANCES_1.png>)   
![EC2_2](<screenshots/8. CREATE EC2 INSTANCE_2.png>)    
    
6. Mount and confirm EFS on EC2 instances
![Mount 1](<screenshots/9. MOUNT ON EC2_1.png>)     
![Mount 2](<screenshots/10. MOUNT ON EC2_2.png>)    
---
title : "Setting up AWS EC2"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---
Step 1: Access the AWS Management Console
-----------------------------------------
[Access the AWS Management Console](https://console.aws.amazon.com/)

![Management Console](../../images/2.prerequisite/console.png)

Step 2: Create a EC2 Instance
-----------------------------
1. In the AWS Management Console, click on the Services menu and select EC2.
![Select EC2](../../images/2.prerequisite/image14.png)

Step 3: Launch Instance
-----------------------
Click on the Launch Instance button. In this step, you can set the configuration based on your requirement and I choose ubuntu as the operating system.

![Launch Instance](../../images/2.prerequisite/image15.png)

Step 4: Set security group
--------------------------
After launching the instance, you need to set the security group. Click on the Security Group and add the inbound rule for the instance.

![Security Group](../../images/2.prerequisite/image16.png)

Select the security group and click on the Inbound tab. Click on the Edit button and add the rule for the instance.
Create port 8080 for HTTP with source 0.0.0.0.

After adding the rule, you can access the instance from your local machine with the public IP address.

---
title : "Setting up AWS S3"
date : "`r Sys.Date()`"
weight : 2
chapter : false
pre : " <b> 2.2 </b> "
---
Step 1: Access the AWS Management Console
-----------------------------------------
[Access the AWS Management Console](https://console.aws.amazon.com/)

![Management Console](/images/2.prerequisite/console.png)

Step 2: Create a S3 Bucket
![Create S3 Bucket](/images/2.prerequisite/image11.png)

Step 3: Setting configuration for the S3 Bucket
-------------------------------------------------
In this project, I choose the default setting for the S3 bucket. You can choose any setting as per your requirement. But you should notice this setting to access the bucket from your local machine.

![Setting Configuration](/images/2.prerequisite/image12.png)

Unselect the Block all public access and acknowledge that the bucket will be public.

After creating the bucket, we should create IAM user and assign the policy to access the bucket.

Step 4: Create IAM
------------------
1. In the AWS Management Console, click on the Services menu and select IAM.
2. Click on the Users menu and click on the Add user button.
3. Enter the user name and select the Programmatic access.
4. Click on the Next: Permissions button.
5. Click on the Attach existing policies directly button.
6. Search for the AmazonS3FullAccess policy and select the checkbox.

After creating the user, you will get the Access key and Secret key. You should note this key because you will use this key to access the S3 bucket from your local machine.

![Access Key](/images/2.prerequisite/image13.png)

This is the end of the AWS S3 setup. Now, you can access the S3 bucket from your local machine.
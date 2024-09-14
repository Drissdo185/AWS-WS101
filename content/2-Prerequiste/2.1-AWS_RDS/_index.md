---
title : "Preparing AWS RDS"
date : "`r Sys.Date()`"
weight : 1
chapter : false
pre : " <b> 2.1 </b> "
---

Step 1: Access the AWS Management Console
-----------------------------------------
[Access the AWS Management Console](https://console.aws.amazon.com/)

![Management Console](../images/2.prerequisite/console.png)

Step 2: Create a DB Instance
----------------------------
1. In the AWS Management Console, click on the Services menu and select RDS.
![Select RDS](/images/2.prerequisite/image2.png)

2. Click on the Create database button.
![Create Database](/images/2.prerequisite/image3.png)

Step 3: Setting configuration for the DB instance
-------------------------------------------------
In this project, I choose PostgreSQL as the database engine. You can choose any database engine as per your requirement.
![Select Engine](/images/2.prerequisite/image4.png)

Every setting depends on your requirement. However, you should note the following this point:

![Setting Configuration](/images/2.prerequisite/image5.png)

You should follow this setting, because when you choose `Yes` for the Public accessibility, you can access the database from your local machine.

#Step 4: Security Setting

After create successful DB instance, access the Security Group and add the inbound rule for the database.
![Security Group](/images/2.prerequisite/image6.png)
Select the security group and click on the Inbound tab. Click on the Edit button and add the rule for the database.
![Inbound Rule](/images/2.prerequisite/image7.png)
Add the rule for the database and click on the Save button.
![Add Rule](/images/2.prerequisite/image8.png)



After adding the rule, you can access the database from your local machine with endpoint and port number.
![Endpoint](/images/2.prerequisite/image9.png)

![Connection](/images/2.prerequisite/image10.png)

This is the end of the AWS RDS setup. Now, you can access the database from your local machine.





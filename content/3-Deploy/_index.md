---
title : "Simple Web Application Deployment"
date : "`r Sys.Date()`"
weight : 3
chapter : false
pre : " <b> 3. </b> "
---

In this section, we will deploy a simple web application on AWS. We will use the following services:

Step 1: Connect to the EC2 instance using SSH
------------------------------------
Open the terminal and connect to the EC2 instance using the following command:
```bash
ssh -i "your-key.pem" ubuntu@your-public-ip
```
Step 2: Install Docker
----------------------
Run the following command to install Docker on the EC2 instance:
```bash
sudo apt-get update
sudo apt-get install docker.io
```
Step 3: Pull the Docker image
-----------------------------
At the step, I have already pushed the Docker image to the Docker Hub. You can pull the image using the following command:
```bash
docker pull datdt185/appjava
```
Link to the Docker image: [datdt185/appjava](https://hub.docker.com/r/datdt185/appjava)

Step 4: Run the Docker container
--------------------------------
After pulling the Docker image, you can run the container using the following command:
```bash
docker run -d -p 8080:8080 datdt185/appjava
```
Currently, the application is running on the EC2 instance. You can access the application using the public IP address and port 8080.
You can use features of the application such as:
- Import data from a file excel to PostgreSQL: http://your-public-ip:8080/products/upload-customers-data?
![Import Data](/images/3.deploy/image.png)
Result:
![Result](/images/3.deploy/image1.png)
- Upload Image to S3: http://your-public-ip:8080/products/upload-image
![Upload Image](/images/3.deploy/image2.png)
Result:
![Result](/images/3.deploy/image3.png)

## Conclusion

In this section, we have deployed a simple web application on AWS. We have used Docker to run the application on the EC2 instance. You can access the application using the public IP address and port 8080. The application provides features such as importing data from a file excel to PostgreSQL and uploading an image to S3. In the next workshop, we will optimize source code and update more about security such as VPN, public and private subnet, and build CI/CD pipeline.





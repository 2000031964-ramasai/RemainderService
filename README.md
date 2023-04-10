# To-Do / Remainder Service


## Project Description

Basically this project is about notifying the users about their To-do/Remainders when they have. They have to just include their what ever the remainder they have. They will get the remainder on that day. This application was developed using Amazon Web Services. I used different services for this application to be complete.

### Architecture
The architecture of the application is as follows -
![Alt text](https://2000031964s3-app.s3.us-east-2.amazonaws.com/arch3.png "Architecture")

### Services Used

**AWS Amplify** : AWS Amplify is a development platform that allows developers to easily create and deploy scalable, secure, and feature-rich web and mobile  applications.

**AWS Lambda** : AWS Lambda is a serverless computing service provided by AWS that lets you run your code without provisioning or managing servers.

**AWS API Gateway** : API Gateway is a fully managed service provided by AWS that enables developers to create, deploy, and manage secure APIs at any scale, making it easy to connect applications to data and services hosted in AWS or outside of AWS.

**AWS DynamoDB** : Amazon DynamoDB is a fully managed NoSQL database service provided by AWS that provides fast and predictable performance with seamless scalability, making it an ideal choice for applications that require low-latency data access at any scale.

**AWS SES** : AWS SES (Simple Email Service) is a cloud-based email sending service provided by AWS that allows developers to send transactional email, marketing messages, and other types of high-quality content to their customers in a reliable and cost-effective manner.

**AWS Cloud Watch** : Amazon CloudWatch is a monitoring and observability service provided by AWS that provides real-time monitoring and logging for AWS resources and applications, enabling you to collect, monitor, and analyze metrics, logs, and events to ensure that your infrastructure and applications are running smoothly.

### Functioning
- First of all User tries to access the page which is deployed in AWS Amplify.
- That request is sent to AWS Lambda through API Gateway method which is defined in the HTML Code.
- The details will be stored into dynamodb with the help of Lambda.
- Using the cloud watch which is triggering daily once will read the table and if the column date and current date is matched then mail will be sent to that user email using AWS SES.


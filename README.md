# Individual Project 4: Serverless Data Engineering Pipeline

## Objectvices of Project
This project reproduces the architecture of the example serverless data engineering project or perform something similar using only serverless technologies.
AWS lambda was used to have serverless application architecture.


## Progress



### week 1

- Created SAM application

AWS SAM (Serverless Application Model) is a framework for building serverless applications on AWS (Amazon Web Services). It is an open-source framework that extends AWS CloudFormation to provide a simplified way of defining the Amazon API Gateway APIs, AWS Lambda functions, and Amazon DynamoDB tables needed by your serverless application.

1. `sam init`
a command that initializes a new serverless application project by creating a sample template and directory structure.


2. `sam build --use-container`
a command to build a deployment package for a serverless application using a Docker container.
When you run this command, SAM will package and build your code, including all the dependencies and libraries required by your application, inside a Docker container that matches the AWS Lambda environment. This ensures that the deployment package is consistent and that any native dependencies are compiled correctly.

<img width="1113" alt="image" src="https://user-images.githubusercontent.com/104106034/228634746-93721e6c-5da9-4b5c-9bd2-a4cc2751e147.png">


3. `sam validate`
a command that checks the syntax and semantics of the AWS SAM template and verifies that it is valid according to the AWS SAM specification. If the template is not valid, the command will return an error message indicating the issues with the template.

<img width="1126" alt="image" src="https://user-images.githubusercontent.com/104106034/228634806-1e27e311-9f1f-4cc4-8951-1373211e74ca.png">


4. `sam local invoke`
 a command to invoke a Lambda function locally on your development machine. It allows you to test your Lambda function code locally and get immediate feedback on its behavior.

<img width="1114" alt="image" src="https://user-images.githubusercontent.com/104106034/228634865-66ce3579-1734-4c59-8b17-babcf3eea6b1.png">

<img width="1124" alt="image" src="https://user-images.githubusercontent.com/104106034/228634949-b27d1f0a-3d2e-4a01-bae6-cf549fe2efd5.png">


5. `sam local start-api`
a command that allows you to locally test and debug your serverless APIs using a local API Gateway.
When you run sam local start-api, it starts a local API Gateway and listens to HTTP requests on a specified port. It reads the template.yaml or template.yml file in the current directory to determine the API's configuration and which Lambda functions to invoke for each API endpoint.

<img width="1116" alt="image" src="https://user-images.githubusercontent.com/104106034/228635139-7e81c7df-31aa-46a0-a87e-efffbf51e922.png">


6. `curl <address-you-get-from-previous-command>`

<img width="1116" alt="image" src="https://user-images.githubusercontent.com/104106034/228635196-0a741446-0ace-4bbd-8fc2-4c92e5a317e4.png">

- Lambda Function Created
<img width="1391" alt="image" src="https://user-images.githubusercontent.com/104106034/228635411-41440eeb-137e-44a5-9225-8a87c7c3eb7e.png">

- API Getaway can be monitored through logs in CloudWatch
<img width="1412" alt="image" src="https://user-images.githubusercontent.com/104106034/228635291-1d975d9e-9162-4b97-a14c-539d5cb0755c.png">


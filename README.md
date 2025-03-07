AWS Add-to-Cart Project

Project Overview : 

This project is an Add-to-Cart feature for an e-commerce platform, built using AWS services. It allows users to add products to their cart, store cart details in DynamoDB, and retrieve them later.

> Features :

Users can add products to their cart.

Cart data is stored in AWS DynamoDB.

API Gateway routes requests to AWS Lambda functions.

AWS S3 hosts the frontend.

CloudFront is used for content delivery.

IAM roles ensure secure access to AWS resources.

> Technologies Used : 

AWS Lambda (Backend logic)

API Gateway (Handling API requests)

DynamoDB (Storing cart details)

S3 (Frontend hosting)

CloudFront (Content delivery)

IAM (Security and access management)

> Architecture :

1. User interacts with the frontend hosted on S3.

2. API requests are sent via API Gateway.

3. Lambda functions process add-to-cart requests.

4. Product details are stored in DynamoDB.

5.Responses are sent back to the frontend.

6. CloudFront optimizes content delivery.


> Deploy Backend (Lambda, API Gateway, DynamoDB) :

Create a DynamoDB table named CartTable with userId as the partition key.

Deploy Lambda functions for handling add-to-cart actions.

Set up API Gateway to invoke Lambda functions.

Grant necessary IAM roles.


Deploy Frontend (S3 & CloudFront) : 

Upload frontend files to an S3 bucket.

Enable static website hosting.

Use CloudFront for faster content delivery.

> Future Enhancements :

Implement user authentication using Cognito.

Add real-time cart updates with WebSockets.

Integrate a payment gateway.


Author

NithuContact: [nithinofficial2318@gmail.com]

License

This project is licensed under the MIT License.

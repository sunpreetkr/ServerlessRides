# AWS Project - A Full End-to-End Web Application with 7 Services

🌟 Project Overview — Wild Rydes (AWS Serverless Ride Sharing App)

Serverless Rides/ Wild Rydes is a fully serverless ride-sharing web application built on AWS, where users can request a mythical unicorn ride based on their location. This project is based on the AWS Wild Rydes sample architecture and demonstrates how multiple cloud services work together to build a scalable, production-style application.

The application follows a modern event-driven, serverless architecture using AWS managed services to eliminate the need for server management while enabling automatic scaling, high availability, and secure access control.

🏗️ Architecture Overview

The system integrates multiple AWS services to deliver a complete full-stack solution:

Frontend Hosting: AWS Amplify hosts and deploys the web application with CI/CD integration from GitHub.
Authentication: Amazon Cognito manages user sign-up, login, and JWT-based authentication.
API Layer: Amazon API Gateway exposes secure REST endpoints and integrates with Cognito authorizers.
Backend Logic: AWS Lambda processes ride requests, assigns a random unicorn, and handles business logic.
Database: Amazon DynamoDB stores ride details such as ride ID, user information, and timestamps.
Security: IAM roles control secure access between Lambda and DynamoDB.

🔄 How It Works
Users access the web application hosted on AWS Amplify.
They register or log in using Amazon Cognito authentication.
After authentication, users request a ride by selecting a pickup location.
API Gateway receives the request and validates the user via Cognito.
AWS Lambda processes the request:
Generates a unique Ride ID
Selects a random unicorn from a predefined fleet
Stores ride details in DynamoDB
The system returns ride confirmation details including estimated arrival time and assigned unicorn.

⚙️ Key AWS Services Used
AWS Amplify (Frontend Hosting & CI/CD)
Amazon Cognito (Authentication & Authorization)
Amazon API Gateway (REST API Management)
AWS Lambda (Serverless Backend Logic)
Amazon DynamoDB (NoSQL Data Storage)
AWS IAM (Access Control & Permissions)
GitHub (Source Code Management & Deployment Trigger)

🎯 Key Features
Fully serverless architecture (no infrastructure management required)
Secure authentication using JWT tokens (Cognito integration)
RESTful API built with API Gateway and Lambda
Event-driven backend logic
Scalable NoSQL database with DynamoDB
Continuous deployment via GitHub and AWS Amplify
💡 Purpose of the Project

This project is designed as a hands-on AWS learning exercise to demonstrate:

Serverless application development
Cloud-native architecture design
Authentication and authorization flows
API integration with backend services
Infrastructure automation and CI/CD pipelines

🚀 Outcome

By completing this project, we get a fully functional cloud-hosted web application that showcases real-world AWS service integration and modern serverless design principles.

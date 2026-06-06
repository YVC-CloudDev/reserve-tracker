# 🪖 Reserve Tracker

A serverless AWS-based web application for managing and tracking military reserve duty activities.

The system allows users to record reserve activities, monitor total reserve days, view activity history, and securely store data in the AWS Cloud.

---

# 🚀 Features

- User login using email address
- Add reserve duty activities
- View activity history
- Delete activities
- Track total reserve days
- Count total activities
- Count unique military units
- Secure cloud-based data storage
- Responsive and modern user interface
- HTTPS secured website

---

# 🏗️ Architecture

![Architecture](architecture.png)

---

# ☁️ AWS Services Used

| Service | Purpose |
|----------|----------|
| Amazon Route 53 | DNS Management |
| AWS Certificate Manager (ACM) | SSL/TLS Certificate |
| Amazon CloudFront | Content Delivery Network (CDN) |
| Amazon S3 | Static Website Hosting |
| Amazon API Gateway | REST API Management |
| AWS Lambda | Serverless Backend Logic |
| Amazon DynamoDB | NoSQL Database |

---

# 🔄 Application Flow

1. The user accesses the application through a web browser.
2. Route 53 resolves the custom domain name.
3. CloudFront delivers the website securely using HTTPS.
4. Static files (HTML, CSS, JavaScript) are loaded from Amazon S3.
5. API requests are sent to Amazon API Gateway.
6. API Gateway invokes AWS Lambda functions.
7. Lambda processes the request and interacts with DynamoDB.
8. DynamoDB stores or retrieves activity data.
9. The response is returned to the user interface.

---

# 📐 Architecture Overview

```text
User
 │
 ▼
Route 53
 │
 ▼
CloudFront
 │
 ├── ACM Certificate
 │
 ├── S3 Static Website
 │
 └── API Gateway
          │
          ▼
        Lambda
          │
          ▼
       DynamoDB
```

---

# 🛠️ Technologies

## Frontend

- HTML5
- CSS3
- JavaScript

## Backend

- AWS Lambda (Node.js)

## Cloud Services

- Amazon S3
- Amazon CloudFront
- Amazon Route 53
- AWS Certificate Manager (ACM)
- Amazon API Gateway
- Amazon DynamoDB

---

# 📂 Project Structure

```text
ReserveTracker
│
├── index.html
├── style.css
├── script.js
├── logo.png
├── architecture.png
└── README.md
```

---

# 🗄️ Database Schema

### DynamoDB Table: ReserveTracker

| Attribute | Type |
|------------|------|
| soldierId | String |
| email | String |
| date | String |
| unit | String |
| activity | String |
| days | Number |

---

# 🔐 Security

- HTTPS enabled using AWS Certificate Manager (ACM)
- Secure CloudFront distribution
- Serverless backend architecture
- Data stored securely in Amazon DynamoDB
- API access managed through Amazon API Gateway

---

# 📸 Screenshots

## Login Screen

_Add screenshot here_

## Dashboard

_Add screenshot here_

## DynamoDB Table

_Add screenshot here_

---

# 🎯 Project Objectives

The purpose of this project is to demonstrate the implementation of a complete serverless cloud application using AWS services.

The project integrates:

- Static website hosting
- Global content delivery
- Custom domain configuration
- SSL certificate management
- REST API development
- Serverless computing
- Cloud database integration

---

# 👨‍💻 Author

**Or Moskovich**
** maoz nachom**

B.Sc. Information Systems

Yezreel Valley College

2026

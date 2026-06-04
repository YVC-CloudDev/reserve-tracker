# Reserve Tracker

A serverless web application for tracking reserve duty activities and reserve days.

## Project Overview

Reserve Tracker allows users to:

- Add reserve duty activities
- View all reserve activities
- Track total reserve days
- Delete activities
- Store data permanently in the cloud

The application is built entirely on AWS using a serverless architecture.

## Architecture

User Browser
     |
     v
CloudFront
     |
     v
S3 Static Website
     |
     v
API Gateway
     |
     v
AWS Lambda
     |
     v
DynamoDB

## AWS Services Used

### Amazon S3
Hosts the static website files.

### Amazon CloudFront
Provides global content delivery and HTTPS access.

### Amazon API Gateway
Handles REST API requests from the website.

### AWS Lambda
Processes business logic for:
- Creating activities
- Retrieving activities
- Deleting activities

### Amazon DynamoDB
Stores reserve duty records.

### Amazon CloudWatch
Used for monitoring and troubleshooting Lambda executions.

### AWS IAM
Manages permissions between AWS services.

## Features

### Add Activity
Users can add:

- Date
- Unit
- Activity Type
- Number of Reserve Days

### View Activities

Displays:

- Date
- Unit
- Activity
- Days

### Delete Activity

Users can remove activities from DynamoDB.

### Total Reserve Days

Automatically calculates and displays the total number of reserve days.

## Technologies

### Frontend

- HTML
- CSS
- JavaScript

### Backend

- AWS Lambda (Node.js)
- API Gateway

### Database

- DynamoDB

### DevOps

- GitHub
- GitHub Actions
- AWS

## API Endpoints

### Get All Activities

```http
GET /activities
```

### Create Activity

```http
POST /activity
```

Request Body:

```json
{
  "date": "2026-06-04",
  "unit": "123",
  "activity": "Training",
  "days": 5
}
```

### Delete Activity

```http
DELETE /activity/{id}
```

## Repository

GitHub Repository:

https://github.com/ormosko28/reserve-tracker

## Live Website

CloudFront URL:

http://d1vvvoc6hvh2me.cloudfront.net

## Author

Or Moskovich

B.Sc. Information Systems

Yezreel Valley College

## Course Project

Cloud Computing Project

Serverless Application on AWS

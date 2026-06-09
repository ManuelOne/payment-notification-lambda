# Payment Notification Processor (AWS Lambda)

## Overview

This project is a serverless payment notification processor built with Python and AWS Lambda.

The function receives payment details, validates the input, generates a transaction reference, and returns a structured JSON response. It also logs processing details to Amazon CloudWatch Logs for monitoring and troubleshooting.

## Features

* Serverless architecture using AWS Lambda
* Python 3.12 runtime
* Environment variable configuration
* Input validation
* Structured JSON responses
* Automatic CloudWatch logging
* No server management required
* Scales automatically based on demand

## Test Event

<img width="1880" height="683" alt="image" src="https://github.com/user-attachments/assets/5d42b826-a396-4255-9edc-66bd7ce334e3" />


```json
{
  "amount": 50000,
  "sender": "Emeka Eze",
  "recipient": "Adaeze Obi"
}
```

## Successful Execution

<img width="1895" height="1030" alt="image" src="https://github.com/user-attachments/assets/8675fb31-ecef-47c3-bd49-0957405214c7" />


```json
{
  "statusCode": 200,
  "body": {
    "status": "Payment Processed",
    "sender": "Emeka Eze",
    "recipient": "Adaeze Obi",
    "amount": "NGN 50,000.00"
  }
}
```

## CloudWatch Logs

<img width="1900" height="900" alt="image" src="https://github.com/user-attachments/assets/c88a689e-f75e-4349-8843-c84468b6a884" />



## Technologies Used

* AWS Lambda
* Python 3.12
* Amazon CloudWatch
* JSON

## Learning Outcomes

Through this project, I learned:

* How to create and deploy AWS Lambda functions
* Event-driven programming concepts
* Environment variable management
* Input validation techniques
* CloudWatch logging and monitoring
* Serverless application development


## 🔗 API Endpoint
https://1d4fg23413.execute-api.us-east-1.amazonaws.com/prod/payments

## 📘 API Documentation

Full OpenAPI specification is available in this repository:

 `openapi.yaml`

The file defines:
- Endpoints
- Request/response schemas
- Example payloads


## Author

Manuel

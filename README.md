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

## Sample Event

```json
{
  "amount": 50000,
  "sender": "Emeka Eze",
  "recipient": "Adaeze Obi"
}
```

## Sample Response

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

## Author

Manuel

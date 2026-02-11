# Kanbanix Notification Service

Kanbanix Notification Service manages event driven notifications across the platform.

It stores and delivers alerts related to task updates, mentions, board activity, and system events.

## Responsibilities

- Store user notifications
- Deliver real time alerts
- Mark notifications as read
- Handle event triggered messaging
- Provide notification retrieval APIs

## Architecture

Fully serverless architecture:

- AWS Lambda (business logic)
- Amazon DynamoDB (notification storage)
- Amazon API Gateway (REST or WebSocket API)
- Amazon SNS (optional event publishing)
- AWS IAM for secure access control

## Event Flow

1. Task or board event occurs
2. Event triggers Lambda
3. Notification stored in DynamoDB
4. Frontend retrieves notifications via API Gateway
5. Optional WebSocket push for real time updates

## Deployment

- Infrastructure as Code (AWS SAM or Serverless Framework)
- GitHub Actions CI/CD
- Fully eligible for AWS Always Free Tier usage

## Scalability

- Auto scaling Lambda functions
- No server management
- Event driven architecture
- Horizontally scalable design

## Portfolio Value

Demonstrates:

- Event driven system design
- Serverless microservice architecture
- DynamoDB data modeling
- Real time notification patterns

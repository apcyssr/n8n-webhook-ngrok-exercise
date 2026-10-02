# n8n Webhook + ngrok Exercise

## Objective

This exercise demonstrates how to connect an external HTTP request
to an n8n Webhook using ngrok.

## Workflow

Postman → ngrok → localhost:5678 → n8n Webhook → Respond to Webhook

## Configuration

- HTTP Method: POST
- Webhook Path: webhook-test
- Authentication: None
- Response: Using Respond to Webhook Node

## Test Data

{
  "name": "Apichaya",
  "message": "Hello n8n"
}

## Result

The request was successfully received by n8n through the ngrok tunnel.

## Evidence

### 1. n8n Workflow

![n8n Workflow](screenshots/01_n8n_workflow.png)

### 2. ngrok Forwarding

![ngrok](screenshots/02_ngrok.png)

### 3. Postman Response

![Postman Success](screenshots/03_postman_success.png)

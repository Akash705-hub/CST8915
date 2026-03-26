# CST8915 Lab 7: Introduction to Kubernetes Basics

- **Student Name**: Akash Patel
- **Student ID**: 041269598
- **Course**: CST8915 Full-stack Cloud-native Development
- **Semester**: Winter 2026

---
Note: I attached the screenshot for reference
---

## Analysis

### Configuration Problem
- RabbitMQ is deployed as a stateless Deployment with no persistent storage, so every time the pod restarts it loses all queues, messages, and internal state.
### Whether RabbitMQ is a stateless or stateful application
- RabbitMQ is a stateful application
### The implications of running RabbitMQ without persistent storage
- All messages are lost when the pod restarts
- User accounts and configuration reset to defaults
- All queues and exchanges are lost unless recreated by the application
### What happens when the RabbitMQ pod is deleted or restarted
- A new RabbitMQ pod is created with a fresh empty data directory
- All messages are lost even queues, users and other information.
- Any in‑flight messages are permanently lost.
### Potential solutions to this problem (research-based)
- We can add persistent storage.
- Also we can use managed message broker service like Azure Service Bus, Google Pub/Sub.
### Does using Azure Service Bus solve the issues identified with RabbitMQ Configuration in this Lab?
- Yes, Service Bus is fully managed, highly available, durable, automatically replicated and persistent by default.
- It removes all the problems that we are facing with RabbitMQ in Kubernetes.




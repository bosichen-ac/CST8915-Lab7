# CST8915 Lab 7: Introduction to Kubernetes Basics

**Student Name**: Bosi Chen\
**Student ID**: 041040774\
**Course**: CST8915 Full-stack Cloud-native Development\
**Semester**: Winter 2026

---

## Demo Video

🎥 [Watch Demo Video](https://youtu.be/QF5J1nAyQIQ)

---

## RabbitMQ Configuration Issues

The RabbitMQ is a stateless application in this case. 

When the RabbitMQ pod is deleted or restarted, a new pod will be created by the kubernetes, but the old container storage will be lost.

Potential solution: make the service stateful by using StatefulSets.

The Azure Service Bus will solve this issue. It is a fully managed messaging system, best suited for microservice-to-microservice communication where reliability and guaranteed delivery are critical.
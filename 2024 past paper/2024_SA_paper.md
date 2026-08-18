# 2024 Software Architecture Past Paper

University of Ruhuna  
Faculty of Engineering  
End-Semester 8 Examination in Engineering: October 2024

Module Number: EE8217  
Module Name: Software Architecture  
Time: Three Hours

Answer all questions. Q1 carries 25 marks, Q2 carries 15 marks and Q3 carries 10 marks.

## Q1

Answer the questions below based on the given scenario.

### User Requirement

The requirement is to build a cloud-based security and monitoring system. Users should have the ability to install various sensors, such as door sensors and motion detectors, in the locations they wish to monitor.

The system must effectively gather data from sensors and store it in a cloud database. Additionally, it must promptly notify users in the event of a security breach. Initially, the system will send email alerts for breaches, with future versions potentially supporting SMS and other notification methods. Users should have visibility into sensor status and historical alerts, accessible through both a web portal and a mobile app. Registration of new sensors can be conveniently done via the mobile app or web portal.

Users will be subject to a monthly fee based on the number of sensors registered in the system.

### The Architecture of the System

For implementation, the data flow architecture will be used to collect sensor readings, by creating a separate data ingestion service. The system also comprises a backend REST API, a database, a mobile app, and a single-page web app. Furthermore, a third-party payment gateway integration will be utilised for payment processing, as well as email notifications through a third-party email service. An identity management system, such as Keycloak, will also be integrated to perform authentication and access management.

### Q1(a)

Draw a context diagram for the above system.  
[3 marks]

### Q1(b)

Draw a container diagram for the above system.  
[3 marks]

### Q1(c)

What type of a database is suited to store the sensor data and other relevant data in this system? Defend your answer.  
[3 marks]

### Q1(d)

Draw a component diagram for the backend API container.  
[5 marks]

### Q1(e)

Mention a suitable technology stack (programming language/framework) that you can use to build the backend API application. Describe one advantage of using the mentioned technology.  
[2 marks]

### Q1(f)

Mention a suitable technology stack (programming language/framework) that you can use to build the single-page application. Describe one advantage of using the mentioned technology.  
[2 marks]

### Q1(g)

This system relies on many external services like email and payment processors. Mention two advantages and one disadvantage of using these outside services in software implementation.  
[3 marks]

### Q1(h)

Draw a simple diagram to show the data flow of the data ingestion component.  
[4 marks]

## Q2

### Q2(a)

Briefly explain the following design elements in a software design model.

1. Architectural elements
2. Deployment-level design elements

[5 marks]

### Q2(b)

Consider the following interface designed by a developer for an SMS-sending component.

```java
interface SMSService {
    void sendWithABC(Sms sms);
    void sendWithPQR(Sms sms);
}
```

Discuss the issues of this interface concerning reusability. Suggest an improved way to design this interface.  
[5 marks]

### Q2(c)

Explain how to apply pattern-based design to architect a software system. Illustrate your explanation with an example.  
[5 marks]

## Q3

### Q3(a)

Explain how to apply the concept of abstraction in software design subtasks. Provide a real-world software example to support your explanation.  
[5 marks]

### Q3(b)

Assume you encounter a scaling issue with a monolithic application. Explain an approach to progressively transition this application to a microservices architecture to address the problem. Use an example software application to illustrate your approach.  
[5 marks]

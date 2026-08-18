# 2026 Software Architecture Past Paper

University of Ruhuna  
Faculty of Engineering  
End-Semester 8 Examination in Engineering, May 2026

Module Number: EC6208  
Module Name: Software Architecture (C-23)  
Time: Three Hours

Answer all three questions.

## Q1

Answer the questions below based on the given scenario.

A newly established government-owned public transportation provider in Sri Lanka called **Lanka Metro Transit Services** plans to modernize urban bus transportation by introducing a smart digital transportation platform to improve passenger convenience, operational efficiency, and real-time monitoring of bus operations.

Your software company has been awarded this project, and your team is tasked with designing and implementing the system. Business analysts in your team have already gathered and finalized the functional requirements for the application.

Passengers should be able to use a mobile application to:

- register and manage their accounts,
- search available bus routes,
- view live bus locations on a map,
- estimate bus arrival times,
- digitally purchase tickets,
- and receive journey notifications.

Each bus should contain a GIS tracking device that periodically sends location updates to the backend system in real time.

Conductors should use handheld ticketing devices to validate QR-code-based digital tickets issued to passengers. The handheld devices should continue functioning during intermittent network connectivity and synchronize ticketing transactions automatically once connectivity is restored.

Passengers should be able to make payments using cards, mobile wallets, and LankaQR-supported applications. A third-party payment gateway called **PayMasterLK** can be used for payment processing.

A web-based operations dashboard should be implemented for transport administrators to:

- monitor buses in real time,
- track route delays,
- manage ticket pricing,
- view ticket sales reports,
- and monitor failures of GIS devices and handheld ticketing devices.

If a bus is significantly delayed, SMS notifications should automatically be sent to affected passengers. A third-party SMS service called **NotifyLK** can be used for sending SMS notifications.

All payment failures should be logged and displayed in the operations dashboard. In addition, an email notification should be sent to designated administrators for critical payment failures. A third-party email service called **Mailgun** can be used for sending emails.

The system must reliably support thousands of concurrent passengers during Colombo peak office hours and continue operating reliably under intermittent network connectivity conditions.

Assume that the architects in your team have decided to build:

- a separate backend application following the REST architecture,
- a separate frontend mobile application for passengers,
- and a separate web-based admin dashboard for transport administrators.

### Q1(a)

Draw a context diagram for the above system.  
[5 marks]

### Q1(b)

Draw a container diagram for the above system.  
[5 marks]

### Q1(c)

Identify the major functional components that should exist in the backend architecture of the above system and briefly explain the responsibility of each component.  
[5 marks]

### Q1(d)

Briefly explain what is meant by system resilience in distributed systems. Identify three ways a system can be designed to continue functioning when some components fail or when the system is under high load.  
[3 marks]

### Q1(e)

Draw a deployment diagram for a cloud-based deployment of this system.  
[4 marks]

### Q1(f)

Third-party integrations may introduce reliability issues into distributed systems. Mention one suitable system integration pattern that can be used to handle failures in external service calls and briefly explain how it helps.  
[3 marks]

## Q2

### Q2(a)

It is usually preferred to define and finalize the architecture of a software system before moving on to the implementation phase of the system. Name three advantages of defining a proper architecture to a system before the implementation of the system.  
[3 marks]

### Q2(b)

Briefly explain the following design principles used in component-based design:

1. Common Closure Principle (CCP)
2. Common Reuse Principle (CRP)

[4 marks]

### Q2(c)

Briefly explain how applying the principle of separation of concerns in component-based design improves system maintainability and extensibility.  
[3 marks]

## Q3

### Q3(a)

Name three main components of an Event Driven Architecture (EDA).  
[3 marks]

### Q3(b)

Briefly explain the difference between Monolithic and Microservice architectures in terms of:

1. Service granularity
2. Communication style
3. Deployment independence

[4 marks]

### Q3(c)

In a distributed system, a business process may involve multiple independent services. In your answer, briefly describe the role of compensating actions in the SAGA pattern.  
[5 marks]

### Q3(d)

Briefly explain what is meant by cascading failures in distributed systems and why they are particularly dangerous in tightly coupled architectures. Briefly mention one technique used to isolate failures and prevent system-wide impact.  
[3 marks]

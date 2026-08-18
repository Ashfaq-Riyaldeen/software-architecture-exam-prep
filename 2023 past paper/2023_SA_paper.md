# 2023 Software Architecture Past Paper

University of Ruhuna  
Faculty of Engineering  
End-Semester 8 Examination in Engineering: September 2023

Module Number: EE8217  
Module Name: Software Architecture  
Time: Three Hours

Answer all questions. Q1 carries 20 marks and the rest of each carries 10 marks.

## Q1

Answer the questions below based on the given scenario.

Assume that you are a software architect of a software company and your team is assigned to build a fuel quota management system for the general public in order to manage a fuel crisis in the country.

Any vehicle owner should be able to register on the platform via an online portal by providing the vehicle details. The system should validate the vehicle details by connecting to the Database of the Department of Motor Traffic. If the provided information is correct, it should generate a QR code which is unique to the particular vehicle.

The fuel station owners should be able to register themselves by accessing an online portal built especially for fuel station owners.

An employee-only web portal should be available for the administrators to monitor and perform operational tasks related to fuel distribution tracking and fuel station registrations.

An Android mobile app should be implemented for the fuel station operators in order to scan the QR codes of the vehicles and see the available balance fuel quota. Once the fuel pumping is finished for a vehicle, the fuel station operator should enter the pumped amount of litres into the mobile app. Upon entering the pumped amount of litres, the vehicle owner should receive an SMS with the details. The well-known SMS gateway called **SRI-SMS** can be used for SMS sending.

Assume that you have decided to build a separate backend REST API application and separate front-end applications for each portal.

### Q1(a)

Draw a context diagram for the above-mentioned fuel quota management system.  
[3 marks]

### Q1(b)

Draw a container diagram for the above-mentioned system. Clearly mention the technology stack for each container. Briefly explain the reasons behind selecting each technology.  
[4 marks]

### Q1(c)

Draw a component diagram for the backend container of the above system.  
[4 marks]

### Q1(d)

List down the specification (format) of an API call which can be used to register a vehicle in the system. Your answer should mention the HTTP method, the path, and the parameters of the API call. No need to write any source code.  
[3 marks]

### Q1(e)

Mention an authentication method for the REST API.  
[2 marks]

### Q1(f)

Assume that you have deployed this system in a cloud server and made an announcement to the general public asking them to register their vehicles on the platform. Mention one major issue which could occur when a large number of vehicle owners try to access the portal for registration. Explain a quick and cost-effective solution for the mentioned issue.  
[4 marks]

## Q2

### Q2(a)

Explain the Process-Related View of a component in component level design.  
[3 marks]

### Q2(b)

How do modern front-end frameworks and libraries promote and facilitate the adoption of a component-based architecture for front-end development?  
[3 marks]

### Q2(c)

Explain the Common Closure Principle (CCP) in component level design with an example.  
[4 marks]

## Q3

### Q3(a)

You are tasked with designing the architecture for a recommendation system for an e-commerce platform. The goal is to provide personalized product recommendations to users based on their browsing and purchase history. The system needs to collect user interactions, process this data, and generate recommendations using machine learning models.

Draw a simple diagram to show the architecture of the data ingestion part using a data flow architecture. The architecture should outline how you would fetch and store user interactions, such as product views, cart additions, and purchases, into a data storage system and prepare the data for subsequent machine learning processing.  
[4 marks]

### Q3(b)

What is meant by cross cutting concerns in Layered architecture? Provide one example for cross cutting concerns.  
[2 marks]

### Q3(c)

Compare and contrast microservices architecture with monolithic architecture, considering key aspects such as scalability, development complexity, maintenance, and deployment.  
[4 marks]

## Q4

### Q4(a)

Explain the concept of pattern-based design in software architecture.  
[2 marks]

### Q4(b)

Discuss the various levels (kinds) of patterns and their importance in software development.  
[2 marks]

### Q4(c)

Explain a real world software development related use case where an object-oriented design pattern can be used. Mention the advantages of using the mentioned design pattern for the mentioned scenario.  
[4 marks]

### Q4(d)

Briefly explain a common design mistake in pattern-based design and mention how to avoid such a mistake.  
[2 marks]

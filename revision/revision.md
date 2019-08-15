# Revision for CSC Exam

## Topics

-   Http
    -   Methods
    -   Statelessness
-   Web Api
    -   Url route Best Practices
    -   Security
    -   Validation
-   Web Server
    -   Sessions
-   Cloud services
    -   Benefits
    -   SPI
    -   Micro Services
-   Cloud services terminolgy
    -   Scaling Horizontally
    -   Scaling Vertically
-   AWS
    -   Queue
    -   S3
-   Azure
    -   Queue
-   Service Oriented Architecture
-   SOAP WSDL
-   XPath

## Http

### Methods

Topic A

[https://restfulapi.net/http-status-codes/](https://restfulapi.net/http-status-codes/)

Know what the different methods means in a REST web service

### Statelessness

Topic A

[https://stackoverflow.com/questions/13200152/why-is-it-said-that-http-is-a-stateless-protocol](https://stackoverflow.com/questions/13200152/why-is-it-said-that-http-is-a-stateless-protocol)

Understand what HTTP statelessness means
Find out the Pros and Cons of HTTP statelessness

## Web Api

### Url route Best Practices

Topic C

What are the best practices for formatting a Web Api Url

-   Versioning
-   Controller name to be plural
-   Route format to get a list of resource
-   Route format to get a specific resource
-   Route format to create a resource
-   Route format to update a resource
-   Route format to delete a resource

### Security

How HTTPS / SSL works

### Validation

-   Attribute validation

### Requests and Response

-   Know how a HTTP REST request and response message looks like
    -   Use postman to take a look at the raw HTTP messages

## Webserver

### Sessions

Topic G

-   Asp Net sessions are `In Process Memory` by default
-   When Webserver exists in multiple instances, session state is not shared across each instance
-   Need a storage area that is accessible to all instances to store sessions to maintain session state across all instances

## Cloud Services

### Benefits

Topic E

-   Reliable
-   Scalable
-   No upfront capital needed
-   Security implemented
-   Pay as you go

Read more about [cloud services pros and cons](https://www.linkedin.com/pulse/11-pros-cons-cloud-computing-everyone-should-know-umesh-singh/)

Understand how Queues and Cache can help a web service

### SPI

Topic E

-   S is Software as a Service (SaaS)
    -   Literally a software provided as a service to consumers
    -   gmail
    -   gdocs
    -   google sheets
    -   Office 365
-   P is Platform as a Service (PaaS)
    -   Platforms are items that developers/programs can work with which are provided as a service
    -   AWS S3
    -   AWS RDS
    -   AWS Beanstalk
    -   Azure Storage Account
    -   Azure Sql
    -   Azure Web App
-   I is Infrastructure as a Service (IaaS)
    -   Infrastructure meaning the hardware level being provided as a service
    -   AWS EC2
    -   Azure VM

### Microservices

Topic D, Topic 5

[AWS explaining Microservices](https://aws.amazon.com/microservices/)

[Why have queues for microservices](https://read.acloud.guru/scaling-microservices-with-message-queue-2d389be5b139)

## Cloud Service Terminology

-   Scaling Horizontally
    -   Increase or decrease the number of instances to handle varying amount of traffic
-   Scaling Vertically
    -   Increase or decrease CPU / RAM / Storage of a single instance to handle varying amout of traffic

## AWS

### Queue

-

### S3

Topic F

How does S3 confirm that it received the correct file that it was sent.

[S3 Common Request Headers](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonRequestHeaders.html)

[S3 Common Response Headers](https://docs.aws.amazon.com/AmazonS3/latest/API/RESTCommonResponseHeaders.html)

## Azure

[How to query status of Azure Queue](https://docs.microsoft.com/en-us/rest/api/storageservices/get-queue-service-stats)

## Service Oriented Architecture

Topic D, Topic 5

Understand the SOA diagram and what the SOA concept means.

## SOAP

Topic D, Topic 5

-   Understand and know the function of WSDL
-   Know how to add SOAP service reference in Asp.Net Framework
-   Know what transport protocols SOAP can use
-   Know how to read a WSDL to find out what operation it supports

# Topic E - Cloud Storage service

## Objectives

-   What is AWS S3
    -   Benefits of S3
    -   CORS configuration
-   Azure Storage Account
-   Azure SQL
    -   Benefits of Azure SQL instead of setting up a SQL Server on a VM yourself
-   What is DynamoDB
-   Queue Concept
    -   Azure Queue
    -   AQS SQS

---

## What is AWS S3

S3 stands for "Simple Storage Service". It is a blob storage service.

Blob stands for "Binary Large OBject"; blob is essentially data.

So S3 is a data storage service. S3 can store almost anything: images, documents, random words, random numbers, anything that can is essentially data.

### Benefits of S3

-   Do not need to buy own storage devices like HDD | SSD.
-   Data stored on S3 can be easily configured to be accessible from anywhere in the internet
-   Easily scalable
-   Pay only for what you use (storage space, bandwidth)
-   Can move data that is no longer used as often but still needed regardless to a cheaper service called Amazon Glacier

#### Introduction to Amazon Simple Storage Service (S3) - Cloud Storage on AWS

[![Introduction to Amazon Simple Storage Service (S3) - Cloud Storage on AWS](https://img.youtube.com/vi/rKpKHulqYOQ/0.jpg)](https://www.youtube.com/watch?v=rKpKHulqYOQ)

### CORS Configuration

Some application you build might require access to S3 from the browser. You would then need to configure CORS for your S3 bucket.

Read [AWS documentation](https://docs.aws.amazon.com/AmazonS3/latest/dev/cors.html) for more info

---

## Azure Storage Account

Azure Storage Account is a service provided by Microsoft to deal with Table (NoSQL and other document based databases), Blob (like AWS S3), and Queues.

Has similar benefits such as "Only pay for what you use" and "Scalable"

Read more [here](https://docs.microsoft.com/en-us/azure/storage/common/storage-introduction)

---

## Azure SQL

Azure SQL is "SQL database as a Service". The SQL server has been setup for you so that you can simply utilise the database without doing all the initial setup.

Read more [here](https://azure.microsoft.com/en-in/services/sql-database/)

> Azure SQL Scales Vertically

### Benefits of Azure SQL instead of setting up a SQL Server on a VM yourself

-   Don't need to install the software yourself
-   Easily configure firewall access to your database through the web portal instead of RDP into VM to setup
-   Don't need to update the VM the SQL Server is on
-   Need not worry about VM hardware failure

## DynamoDB

It is a key-value and document database. NoSQL.

What is NoSql? Read [here](https://www.mongodb.com/nosql-inline)

Read more [here](https://aws.amazon.com/dynamodb/)

> DynamoDB Scales Horizontally

## Queue Concept

In this context what we mean more specifically is a "Message Queue".

[Why you would want to use message queues](https://stackify.com/message-queues-12-reasons/)

#### Priority Queue

![Priority Queue](https://lh4.googleusercontent.com/i0aEIRUDm47hXLlVuB2XZN9ev4N_z4rLjZ0U_sCMYzQVMOw62U6hhhvbQbVvmPYzgGKjsB0yZib02TJrIYg4IF802mBtrDw37CInifUn0DF3Gjoj5Ze8PmEbKz3Bf23Yk7Yt)

#### Queue based load leveling

![Queue based load leveling](https://lh4.googleusercontent.com/i0aEIRUDm47hXLlVuB2XZN9ev4N_z4rLjZ0U_sCMYzQVMOw62U6hhhvbQbVvmPYzgGKjsB0yZib02TJrIYg4IF802mBtrDw37CInifUn0DF3Gjoj5Ze8PmEbKz3Bf23Yk7Yt)

[Different usage of queues in terms of RabbitMQ](https://www.rabbitmq.com/getstarted.html) (Also applies to most message queues)

[Azure Queue](https://azure.microsoft.com/en-us/services/storage/queues/)
[AWS SQS](https://aws.amazon.com/sqs/)

# CSC Assignment 2 AY 19/20

## Actual Assignment Document Link

[https://docs.google.com/document/d/14QpqXRWT6jZVE7DOxP33mwUSJcm3XdbAQnS64W1y4Co/](https://docs.google.com/document/d/14QpqXRWT6jZVE7DOxP33mwUSJcm3XdbAQnS64W1y4Co/)

## Instructions

1.  You may work in a group of maximum 4 students. Each group needs to implement 4 ADDITIONAL Features. 5 additional features need to be implemented if the group size is 5. Please consult your tutors for the additional features.

2.  You should finish your assignment and submit your documentation before 23:59 on 11/August/2019 (Sunday)

3.  You are required to demonstrate your skills and capability in design and implementation of multi-tier distributed applications using Web services and cloud Services in the AWS, on top of it, feel free to try Azure Cloud, OR AWS OR other cloud.(BLUEMIX)

4.  You should focus on the Web service design and implementation, instead of client interface design.

5.  An interview session will be done at the end of the assignment. All members of the group have to be present; no mark will be awarded if you did not attend the interview session.

6.  Hard copy of your documentation needs to be submitted during interview time.

---

## User Intefrace for Assignment 2

1.  User Registration page

2.  User Login page

3.  User profile management page

    -   To update their personal particulars

4.  User Create Talent page

    -   Fill in talent information
    -   Upload talent photo

5.  User View his own talents page

    -   View talent information
    -   View talent photo
    -   Searchable

6.  Everyone View All talents page

    -   Searchable
    -   Disqus comments

7.  User Update his talent page

8.  User Delete his talents

---

## Core Cloud / Webservices for Assignment 2

1.  Account Web Service

    -   Users can register
    -   Users can login via JWT Bearer Token
    -   Users can update their personal particulars

2.  Email Web service (SOAP)

    -   Create a Email Web Service using SOAP
    -   The application will utilise the created email web service to send emails to users

3.  Image Web Service

    -   Use S3 or Azure Blob Storage
    -   Allow users to upload photos
    -   Allow users to view photos

4.  Captcha Web Service

    -   When user registers, they will be prompt with a captcha to check if they are human
    -   reCAPTCHA or [others](https://www.dtelepathy.com/blog/design/captcha-alternatives-better-ux)

5.  CRUD Talents

    -   Users can create talents
        -   Model Validation
            -   Use Regex on at least one of the fields to validate
    -   Users can view talents
    -   Users can update their talents
        -   Model Validation
            -   Use Regex on at least one of the fields to validate
    -   Users can delete their talents
    -   To be secured with SSL and JWT Bearer Token

6.  Store session data in DynamoDB (NoSQL)
    -   Refer to [assignment 2 appendix D](https://docs.google.com/document/d/14QpqXRWT6jZVE7DOxP33mwUSJcm3XdbAQnS64W1y4Co/edit#bookmark=id.e25eyvhi40o3)
    -   Or google it yourself

---

## Advanced Tasks

1.  Google Authenticator

    -   Two factor authentication

2.  Offline feature

    -   Users can still view talents' information and photo even if website is down
    -   PWA (Progressive Web App) for Websites
    -   Custom caching for Mobile apps

3.  Do not store credentials for AWS or Azure in the source code

    -   Environment variables or secret files that are not pushed to version control

4.  Hosting the application

    -   Host on AWS EC2 with this [practical](https://docs.google.com/document/d/1YvRloJnBKozgV8BZqQnLAZrJm-MZbUumh4U7SXZa1l8/edit?usp=sharing)
    -   Host on AWS Elastic Beanstalk with this [practical](https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/create_deploy_NET.quickstart.html)

5.  Maintain Session Status accross different devices

6.  Implementing Failover feature for talent service

7.  Web Services (APIs) and Web server (server that serves the web pages) to be hosted separately

8.  Schedule your EC2 instance to only run 8am to 10pm

---

## Assessment Criteria

| Item                                                               | Percentage |
| ------------------------------------------------------------------ | ---------- |
| Setup for Windows Azure/AMS development environment                | 5%         |
| Detailed Architecture for Application (documentation)              | 5%         |
| Web Services                                                       | 30%        |
| External Web Service                                               | 10%        |
| User Interface (usability)                                         | 5%         |
| Exception Handling                                                 | 10%        |
| Coding Convention and Documentation of the Web Services            | 5%         |
| Additional Functionality and Feature for Web Services              | 10%        |
| Validation, Security, scalability, performance and Maintainability | 20%        |
| Total                                                              | 100%       |

---

## List of services

-   Disqus (Comments service)
-   Captcha
-   Stripe (Payment service)
-   S3 (Blob storage service)
-   Cloudinary (Image storage service)
-   Clarifai (Image recognition service)
-   Google Authenticator
-   CDN
-   Email Web Service (Make your own SOAP service then call it in the actual Talent Search project)
-   EC2 (VM, infrastructure as a service)
-   Elastic Beanstalk (Web app hosting, platform as a service)
-   DynamoDB

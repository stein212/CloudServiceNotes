# CSC Assignment AY 19/20

## Instructions

1.  This is an individual assignment.

2.  You should finish your assignment and submit your documentation before 10:00 pm on 23 June 2019 (Sunday)

3.  You are required to demonstrate your skills and capability in design and implementation of Web API, and consuming the Web API.

4.  An interview session will be done at the end of the assignment. No mark will be awarded if you did not attend the interview session.

---

## Tasks

### Task 1

-   [Practical 1](https://docs.google.com/document/d/1t-mTUI2V1UIySb-VDOgZ6m0c9NBJVOmcaIdnIlx9CVg/edit#bookmark=id.9ato13epfk99)

    -   Part D

        -   Register with [world weather online](https://developer.worldweatheronline.com/)

    -   Part E (Demo during interview)

        -   Use postman to test the api

    -   Part F (Demo during interview)

        -   Show that you are able to call the api using C# (webform, mvc, console)
        -   Get the API to return XML
        -   Show the XML on a page or print into console

    -   jQuery (Demo during interview)

        -   Call the api using jQuery (`fetch` and `axios` or other http library are also allowed)
        -   Get the API to return JSON
        -   Show the JSON on a page or print into console

    -   Draw Diagram to show differences between using C# and jQuery (or javascript) to call the web service
        -   Draw a diagram that shows some sort of difference base on your understanding

-   Deliverables
    -   Source code (C# project and html file for jQuery/javascript calling api)
    -   Diagram
    -   Demo C# and jQuery/javascript api calls

---

### Task 2

-   [Practical 2 Part 2](https://docs.google.com/document/d/1fQCyw4GJJcSDXCAzRe9RRso-ldYJ3Ygay3UMnpahQM0/edit#bookmark=id.uu2kbbog5u9d)

    -   Follow the practical to create a WEB API project (Show source code during interview)
        -   CRUD Product (Demo during interview) (Take screenshot of using postman to do CRUD)

-   [Practical 3 Part 1](https://docs.google.com/document/d/1a-Q5qkz5xAfHDKnN15zJPM69xpfsH-x7bWPAQid-m7U/edit#heading=h.i10i9kig19vg)

    -   Validate model data using Data annotations
        -   postman to show errors when posting incomplete/wrong data (Take screenshot of using postman to trigger the validation errors)
            -   Over-Posting error may not work

-   Deliverables
    -   Source code (C# WEB API project)
    -   WEB API Document (Create your own documentation if needed)
    -   postman screenshots (CRUD and validation errors)
    -   Demo the WEB API

---

### Task 3

Follow the videos in this [link](http://mycsc.net/uncategorized/web-api-2-security-authentication-bearer-token-tutorial/) to make a web api project with bearer token

-   The videos are for ASP.NET Framework
-   This workflow does not work on ASP.NET Core

-   If you want to do bearer token with ASP.NET Core, you will have to search for online resources to guide you

-   Deliverables

    -   Source code (C# WEB API project with bearer token implemented)

        -   Should contain a simple webpage that allows for

            1.  Invoking an api
            2.  Registering a user
            3.  User login

            Example for the above 3 points can be seen in Mr Ji's website

    -   WEB API Document (Create your own documentation if needed)
    -   Demo the simple webpage during interview

---

### Task 4

-   Talent Search (ASP.NET Framework) ([Task link](http://mycsc.net/cloud-service/restful/e-learning-week-activity/))

    -   Task 1

        -   Create a web form project that will be used for the rest of the tasks

    -   Task 2

        -   Download the zip
        -   Create a new folder in the web form project created in task 1
        -   Name the new folder "SearchTalent"
        -   Extract the contents of the zip to the new folder
        -   Run the index.html file (ensure it is under `localhost` and not as a `file:///`)
        -   Test the search
        -   Modify the search code to allow searching by Name and Bio

    -   Task 3

        -   Cloudinary (Image hosting service)
            -   Create an account with cloudinary
            -   Upload the images to cloudinary
            -   Update the code to use the images hosting in cloudinary instead of using the local images

    -   Task 4
        -   Talent Restful service (Talent WEB API)
            -   Follow this [link](https://docs.google.com/document/d/1NHjfY4ypOxnfB5JfY_g_yr14hPVZFf5-8248H1JeZD0/edit)
            -   Create CRUD for talent search
            -   postman screenshot of CRUD
        -   Optional:
            -   Host the Talent WEB API in Azure, AWS or Google Cloud

-   Deliverables
    -   Source code (C# Web form and WEB Api project)
    -   WEB API Document (Create your own documentation if needed
    -   postman screenshot
    -   Demo

---

### Task 5

-   Enable HTTPS for Talent WEB API Project

    -   [Youtube video to enable https](https://www.youtube.com/watch?v=xIzlD-frEw4&t=179s)

-   Deliverables
    -   Demo (Show that https is in effect)

---

### Task 6

-   Stripe [gdoc for implementing sample page link](https://docs.google.com/document/d/1sBDyVmLOHkDB5cHqbnG3mzuwwv6y5QSMWhifBxKxvvI/edit?usp=sharing)

    -   Implement a page that does sample stripe charge
    -   Sequence Diagram
    -   Refer to the official [stripe github repo](https://github.com/stripe/stripe-dotnet) for more information on how to implement it

-   Store Talent photos in AWS S3

    -   Similar to Task 4.3, you will now utilise AWS S3 instead of cloudinary to store the photos
    -   [AWS Educate Account](https://aws.amazon.com/education/awseducate/) to get a student account
    -   OR just make a normal AWS account and use [free tier](https://aws.amazon.com/free/?all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc&awsf.Free%20Tier%20Types=categories%23featured)

-   Deliverables
    -   Demo
    -   Sequence diagram of how the stripe charge happened
    -   Change Task 4.3 to use images in AWS S3 and demo it

---

### Task 7 (Optional)

-   Develop a web / mobile app to allow users to:

    -   Upload an image
    -   Then system will use clarifai to tag the image

-   Deliverables
    -   Demo
    -   Source code

---

### Others (notes)

-   Ensure you are able to explain the different tasks
-   Ensure code is properly formatted (proper identation, naming conventions)
-   Efficient code
-   Robustness and security of code
    -   Web API latency should be simulated and AJAX loading Gif should be displayed to users.
    -   In case of network/server failure, your application should be able to detect and recover from the errors(RE-TRY).
-   For submission, separate each task into their own folder and then zip all the folders into 1 zip
-   Zip name convention: class+id+name+Assignment01 (e.g. DIT-3A03-1612345-Chin Chia Ho-Assignment01)

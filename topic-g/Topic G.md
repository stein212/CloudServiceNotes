# Topic E - Develop Web Service

## Objectives

-   Http Statelessness
-   Load Balancing
-   Caching

---

## Http Statelessness

Http is a stateless protocol, meaning that the server receiving the http requests does not track the caller.

An example is that SP's blackboard does not care which laptop you login, as long as you pass in the correct credentials, it will give the browser a cookie that denotes you.

The cookie is not tracked by the server either, as the cookie will be sent along with every http request you make to blackboard.

More on [why it is stateless](https://stackoverflow.com/questions/13200152/why-is-it-said-that-http-is-a-stateless-protocol)

And the [why sessions is not really a state in http](https://stackoverflow.com/questions/13200152/why-is-it-said-that-http-is-a-stateless-protocol)

[Advantages of http statelessness](https://restfulapi.net/statelessness/)

---

## Load Balancing

As the traffic to your web server increases, we have 2 choices: upgrade the web server hardware specs, or spin up another web server to handle the load

-   Upgrade the web server (vertical scaling)

    -   Pay for a more expensive and faster web server
    -   There is a limit to how fast a web server can be, thus a limit to how many traffic it can handle

-   Spin up another web server
    -   Pay for another instance of the web server
    -   No limit to handling traffic as you can just keep spinning up more web server instances
    -   Need to manage session data between instances

![Load balancing in action](https://lh3.googleusercontent.com/pEQltdEtheUrZqIE0q5rMUBbDr9YLUov3MZdXZ5EyDdJPzC139rKrJLib-T-slIBTLuWmaqg72U_2l22-0S-BJIUo67fVneH1abhIZh4UXcT0QhwzJVM-fSDk37UYDu-xHmw)

---

## Caching

Caching is regarding data caching, more specifically caching your database results

Some common challenges of database are:

-   Slow query processing
    -   Some database queries, no matter how optimised your database design is, will take a certain amount of time, which sometime is not fast enough
-   Scaling costs
    -   Creating a new read replica of the main database still costs money, and spinning more up will cost even more
    -   Similar to read replica, multiple writable database instance may cause inconsistent data across all database instances, and cost money
-   Difficult data access
    -   Some queries may require joins to other tables to get the data we need which is not optimal

![Caching diagram](https://lh3.googleusercontent.com/yG27iyWpyoHPnc1gn6bxtC8qY57oFSYM4NZcunb1NF2uBdi7nr0aa1C7WLT-oTJVCtiyY5Lh408l2RlrBjGdzoFkqePPl_r_0p-KhfbwbkrdRNs_iRhQ_mUSJ4l-ErBKLRtg)

Enter caching. We can mitigate those challenges for frequently accessed read data (meaning unlikely to change data but frequently needed).

If we simply cache the results of frequently needed and rarely changed data, we can bypass the query processing, reduce the need to scale, and difficult data access. This works simply because the result is already cached and ready to be returned again.

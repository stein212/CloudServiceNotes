# Topic E - Introduction to Cloud Computing

## Objectives

-   What is Cloud Computing
-   Why utilise Cloud Computing
-   Cloud Computing Services available
-   Types of Cloud
-   Utility Based Model: SPI
-   Multitenant Architecture
-   Questions from slides

---

## What is Cloud Computing

> Simply put, cloud computing is the delivery of computing services—including servers, storage, databases, networking, software, analytics, and intelligence—over the Internet (“the cloud”) to offer faster innovation, flexible resources, and economies of scale. You typically pay only for cloud services you use, helping lower your operating costs, run your infrastructure more efficiently and scale as your business needs change. - [Microsoft](https://azure.microsoft.com/en-in/overview/what-is-cloud-computing/)

---

## Why utilise Cloud Computing

### Cost

Traditionally, companies had to host their own services, which means they need to deal with procuring the equipment, space, people, licenses, etc that is needed to set up. This procurement results in a high initial upfront costs. Furthermore, they still need to maintain the hardware themselves.

With cloud computing, the setup and maintenance is relegated to the cloud service provider (such as Azure, AWS, Google Cloud). These providers charge based on usage, thus companies only pay as they use, allowing them to avoid sinking too much capital at the start.

### Scalability

Cloud computing allows users to scale according to their needs, be it to support targeting a bigger audience or to accomodate for spike in internet traffic.

![Infrastructure Cost vs Time](https://image.slidesharecdn.com/aws-keynote-100419170737-phpapp01/95/the-cloud-as-a-platform-by-jinesh-varia-26-728.jpg?cb=1434492015)

### Reliability

Mainstream Cloud Computing services are reliable due to redundancies built into their infrastructure. If a server goes down, another server is already on standby to take over; if a storage drive corrupts, the data is available on a separate storage drive; if a datacenter is down, your services are still accessible from another datacenter.

![Fault tolerance](https://thumbs.gfycat.com/ColorlessNeighboringLeafcutterant-small.gif)

---

## Cloud Computing Services available

![Cloud Providers](https://zdnet2.cbsistatic.com/hub/i/r/2018/02/09/1a47f155-1262-4ead-838d-97ec0e662d09/resize/770xauto/1c0e60f3350a67160b54debb5c002a0b/stacking-up-cloud-vendors-2018-right-scale-2.png) (From ZDNet)

---

## Types of Cloud

### Public cloud

Public clouds are owned and operated by a third-party cloud service providers, which deliver their computing resources, like servers and storage, over the Internet. Microsoft Azure is an example of a public cloud. With a public cloud, all hardware, software, and other supporting infrastructure is owned and managed by the cloud provider. You access these services and manage your account using a web browser.

### Private cloud

A private cloud refers to cloud computing resources used exclusively by a single business or organisation. A private cloud can be physically located on the company’s on-site datacenter. Some companies also pay third-party service providers to host their private cloud. A private cloud is one in which the services and infrastructure are maintained on a private network.

### Hybrid cloud

Hybrid clouds combine public and private clouds, bound together by technology that allows data and applications to be shared between them. By allowing data and applications to move between private and public clouds, a hybrid cloud gives your business greater flexibility, more deployment options and helps optimise your existing infrastructure, security and compliance.

---

## Utility Base Cloud: SPI

### Infrastructure as as Service (IaaS)

IT infrastructure such as servers, virtual machines (VMs), storage, and network are rented out to users.

### Platform as as Service (PaaS)

Users rent an environment for running their applications. Users need not worry about underlying servers, storage, network (built on top of IaaS)

### Software as as Service (SaaS)

Literally Software as a Service. Software such as Google Apps, Microsoft 365 on a subscription plan.

![SPI](spi.png) (From Microsoft)

## Multitenant Architecture

Multiple tenants (could be users, groups or other services) have access to the same service but with their own specific privileges. Essentially sharing the service.

Example is Google Drive: Users all the same service (google drive) but are only allowed access to files and folders that they have permission for.

---

## Questions from slides

1. In a traditional environment, when you make a capacity decision before you deploy a system, you might end up with expensive idle resources or with the performance implications of limited capacity. Which technique can help you address this in a cloud-based environment?

    a. Allow for evolutionary architecture.  
    b. Lower the risk of architecture change.  
    c. Scale up and scale down automatically.  
    d. Test systems at production scale.

2. When will cloud computing provide the most value?

    a. A company has several thousands of documents that need to be indexed in many months.  
    b. A company has several hundreds of documents that need to be indexed in a few minutes.  
    c. A company has to process their payroll actives at the end of each pay period in batch mode.  
    d. A company has purchased additional hardware in order to process their payroll activities faster at the end of each pay period.

3. Which delivery model is an example of a cloud computing environment that provides end users with a web based e-mail service?

    a. Software as a Service  
    b. Platform as a Service  
    c. Computing as a Service  
    d. Infrastructure as a Service

<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
Answers: c, c, a

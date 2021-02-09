# Service Oriented Architecture

### What is SOA?

According to [Wikipedia](https://en.wikipedia.org/wiki/Service-oriented_architecture),
> Service-oriented architecture (SOA) is a style of software design where services are provided to the other components by application components, through a communication protocol over a network. An SOA service is a discrete unit of functionality that can be accessed remotely and acted upon and updated independently, such as retrieving a credit card statement online. SOA is also intended to be independent of vendors, products and technologies.


This definition is quite overwhelming, so to understand it in an easy and detailed  way let’s break it down into smaller parts and then try to learn them one at a time. But before diving deep into this, it is also important to know *Why there is a need for SOA or any other architectural style* and *Which style is used prior this?*

### Evolution of SOA
As we all know, to accomplish any software engineering task some basic conventions and procedures need to be followed. So, the initial conventions or style that followed in software development is **Single-Tier Architecture**.

![Single Tier Architecture diagram](https://mk0softwaretest02r6g.kinstacdn.com/wp-content/uploads/2016/06/one-tier-software-architecture.png)

In this type of architecture, there is a single machine which acts as a container and all the layers(Presentation layer, Bussiness Logic layer or Database layer) are kept in the same container. Thus it is called **Monolithic Architecture**.

Due to this reason, the above architectural style of software development is:
* *Not Flexible*: It is very difficult to update the code base and make changes in the technology stack used.

* *Less Reliable*: If even a single feature of the system fails the entire system needs to be step down from the production/live.

* *Not Scalable*: The rebuild is mandatory to scale the project as it is programmed hierarchically.

* *No Scope of Continous Development*: building and deployment of features are not possible simultaneously.
 

Thus, the entire software community necessitates a model which can be a perfect fit for complex architectures(where monolithic style fails). So, Here comes SOA as a saviour😎 for the entire development community.

### SOA and its princilples

SOA is an approach to distributed system architecture that employs loosely coupled services, standard interfaces and protocols to deliver seamless cross platform integration. It is used to integrate widely divergent components by providing  them with a common interface and a set of protocols for them to communicate through service bus.

In SOA, the enire application is not built at once. Here,it is broken down into small functional pieces known as services and after building these services the results are combined to reach the desired result.

The main benefit of SOA or any multi-tier architechtural style is it provided hetrogenous interoperability.

This simple means that we can create each service into a different technology/tool and then only we need to find out the medium of communication among them.

![Heterogeneous Interoperability in SOA](https://www.oreilly.com/library/view/microservices-vs-service-oriented/9781491975657/assets/mvso_0402.png)

### USE CASE
To make it clear further let’s take an example of website to book a cab and pay the bill. 

One approach to this is create the entire system from the scratch, this process can take an year or so. Or even after that there is not any assuring that system will not fail or will not need any updates in future.

Now the other way is to divide the application/sytem into sub systems and then choose vendors for the services/sub-systems in the market and Integrate them to create your own product.Here the only task left is to create a common interface for the all these services to communicate with each other.

![SOA Use Case](https://drive.google.com/file/d/1BMzLHt8jC5cD14wH9Zcp9rPuZFt3p0Os/view?usp=sharing)

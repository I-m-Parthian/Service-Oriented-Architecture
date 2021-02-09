# Service Oriented Architecture

### What is SOA?

According to [Wikipedia](https://en.wikipedia.org/wiki/Service-oriented_architecture) ,
> Service-oriented architecture (SOA) is a style of software design where services are provided to the other components by application components, through a communication protocol over a network. A SOA service is a discrete unit of functionality that can be accessed remotely and acted upon and updated independently, such as retrieving a credit card statement online. SOA is also intended to be independent of vendors, products and technologies.


This definition is quite overwhelming, so in-order to understand it in an easy and detailed  way let’s break it down into smaller parts and then try to learn them one at a time. But before diving deep into this, it is also important to know '*Why there is a need for SOA or any other architectural style?*' and '*Which style is used prior to this?*'

### Single Tier/Monolithic Architecture
As we all know, in order to accomplish any software/engineering project some basic conventions and procedures need to be followed. So, the initial convention or style that followed in the software development is **Single-Tier Architecture**.

![Single Tier Architecture diagram](https://mk0softwaretest02r6g.kinstacdn.com/wp-content/uploads/2016/06/one-tier-software-architecture.png)

In this type of arcitecture only the authorised users can access/view the info. So,can't be used for public presentational projects.

Secondly, all the layers(Presentation layer, Bussiness Logic layer or Database layer) are stored on a single machine due to this:
* Difficult to maintain as single system needs to bear the entire load
* *Less Reliebility* : There is no backup system in case of system failure or server down
 * *No Flexibility* : Difficult to update the code base and no Reusability
 * *Not Scalable* : vvkjvbdfvk

Now, the entire software commmunity is need of a model which can provide:
* Scalability
* Reusability
* Parallel maintainence and Updation
* Interoperability

and many more...


So, Here comes SOA as a saviour😎 for the entire devlopment community.

SOA is an approach to distributed system architecture that employs loosely coupled services, standard interfaces and protocols to deliver seamless cross platform integration. It is used to integrate widely divergent components by providing  them with a common interface and a set of protocols for them to communicate through service bus.

![Heterogeneous Interoperability in SOA](https://www.oreilly.com/library/view/microservices-vs-service-oriented/9781491975657/assets/mvso_0402.png)

### USE CASE
To make it clear further let’s take an example of website to book a cab and pay the bill. 

One approach to this is create the entire system from the scratch, this process can take an year or so. Or even after that there is not any assuring that system will not fail or will not need any updates in future.

Now the other way is to divide the application/sytem into sub systems and then choose vendors for the services/sub-systems in the market and Integrate them to create your own product.Here the only task left is to create a common interface for the all these services to communicate with each other.

![SOA Use Case](https://drive.google.com/file/d/1BMzLHt8jC5cD14wH9Zcp9rPuZFt3p0Os/view?usp=sharing)

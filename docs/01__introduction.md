---
title: Training 01 - Introduction
date: 2020-10-09
authors: Hing-Wah.Kwok@dst.defence.gov.au, Philip.Cutler@dst.defence.gov.au
---

<!-- # Training 01 - Introduction -->

Welcome to our repository of information on cloud native, and cloud native technologies. If you are viewing this on GovTEAMS, hold down ctrl when clicking to follow links.

This information is written in markdown, a language for creating formatted text. It's stored in [Bitbucket](https://bitbucket.dsto.defence.gov.au/projects/DO/repos/devops-training-material/browse), a [git-based source code repository](../docs/02_software-development-basics). There are other files in the repository for linting, which flags programming and stylistic errors, and you can learn more at the [pre-commit project](https://pre-commit.com/).

Please add information to these pages that you think might be useful for others.

## Introduction to cloud computing

From a user perspective, the cloud is thought of as 'computer systems owned by someone else, accessible over the internet.' Watch [What is the cloud? | CNBC Explains (3:00)](https://www.youtube.com/watch?v=i9x0UO8MY0g) on YouTube.

But the cloud is more than online data storage and online applications. It has a range of technologies that are changing the application and IT operations landscape.

Cloud computing technologies are grouped into different service models:

* [Software as a Service (SaaS)](#saas)
* [Infrastructure as a Service (IaaS)](#iaas)
* [Platform as a Service (PaaS)](#paas)
* [Containers as a Service (CaaS)](#caas)
* [Functions as a Service (FaaS)](#faas).

Applications that are built to take advantage of the cloud, are called [cloud native](#cloudnative).

### Cloud computing service providers

Cloud platforms provide cloud computing services, like virtual machines and data storage, accessed across the internet. These services can be accessed immediately, offer usage-based pricing, and have large data centres.

Major cloud providers include:

* Amazon Web Services
* Microsoft Azure
* Google Cloud Platform
* IBM Cloud.

#### Public cloud

Public cloud is a term used to describe services from cloud computing service providers.

#### Private cloud

Private cloud is when you run public cloud technologies in on-premises data centres. A private cloud is not a traditional on-premise data centre.

Private clouds give you access to modern application services, like [serverless computing](https://en.wikipedia.org/wiki/Serverless_computing) (serverless computing lets you build and run applications and services without thinking about servers).

Like public clouds, internal customers can provision their own virtual resources to build, test, and run applications.

#### Hybrid cloud

Hybrid cloud is a combination of public cloud platforms with private cloud technology to create a hybrid of both.

Hybrid cloud scenarios include:

* Applications in the public cloud using databases in the customers data center.
* Parallel environments in which applications can move between private and public clouds.
* Virtualised data centre workloads that replicate to the cloud during peak use.

#### Multicloud

When a single organisation uses more than one cloud platform, it's called multicloud.

### <a name="cloudnative"></a>Cloud native computing

Cloud native is a model of application creation and delivery. Cloud native computing is complementary to DevOps. It fully exploits the power of cloud computing. The [Cloud Native Computing Foundation (CNCF)](#cncf) supports the adoption of the cloud native model for applications.

Cloud native applications can be hosted in the public cloud, private cloud, or a hybrid solution.

Cloud native applications are:

* Scalable
* Resilient
* Manageable
* Observable.

The benefits of using cloud native technologies for developing and deploying applications include:

* Increased speed and agility of development and management
* Built-in application resilience
* Increased developer productivity
* Simplifies and strengthens deployment by using continuous delivery
* Simplifies operations
* Optimises resource use
* Automated deployment scaling
* Application is portable to other clouds
* Faster product delivery to customers.

Cloud native technologies include:

* Containers
* Service meshes
* [Microservices](../docs/06_architecture-Software.md)
* Immutable infrastructure
* Declarative APIs.

Watch [Keynote: What is Cloud Native and Why Should I Care? - Alexis Richardson, CEO of Weaveworks (20:21)](https://www.youtube.com/watch?v=TKYAI19OE-c).

### <a name="cncf"></a>Cloud Native Computing Foundation (CNCF)

The CNCF, a sub-foundation of [The Linux Foundation](https://linuxfoundation.org/), aims to support the adoption of the Cloud Native model for applications. They support the open-source development of projects that support Cloud Native computing. See the [formal definition of the CNCF](https://github.com/cncf/toc/blob/main/DEFINITION.md).

The CNCF curate and promote a list of trusted tools (paid and open-source) called the [Cloud Native Interactive Landscape](https://landscape.cncf.io/).
For organsations just starting their cloud journey, there is the [Cloud Native trail map](https://github.com/cncf/landscape/blob/master/README.md#trail-map). For insight into what other companies recommend, see the [Cloud Native End User Tech Radar](https://radar.cncf.io/).

Another good reference for technologies is the [ThoughtWorks Technology Radar](https://www.thoughtworks.com/radar).

For insight into the CNCF, watch the [Keynote: End to End: The Foundation of Doers - Priyanka Sharma, General Manager, CNCF (13:32)](https://www.youtube.com/watch?v=u71aL6aVDPg).

### <a name="saas"></a>Software as a service (SaaS)

SaaS is when an application is hosted in the cloud.

Saas gives the opportunity for multi-tenant applications. Traditional arrangements involved a separate instance of an application to be run for each organsation, but with multi-tenancy, a single application can be shared by multiple customers. Each customer has its own data, and the application keeps the data separate and secure. Not all cloud applications use multi-tenancy.

SaaS applications can offer extensive configuration options to customers, and enable customers to code their own changes or additions.

Popular SaaS products include Microsoft 365, Google Workspace, and Salesforce.

From the customers perspective, there are many benefits to using a SaaS application, as they often have:

* No installation
* Pay only for what you use
* Free trials
* Lower up-front costs
* Saves on-premises resourcing, such as servers and IT staff
* Simple and easy upgrades

There are also some risks with using a SaaS application, from the customers perspective:

* Need to trust the SaaS provider for availability and security
* Legal or regulatory requirements for data storage
* Multi-tenant applications can reduce customisation
* Integration with existing on-premises applications can be harder
* Can experience reduced performance compared with on-premises applications.

From a software vendors perspective, there are many benefits:

* A more predictable revenue stream
* Can sell directly to business decision makers instead of IT
* Reduced support costs by using multi-tenant applications
* Can gather more data on customer use of the application
* Can broaden the market potential

There are also some risks a software vendor needs to consider before developing and delivering their application in the cloud:

* The application should demonstrate real value up-front in free trials
* Revenue can come in slower
* Multi-tenant applications could limit the ability to sell customisation services
* Could find customer resistance to using the cloud
* Could require significant business changes, for example, changes to app development, IT operations, pricing, and sales.

### <a name="iaas"></a>Infrastructure as a service (IaaS)

IaaS provides storage and compute services on a pay-per-use basis. They offer services including:

* Highly scalable databases
* Virtual machines
* Virtual private networks
* Big data analytics
* Developer tools
* Machine learning
* Application monitoring.

### <a name="paas"></a>Platform as a service (PaaS)

PaaS is a development environment to create, host and deploy applications in the cloud.

### <a name="caas"></a>Containers as a service (CaaS)

Instead of working at the virtual machine level, with CaaS you can instead deploy and manage containers. This often uses [Kubernetes](#k8s).

### <a name="faas"></a>Functions as a service (FaaS)

FaaS is the cloud version of serverless computing. It adds a layer of abstraction to PaaS, so you don't need to think about VMs or containers, and instead you build your applications as functions and set those functions to be triggered by certain events. FaaS can cost less, since your functions consume no IaaS resources until an event occurs, so the pay-per-use fees are lowered.

## <a name="k8s"></a>Kubernetes

Kubernetes is a container orchestrator. For an introduction, watch [The Illustrated Children's Guide to Kubernetes (8:02)](https://www.youtube.com/watch?v=4ht22ReBjno) on YouTube.

Free training: [Introduction to Kubernetes](https://www.edx.org/course/introduction-to-kubernetes#!)
Difficulty: Beginner
Length: 4-5 weeks, 2-3 hours/week
Who It’s For: Developers and system administrators who want to get started with Kubernetes.

View and watch hundreds of [Cloud Native webinars](https://www.cncf.io/online-programs/).

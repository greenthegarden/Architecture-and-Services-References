---
title: Training 02 - Software Development Basics
date: 2020-10-09
authors: Hing-Wah.Kwok@dst.defence.gov.au, Philip.Cutler@dst.defence.gov.au
---

<!-- # Training 02 - Software Development Basics -->

> As with any task software development has many fundamental **tools of the trade**.

## Source code

Source code is the code of a computer program, written by programmers in plain text and understandable by a human being. Source code gets transformed into the machine code of 1s and 0s and this tells the computer what to do.

Source code can be proprietary or open-source. Open-source means that the computer program code is shared for all to use.

Source code is what computer programmers create when they make computer programs. It often relies on supporting files, such as images.

### Source control

Source control is tracking and managing changes to your code over time. Like using 'Track Changes' in a word document.

### Source control management (or version control system)

A system that enables source control. It provides the projects change  history, and provides methods of managing conflicting code changes (for example, two people both modify the same section of code).

Source control management system benefits:

* Easily revert changes in the project back to a previous point in time
* Allows for multiple people to contribute modifications to the code in a pre-determined, controlled manner
* Keeps a history of your project from the viewpoints of its changes
* Makes troubleshooting simpler by seeing who made what changes, when.

Source control management system examples:

* [Git](#git)
* [Mercurial](https://www.mercurial-scm.org/)
* [Apache Subversion](https://subversion.apache.org/)
* [Azure DevOps Server](https://azure.microsoft.com/en-au/services/devops/server/) (previously known as Team Foundation Server).

#### <a name="git"></a>Git

Git is a mature, actively maintained open-source source code management system created in 2005.

Git is a distributed version control system, which means every team member has a copy of the project locally on their computer. This is contrasted to a centralised version control system where all team members connect to a single server, which will prevent programmers from continuing to work if they cannot access the server.

To learn git:

* Watch the [learn Git videos](https://git-scm.com/videos)
* View the [Git website]([Git](https://git-scm.com/)
* View the [Git docs]().
* Watch [Git Tutorial for Beginners: Learn Git in 1 Hour](https://www.youtube.com/watch?v=8JJ101D3knE) (1:09:13) on YouTube
* Use Atlassians [Git commands cheat sheet](onenote:#section-id={878FE29D-7937-4B76-878B-4B2DB9B96219}&end&base-path=https://consiliumt-my.sharepoint.com/personal/kaylan_lily_consilium_technology/Documents/Kaylan%20@%20Consilium%20Technology%20Pty%20Ltd/DevOps.one).

## Software version numbers

Software versioning gives a unique name or version numbers to the state of the software.

There are often tracked using two versioning schemes:
1. An [internal version number](https://en.wikipedia.org/wiki/Software_versioning#Internal_version_numbers)
1. A release version such as a [project code name](https://en.wikipedia.org/wiki/Code_name#Project_code_name), or [semantic versioning](https://semver.org/).

### Semantic Versioning Summary, version 2.0.0

Given a version number MAJOR.MINOR.PATCH, increment the:

1. MAJOR version when you make incompatible API changes,
1. MINOR version when you add functionality in a backwards compatible manner, and
1. PATCH version when you make backwards compatible bug fixes.
Additional labels for pre-release and build metadata are available as extensions to the MAJOR.MINOR.PATCH format.

Read more about [Semantic Versioning](https://semver.org/).

## References

### Articles

- Version Control
  - [What is Version Control](https://www.atlassian.com/git/tutorials/what-is-version-control)
- Build Automation
  - TBD
- Package Dependency Management
  - [What is a Package Dependency Manager](https://blog.sonatype.com/what-is-a-package-dependency-manager)
- Unit Testing
  - TBD

### Books

- Git
  - [Pro Git](https://git-scm.com/book/en/v2) - by Scott Chacon and Ben Straub
- Unit Testing
  - Python
    - [Python Testing with pytest](https://learning.oreilly.com/library/view/python-testing-with/9781680502848/) - by Brian Okken

## Technologies

- Git
  - [Git](https://git-scm.com/)
- Version Control
  - [Version Control in VS Code](https://code.visualstudio.com/docs/editor/versioncontrol)
  - [GitLab](https://about.gitlab.com/)
  - [BitBucket](https://bitbucket.org/product)
- Build Automation / Package Managers
  - Java
    - [Gradle](https://gradle.org/)(Java)
  - JavaScript/TypeScript
    - [Node Package Manager (npm)](https://www.npmjs.com/)
  - Python
    - [pip](https://pypi.org/project/pip/)
    - [conda]
- Package Dependency Management
  - [Nexus Repository OSS](https://www.sonatype.com/nexus/repository-oss)
  - [Artifactory](https://jfrog.com/artifactory/)

## Cloud computing

From a user perspective, the cloud is thought of as 'computer systems owned by someone else, accessible over the internet.' Watch [What is the cloud? | CNBC Explains (3:00)](https://www.youtube.com/watch?v=i9x0UO8MY0g) on YouTube.

But the cloud is more than online data storage and online applications. It has a range of technologies that are changing the application and IT operations landscape.

Cloud computing technologies are grouped into different service models:

* Software as a Service (SaaS)
* Infrastructure as a Service (IaaS)
* Platform as a Service (PaaS)
* Containers as a Service (CaaS)
* Functions as a Service (FaaS).

Applications that are built to take advantage of the cloud, are called Cloud Native.

### Cloud computing service providers

Cloud platforms provide cloud computing services, like virtual machines and storage, accessed across the internet. These services can be accessed immediately, offer usage-based pricing, and have large data centres.

Major cloud providers include:

* Amazon Web Services
* Microsoft Azure
* Google Cloud Platform
* IBM Cloud

#### Private cloud

Private cloud is when you run IaaS public cloud technologies in on-premises data centres. A private cloud is not a traditional on-premise data centre.

Private clouds give you access to modern application services, like serverless computing.

Like public clouds, internal customers can provision their own virtual resources to build, test, and run applications.

#### Hybrid cloud

Hybrid cloud is a combination of public cloud platforms with private cloud technology to create a hybrid of both.

Hybrid cloud scenarios include:

* Applications in the public cloud using databases in the customers data center.
* Parallel environments in which applications can move between private and public clouds.
* Virtualised data centre workloads that replicate to the cloud during peak use.

#### Multicloud

When a single organisation uses more than one cloud platform, it's called multicloud.

### Cloud Native Computing

Cloud Native is a model of application creation and delivery. Cloud Native computing is complementary to DevOps. It fully exploits the power of cloud computing.

Cloud Native applications can be hosted in the public cloud, private cloud, or a hybrid solution.

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

Cloud Native technologies include:

* Containers
* Service meshes
* Microservices
* Immutable infrastructure
* Declarative APIs.

Cloud Native technologies support applications that run on Cloud platforms. These applications are:

* Scalable
* Resilient
* Manageable
* Observable.

Watch [Keynote: What is Cloud Native and Why Should I Care? - Alexis Richardson, CEO of Weaveworks (20:21)](https://www.youtube.com/watch?v=TKYAI19OE-c).

### Cloud Native Computing Foundation (CNCF)

The CNCF, a sub-foundation of [The Linux Foundation](https://linuxfoundation.org/), aims to support the adoption of the Cloud Native model for applications. They support the open-source development of projects that support Cloud Native computing. See the [formal definition of the CNCF](https://github.com/cncf/toc/blob/main/DEFINITION.md).

The CNCF curate and promote a list of trusted tools (paid and open-source) called the [Cloud Native Interactive Landscape](https://landscape.cncf.io/).
For organsations just starting their cloud journey, there is the [Cloud Native trail map](https://github.com/cncf/landscape/blob/master/README.md#trail-map). For insight into what other companies recommend, see the [Cloud Native End User Tech Radar](https://radar.cncf.io/).

For insight into the CNCF, watch the [Keynote: End to End: The Foundation of Doers - Priyanka Sharma, General Manager, CNCF (13:32)](https://www.youtube.com/watch?v=u71aL6aVDPg).

### Software as a Service (SaaS)

SaaS is when an application is hosted in the cloud.

Saas gives the opportunity for multi-tenant applications. Traditional arrangements involved separate instance of an application is run for each organsation, but with multi-tenancy, a single application can be shared by multiple customers. Each customer has its own data, and the application keeps the data separate and secure. Not all cloud applications use multi-tenancy.

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

There are also some risks a software vendor would need to consider before developing and delivering their application in the cloud:

* The application must demonstrate real value up-front in free trials
* Revenue can come in slower
* Multi-tenant applications could limit the ability to sell customisation services
* Could find customer resistance to using the cloud
* Could require significant business changes, for example, changes to app development, it operations, pricing, and sales.

### Infrastructure as a Service (IaaS)

IaaS provides storage and compute services on a pay-per-use basis. They offer services including:

* Highly scalable databases
* Virtual machines
* Virtual private networks
* Big data analytics
* Developer tools
* Machine learning
* Application monitoring.

### Platform as a Service (PaaS)

PaaS, designed primarily for new applications, allow you to run applications simpler, without access to the virtual machine. It takes care of a lot of the virtual machine housekeeping for you.

PaaS is faster for building and running applications than IaaS.

### Containers as a Service (CaaS)

Instead of working at the virtual machine level, with CaaS you can instead deploy and manage containers. This often uses Kubernetes.

### Functions as a Service (FaaS)

FaaS is the cloud version of serverless computing. It adds a layer of abstraction to PaaS, so you don't need to think about VMs or containers, and instead you build your applications as functions and set those functions to be triggered by certain events. FaaS can cost less, since your functions consume no IaaS resources until an event occurs, so the pay-per-use fees are lowered.

## Kubernetes

Kubernetes is a container orchestrator. For an introduction, watch [The Illustrated Children's Guide to Kubernetes (8:02)](https://www.youtube.com/watch?v=4ht22ReBjno) on YouTube.

Free training: [Introduction to Kubernetes](https://www.edx.org/course/introduction-to-kubernetes#!)
Difficulty: Beginner
Length: 4-5 weeks, 2-3 hours/week
Who It’s For: Developers and system administrators who want to get started with Kubernetes.

View and watch hundreds of [Cloud Native webinars](https://www.cncf.io/online-programs/).

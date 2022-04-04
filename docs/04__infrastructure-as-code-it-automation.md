---
title: Training 04 - Infrastructure as Code & IT Automation
date: 2020-10-09
authors: Hing-Wah.Kwok@dst.defence.gov.au, Philip.Cutler@dst.defence.gov.au
---

<!-- # Training 04 - Infrastructure as Code & IT Automation -->

> **The goal is to automate** as much of the software delivery process as possible. That means that you manage your infrastructure not by clicking around a web page or manually executing shell commands, but through code.

## References

### Articles

- [What is cloud computing? Everything you need to know now](https://www.infoworld.com/article/2683784/what-is-cloud-computing.html)
- [What is Infrastructure as Code?](https://www.hashicorp.com/resources/what-is-infrastructure-as-code)
- [What's IT automation?](https://www.redhat.com/en/topics/automation/whats-it-automation)

### Books

- [Terraform: Up & Running, 2nd Edition Book](https://learning.oreilly.com/library/view/terraform-up/9781492046899/) by Yevgeniy Brikman
- [Infrastructure as Code, 2nd Edition Book](https://learning.oreilly.com/library/view/infrastructure-as-code/9781098114664/) by Kief Morris

### Tutorials

- [Infrastructure As Code Tutorial](https://github.com/Artemmkin/infrastructure-as-code-tutorial)

## Executive summary

A DevOps practice used in conjunction with continuous delivery, infrastructure as code (IaC) lets you manage your infrastructure using source-controlled code instead of a manual process.

IaC introduces automation, replicability, reliability, and increases speed for provisioning. It reduces human error and costs.

### Overview

Infrastructure as code is an important part of DevOps. Machine-readable definition files manage and provision infrastructure, and management of that code is done with source control, like developers do with application code. If the team needs to make changes to some infrastructure configuration, they make those changes in the code.

By defining your environments in source-controlled code, you can easily replicate the environment, or see what changes were made, by whom, when.

There are continuous configuration automation tools available, that extend IaC. These tools provide visibility, efficiency, and flexibility with enterprise-level security and compliance.

Learn more:

* [What is Infrastructure as Code? by Microsoft](https://docs.microsoft.com/en-us/devops/deliver/what-is-infrastructure-as-code)
* [What is Infrastructure as Code (IaC)? by Red Hat](https://www.redhat.com/en/topics/automation/what-is-infrastructure-as-code-iac)

### Problems it attempts to solve

Managing, and administering infrastructure is traditionally a time consuming, primarily manual process. Developers could be left waiting on the manual provisioning and configuration of required infrastructure by operations staff.

Undocumented, ad-hoc changes known as configuration or environment drift can happen, and cause environments to be difficult to replicate and manage.

## Benefits of Infrastructure as Code

At a high level, infrastructure automation:

* automates configuration management
* makes your systems more stable and reliable
* makes your infrastructure processes more repeatable
* enforces consistency, eliminating environmental drift
* provides scalable and rapid server provisioning reduces costs.

More specific benefits of IaC:

- **Self-Service**
  - Most teams only have a small number of sysadmins who can access production
  - If defined as code, the entire deployment process can be automated
- **Speed and Safety**
  - If the deployment process is automated, it’ll be significantly faster, since a computer can carry out the deployment steps far faster than a person;
  - safer, since an automated process will be more consistent, more repeatable, and not prone to manual error.
- **Documentation**
  - IAC acts as documentation, allowing everyone in the organisation to understand how things work
- **Version Control**
  - Storing your IAC in version control means the entire history of your infrastructure is now captured in the commit log
- **Validation**
  - for every single change, you can perform a code review, run a suite of automated tests, and pass the code through static analysis tools, all practices that are known to significantly reduce the chance of defects
- **Reuse**
  - You can package your infrastructure into reusable modules, so that instead of doing every deployment for every product in every environment from scratch, you can build on top of known, documented, battle-tested pieces

## Categories of Infrastructure as Code Tools

### Provisioning Tools

- Used to not only create servers, but also databases, caches, load balancers, queues, monitoring, subnet configurations, firewall settings, routing rules, SSL certificates, and almost every other aspect of your infrastructure
- Examples:
  - [Terraform](https://www.terraform.io/)
  - [AWS CloudFormation](https://aws.amazon.com/cloudformation/)
  - [Azure Resource Manager](https://azure.microsoft.com/en-au/features/resource-manager/)
  - [OpenStack Heat](https://docs.openstack.org/heat/latest/)

### Configuration Management Tools

- Designed to install and manage software on existing servers
- Used to manage large numbers of remote servers
- Examples:
  - [Ansible](https://www.ansible.com/)
  - [Chef](https://www.chef.io/)
  - [Puppet](https://puppet.com/)
  - [SaltStack](https://www.saltstack.com/)
- Video Tutorials : [Ansible 101 | Jeff Geerling ](https://www.youtube.com/playlist?list=PL2_OBreMn7FqZkvMYt6ATmgC0KAGGJNAN)

### Server Templating Tools

- The idea behind server templating tools is to create an image of a server that captures a fully self-contained “snapshot” of the operating system
- Virtual Machines virtualize the hardware, whereas Containers virtualize only user space. More info: [What is a Container?](https://www.docker.com/resources/what-container)
- Virtual Machine Examples:
  - [Packer](https://www.packer.io/)
  - [Vagrant](https://www.vagrantup.com/)
- Containerisation Examples:
  - [Docker](https://www.docker.com/)
  - [Podman](https://www.podman.io/)

### Orchestration Tools

- Deploy VMs and containers, making efficient use of your hardware.
- Roll out updates to an existing fleet of VMs and containers using strategies such as **rolling deployment**, blue-green deployment, and canary deployment.
- Monitor the health of your VMs and containers and automatically replace unhealthy ones (**auto healing**).
- Scale the number of VMs and containers up or down in response to load (**auto scaling**).
- Distribute traffic across your VMs and containers (**load balancing**).
- Allow your VMs and containers to find and talk to one another over the network (**service discovery**).
- Examples:
  - [Kubernetes (K8s)](https://kubernetes.io/)
  - [Amazon ECS](https://aws.amazon.com/ecs/)
  - [Nomad](https://www.nomadproject.io/)
  - [OKD](https://www.okd.io/) - Community distribution of Kubernetes that powers [Red Hat OpenShift](https://www.openshift.com/)
  - [K3s](https://k3s.io/) - Lightweight Kubernetes
- Tutorials:
  - [Bootstrap Kubernetes the hard way on Google Cloud Platform. No scripts.](https://github.com/kelseyhightower/kubernetes-the-hard-way)

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

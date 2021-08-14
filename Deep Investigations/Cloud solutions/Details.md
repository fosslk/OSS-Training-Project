# Nextcloud

## Table of contents

- [Objective](#objective)
- [Introduction](#introduction)
    - [Why we choose](#why-we-choose)
    - [Learing outcomes](#learning-outcomes)
- [History](#history)
- [Installation](#installation)
    - [System requirements](#system-requirements)
        - [Server](#server)
        - [Desktop Client](#desktop-client)
        - [Web Application](#web-application)
    - [Prerequisites for manual installation](#prerequisites-for-manual-installation)
    - [Installation on Ubuntu 20.04 LTS](#installation-on-ubuntu-20.04-lts)
- [Features](#features)
- [FAQ](#faq)
    - [References](#references)
- [Quiz](#quiz)

## Objective

By the end of this course, you will be able to,
- Host your own collaboration platform.
- Get to know how to manage your data without using any third-party resources and thus get complete control of your organization’s data.
- Facilitate secure communication and collaboration for your organization.
- Storing files and photos, collaborating, sharing contacts and calendars within your server group. 
- Learn a security-first solution that puts you in complete control over the location and access policies of data.


##  Introduction

Nextcloud is a fully featured on-premises solution to share and collaborate documents, send and receive emails, manage all audio/video conferencing, manage contacts, manage schedules, etc. Nextcloud is scalable from home office solutions to full sized data center solutions that support millions of users.

Nextcloud permits user and group administration via [LDAP](https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol) or [OpenID](https://en.wikipedia.org/wiki/Lightweight_Directory_Access_Protocol). Content can be shared by defining granular read/write permissions between users and groups. Alternatively, Nextcloud users can create public URLs when sharing files. Logging of file-related actions and disallowing access based on file access rules are also available.

Nextcloud can be extended with plugins to add extra functionalities to the system. The **Nextcloud App store** can be found [here](https://apps.nextcloud.com/), and it contains **more than 200 plugins**. Some of the functionalities that you can add to Nextcloud are as follows.

- Calendars
- Forms
- URL shortening services
- Web analytics
- Map viewers
- Ebook viewers
- Browser-based text editors

and much more.

### Why we choose

Nextcloud is the most popular self-hosted EFSS (**E**nterprise **F**ile **S**ync and **S**hare) and Content Collaboration Platform. Hence the following features make Nextcloud the best choice among others.

- **Security**
    - Nextcloud is developed in a security-focused process. In that manner, Nextcloud provides numerous industry-leading features to ensure the security of their system, such as 2-factor authentication, machine-learning based login protection, brute-force protection, end-to-end and server-side encryption.

- **Largest ecosystem**

    - With the support of add-on integration, Nextcloud provides the largest ecosystem with the widest range of add-on capabilities to increase security, team productivity, and infrastructure features.

- **Easy to use**

    - Nextcloud is very easy to implement in a self-hosted server, hence it eliminates the headaches of system engineers in the industry. Moreover, Nextcloud provides a fully featured but not overwhelming user interface, which signifies the system’s user friendliness from the perspective of a regular user.

- **Large community support**

    - Nextcloud has broad community support in the development perspective and in a large community to answer questions that occur when using Nextcloud on a day-to-day basis. With the large community of developers, it helps to debug and improve the system in a short time as well. The community forum of Nextcloud, which is **Nextcloud Forum** could be accessed from [here](https://help.nextcloud.com/).

- **Accessibility features**
    - Nextcloud provides many accessibility features to make their services available for a broader user base, such as
        - Keyboard and screen reader navigation
        - WCAG 2.1 - compliant contrast
        - Dyslexia-friendly font

- **Free client software**
    - Nextcloud’s client apps for Android, iOS, and desktop systems allow you to manage your data easily.

### Learning outcomes

[TODO] fill me with a description

## History

__Nextcloud__ was first developed in 2016. Previously, in 2016, OwnCloud, an open-source software first developed in 2010, was released, allowing you to run a personal cloud file storage service. OwnCloud split, and many of the original developers forked the source code to create NextCloud, a competing product.

## Installation

The Nextcloud server software can be installed free of charge on Linux, and the client software can be installed on computers running Windows, OS X, or Linux. Mobile apps are also available for Android and iOS. [Check here](https://nextcloud.com/install/) for more details.

### System requirements

Here are the recommended system requirements for running an on-premises NextCloud server in your organization.

#### Server

- Operating System
    - __Ubuntu 20.04 LTS (recommended)__
    - Red Hat Enterprise Linux 8
- Database
    - __MySQL 8.0+ (recommended)__
    - MariaDB 10.2+
- Web Server
    - __Apache 2.4 with mod_php or php_fpm (recommended)__
    - Nginx with php-fpm
- PHP Runtime
    - __Version 8.0 (recommended)__
    - Version 7.4
    - Version 7.3
- Memory
    - Memory requirements for running a NextCloud server vary depending on the number of users, files and volume of server activity. Recommended minimum memory for the NextCloud server is __512MB__.

#### Desktop Client

For a better and stable experience, use the latest version of your operating system. Below are some of the tested OS versions for popular platforms.

- Windows
    - Windows 7+
- macOS
    - macOS Lion (10.7)+ (64-bit only)
- Linux
    - CentOS 6.5+
    - Ubuntu 14.04+
    - Fedora 21+
    - openSUSE 13
    - SUSE Linux Enterprise 11 SP3+
    - Debian 8 (Jessie)+
    - Red Hat Enterprise Linux 7

#### Web application

For the best experience with the web interface, use the latest and supported browser version from the following list.

- Microsoft Internet Explorer 11 (latest version)
- Microsoft Edge
- Mozilla Firefox
- Google Chrome/Chromium
- Apple Safari

Up-to-date system requirements for running a next-cloud server can be found [here](https://docs.nextcloud.com/server/latest/admin_manual/installation/system_requirements.html).

### Prerequisites for manual installation

### Installation on Ubuntu 20.04 LTS

## FAQ

1. Is Nextcloud OpenSource?
    - Yes, it is.
1. Should we share our source code that connects to Nextcloud?
    - No, since Nextcloud will communicate with your backend systems over external APIs, there is no need for your organization to share your source codes.
1. Who uses Nextcloud in Sri Lanka?
    - The Document Management System (DMS) of University of Moratuwa is running on Nextcloud.


### References

[TODO] fill me with a description

## Quiz

[TODO] fill me with a description
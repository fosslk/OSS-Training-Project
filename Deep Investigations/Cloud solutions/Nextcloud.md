# Nextcloud

## Table of contents

- [Introduction](#introduction)
    - [Why we choose](#why-we-choose)
    - [Learing Outcomes](#learning-outcomes)
- [History](#history)
- [Installation](#installation)
    - [System requirements](#system-requirements)
        - [Server](#server)
        - [Desktop Client](#desktop-client)
        - [Web Application](#web-application)
    - [Prerequisites for manual installation](#prerequisites-for-manual-installation)
    - [Apache Web server configuration](#apache-web-server-configuration)
    - [Installation on Ubuntu 20.04 LTS](#installation-on-ubuntu-20.04-lts)
- [Course Content (Demonstration Videos)](#course-content-(demonstration-videos))
- [FAQ](#faq)
- [References](#references)

##  Introduction
---

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
---

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

### Learning Outcomes
---

By the end of this course, you will be able to,
- Host your own collaboration platform.
- Get to know how to manage your data without using any third-party resources and thus get complete control of your organization’s data.
- Facilitate secure communication and collaboration for your organization.
- Storing files and photos, collaborating, sharing contacts and calendars within your server group. 
- Learn a security-first solution that puts you in complete control over the location and access policies of data.

## History
---

__Nextcloud__ was first developed in 2016. Previously, in 2016, OwnCloud, an open-source software first developed in 2010, was released, allowing you to run a personal cloud file storage service. OwnCloud split, and many of the original developers forked the source code to create NextCloud, a competing product.

## Installation
---

The Nextcloud server software can be installed free of charge on Linux, and the client software can be installed on computers running Windows, OS X, or Linux. Mobile apps are also available for Android and iOS. [Check here](https://nextcloud.com/install/) for more details.

### System requirements

Here are the recommended system requirements for running an on-premises NextCloud server in your organization.

#### **Server**

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

#### **Desktop Client**

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

#### **Web application**

For the best experience with the web interface, use the latest and supported browser version from the following list.

- Microsoft Internet Explorer 11 (latest version)
- Microsoft Edge
- Mozilla Firefox
- Google Chrome/Chromium
- Apple Safari

Up-to-date system requirements for running a next-cloud server can be found [here](https://docs.nextcloud.com/server/latest/admin_manual/installation/system_requirements.html).

### Prerequisites for manual installation
---
There are several PHP modules which are required in order to install Nextcloud on an Ubuntu server. All the required PHP modules are included in the NextCloud .tar installation archive. Refer the [Nextcloud Documentation](https://docs.nextcloud.com/server/latest/admin_manual/installation/source_installation.html#prerequisites-for-manual-installation) to find out all the required and optional PHP modules.

### Apache Web server configuration
---

We have to configure the Apache Web Server in order to have pretty URLs, enable SSL, use the directory-based installation and virtual installation. Hence, we have to edit the nextcloud.conf file and configure the Apache server.

Follow [this guide](https://docs.nextcloud.com/server/latest/admin_manual/installation/source_installation.html#apache-web-server-configuration) to make the above mentioned changes. After completing all the required prerequisites and configuring the Apache web server you are ready to install Nextcloud on Ubuntu.

### Installation on Ubuntu 20.04 LTS
---

1. Download the latest installation script.
1. Run the script with:
```
sudo bash nextcloud_install_production.sh
```
After installing Nextcloud files, the last step to complete the installation is running the Installation Wizard.

1. Point your web browser to http://localhost/nextcloud
1. Enter your desired administrator’s username and password.
1. Click **Finish Setup**

### Course Content (Demonstration Videos)

This section contains all videos that we are going to produce under each section. Please note that these videos can be a one video or multiple videos for the relevant section based on the video duration of each sections and subsections.

1. Introduction
    - What **E**nterprise **F**ile **S**ync and **S**hare (EFSS) system.
    - What is Nextcloud
    - History of Nextcloud
    - Importance of Nextcloud
1. Ready for Nextcloud Installation
    - Prerequsite PHP modules
    - Apache web server configuration
    - Installation methods
1. Nextcloud Installation
    - Install Nextcloud on Ubuntu server using **Intallation script**
    - Nextcloud Initial configurations
    - Configure Nextcloud further
        - Configure Data directory location
        - Configure Database
        - Configure Trusted domains
1. Essential Plugin Installtion for Nextcloud
    - Calendars
    - Tasks
    - Forms
    - Ebook viewers
    - Browser-based text editors
    - Annoucement Center
    - Talk (Chat, video & audio-conferencing using WebRTC)

## FAQ
---

1. Is Nextcloud OpenSource?
    - Yes, it is.
1. Should we share our source code that connects to Nextcloud?
    - No, since Nextcloud will communicate with your backend systems over external APIs, there is no need for your organization to share your source codes.
1. Who uses Nextcloud in Sri Lanka?
    - The Document Management System (DMS) of University of Moratuwa is running on Nextcloud.


## References
---

- [Nextcloud official website](https://nextcloud.com)
- [Nextcloud forums](https://nextcloud.com)
- [Nextcloud documentation](https://docs.nextcloud.com)

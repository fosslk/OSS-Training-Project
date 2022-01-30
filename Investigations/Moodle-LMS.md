Moodle Learning Management System

## Introduction

* Moodle also known as (Modular Object-Oriented Dynamic Learning Environment) is a free and open source online Learning Management System that allows instructors to establish their own private website with dynamic courses that allow students to learn at their own pace, anywhere at any time.
 
* Since Moodle is one of the top open source Learning Management Systems available in the world most of the higher education institutions use it as their main eLearning platform. Moodle is written in PHP and distributed under the GNU General Public Licence.
 
* Moodle is developed on pedagogical principles. So that it can be used not only at universities and higher education institutions but also for blended learning, distance learning, flipped classrooms, etc.




=> History

* Martin Dougiamas designed the Moodle platform while pursuing a postgraduate degree at Curtin University of Technology in Australia. In 2002, he worked as a university Webmaster and a system administrator for the WebCT installation. He began developing Moodle in order to fix some issues with WebCT. 

* The original version of the Moodle was intended for small classrooms and a case study, but later since it was developed as an open source platform, many developers and other volunteers from all around the world progressively added new features making it one of the most popular free and open source Learning Management Systems in the world.




=> Main features 

* Moodle's worldwide numbers of more than 213 million users across both academic and enterprise level usage makes it the world's most widely used open source learning management platform. It’s major features are as follows ;

-> Open source.
-> Accessible for all.
-> Security & privacy.
-> Flexible learning.
-> Mobile learning.
-> Easy integration.    
-> Multi language support.
-> Much effective collaborative tools.
-> User-friendly ecosystem.
-> Inbuilt notifications and plugin management.
-> Online Portal and Quiz wizard.
-> Course material management.
-> Availability of course design structures.
-> Availability of calendars.




=> Advantages of the Moodle Learning Management System

* Moodle allows for many different types of content formats to be uploaded and available for use by the students and the instructor. 

* Moodle not only allows for learning to be done online or at a distance but also it allows for resources to be available to students who are in instructor-led classes.
 
* Moodle also has different options and tools available for use. Moodle allows for communication to happen between the instructor and students and students can also communicate with each other. Communication in Moodle ranges from forums, blogs, chats and messages among the individuals who are enrolled within a course.

* Further Moodle also has some additional plus points. Since it’s an open source learning management system it’s widely available and it has loads of features and content available which are familiar and customizable which makes it a user-friendly and effective learning man.




=> Disadvantages of the Moodle Learning Management System

* Even though the system has some advantages and is respected by a few institutions, there are a few problems and cons. This is, of course, because nothing can be perfect.

* The first big issue is the fact that Moodle is not fully developed to cope with big projects. While it may be useful for colleges or universities of small to medium size, the system might not work efficiently with larger schools or serve as a great way to conduct all classes in a city.

* The latter example is more hypothetical than factual, but if a Board of Education were to experiment with such an idea, Moodle may not be the wisest choice. Along these same lines, the more students that access the platform, the slower the system becomes. This can be troublesome for students when they are trying to take quizzes or tests, or just simply trying to access the course content. The website can also shut down on occasion, blocking the opportunity for students to access course materials.

* In addition to the lack of complete development, Moodle users frequently complain about the troubles they experience with customization. In order to perform efficient customization, you are going to need to know how to program and have some type of knowledge when it comes to coding.




=> Pricing of the Moodle Learning Management System

* Since Moodle is provided freely as Open Source software, under the GNU General Public Licence, anyone can adapt, extend or modify Moodle for both commercial and non-commercial projects without any licensing fees and benefit from the cost-efficiencies, flexibility and other advantages of using Moodle.

* Pricing of the Moodle Learning Management System is based on the number of users and file storage.

Accordingly subscription plans are as follows:

** Free plan $0 ( upto 50 users, 200MB of storage)
** Starter plan $80/year (50 users, 200MB) with some add-on features.
** Moodle for Educational institutions plans are of three types and they are as follows:
                                                                                         Mini: $250/year (100 users, 200MB)
                                                                                         Small: $500/year (200 users, 400MB) 
                                                                                         Medium: $1,000/month (500 users, 1GB)




=> Installation guide of the Moodle Learning Management System

Basic Requirements

* You will need a working web server (e.g. Apache), a database (e.g. MySQL, MariaDB or PostgreSQL) and have PHP configured. See the release notes in the dev docs for software requirements.
* Moodle requires a number of PHP extensions. However, Moodle checks early in the installation process and you can fix the problem and restart the install script if any are missing.
* If you want Moodle to send email (you probably do) you need a working Sendmail (Unix/Linux) on your server or access to an SMTP mail server.



1) Getting Moodle

You have two basic options:
Download your required version from https://download.moodle.org/ ... OR
Pull the code from the Git repository (recommended for developers and also makes upgrading very simple):
git clone -b MOODLE_310_STABLE git://git.moodle.org/moodle.git 

(this fetches a complete copy of the Moodle repository and then switches to the 3.11 Stable branch.)
Note: Only download Moodle from one of the moodle.org sources. Other versions (e.g. control panel based installers, Linux distribution repositories, other "one click" installers) cannot be guaranteed to work properly, be upgradable or be supportable.



2) Create a database

Using your chosen database server, create a new empty database. The default encoding must be UTF8. 
For example, using MySQL:
CREATE DATABASE moodle DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;

Create a user/password combination with appropriate permissions for the database. 
For example (MySQL again):
mysql> GRANT SELECT,INSERT,UPDATE,DELETE,CREATE,CREATE TEMPORARY TABLES,DROP,INDEX,ALTER ON moodle.* TO 'moodleuser'@'localhost' IDENTIFIED BY 'yourpassword';

Notes: It is important to GRANT ON moodle.* as the database name including the '.*' and not just the bare database name. Save this password you use for the Moodle user, since you will need it later in the install.
Create data directory
Create an empty directory to hold Moodle files. It must not be in the area served by the web server and must have permissions so that the web server user can write to it. Other than that it can be located anywhere. Typically, either make it owned by the web server user or give it write permissions for 'everyone'. If it is on a shared/NFS drive then read Caching - Moodle caches to this disk area by default and a slow share will mean terrible performance.



3) Install Moodle code

If you downloaded the zip or tgz file earlier, then unzip / untar / move / copy the Moodle code (obtained above) so that it will be served by your web server (e.g. on Debian based Linux, move to /var/www/html/moodle)
Check the permissions and make sure that the web server does not have permissions to write to any of the files in the Moodle code directories (a very common root cause of sites being hacked).
If you need to, configure your web server to serve the Moodle site with your chosen URL.
Configure Moodle
In the Moodle code directory, find the file config-dist.php and copy it to a new file called config.php (but read the next step, 'Install Moodle', first).
Edit config.php with your favourite editor and change the appropriate settings to point to your site, directories and database. 
Note: the Moodle install script will create config.php for you if it does not exist but make sure you (re-)set permissions appropriately afterwards.



4) Install Moodle

Go to the URL for your moodle site in a browser (installation will complete automatically) or run the command line version at (requires cli version of PHP):
/usr/bin/php /path/to/moodle/admin/cli/install.php
 
The CLI creates the config.php for you and will not run if you created one in the previous step.
After completing the install make sure your file permissions are ok for the Moodle program files (not writeable by web server) and the Moodle data files (writeable by web server).
Set up cron
You will need a cron job to run periodically. It is recommended that the cron is run every minute, as required for asynchronous activity deletion when using the recycle bin. A typical Unix cron entry will be as follows:
* * * * *    /usr/bin/php /path/to/moodle/admin/cli/cron.php >/dev/null

Your site will not work properly unless cron is running regularly. It is very important you do not skip this step.
 


Congratulations!
You are now ready to use your Moodle site. 
If you run into problems, check the Installation FAQ and visit the Installation help forum.


=================================================================================================================================================================================

(University : ICBT Kandy Campus)

Contributors : => Poojith Obeysekara
               => Deshan Wickramaarachchi
               => Bishmi Dissanayake



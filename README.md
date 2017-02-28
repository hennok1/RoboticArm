F.I.M.P. Project
================

Project members: Tanav Sharma, Alay Lad, Hennok Tadeese

 

Declaration of Joint Authorship
===============================

The F.I.M.P. robotic arm project consist of three group members (Hennok Tadesse,
Tanav Sharma, and Alay Lad) and is a joint effort on the completion of the
project. The work for the project has been divided equally among the group members.
Alay Lad has worked on the hardware aspect of the project; which includes working
with the flex sensors, creating the PCB’s, and working with the servo motors for
the robotic arm. Hennok Tadesse has worked on the design and functionality of
the mobile application. Tanav Sharma has worked on the database in terms of setting it
up, connecting it with the app and maintaining it. Testing and maintenance for
the hardware and software has been tested by all three members equally and all
project updates and changes have been checked and approved by all members.

Approved Proposal
=================

September, 2016

*Proposal for the development of FIMP*

Prepared by Tanav, Alay, and Hennok  
*Computer Engineering Technology Student*  
github.com/hennok129/RoboticArm

**Executive Summary**

As a student in the Computer Engineering Technology program, I will be
integrating the knowledge and skills I have learned from our program into this
Internet of Things themed capstone project. This proposal requests the approval
to build the software app that will connect to a hardware as well as to a mobile
device application. In the app, we will have incorporated a controller that will
be used to control the hardware. The database will store the coordinates of the
robot arm and the angles that the motor and arms need to be when it returns to
rest position. The mobile device functionality will include some very basic test
functions and commands to move the arm. It will create logs and save that data,
so the developer can later look it at and make improvements to the hardware or
software and other users can use these logs to reproduce experiments. In the
winter semester I plan to form a group with the following students (Alay Lad,
Hennok Tadesse, and Tanav Sharma), who are also making similar app this term and
working on the mobile application with Tanav Sharma, Alay Lad, and Hennok
Tadesse. The hardware will be completed in CENG 317 Hardware Production
Techniques independently and the application will be completed in CENG 319
Software Project. These will be integrated together in the subsequent term in
CENG 355 Computer Systems Project as a member of a 2 or 3 student group.

**Background**

This project will solve many problems. Along with solving problems it will also
be very innovative. It will help gamers with better precision, and interact with
games. Scientists and engineers can use this arm, for experiments where they
need to have certain amount of distance clearance from the test site. The app 
will be saving information received from the arm, and provide logs, 
so the user can use it to make his/her reports and also use the information
to make changes to better the app or hardware.

Abstract
========
The purpose of the fully innovated microprocessor (F.I.M.P.) project is to use
and control robotic arm equipment from a safer environment to lower the risk of
work place injuries. The technical report will go over the way the Fully
Innovated Micro Processor(F.I.M.P.) robotic arm project works and the main
components and features of the project. Components such as the flex sensors,
mobile app, and the robotic arm will all be explained in great detail. The four
flex sensors will be attached to a glove that will control the robotic arm with
pressure from the user’s fingers. The mobile app will also be used to control
the robotic arm but with four sliding bars instead of a sensor. The mobile app
will include features such as allowing the user to record logs. The robotic arm 
will consist of acrylic parts and four micro servo motors that move each joint 
of the robotic arm. The robotic arm is then connected to a Raspberry Pi 3 that 
will be the middle point that will control the robotic arm whether its from the 
flex sensors or the mobile app. These three key components are the main focus of
the technical report because it will go over the basic workings of the project 
and give users the full understanding of this project.

Table of Contents
=================

[Declaration of Joint Authorship](#_Toc473019556)

[Approved Proposal](#_Toc473019557)

[Abstract](#_Toc473019558)

[1. Introduction.](#_Toc473019559)

[1.1 Technical Problem](#_Toc473019560)

[1.2 The Why](#_Toc473019561)

[1.3 Problems Encountered](#_Toc473019563)

[2. Project Description](#_Toc473019564)

[2.1 Problem](#_Toc473019565)

[2.2 Rationale behind Project](#_Toc473019566)

[2.3 Project Scope](#_Toc473019567)

[2.4 Software Requirement Specifications](#_Toc473019568)

[2.4.1 Database Breakdown](#_Toc473019569)

[2.4.2 Application Breakdown](#_Toc473019570)

[2.4.3 Hardware Breakdown](#_Toc473019571)

[3. Content](#_Toc473019572)

[4. Bibliography](#_Toc473019573)

[5. Appendices](#_Toc473019574)

1.  References

 

 

1. Introduction
===============

1.1 Technical Problem
---------------------

>   We have innovated technology to great measures and even till this day,
>   inventors and innovators continue to improve our lives with technology.
>   Jobs such as an Aircraft Engineer or a Power line Technician put their lives 
>   at risk, by working up-close dangerous moving parts and high amounts of voltage. 
>   Due to these dangers, employees' are getting injured at the workplace. With the help
>   of Robotic Arm, we aim to prevent these injuries from happening.

1.2 The Why
-----------

>   This project was undertaken because using a robotic arm that can be
>   controlled via mobile app or with a glove, prevents from injury/death as it
>   allows the technicians to work from a safe distance. It also allows them to
>   have similar precision as they would have had when they were actually there.

1.3 Problems Encountered
------------------------

>   There were many problems we encountered while working on this project. Some
>   of these issues involved us burning our motors due to incorrect voltages
>   applied. Our main problem came was when we attempted to connect the app and
>   hardware. We also had issues with allowing the Raspberry Pi connect to an
>   enterprise network, but this issue was resolved by running a simple bash
>   program.

 

 

2. Project Description
======================

2.1 Problem
-----------

2.2 Rationale behind Project
----------------------------

2.3 Project Scope
-----------------

2.4 Software Requirement Specifications
---------------------------------------

### 2.4.1 Database Breakdown

There will be a Amazon Database; a service provided by Amazon. When creating
an account with Amazone Web Server, I need to create a php file for the register 
activity. I also need to create one file for the login activity. To connect the app
to the database, I created a "init.php" file. This file is in charge for establishing 
connection to the database. All of these files are in-charge of the backend process of
the database. This database will be responsible for holding user account information,
for example user credentials for the login/register function. This database will also
contain many tables under the user account as the user will able to create multiple
logs with in a day and each log will be stored in its own table. The breakdown of the
fields is stated below.

1.  **User Account**

    1.  This table is generated when the user registers

    2.  It holds the users first name, last name, username as well as the password.

        When registering, if an username already exists on the database, it
        will advise the user that “User already exists”. When logging in, if the user
        enters wrong credentials, it will advise the user “Wrong Credentials”

2.  **Logs**

    1.  This table is generated under the users account and is linked with user
        unique id.

    2.  This table is generated when user launches the controller function in
        the app, and is asked if they would like to start a log.

    3.  It creates the table with title of the current date and time on the
        system and stores the motors start and end coordinates for each of the four
        motor.

    4.  User will able to create multiple logs with in a day.

The purpose of the database is mainly to allow the user to create a personal
account, and to allow other users to access logs from other users. Creating a
table with the date and time, under the user’s unique id, will inform others
whose logs are being accessed from which date and time. The administrator may
choose to restrict certain logs to certain user and/or departments.

These logs can be used for research/development reasons only, which is stated in
the Terms and Condition document provided with the product and also displayed to
the user when launching the app.

(Developed by Tanav Sharma)

### 2.4.2 Application Breakdown

The overall concept of the mobile app for the project is to control the four
servo motors of the robotic arm and keep logs on the user’s actions. The first
screen of the app will be the login screen which will require an email and
password to create and login to an account. The accounts are used to hold
individual logs of the user’s controller usage. When logged in, the user is
presented with two option; controller and user logs.

The first option of the application is to control the motor with four sliders
that will control the arms movements. When the application first begins, the
sliders will be set to a default (centered) position. When exiting the
application, the robotic arm will return to its default position after all
created movements.

During the controller screen, the application will have logs of the user’s usage
and will be presented in the user log screen. The user logs will contain the log
of all the users usage of the app based on the users in the database. In
conclusion, the login screen, controller screen, and user logs are the three key
features of the application. The key developer of this application will be
Hennok Tadesse with some help from Tanav Sharma.

(Developed by Hennok Tadesse)

### 2.4.3 Hardware Breakdown

**ROBOTIC ARM**

FIMP project aims to bring a simple Robot Arm well within the reach and budget
of the average educator, student, parent or child. The design brief we set out
with was to build a full robot arm kit with standard low cost screws, low cost
servo motors and using less than 300 x 200mm (\~A4) of acrylic

**MCP3008**

In order to measure the X and Y voltages I decided to use an MCP3008 10 bit
Analogue to Digital Converter. These devices are cheap, easy to setup and allow
8 analogue inputs to be read by the Pi using its SPI interface.

**Adafruit 16-Channel PWM**

The Raspberry Pi is a wonderful little computer, but one thing it isn't very
good at is controlling DC Servo Motors - these motors need very specific and
repetitive timing pulses to set the position. Instead of asking the Pi Linux
kernel to send these signals, pop on this handy HAT! It adds the capability to
control 16 Servos with perfect timing. It can also do PWM up to 1.6 KHz with 12
bit precision, all completely free-running.

**Flex Sensor 4.5**

A simple flex sensor 4.5" in length. As the sensor is flexed, the resistance
across the sensor increases. Patented technology by Spectra Symbol - they claim
these sensors were used in the original Nintendo Power Glove.

The resistance of the flex sensor changes when the metal pads are on the outside
of the bend.

Content
=======

Bibliography
============

Appendices
==========

References
==========

<div align="center">

# Using Septentrio's Receiver and Topcon TopNet live correction services for precise positioning

## GENERAL CONTEXT OF THIS GUIDE

GNSS (Global Navigation Satellite System) technology has changed the way we navigate and position ourselves, with applications in various industries including transportation, surveying and agriculture. However, atmospheric conditions and signal blockages can affect the accuracy of GNSS location information. 

GNSS corrections are used to mitigate these effects and improve the accuracy of position measurements. In recent years, there has been a growing demand for high-accuracy positioning, which has led to the evolution of GNSS correction mechanisms such as OSR, SSR or LBand delivery. Standardization is not yet established, making it challenging for users to access and use these corrections. 

To address this challenge, it is useful to create an ecosystem around GNSS corrections that is agnostic. This repository is part of a set of guides and documentation and explores a way of running Topcon's TopNet Live corrections on your system quickly. Making it easy for users/integrators to evaluate and access these service. Platforms like Github enable documentation and the creation of demonstrators to allow users to try out different correction services with ease.

| <a href="https://github.com/septentrio-gnss/SeptentrioAgnostic#set-up-guide-to-use-third-party-osr-and-ssr-correction-services-with-septentrios-receivers-for-precise-positioning">To access the GitHub homepage to which this guide belongs, click here</a>|
|---|

## MAINTAINER
  
| GitHub |
|--------|
| <a href="https://github.com/septentrio-users">septentrio-users</a> </br> |    

## DO YOU HAVE ANY QUESTIONS? CONTACT SEPTENTRIO SUPPORT TEAM

| <a href="https://web.septentrio.com/GH-SSN-support ">Septentrio Support Page</a>|
|---|

## SEPTENTRIO LINKS FOR USERS
 
| Contact                                                                          | Septentrio Home Page                                                        |
|----------------------------------------------------------------------------------|-----------------------------------------------------------------------------|
| <a href="https://web.septentrio.com/GH-SSN-contact ">Septentrio Contact Page</a> | <a href="https://web.septentrio.com/POI-SSN-home">Septentrio Home Page</a> |

## DISCLAIMER
  
This set of guidelines consist of a several practical examplse to help Septentrio Module users and developers to integrate third party GNSS corrections. The guidelines are based on a concrete setup, which you may or may not use to follow the integration guidelines.

It is desirable to mention the disclaimer about that setup and the guides in general before starting reading this guide.
  
| <a href="https://github.com/septentrio-gnss/SeptentrioAgnostic/tree/main/Receiver%20and%20Raspberry%20Setup#disclaimer">Click here to know more about the Setup in which these guides are based and general implementation documentation disclaimer</a> |
|---|

</div>

## TABLE OF CONTENTS

<!--ts-->

* [Introduction](#introduction)
* [Who is Topcon?](#who-is-topcon-navigation)
* [Is the project Open Source?](#is-the-project-open-source)
* [Receiver and Raspberry Pi 4 Setup](#receiver-and-raspberry-pi-4-setup)
* [OSR Corrections Implementation](#osr-corrections-implementation)

<!--te-->

## INTRODUCTION

This repository consists in a how-to guide for the implementation of a system that uses a Raspberry Pi 4 Model B in combination with a Septentrio Module to obtain Topcon's TopNet live corrections for precise positioning. If you want to know more about the different Septentrio modules and products you can visit the following link: 

<div align="center">

| <a href="https://web.septentrio.com/TOP-SSN-RX">Click here to the access to the all Septentrio GNSS Modules page.</a> |
|---|
   
</div>

The connection to Topcon's TopNET live can be done via **NTRIP protocol**.

<div align="center">

| <a href="https://pointonenav.com/docs/">Click here to the navigate to Polaris Examples, tutorials, datasheets and API references.</a> |
|---|
   
</div>

If you have any questions or feedback, please don't hesitate to reach out to <a href="https://web.septentrio.com/GH-SSN-support ">Septentrio support page.</a>

## WHO IS TOPCON?

<p align="center">
    <img src="doc_resources/topcon_logo.png" width="50%">

Topcon Corporation is a Japanese multinational company that specializes in the design and manufacture of optical, surveying, and geolocation equipment. The company was founded in 1932 and is headquartered in Tokyo, Japan. Topcon's products and services are used in various industries, including construction, agriculture, healthcare, and geospatial applications. 

TopNET Live is a real-time GNSS (Global Navigation Satellite System) correction service offered by Topcon Positioning Systems, a division of Topcon Corporation. TopNET Live is designed to provide high-precision positioning data to GNSS users in various industries, including surveying, construction, agriculture, and more.

<div align="center">
   
| <a href="https://topcon.com">Click here to navigate to Topcon's official web page.</a> |
|---|
      
</div>

## IS THE PROJECT OPEN SOURCE?

This implementation guide for the Topcon TopNET live correction services offered by Topcon is open-source. That is, this repository does not contain any code created or modified by us, but is a guide to using the their code/repository to use their correction services with Septentrio receivers. Therefore, this guide could be modified thanks to the feedback of the users who use it, so you are welcome to leave us your opinion or suggestions for improvement.

## RECEIVER AND RASPBERRY PI 4 SETUP
While NTRIP is embedded in Septentrio receivers, some customers might want to run these corrections on their own CPU.  
On top of NTRIP in the receiver the implementation of this service is based and tested on a specific setup.
This setup consists of two main elements and their wiring and peripherals. These elements are the Mosaic-Go Module evaluation kit and a Raspberry Pi 4 Model B. 

<div align="center">
    
| <a href="https://github.com/septentrio-gnss/Septentrio_AgnosticCorrectionsProgram#set-up-guide-to-use-third-party-osr-and-ssr-corrections-with-septentrios-receivers-for-precise-positioning"> Click here to acces to the Set Up Guide to use Third Party OSR and SSR correction services with Septentrio's Receivers for precise positioning.</a> |
|---|
    
</div>

It is necessary to follow the instructions of the previous setup installation guide, to return to this point for the implementation of the Topcon's Topnet live corrections service.

## OSR Corrections Implementation

To implement OSR Corrections (RTK) in the setup mentioned previously, check the following guide called: 

<div align="center">

| <a href="https://github.com/septentrio-gnss/TopconCorrectionsWithSeptentrio/tree/master/osr#using-septentrios-receiver-and-topcon-osr-corrections-for-precise-positioning">Using Septentrio's Receiver and Topcon's OSR (RTK) corrections for precise positioning.</a> |
|---|

   
</div>

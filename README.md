# PLC_programming

## Motivation
PLC is the core of modern industrial control.  
It's not just used in manufacturing lines but also in power plants as part of SCADA systems or even in industrial robots.  
There is a reason some of top robotics companies such as ABB, Mitsubishi, Omron are PLC manufacturers, too.  

## Advantage/Disadvantage of PLC
PLC has some advantages and disadvantages comparing to Arduino, a famous DIY controller, or even using a PC as a controller.  
Advantages:  
1. Industrial grade (durable, milli-second level response, higher endurance against dust, temperature and continuous use, longevity, etc)  
2. Easier maintenance  
3. Built-in debug/diagnosis  

Disadvantage:  
1. Expensive - cheaper ones cost about $$$ (without software license), usually a few thousands to tens of thousands.  
2. Entry-barrier - requires electrical knowledge  
3. Limited data processing capacity - may not be suitable to handle data for DL/ML  
4. Lack of version control

## PLC Device Selection: Allen Bradley (AB) MicroLogix 1100
Good video explaning 3 popular big PLC brands around the world.
[![IMAGE](http://img.youtube.com/vi/Nsx-LTd2IXM/0.jpg)](https://youtu.be/Nsx-LTd2IXM)  

AB from Rockwell Automation is the most popular PLC brand in U.S. Even our team at work use AB PLC.  
This is one of the reasons I chose AB PLC even though there are cheaper models from another brand.  

There is actually cheaper AB PLC models from AB, Micro PLC's although not mentioned in the video.
The problem of Micro models is its software - CCW (Connected Components Workbench).  
It's totally different from standard PLC Logix software - RsLogix 5000 and 500 (tone down version of 5000).  

On the other hand, regular RsLogix software is very expensive for personal try, around a thousand of USD.  

Here is the download/install instruction for free RSLogix 500 Lite for MicroLogix 1100.
https://www.theautomationstore.com/rslogix-500-training-downloading-and-installing-rslogix-500-and-rslinx-for-free/


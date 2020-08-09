# PLC_programming

## Motivation
PLC is the core of modern industrial control.  
It's not just used in manufacturing lines but also in power plants as part of SCADA systems or even in industrial robots.  
There is a reason some of top robotics companies such as ABB, Mitsubishi, Omron are PLC manufacturers, too.  

## Advantage/Disadvantage of PLC
In summary,  
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

--

Using a PLC is common practice only in industrial robotics, not common in other robotics projects for several reasons.  

For example, controller for automotive or aerospace (NASA rovers) often requires higher standard than what PLC can deliver  
– micro-second response vs milli-second PLC response, heat endurance near the hot engine (some PLC’s have higher heat endurance though),  
radiation exposure from the outer space, etc. In addition, it might not be an economical choice when there is a high manufacturing volume  
like vehicle models. It’s simply much cheaper to develop a PCB from scratch.

On the other hand, robotics projects in a much less sensitive environment such as a research lab in some university,  
where only the proof of concept had to show, likely wants to do latest, advanced perception such as ML/DL rather than reliable,  
industrial grade control. However, PLC inherently has very small memory/storage size, not suitable for such advanced perception  
that requires massive data. PLC is only good for control, but a robot needs both perception and control.  
These projects are usually very budget limited, expensive PLC is likely not an option.

Another entry barrier is the PLC programming knowledge itself. There is a technological blind spot inherent to PLC.  
Learning PLC requires certain level of multi-disciplinary knowledge in both electrical circuitry and programming.  
PLC knowledge is more abundant in industrial automation (Electrical Engineering dept.) than robotics field (Computer Engineering/Science dept.).  
But at the same time, PLC is something that has developed for a few decades just like any other programming languages  
(history of PLC & ladder logic is older than C++), and it takes years of learning and experience to master it.  
This often prevents researchers to try PLC from the first place. 


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


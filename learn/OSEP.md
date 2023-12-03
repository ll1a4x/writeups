# My OSEP Learning and Exam Experiences

---

- [My OSEP Learning and Exam Experiences](#my-osep-learning-and-exam-experiences)
	- [Introduction](#introduction)
	- [The Learning Environment](#the-learning-environment)
	- [The Exam](#the-exam)
	- [Conclusion](#conclusion)


---
## Introduction

OSEP (Offensive Security Experienced Penetration Tester), aka PEN-300, is a directly follow-up of OSCP(PEN-200). Other than standalone machines and a small AD environment without strong defenses enabled in OSCP exam, the OSEP exam concentrates on bypassing the common defenses such as Windows Defender, AVs, Powershell AMSI, Application Whitelisiting, Network Filters, and so on in a simulated corporate network. This course also teaches how to write the customized C# code, Powershell payload, and VB macros with techniques like process injection, DLL injection, process hollowing, and so on. OSEP is completely based on the Active Directory that contains both Windows and Linux machines. Active Directory knowledge has very a heavy weight in OSEP. Please refer to the official high-level intro in this link: https://www.offsec.com/courses/pen-300/

I have passed OSCP last year and I'm curious and hungry to learn new knowledge in OSEP. So, I registered this course. I don't think OSCP certification is a hard prerequisite for OSEP at this time. But it's highly recommended to have OSCP passed or the equivalent knowledge/experience before taking the OSEP exam.


---
## The Learning Environment

The course materials are awesome to explain the concepts in details. But you still have to actually do it on your own to learn. It's highly recommended to complete all course exercises including the extra mile exercises before taking the exam. Understanding the course materials is the foundation of passing the exam.

OffSec has a great community to support the students learning experiences. I learned something new that's not in the course materials in the OffSec discord channel. If you have any questions or issues like the network connection, don't hesitate to reach out OffSec support team in Discord or by emails.

There are 6 challenging labs. Challenge 1-4 are specifically for some particular topics in the course materials. The complexity of Challenge 5 and 6 is very alike the real exam. Highly recommend to complete these challenges after completing course materials and before taking the exam. You may go over them for multiple times and applied varied techs to achieve the same goals. Remember, the more techs you know, the higher chance to pass the exam. This is called Offense-In-Depth, which is a mindset to fight against Defense-In-Depth.

After you have done completely the course materials and the lab challenges, it's also highly recommended to do your own additional research to learn the latest techs of bypassing defense mechanisms relevant with the course content. OffSec emphasizes the "Out-of-Box" thinking. In order to have the "Out-of-Box" thinking, you really have to extend what you have already learned to handle with the new challenges.


---
## The Exam

This is a challenging exam even for experienced penetration testers. 

Before the exam, it's highly recommended to read the OSEP Exam Guide here: https://help.offsec.com/hc/en-us/articles/360050293792-OSEP-Exam-Guide. Make sure you prepare well for the logistics for the exam. The exam is 47 hours and 45 minutes, which is basically twice time of OSCP. Good time management and taking regular breaks are the key to the success.

OSEP Exam has very restricted requirements to pass it. The most noticeable requirement is that opening a cmd prompt or powershell window to print the flag on the RDP session does NOT count as a valid proof. Before taking the exam, I sent the email to confirm this with the support team. This is different from OSCP Exam. So, this means even if you have a RDP session, you still have to invoke a remote interactive shell of the target machine in kali and then print the content of the flag along with the IP of the target. You also need the screenshot for it. We may still use the RDP session as the means to achieve the goal. But, we must have the `remote interactive shell` of the targets in kali.

Other requirements in the exam report are listed in the Exam Guide link above. Passing or failing is based on the submitted Exam report and partial points may be granted. So, please read the Exam Guide carefully and contact OffSec support team if you have any questions.

The overall exam process is very smooth and thanks to the support of the exam proctors. However, I did struggle in the halfway of the exam. I thought I could fail for a couple of times because I was far behind the progress to complete all requirements after 32/48 hours were gone. Good thing was that I took regular breaks and did not give up. At a moment latter, I suddenly thought differently to discover a new angle of breaking the wall. After that, everything was getting much easier. I was able to complete the requirements to pass the Exam after 38/48 hours were gone. Next, I took a break after reverting the machines (it's taking some time to get all of them ready). Then, I came back to reproduce what I have done, organize my notes for writing the report, and take screenshots. 

Just prior to 30 minutes of ending the exam, I claimed to terminate it early. I took a break first and came back to write the initial report with my notes and screenshots. After some good sleeping, I reviewed and proofread my initial report to fix typos and the unclear description. I submitted the report just 2 hours before the deadline of the report submission.

Finally, I received the official email to claim that I passed the OSEP Exam at the time around 38 hours after I submitted the exam report. Thanks for the quick notification, OffSec! So, I won't get too nervous over the Weekend!


---
## Conclusion

After passing the OSEP exam, I become more confident for penetrating the AD environment with the hardening mechanisms. The ideas, methodology, and mindset in OSEP are greatly helping my career as a penetration tester!

My primary motivation is having fun and learning new things. This is an absolute fun experience to learn something new for my penetration career! I will continue the other 300 level courses in my learning journeys.


Lynden L.  
Dec 3, 2023

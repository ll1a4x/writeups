# My OSCP Journey

---
## Table Of Contents
- [Introduction](#introduction)
	- [About This Writeup](#about-this-writeup)
	- [About Me](#about-me)
	- [Why I Began The OSCP Journey?](#why-i-began-the-oscp-journey)
- [How I Prepared For OSCP?](#how-i-prepared-for-oscp)
- [Timeline](#timeline)
- [The 1st Attempt - Almost Passed](#the-1st-attempt---almost-passed)
	- [Reschedule The Exam ](#reschedule-the-exam)
	- [Three Mistakes](#three-mistakes)
	- [The End](#the-end)
- [The 2nd Attempt - Passed With High Confidence](#the-2nd-attempt---passed-with-high-confidence)
	- [Fix Logistics Issues](#fix-logistics-issues)
	- [Try Harder And Try Others](#try-harder-and-try-others)
	- [Critical Moment](#critical-moment)
	- [Exam Report](#exam-report)
	- [Result](#result)
- [Conclusion](#conclusion)
	- [Personal Feelings](#personal-feelings)
	- [Personal Suggestions](#personal-suggestions)
	- [To Be Continued...](#to-be-continued)

---
## Introduction

### About This Writeup

This writeup is all about the learning experiences of passing OSCP (Offensive Security Certified Professional) certificate by Lynden (github: https://github.com/ll1a4x/). This writeup won't show everything about OSCP, especially those official information like the OSCP exam format/registration, etc. Please go to OSCP's official website for the complete and accurate information and instructions. This writeup may or may not be beneficial for those who are studying for OSCP. After all, different people have different ways of studying. But, hopefully, this writeup may give the readers some new ideas for their own learning journeys for OSCP or other learning in information security.

### About Me

- Enthusiasm/curiosity about information security. Especially, the offensive security is what I truly love to do.
- Growth mindset for learning security. I enjoy learning new ideas/concepts/tricks/methodologies.
- Resilience/fortitude to overcome obstacles in the learning journey.
- Education: Bachelor degree in Mathematics; Master degree in Computer Science (I was studying OSCP during the last 2 quarters of completing Master degree.)
- Certifications before OSCP: CompTIA Security+ and Mile2 Certified Penetration Testing Engineer
- Work experiences: 4 years of radio/satellite communication equipment maintainer in the US Air Force; AND a summer internship in the blue team of a financial company.

### Why I Began The OSCP Journey?

When I was a remote intern working in the blue team in the Summer 2021, I received constructive advices from my mentor and colleagues. I think working in the blue team and defensive security is fun, but I prefer red team and offensive security. Then, my mentor told me OSCP is a highly valued certification to step into offensive security. At the same time, one of colleagues introduced TryHackMe.com and HackTheBox.com. I played some rooms on TryHackMe.com and I like the CTF-style learning environment. Then, I unofficially entered the journey of learning OSCP.

---
## How I Prepared For OSCP?

As I mentioned before, TryHackMe (THM) and HackTheBox (HTB) are two useful resources. In addition, Offensive Security Proving Grounds Practice is highly recommended. The official topic exercises and PEN-200 lab are the official materials you should NOT miss. There are also other online resources. Google will be your best friend to learn hacking if you know how to ask the right questions. GitHub is also one of the most frequent websites I visit and there are many useful exploit code and open-source code. Let me discuss more details about these learning resources.

- TryHackMe.com  
	This is excellent for beginners. I became a member of both THM and HTB at the same time. I did have some knowledge in security and knew some (but not a lot of) Linux operating system. I feel like HTB is for security professionals with some experiences (2+ years). Then, I switched to the THM. Many rooms have step-by-step walkthroughs and hints. So, the beginners won't lose their ways while learning new things. Some rooms are more like HackTheBox style for challengers. One con for these step-by-step walkthroughs is that people may be overconfident for the skills learned in these walkthroughs. They learned these knowledge in the well-structure learning environment. But, discovering them in a highly uncertain environment is a different story. Overall, this is a good start.

- HackTheBox.com  
	This is a more challenging resource than THM. In most time, you were just given a IP and then hack it with very few instructions/directions/hints. This is definitely a better training for the hacker's mindset. But this is not beginner-friendly. Usually, you are required to know the fundamental host/IP/port/web scanning techniques. This is not recommended for complete beginners. New guys may be discouraged or get bored to learn on HackTheBox. But, for those with some experiences in offensive security, it's a good resource that you may always learn something new! Even though those new things may not be very relevant or too advanced for OSCP exam, they are still useful for the offensive security career!

- Offensive Security Proving Grounds Practice 
	This is the resource that's closest to the standalone machines in the real OSCP exam. Well, they are not exactly the same. You can only pwn one machine at one time on the PG Practice. The machines with the officially rated Easy and Intermediate are highly recommended to complete. These machines are not as hard as the machines on HackTheBox that may contain really weird tricks. These machines are much more relevant with the OSCP exam and the PEN-200 course materials. If the official PEN-200 lab is the bare minimum, then PG Practice is more like the "standard examples". Many machines in PEN-200 lab are just straightforward using one or two vulnerabilities. But, many machines in PG Practice are chaining with two or more vulnerabilities that require more in-depth enumerations and creative ways of exploiting. By the way, I don't recommend you to do those machines with the officially rated Hard if you don't have enough time. But, if you like challenges, definitely pwn some of them. 

- The official topic exercises and PEN-200 lab  
	When you buy the OSCP bundle, you have the official access to study materials and one voucher of OSCP exam. They are binding with each other. The study materials contain fundamental content (web readings, videos, and a personal PDF book), topic exercises (relevant CTF-style challenges), and the lab network (contain total 75 vulnerable machines and their associated 5 networks: Public, Sandbox, Development, IT, and Administrative).  
	The fundamental content is great for beginners for learning Linux command line, bash script, information gathering, web app penetrations, active directory, and so on. There are 25 chapters when I access it from Feb 2022 to May 2022. At the end of some sections, you will be given CTF-style challenges to practice and hone your skills learned from the materials. Most of them are straightforward. But some of them are challenging and you have to think about for some while.  
	The lab network overall is a great emulation to the real-world scenarios. The fake networks provide a good environment to practice pivoting and port redirection cross different networks. You may also practice your skills to pwn some machines as standalone boxes. Each of 75 machines must be pwned with at least one way to get root or administrative right. Pwning these machines is a good way to learn the classical vulnerabilities and improve your methodologies. However, these vulnerabilities may be oversimplified or out-of-date comparing to the machines on HTB. Even comparing with Offensive Security Proving Grounds Practice, these machines are relatively naive. There are also 3 active directory set you can learn. One is the example AD set with step-by-step walkthrough in the learning materials and the other two are for the learners to discover and practice.  
	- About the bonus point: https://help.offensive-security.com/hc/en-us/articles/360040165632#bonus-points  
		You can get ten (10) bonus points if you `(1) submit at least 80% of the correct solutions for topic exercises in every topic in the PEN-200 course and (2) submit 30 correct proof.txt hashes in the Offsec Platform`. It's highly recommended to meet these requirements to get 10 bonus points.

- Google, GitHub, and other resources  
	The key to ask Google is asking the relevant content like the version of a application, aliases of some vulns, mutant versions of a vuln, and so on. You may also search something you don't know in the enumeration phase. Sometimes, you have to search with multiple keywords to extract only a tiny portion of information.  
	GitHub is one of my favorite exploit searching resource besides exploitDB and `searchsploit`. I often find many useful exploit code that I cannot find on exploitDB. You may also find some technical writeups and debugging information on GitHub.  
	There are other useful online resources like StackOverflow, reddit, twitter, medium, etc. Try to always begin with the most relevant keywords from your enumeration phase and then narrow down to extract the information that's useful for your scenario. It's really easy to get flooded by the information ocean. 
	- TJ Null's OSCP-like boxes list: https://docs.google.com/spreadsheets/d/1dwSMIAPIam0PuRBkCiDI88pU3yzrqqHkDtBngUHNCw8/edit#gid=1839402159 
	I followed this list to prioritize those OSCP-like boxes to complete! You don't have to do all of them. But make sure do some and learn valuable lessons.  
	- IppSec's YouTube channel: https://www.youtube.com/c/ippsec 
	While I was doing HackTheBox machines, I found this youtube channel is very useful and learned something not in the official PEN-200 materials but still useful for OSCP exam! Even if I know how to pwn a box, I still watch IppSec's videos to see any new ways of pwning the box.

---
## Timeline

- July - November, 2021  
	- Heard about OSCP exam and consider passing the OSCP as one of my career goals in the summer 2021
	- Played THM and HTB to learn fundamentals and get familiar with the CTF environment (unofficial preparations)

- December, 2021 - January, 2022  
	- Noticed OSCP exam structure changes and adjust my study plan to focus more on Active Directory (official preparations began)  
	- Pwned some boxes on HackTheBox and Offensive Security Proving Grounds Practice by following TJNull's list of the OSCP-like boxes  

- February - April, 2022  
	- Officially enrolled into 90-day PEN-200 course and its lab network
	- Completed all topic exercises in the fundamental content materials
	- Gained root/administrative right and submitted flags for all 75 boxes. If I have more time, I hope I can pwn them with multiple distinct methods. For the majority of the PEN-200 lab boxes, I pwned them with a single method. For some machines (10-20), I had multiple methods (including both initial access and privilege escalations). For very few boxes (under 5), I had more than two methods.

- May - Mid-June, 2022  
	- Taking a break for studying OSCP exam since I was focusing on my Master degree and graduated in Mid-June.

- June 21st, 2022
	- Failed the 1st attempt with 50 exam + 10 bonus points. I was very close to pass it. I will analyze multiple factors to fail this attempt in the next section.

- End of June - Beginning of August, 2022
	- Continue pwning more boxes on Offensive Security Proving Grounds Practice  
	- Refreshed and analyzed why I failed on the 1st attempt and fixed them in the 2nd attempt

- August 11st, 2022
	- Passed the 2nd attempt with 90 exam + 10 bonus points if no deduction points on my exam report

---
## The 1st Attempt - Almost Passed

### Reschedule The Exam  
Initially, I scheduled this attempt in Mid-May, right after my 90-day access to PEN-200 course expired. However, I was also busy for my school work during this period. I did not feel it's a good time to take OSCP in Mid-May. Then, I rescheduled it to June 21st. My schoolwork ended on June 9th. Then, I just spent a couple days to relieve from the stress and move toward to OSCP exam. I just had about 10 days before the OSCP exam. I decided quickly going through some materials, especially the Active Directory and began pwning some boxes on Proving Grounds practice. Also, the most important thing is reading the official instructions on Offensive Security website about OSCP. I found that I need to schedule a test session for checking my webcam since I was using Kali Linux on the bare mental machine (no Kali VM on Windows host or other host OS, the Kali is the host OS on my laptop).

### Three Mistakes
The first mistake I made was underestimating the logistics in the exam procedures. I had my Kali on the bare metal directly, but I installed some apps on the Kali. Those apps were kind of conflicting with each other, especially with the default updates from Kali official release. I should reinstall the Kali to be the official default version, but I did not. Also, I usually used my 32-inch monitor as the 2nd monitor. But, during the test session for the webcam, the dual monitor setting was not working somehow. I frankly thought I could spent some time to fix it on the day of exam. Well, this was NOT a good idea.

At the night before the exam day, I was super excited and my brain was acting like dancing at a bar. I could not sleep well. I was almost sleepless all night. This was the second mistake I made.

On the exam day, I still connected the 32-inch external monitor to my laptop. In the proctoring procedures, the webcam plugin was crashing with the external monitor somehow to freeze my laptop and I had to restart the computer to connect back. I spent some time and could not find a perfect way to utilize my external monitor and satisfied the proctor's requirements. Then, I had to give up using the nice 32-inch monitor and just used the internal 15.6-inch monitor. The proctor told me I had to unplug and move the external monitor away from my desk. Then, I followed his instructions. After everything was set, one hour was already wasted and I had about 22 hours 45 minutes left.

Then, I began with the Active Directory set. I was confident with it and know it's a huge portion of the exam. The initial access was straightforward. But, I spent more time than I expected. Later, I was also stuck in the lateral movement for some quite amount of time. It should not be that hard. Maybe the smaller screen made my work hard. As a result I was able to pwn the domain admin. I spent about 6.5 hours for Active Directory set.

I did not know which standalone machine to begin, then I enumerated all of them to see which one might be easier for me. I found a web vuln on a machine to quickly gain the low-priv access. I had 50 exam + 10 bonus points. It's been about 8 hours.

Unfortunately, I did not make any progress later. I thought I could get the root/admin right on the 1st standalone machine, so I spent too much time on it. But nothing worked. This was the third mistake I made - stuck for too long on a single machine. 

### The End
As the time was wasting, my brain began to get exhausted. I did take 10-15 minutes break every 2 hours, ate some snacks, kept myself hydrated, and went to the bathroom when needed. I really felt like my brain did not turn on the switch and I was reluctant to take a long break for sleeping. I was afraid to sleep for overtime. I had tried many things for Privilege Escalation but was still unable to gain the root/admin right on the 1st standalone machine.

Consequently, I failed with 50 exam + 10 bonus points. I did not write/submit the exam report at all. I see it's pointless. But I did get a good sleeping on the 2nd day just after the exam.

---
## The 2nd Attempt - Passed With High Confidence

### Fix Logistics Issues
Within a week of ending the 1st attempt, I actually had some great ideas about those machines after my brain went back to work normally. More importantly, I concluded those three mistakes and fixed them.

I reinstalled Kali on my laptop and tried to use default settings as possible as I can. I was very careful about customizations on the Kali, installed packages/apps, the location of installations, the modified configs, and clearly know what's going on. Also, I set up the backups by using `timeshift`. If there was anything wrong, I could just revert to the old backup. Also, for the 2nd attempt, I would not use any external monitor and just used the internal monitor. I did adjust the settings of colors and font size on the 15.6-inch monitor to make it more friendly to read. That should be enough.

Then, I continue pwning boxes on PG Practice. I pwned all machines with the officially rated Easy and Intermediate and half of machines with the officially rated Hard. I did learn more current tools on these boxes.

Just a week before the 2nd attempt, I stopped updating Kali. I believed that Kali version should be enough for passing OSCP and I just want to make sure there were no uncertain new things on my exam machine.

Just two nights before the exam, I forced myself not to sleep well. Then, in the next night (the night before the exam), I could sleep well since I was not over-energetic. This sleeping schedule worked well on my own body. I had a great sleeping quality before the exam.

### Try Harder And Try Others
On the exam day, I logged in 15 minutes before the start time and finished all proctoring requirements smoothly in about 6 minutes. Then, at the scheduled time, I received the email to connect the VPN. I did not waste any time in this attempt.

As I did in the 1st attempt, I also began the Active Directory set. Well, this set also looked like a straightforward one but I did not find anything for the initial foothold after 30 minutes. I had the feeling I would probably waste too much time.

Then, I moved to the standalone machine 1, this was an easy machine for me, I did something similar in the past. After about 1 hour, I got the low-priv shell. For the privilege escalation part, I quickly got the clue but could not make any progress. One hour was already wasted. I decided to move to the other targets. At this moment, I had 10 exam points in 2.5 hours. 

For the standalone machine 2, the initial foothold was also quick to find. I was able to get the low-priv shell in just about 30 minutes. But, for the privilege escalation, I felt like I knocked the wall again and did not have any ideas. I decided to move to standalone machine 3. At this moment, I had 20 exam points in 3 hours.

For the standalone machine 3, the initial foothold was also straightforward but I noticed there was a rabbit hole. I just tried the one that worked to get the low-priv shell quickly in about 1 hour. The privilege escalation was also straightforward and it's not hard to find the vuln but I had to try multiple times to make it work. Before I tried harder, I took a quick break for about 15 minutes to recharge myself. I was able to get the root/admin shell with a couple trials. At this moment, I had 40 exam points in 5 hours.

Taking another break for about 10 minutes before going back to the standalone machine 1, I felt like I had some new ideas. For this standalone machine 1, instead of following the old clue, I tried some other new ways. Luckily, one of those worked, I was able to get the root/admin shell for this machine. At this moment I had 50 exam points in about 7 hours.

### Critical Moment
This was the critical moment. I just need 10 more points from the root/admin shell on standalone machine 2 with my 10 bonus points to pass OSCP. OR, I had to pwn the whole active directory set. So, I was oscillating between the Active Directory and standalone machine 2. I tried many different ideas but none of them worked after 3 hours. It's been about 10 hours since the start time. 

It looked like finding the right PE method on standalone machine 2 had less work than pwning the whole Active Directory set. However, for those who didn't know the key information, they had "equally" huge work to do. Based on my personal experience in the 1st attempt, I was stuck on the PE of a standalone machine. This time, the standalone machine 2 was very similar to the one in the 1st attempt. So, I decided to focus on the Active Directory set since I did pwn the whole domain in the 1st attempt. I was glad that I made a wise decision at this moment. In addition, even if my brain came up with some bad imaginations of failing again, it still worked logically. This was not like the 1st attempt. I took a 10-min bathroom break before continuing.

After enumerating the foothold on the Active Directory for 2 more hours, I suddenly came up with the right idea to knock on the door! I quickly gained the low-priv shell on the target 1 of the AD set and gained the admin shell on the same target quickly. It's been 12.5 hours. The lateral movement was not as easy as the AD set I did in the 1st exam. But my brain seemed turning on the switch and came up with a bright way for the lateral movement. I was able to move to target 2 of the AD set. Moving to the domain controller was much easier than cracking the initial foothold. Consequently, I was able to pwn the whole domain very quickly. At this moment I had 90 exam points in about 13.5 hours. 

Then, I decided to take a 10-min break to refresh myself. Coming from the break, I took a look on the standalone machine 2 and I still had no ideas for PE part. Since I have enough passing points, it's time to prepare for the report.

### Exam Report
Preparing for the exam report was relatively less stressful. I used the exam template from the official website. What I need to do was carefully examining the procedures of pwning machines and taking screenshots logically and consistently. Make sure my exam report show the step-by-step procedures with specific commands and instructions. I read the exam objectives and the instructions on the official website again. Before I wrote the official exam report, I had my personal notes to organize my ideas and took thorough screenshots. I also reverted all those machines before checking my procedures. After I had done the work, It's been 18 hours. I was kind of tired. I took a shower and went to sleep for about 2 hours. It's been 21 hours.

I did not sleep deeply since I had not finished my work. I submitted the correct proof hashes on the exam panel and then started writing the official exam report for the active directory set. After about 2 hours writing, it looked all good. I did a final check for everything before disconnecting from the VPN. At the moment of 23.5 hours since the exam start time, I requested to end the exam.

Next, I ate and took a good sleeping. Then, I began to write the official exam report by carefully referring the instructions on the official OSCP website. I also proofread a couple times. At the moment of 30 hours since the exam start time, I submitted my exam report. 

### Result
The grading of Offensive Security was quite quick. They even worked on the Weekends. At the moment of 57 hours since the exam start time (9 hours and 15 minutes since the report end time, 27 hours since my submission of exam report), I received the email notification of passing OSCP.

---
## Conclusion

### Personal Feelings
- Offensive Security does an amazing job to provide the learning experiences to help me grow up the hacker's mindset. I love doing the practical hands-on exam! After passing the OSCP, I feel I gain new perspectives for the information security.
- It's completely doable for anyone with high motivation in offensive security, red teaming, or penetration testing but lacks relevant experiences. You need a practical plan and execute it in time. You don't need many years of education (they may be a plus somehow). I read many OSCP journey writeups and I see there are many folks from different backgrounds.
- This exam is not an end goal. This is just a beginning of my career in offensive security. I'm glad to keep learning information security and offensive security. There is much more to dig deeply!

### Personal Suggestions
- Don't underestimate any logistics issues. They could be zoomed in on the exam day. Expect the unexpected and prepare for the worst. Always have plan B.
- Taking your OWN organized notes and review them periodically. I assume you are a normal person instead of a genius. There are already many OSCP notes online, but they are NOT yours. You need to make your own notes. Organizing these notes can help you refresh those knowledge and build the neuron muscles in your brain. You don't have to remember every single detail but at least the key ideas. Reviewing the notes periodically is important since it's easy to forget them if you don't use them very often.
- Use writeups/walkthroughs wisely. Don't stuck too long on one box. Consider the real exam scenario, your time is limited. For a standalone machine, spending about 2-3 hours is decent or 4-5 hours for the hard one. I recommend to read the walkthroughs after 12 hours of making no progress. Make sure you always learn something new by reading writeups/walkthroughs. Think about why they should do that way instead of your own way. Be a thinker instead of a duplicator!
- Make sure learn multiple ways of doing the same thing. The more ways you know, the better! Different methods/tricks come from different ways of thinking. Learning multiple ways can help shape the multidimensional mindset and this is critical to build your creativity. Not every method can apply all scenarios. So, if the method A fails, then try method B, C, ... until some method works. If all existing methods fail, you may have to come up with a completely new way!
- Instead of reading the journeys of passing OSCP for the 1st try without showing any obstacles and such, I recommend to read those who failed multiple times and passed it finally or struggled to barely pass for the 1st try. In this way, you can actually learn something new. If you are not a genius and just a normal person, learning from the mistakes (both from others and yourself) is the most efficient way to learn. Make sure don't repeat those mistakes on your own.

### To Be Continued...
I believe the journey of OSCP exam brings me a strong foundation of hacker's mindset and opens a new world to me in the offensive security. I learned a lot in this journey. I will keep going and have fun while learning hacking! I will start the career in penetration testing and bug bounty soon.

Lynden L.  
Sep 13, 2022  
---
layout: post
title:  "Therac-25-accidents"
date:   2016-02-14 14:38:00 -0600
categories: jekyll update
---

From the readings, what were the root causes of the Therac-25 accidents? What are the challenges for software developers working safety-critical systems, how should they approach these projects, and should they be held liable when accidents happen?

The tragedy of Therac-25 accident is really disturbing. It shows how much responsibility engineers have when working on things critical to human life. To be honest, I myself never strived for perfection when writing programs. There are always some edge cases that come up, so it's hard to cover everything and sometimes I just think these errors would at most make someone frustrated for a little while. This accident makes me realize that I also need to have high standards for my own work as a computer science student.

According to the article <a href="http://hackaday.com/2015/10/26/killed-by-a-machine-the-therac-25/">Killed by a Machine</a>, the Therac-25 machine was made without any hardware interlocks, so that it was controlled by computer only. However, the software system was put into production without sufficient unit test. This approach sounds really unprofessional even according to the standards in software industry. Before every release, engineers are expected to go through a very thorough set of testing, at least for established companies that provide software or service for millions of people. Companies also hire specific testing engineers whose whole responsibility is to test the software system and make sure they are safe and functional. While some startups or smaller companies probably do not have thorough testings and might boast themselves as "move fast" environment, I always thought that is due to their relatively smaller user base. And a few bugs of their service would defintely have much less consequence than the errors of medical devices.

The more disturbing information about Therac-25 is that it is designed to minimize operational cost. A fully computer-controlled machine takes less time to operate, and thus could be used more frequently. The accidents seem to be a result of the flaw in design. The engineers place too much emphasis on improving efficiency that they forgot the number one priority for a medical device - safety. If everyone put patients safety in mind, the accident would likely be avoided.

Medical devices are very different from usual software systems. They are more safety-critical, and has almost zero fault-tolerance. Engineers working on these systems need to be extremely cautious of their work, and comprehensive testings  should be designed before every update. Besides, it's also very important to have experienced engineers to design the whole system, so every part can work together in a comprehensive way. 

It's a really hard to say if the engineers should be responsible for failures in these software systems. I think they should definitely be held responsible for the failures or bugs in their program, but there are many problems that could happen to the system. Sometimes the failures happen because of some system design principles, or some decisions made from the management level. I think we need to make specific guidelines in how programs should be developed and tested, and how responsibilities are divided among different people.
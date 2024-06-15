---
layout: post
title:  "Review : Burp Suite Certified Practitioner (BSCP)"
date:   2024-06-15 17:00:00 +0800
categories: Reviews
tags: certs bscp portswigger burp
---

*"The first step is the hardest, but the second step is even harder."* -- Nathanial Branden

After completing the Certified Bug Bounty Hunter (CBBH) from HackTheBox (HTB), it felt like a natural next step to go for PortSwigger's Burp Suite Certified Practitioner (BSCP) certification. Both are targeted at web application penetration testing, and the overlap between the courses is extensive. However, I definitely underestimated the length of time it would take. What I initially thought would be 2-3 weeks of filling in some knowledge gaps from the CBBH turned out to be 2 months of gruelling grind through an almost unbelievably comprehensive set of materials and lab exercises.

![BSCP Certificate](/assets/img/bscp-certificate.png)

Now, don't get me wrong. I use the word "grind" because by the end of my preparation, it definitely felt like that. But I certainly don't mean it to be negative in any way. I'm still left completely amazed (and thankful) at the amount and depth of material that PortSwigger has made available to the public at virtually no cost. Yes, yes, I know you need a Burp Suite Professional license to take the exam, but you don't actually need to take the exam to benefit from the content. 

To be completely fair, if you're not trying to smash through everything as fast as I was attempting, then maybe it won't feel like a grind at all, but rather an abundunt, knowledge-filled journey through the wonderfully diverse world of web application penetration testing. Additionally, it wasn't technically a requirement to finish all 58 apprentice-level and 168 practitioner-level labs (at the time of writing) in order to take the exam. Unfortunately, I'm a completionist (excluding the considerably more difficult Expert labs... for now) and also an over-preparer, so the self-inflicted "punishment" was almost a necessity for me.

![BSCP Dashboard](/assets/img/bscp-dashboard.png)


**The Course**

In terms of the "course",  there's obviously plenty to get your teeth stuck into. However, unlike the CBBH pathway, where it felt like there was an intended order to the modules, there's considerably less guidance for PortSwigger's Web Security Academy content. You're basically left to your own devices to decide your own path through the maze of topics with labs scattered throughout. Alternatively, you can work your way through the series of labs for each topic like a checklist, referring to the material only if you get stuck and need additional information. Looking back at the PortSwigger site now (over three months since I took the exam), there's a bunch of learning paths that have been added, so this is another possible method and may reduce some of that lack of guidance I referred to earlier.

The labs themselves are numerous and very specific. Each one focuses on a single technique, or even a single aspect of a particular technique. This prevents spending too much time (usually...) trying to discover the vulnerability and allows you to concentrate your efforts primarily on learning exploitation. The intended and community solutions available with each lab are also handy, and enable learning to continue if you're irretrievably stuck or as additional learning if you solved the challenge a different way.

To take the exam, the set of formal "preparation steps" required involve the following :

- 23 practitioner-level labs effectively comprising a lab from each topic
- 8 specific practitioner-level labs that reinforce core web security testing skills
- 5 mystery practitioner-level labs where the vulnerability and objective is unknown
- 1 practice exam

The mystery labs are a good way to practice enumerating the vulnerabilities; however, occasionally, they felt near impossible to figure out without using the hint to learn the objective. If you did all the labs first, and have a good memory, you might be able to avoid this, but I distinctly remember a couple of them being tricky to figure out. Beyond this, I highly recommend taking two practice exams. Both give you a very good feel for the format and challenge provided by the actual exam, as well as the time pressure you'll face. For my part, I "failed" the first practice exam on time. This forced me to re-evaluate my readiness for the exam, eventually leading to a one-week postponement of the exam to squeeze in some much-needed revision and practice time.

**The Exam**

Regardless of what I thought was extensive preparation, there were plenty of nerves when I took the exam. Four hours doesn't feel very long for a practical exam, especially one that covers such an expansive range of techniques. When doing CTF challenges or HTB machines, I often get completely stuck, and then only many hours and a well-toughened forehead from repeatedly smashing it against metaphorical walls can get me through. This fear was obviously exacerbated by my practice exam failure, but at some point you just have to take a punt.

One lesson I did learn from the practice exams that proved invaluable was being prepared with methods to actually *exploit* the various vulnerabilities. It's not enough to pop a simple alert message when you find an XSS issue, for example, you need to be able to use it to steal a session cookie or force a victim to perform an action by submitting a form. You don't want to be spending too long trying to figure that out during the exam, so come armed with a well-tuned exploit-ready cheat sheet with plenty of examples!

Another important tip learned more from reading reviews of the exam than my own experience was based on logic. As with the practice exams, there are effectively three stages to each of the two applications you'll be faced with : Obtain access to a user account, elevate privileges to compromise an administrator, and then read the contents of `/home/carlos/secret` on the web server to obtain the flag. The logic basically suggests that any technique used to achieve one of the stages is *not* going to be the technique used to achieve any subsequent stages for an application. This, combined with the fact that the vulnerability for the next stage is necessarily going to involve any new functionality you've unlocked, really narrows down the amount of enumeration you need to undertake at each stage. This particular [review](https://micahvandeusen.com/burp-suite-certified-practitioner-exam-review/) was extremely useful and contains a table produced by the author that helpfully outlines this logic when applied to all the relevant lab categories. Don't ~~leave home~~ take the exam without it.

In terms of time-management, the only advice I can give is not to panic. Like my first practice exam, solving the first application took just over two hours (over 50% of the time). Fortunately, the second application proved much quicker to solve, so much so, I ended up finishing the exam with over an hour to spare. So, while you need to be aware of the clock, always understand that you can go from zero to flag very quickly.

A final word on the proctoring for this exam. It's not a live proctoring system, but something you basically set up prior to starting the exam to record your screen (only one screen though, oddly). Having not yet done an exam with live online proctoring, I can't say for sure, but this felt a little more comfortable than I imagine live proctoring feels. I did have a moment of panic wondering if I'd selected the correct screen for recording (there's no indication once you start it, so select carefully), but given I was granted the certification, I'm guessing it was fine. Lastly, you do need to submit your Burp file (which is one of the things that requires a professional license, I believe) at the end of the exam, so make sure you've saved your session appropriately.

**Some Statistics**

Similar to my CBBH review, I thought I'd delve into some statistics again. Obviously, the times stated below are going to be different from person to person, based on experience, learning styles, prior knowledge and ability. However, if your situation is similar to mine (see more context from my previous [post](https://offensivelysecured.com/posts/review-certified-bug-bounty-hunter/)), perhaps you'll find it instructive.

- **Study** :
	- **Coursework & labs** : ~56 days (~2-3 hours/day)
	- **Revision & exam preparation** : ~7 days (~3 hours/day)
- **Exam** :
	- **First application** : 2 hours 7 mins
	- **Second application** : 45 mins
	- **Time remaining** : 1 hour 8 mins
- **Waiting for result** : 1 day
- **Procrastinating writing this post** : ~3 months :/

Similar to my figures for the CBBH, those with decent experience in web application pentesting or bug bounty hunting should be able to undercut them considerably. Even moreso if you don't feel the need to complete all the apprentice and practitioner labs before taking the exam.

**Conclusion**

All-in-all, the BSCP certification is definitely a worthy addition to anyone's professional resumé. Understanding the expansive set of techniques explained, explored and tested in PortSwigger's content, labs and exam, will stand you in good stead when approaching any web application penetration testing engagement. Even with my seemingly unsolvable imposter syndrome (more on that in a future post), the lessons learned from my pursuit of this certification have given me added confidence when looking for vulnerabilities on the web. The cost-effectiveness of this certification (or even just the content, if you decide not to sit the exam) is difficult to argue with. And, being the path I myself took, I can highly recommend the one-two punch of the CBBH and BSCP combination for any aspiring web application penetration testers out there.

---
layout: post
title:  "Review : Certified Bug Bounty Hunter (CBBH)"
date:   2024-03-24 22:30:00 +0800
categories: Reviews
tags: certs cbbh htb
---

*"A journey of a thousand miles begins with a single step"* -- Lao Tzu

Towards the end of last year, as the first step of a long overdue push to becoming an ethical hacker, I purchased an annual subscription to [HackTheBox Academy](https://academy.hackthebox.com/) in pursuit of the [Certified Bug Bounty Hunter](https://academy.hackthebox.com/preview/certifications/htb-certified-bug-bounty-hunter) (CBBH) certification. I ended up taking the exam just after the new year, and thankfully received my certification a few weeks later. Given how helpful I'd found other people's reviews in the lead up to purchasing the subscription and in preparation for the exam itself, I thought I should give a quick rundown of my journey too.

![CBBH Certificate](/cbbh-certificate.png)

### The Course

The [Bug Bounty Hunter Job Role Path](https://academy.hackthebox.com/path/preview/bug-bounty-hunter) covers core web application security assessment and bug bounty hunter concepts and techniques. The content itself is divided into 20 modules, comprising markdown text and diagrams, followed by targeted lab exercises. This is something to note if you prefer video-style learning. However, I can't say enough about the material. It's phenomenal. The coverage is very comprehensive, the structure is clear and easy to follow, and the labs are well thought out and effective at reinforcing the lessons learned in each module.

The modules also come with accompanying cheat sheets that many will likely find useful. Personally though, I created my own notes with summaries, commands and solutions for the lab exercises, as I was going through the coursework. During the exam then, I was able to use my own notes and never really referenced the cheat sheets at all. 

One thing I did do, however, was create a streamlined index with quick references and markdown links, that proved very handy for navigating through all my notes when under the pressure of the exam. I highly recommended doing something similar, whether you use the cheat sheets, your own notes, or some hybrid approach, so you're not spending too long trying to find a particular needle in the haystack of all your information. In many instances, the index also provided a solid checklist of steps to take when identifying, and later exploiting, vulnerabilities.

### The Exam

I was pretty nervous when I started the exam. So much so, I accidentally deleted the pre-built [CBBH reporting template](https://www.hackthebox.com/blog/certification-templates) in the [SysReptor](https://docs.sysreptor.com/htb-reporting-with-sysreptor/) system and spent the first half an hour cursing myself while hastily figuring out how to re-add the template (in case this happens to you, create a new project and select the CBBH template in the "Design" dropdown). I'm a massive fan of markdown, so I much preferred using this template over the Word document that officially comes with the exam, but this'll come down to personal preference. 

I obviously can't say too much about the specifics of the exam itself beyond what's already publicly available. I will say though, if you've mastered the course content, you should have no real issues. There wasn't really any surprises and only a few rabbit holes (albeit enough to cost me several hours). Keeping your notes organised is a must though, especially if you find yourself jumping around between machines when stuck, as I did. 

The flags are consistently placed and very obvious when you find them. Submitting them is intuitive and works similarly to entering answers on the lab exercises from the course. Be aware that if you reset the environment, all the flag values change (including ones you've submitted, though your progress is not affected). Just something to keep that in mind when you're taking screenshots of your flags and referencing them in your report.

Writing the report itself was something of a challenge for me, as I'd never really done it before. The CVSS calculator was also a little daunting to start with. However, the "Bug Bounty Hunting Process" module from the course steps through everything pretty clearly. Use the examples they give as a guide and find supporting material on the Internet that you can paraphrase and adapt. For recommendations and references to use with your findings, the [OWASP Cheat Sheet Series](https://cheatsheetseries.owasp.org/) is invaluable. In terms of workflow, I obtained all the flags before beginning the report. This worked out fine as I managed to find all the flags with plenty of time to spare; however, had things worked out differently, this could have left me under pressure to complete the report, so it might be worth considering writing the report as you go. This probably would have helped with screenshots too, as I ended up having to re-compromise some of the machines on later days to take a few screenshots I'd missed.

All in all, the exam process was smooth and painless (accidental template deletion aside). The lack of proctoring is definitely appreciated, as it's something you don't really want to be worrying about when you'd rather be focusing solely on the exam. Hopefully, people doing the right thing and the reporting requirement is enough to maintain certification integrity. If this is part of the reason for the delay between report submission and receiving your final result, it's a small, albeit excruciating, price I'm willing to pay.


### Some Statistics

So I thought I'd outline some of the statistics around time spent preparing for and taking the exam. This is going to vary wildly from person to person, so please take it with a grain of salt. Some people may go through things a lot quicker than I did, and some people may take longer. Much will depend on how quickly you learn, your style of learning, how much time you're able to dedicate to the process, and also (probably the most variable aspect) where you're starting from in terms of experience and knowledge. In any case, it might be helpful to have someone else's numbers to use to estimate the time and effort you may require.

- **Study** :
	- **Coursework** : 26 days (~3-4 hours/day)
	- **Revision & exam preparation** : 3 days (~8-10 hours/day)
- **Exam** :
	- **Pentesting and finding flags** : 2 days (~12 hours/day)
	- **Reporting** : 2 days (~10 hours/day)
- **Waiting for result** : ~19 days (including weekends)
- **Procrastinating writing this post** : ~2 months :/

To give some context to these figures, here's a little background. I have about a decade worth of experience in enterprise networking, bookended by a few years prior as a web application developer and a few years after as a SOC analyst. I've been doing CTFs and HTB machines on-and-off for about 5 years, and the month or so prior to doing the course I finally read through my years-old copy of the Web Application Hacker's Handbook. 

I suspect those who've spent any reasonable time web application pentesting or bug bounty hunting will be able to undercut my numbers by some margin. And, as mentioned earlier, the reporting process was very new to me, so if you have experience in this arena, it will likely take you much less time.

### Reviews

As referenced at the start of the post, I found several people's reviews useful both for convincing me to purchase the Academy subscription to pursue the CBBH (and, in future, the CPTS) and also for preparing to take the exam itself. Here's a few of my favourites:

- [https://bytebreach.com/posts/passing-the-certified-bug-bounty-hunter-cbbh/](https://bytebreach.com/posts/passing-the-certified-bug-bounty-hunter-cbbh/)
- [https://infosecwriteups.com/from-failure-to-success-my-experience-with-the-htb-cbbh-49f2bfd41582](https://infosecwriteups.com/from-failure-to-success-my-experience-with-the-htb-cbbh-49f2bfd41582)
- [https://medium.com/@thewhitehatpanther/my-journey-to-become-certified-bug-bounty-hunter-by-hack-the-box-273dca8d8f85](https://medium.com/@thewhitehatpanther/my-journey-to-become-certified-bug-bounty-hunter-by-hack-the-box-273dca8d8f85)
- [https://www.youtube.com/watch?v=6ISUuMBzCyo](https://www.youtube.com/watch?v=6ISUuMBzCyo)
- [https://www.youtube.com/watch?v=-5s2R0Mldgw](https://www.youtube.com/watch?v=-5s2R0Mldgw) (CPTS vs OSCP)

### Conclusion

This review is longer than I thought it'd be, so I better end it here. Suffice to say, I'm very happy with my purchase of the HTB Academy subscription and much relieved to have achieved the CBBH already. I still have many months left on the annual subscription, so the plan is to continue using it to study for the [Certified Penetration Testing Specialist](https://academy.hackthebox.com/preview/certifications/htb-certified-penetration-testing-specialist) (CPTS) exam soon. This was one of the drivers for going with this option in the first place. That, and the price. Compared to other options on the market, the combination of cost efficiency (especially when doing two certifications) and the availability of coursework and labs for an entire year made this path a clear winner. Anyway, hopefully this rundown of my experience has helped you in some way.

Until the next one, keep hacking!

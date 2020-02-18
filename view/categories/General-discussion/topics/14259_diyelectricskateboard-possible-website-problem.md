# Diyelectricskateboard possible website problem?

### Replies: 19 Views: 1503

## \#1 Posted by: Koto Posted at: 2016-12-06T11:47:29.058Z Reads: 165

```
For me, diy electric skateboards website re-directs to virus filled wesite.
```

---
## \#2 Posted by: treenutter Posted at: 2016-12-06T12:19:22.136Z Reads: 158

```
It is loading normally for me, it is more likely that you have a local virus on your computer. Title edited to avoid confusion.
```

---
## \#3 Posted by: Tuomalar Posted at: 2016-12-06T13:26:28.800Z Reads: 146

```
I haven't used their website with computer for a while but with my phones (android and ios) i have had same problems. I don't know why but some day it just show me these trash sites and the other day it works like it should.
```

---
## \#4 Posted by: mmaner Posted at: 2016-12-06T13:50:48.171Z Reads: 137

```
You guys have a DNS virus.  There's nothing wrong with Dexter's site, I did nslookup's from 3 DNS servers at 3 locations and the all route correctly

    Name:    
    Address:  67.222.5.32

You should probably verify claims like this before you start spreading bullshit, your screwing with a mans living.
```

---
## \#5 Posted by: Tuomalar Posted at: 2016-12-06T15:09:13.691Z Reads: 128

```
Calm down. 
I don't mind that, but any idea why diys website is the only one which do this. I visit like ten to twenty different webpages each day and all of those always work.
```

---
## \#6 Posted by: mmaner Posted at: 2016-12-06T15:12:14.687Z Reads: 126

```
Typically DNS viruses operate on your browsing history.  I would check that your DNS are correct, they are typically the ISP DNS servers.  Also check that your host file doesn't have erroneous entries.

I am calm, I just dont like it when people flipantly make accusations that can cause other people harm...and thats exactly what is happening with this thread.
```

---
## \#7 Posted by: rpn314 Posted at: 2016-12-06T16:11:06.585Z Reads: 116

```
I've had the problem once or twice before. I've found that some DNS services/servers somehow don't have his site listed, and so they send you to a "dummy" site (one of those stupid portal pages or something similar) and thus you get that kind of junk. It's not DIY's problem, it's the internet in-between.
```

---
## \#8 Posted by: NNGG Posted at: 2016-12-06T23:19:45.159Z Reads: 98

```
I have had some issues where the site is just down, like our forum was a couple times, but It always redirects to his usual website. once it up. Please try to investigate them cause of the problem and not assume correlation for diy's site and websites
```

---
## \#9 Posted by: Koto Posted at: 2016-12-08T00:27:51.930Z Reads: 84

```
Randomly fixed! :confused:
```

---
## \#10 Posted by: sl33py Posted at: 2016-12-08T01:08:57.256Z Reads: 84

```
The internet is broken, and my cup holder won't open!  

I'm in IT - i've seen it all (except the cupholder joke is a bit old...).

Dexter's site can be slow, but always has loaded.  Also agree you should do some basic checks before saying something like this - it truly can be a big impact to someone's livelihood.
```

---
## \#11 Posted by: LAVAMAN Posted at: 2016-12-20T18:15:06.575Z Reads: 59

```
Hello,
I am a new member but have been researching on line and reading this forum for a few months. I had the same issue with Dexter's site. Redirects to some other site. I use Norton 360. I ran all the scans and called Norton as well and had them do a complete scan of my machine. They told me my PC was fine. My Norton antivirus software would block my access to DIY site because it would try to load some kind of malware or spyware on my machine. I contacted Dexter about this problem several times and he just said he was sorry and he was aware that some of his customers were experiencing this issue. I don't blame Dexter but I think he has some serious security issues with his site which made me change my mind about buying from him and giving him my credit card information. So I purchased at a higher price from Enertion. I hope he sorts it all out as there are so few people that sell this stuff. I am going to look into the DNS virus you spoke of. If I have it, my antivirus is overlooking it and I want it removed from my PC.
```

---
## \#12 Posted by: rpn314 Posted at: 2016-12-20T18:36:38.633Z Reads: 55

```
You're antivirus is catching it properly. The problem, from what I've experienced, is that you're not actually getting to the real . Somewhere in the middle of you typing in the site in your browser and the request going around it gets sent to the wrong place, a dummy site, that IS filled with junk (and thus your anti-virus sounding the alert, as it should).

I agree that this is really annoying. I'd like to narrow down the issue once and for all and get it resolved. What happens when you put in the IP address directly? Just put in "67.222.5.32" into your browser and see if you get the site. That should be the directly IP address of DIY's site.

I'd also try running a tracert. It's a command that basically starts where you are and traces everywhere it takes you until the site is actually found, and makes a list. On your pc, just open command prompt and run "tracert ". When I run it, I get this:

<img src="/uploads/db1493/original/3X/0/c/0c05dec41bb1d927a0482f2c8a8dc59bf346b760.png" width="690" height="366">

Anyone on a mac who wants to try this as well, trace route is built into the Network Utility (a program that you'd just launch).
<img src="/uploads/db1493/original/3X/5/e/5e3c3235c09669f6de8b4874faa05181dbbfa365.png" width="662" height="500">
```

---
## \#13 Posted by: LAVAMAN Posted at: 2016-12-20T20:26:20.557Z Reads: 49

```
Thanks for the information. Is this something that Dexter can fix on his end? This is impacting his business and needs to be corrected. If I were him I would be pissed! If he owns the rights to his Domain name, this should not be happening. Maybe some of you guys on the forum that are IT types can give Dexter some advice as to how he can gain control of his Domain Name/IP address.
```

---
## \#14 Posted by: LAVAMAN Posted at: 2016-12-20T20:31:26.749Z Reads: 46

```
[quote="rpn314, post:12, topic:14259"]
67.222.5.32
[/quote]

For the record, when I type in IP address you provided, the site loads properly.
```

---
## \#15 Posted by: rpn314 Posted at: 2016-12-20T20:39:00.949Z Reads: 45

```
[quote="LAVAMAN, post:13, topic:14259"]
Maybe some of you guys on the forum that are IT types can give Dexter some advice as to how he can gain control of his Domain Name/IP address.
[/quote]

I am an IT guy...that's why I asked if you could do a trace route, so I can figure out exactly where the issue is and where it's pointing to the wrong place. I had the issue once, and I haven't had it for a while so I can't diagnose it anymore.

[quote="LAVAMAN, post:14, topic:14259"]
For the record, when I type in IP address you provided, the site loads properly.
[/quote]

That means the site is actually fine, and it's the transition from the "" to "67.222.5.32" that is the problem, and the trace route will show exactly what that transition is.
```

---
## \#16 Posted by: mmaner Posted at: 2016-12-20T20:44:57.675Z Reads: 43

```
Its most likely in the Name Server setup at his domain registrar.  Some registrars have crappy DNS, especially if the host is using virtual servers.  I would suggest that moving the domain name to network solutions and double checking the (A) records is the best course.
```

---
## \#17 Posted by: BoardSportsRN Posted at: 2016-12-20T20:47:28.403Z Reads: 43

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#18 Posted by: mmaner Posted at: 2016-12-20T22:02:13.926Z Reads: 42

```
The only reason I would doubt that is because it happened to me once my work desktop, i immediately went to my surface and got the same thing.  Both of these machines have empty host files.  Not saying that it couldn't be both, but its unlikely.
```

---
## \#19 Posted by: meercat Posted at: 2016-12-21T19:56:41.720Z Reads: 32

```
My company implemented new DNS-based security and DIY is now totally blocked (even by direct IP) due to "security". DIY *did* have a detected vulnerability back in Sept. (a Sucuri site check brought something back). It no longer shows that vulnerability, but the site may still be stuck in some block lists. That's my theory anyway. In the past, it's taken me months to get a client's site fully removed from all the various block lists it had gotten put on.
```

---

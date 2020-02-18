# FOCBOX Unity &amp; Enertion&rsquo;s Responsibility To Contribute to OS

### Replies: 56 Views: 1115

## \#1 Posted by: DerelictRobot Posted at: 2019-03-06T03:38:24.427Z Reads: 265

```
Hello all,

Recently I contacted Enertion support asking about the availability of the FOCBOX & FOCBOX Unity technical hardware schematics. I have purchased both controllers either directly from Enertion or through a licensed distributor.

I had looked to see if the latest version of the FOCBOX hardware schematics had been published on Enertion's GitHub account or on the forums but the latest I could find was v1.3.

I emailed Enertion support asking for these directly, and was told to two things.

1) That they had already released the latest FOCBOX hardware schematics on the forums. They provided these in their email response, but I couldn't help but notice the date on the Schematics was the same day of my request. Not sure on that, but I appreciate them providing them so I will refrain from further comment. 

2) I was told that the FOCBOX Unity was not a VESC derivative and therefore they would not be releasing the hardware schematics open source.

The exact response from Bara was:

"The Unity hardware will not be released as it is not based on the Vesc."

Topic 2 is what I would like to have a discussion on. I specifically asked for only the schematics, not the design files, as that aligns with the example that Vedder set with the lastest VESC6 release. For an embedded systems engineer such as myself, this is all I need to be able to contribute.

Now I feel it's pretty safe to say the original FOCBOX is clearly a derivative of VESC. I also feel it's safe to say that the FOCBOX Unity is a derivative design based on the original FOCBOX and by association, also a VESC derivative. 

I'm not going to talk about legality here. I'm going to talk about what I personally feel is right, based on the tenets of open source philosophy. The goal of these open licenses is to encourage innovation and collaboration from the community involved with the project, not to fork & isolate hardware so that it is no longer part of the original open source project. 

Given my experience in embedded systems as well as my contributions to the open source robotics community over the last decade, the claim that the FOCBOX Unity is not a VESC derivative comes across as inaccurate and potentially misleading, and I fear there's a clear conflict of interest here. 

@onloop I ask that you weigh in on this. 

You have benefitted monetarily on the open source work published by Mr. Vedder. I feel it is against the spirit of the open source work in which you have directly benefitted from to create a closed fork and not contribute your improvements. 

If you claim that the FOCBOX Unity is not a derivative of the FOCBOX, which is clearly a VESC derivative: I would be more than happy to volunteer my skillset to shedding some more light on this claim as I have a Unity in my possession and creating an empirical and quantifiable comparison to look further into this is well within my reach. It's about a weekend at most of my time, which I'd gladly donate to support the open source VESC project.

Thanks for taking the time to read. I hope my intentions here are clearly understood.
```

---
## \#2 Posted by: onloop Posted at: 2019-03-06T04:05:38.978Z Reads: 249

```
Thanks for your insight & feedback, I'm happy to try and answer your questions if you have any.

In the meantime please refer to Benjamin Vedders comments about hardware:

> _In the future we will publish the schematics for all official VESC hardware, but not necessarily the complete hardware layout with gerber files. The reason is that unlike the software, the hardware layout is not very reusable when creating new hardware. For example, for creating the VESC6 I made a completely new project in [KiCad](http://kicad-pcb.org/) and only looked at the schematic for HW4.12 to get started. Likewise, when working on a new high power layout that even looks similar to the VESC6 with the L-shape but with 18 MOSTEFs, I created a new project from the start. Once you know how to make a proper high power layout and are familiar with the awesome [KiCad](http://kicad-pcb.org/), it is just faster and simpler to layout everything from the start rather than moving things around. Therefore the software, tutorials and schematics are enough as a great base for making a wide variety of awesome motor controllers. Over 99% of the work is in the software, and the software can be adapted and reused to a great extent, which is why we think the right thing is to keep it free and open source._
> 
> _Another reason for not publishing the official hardware layouts as-is, is that it leads to many companies and individuals who have no background in electronics just giving a github reference to a manufacturer to make hardware and start selling it. Currently there are more than 25 places where V4.x hardware can be bought, with quality varying from excellent to not working at all. If the same thing would happen with the VESC6 it would be confusing for the customers. If you are serious about electronics, the VESC project provides everything you need to make your own custom hardware to fill a missing spot in the market, and then sell it. If electronics is not your area, but you want to sell your own hardware independently anyway, you can refer to the HW4.12 layout or wait for the three shunt reference PCB. We do however recommend and encourage that you get into electronics and design your own hardware if you are serious about what you are doing._

read more here: https://vesc-project.com/
```

---
## \#3 Posted by: b264 Posted at: 2019-03-06T04:07:57.687Z Reads: 239

```
I don't think he's asking about the gerber files.  I'm pretty sure he means the schematics.
```

---
## \#4 Posted by: DerelictRobot Posted at: 2019-03-06T04:10:02.922Z Reads: 237

```
That's correct. I specified I am not looking for the hardware layout. Only Schematics.

I was deliberate in this distinction. I completely understand Vedder's view on this and agree entirely.
```

---
## \#5 Posted by: onloop Posted at: 2019-03-06T04:12:01.293Z Reads: 235

```
We may release the schematic in the future. It's definitely something that has been discussed internally and we may need to revisit this if we are unknowingly in breach of some license or law.

We are not experts on the law regarding this matter, so feedback from the community is appreciated.
```

---
## \#6 Posted by: DerelictRobot Posted at: 2019-03-06T04:13:36.451Z Reads: 231

```
I also specified I'm not talking about the legality of this matter @onloop

I'm talking about the responsibility of contribution and doing what is right. I took time to write what I feel was a thoughtful post. Please take the time to read it, both of your responses so far show me you have not. 

If you do not understand what I'm asking, I'm more than willing to expand.
```

---
## \#7 Posted by: onloop Posted at: 2019-03-06T04:14:41.081Z Reads: 225

```
I read it, thanks for taking the time to put your thoughts down. 

I don't have much more to offer at the moment.
```

---
## \#8 Posted by: DerelictRobot Posted at: 2019-03-06T04:15:07.611Z Reads: 222

```
[quote="DerelictRobot, post:1, topic:86263"]
“The Unity hardware will not be released as it is not based on the Vesc.”
[/quote]

@onloop Could you respond to this then?

That was directly from Enertion support.

The claim is that the Unity is not a VESC derivative. My experience designing these kind of controllers for more than a decade leads me to believe that is not an accurate statement.
```

---
## \#9 Posted by: Blasto Posted at: 2019-03-06T04:18:00.073Z Reads: 214

```
We are able to read a datasheet by ourselves and did not use the vesc4 nor vesc6 schematic
```

---
## \#10 Posted by: onloop Posted at: 2019-03-06T04:21:50.289Z Reads: 216

```
I am not an Electronics Engineer, Nor am I the person who designed the Focbox unity, so I could be technically wrong and I am happy to be corrected.

What I do know is that the Unity is similar in the sense that it has similar components that are commonly used in vesc based motor controllers, it also uses similar code to make the components function as intended.

In saying this it is also unique, because it has new components and new code to make it function slightly differently.

Sorry for the layman's terms
```

---
## \#11 Posted by: Meeep Posted at: 2019-03-06T04:33:27.895Z Reads: 209

```
I could have sworn the Unity webpage used to say "Based on VESC™ Open Source Project." I'm not sure how to verify my claim. If this is true it is evidence that internal debate is occurring and actions are being taken. If I am mistaken I will remove this to avoid confusion. 

I've read through threads on the OS debate between Enertion and the community and while it's not my expertise (and frankly not my concern) I hope that the Unity can do more than unify two motor controllers.
```

---
## \#12 Posted by: DerelictRobot Posted at: 2019-03-06T04:38:17.214Z Reads: 200

```
I can do a bit more detailed comparison between the Unity and the FOCBOX when I land back stateside. 

Just as you are able to read datasheets, I don't technically need the schematics to do this work.

Really though, I think it's fair to say even without in-depth technical analysis that the Unity wouldn't exist without the FOCBOX, and the FOCBOX wouldn't exist without VESC. The technical details aside it very much so fits the layman definition of derivative work.
```

---
## \#13 Posted by: onloop Posted at: 2019-03-06T04:45:25.698Z Reads: 202

```
[quote="DerelictRobot, post:12, topic:86263"]
I can do a bit more detailed comparison between the Unity and the FOCBOX when I land back stateside.
[/quote]

That would be great, thanks for your interest in this project.

Definitely make a post about it, I'm sure there are other people who would apprecaite this too.
```

---
## \#16 Posted by: chaka Posted at: 2019-03-06T17:52:22.606Z Reads: 174

```
Is this a good time to mention the VESC was derived from instaspin? :exploding_head:
```

---
## \#17 Posted by: DerelictRobot Posted at: 2019-03-06T17:54:25.040Z Reads: 175

```
Always my friend!

Derivatives of derivatives of derivatives! How deep does this go?
```

---
## \#18 Posted by: chaka Posted at: 2019-03-06T17:58:24.732Z Reads: 174

```
As far as I am aware, we need only to maintain the use of TI processors to be in compliance with the instaspin tou's.
```

---
## \#19 Posted by: DerelictRobot Posted at: 2019-03-06T17:59:15.472Z Reads: 174

```
Maybe it's time for a purist TI-ESC. That's gonna need a fancy name though.
```

---
## \#20 Posted by: chaka Posted at: 2019-03-06T18:01:14.812Z Reads: 177

```
TEX-ESC??? :sunglasses:
```

---
## \#21 Posted by: trampa Posted at: 2019-03-06T18:20:13.452Z Reads: 179

```
Hi @DerelictRobot, I just read your post here on the Forum. People have asked questions like: Is the Unity more a VESC 4 or VESC 6 based design. 
 
VESC based design means it runs the Vedder code, since 98% of the work is in Software and not in Hardware. Benjamin can design a new ESC within a couple of days. The software takes years to code! Hardware wise you can create endless amounts of derivatives, just like smartphones running Android. Software might need to get more or less changes to run a hardware with changed components / Chipsets, but is not a big deal if you design your hardware wise enough.
 
If you open the Focbox UI, and click on the ABOUT button, you will see that the software is basically a fork of VESC TOOL, Copyright Benjamin Vedder. So yes, the UNITY is a VESC-based design! If it wasn't, it wouldn't need the Vedder Code, simple as that.

For Vedder, sharing knowledge is very important, since he himself learned a lot from open, shared  code, and in consequence he also wants others to be able to learn from his code. Code should be visible and usable. Writing code, interacting with hardware, ultimately means the hardware needs to be understandable as well. There is a link... 

At this stage UNITY is like a Computer that can only run a certain fork of Linux, due to a change in Chipsets. Such Computer don't really exist for a reason. Maintaining an operating system fork for dedicated devices is even to much work for bigger players. Windows RT was binned soon after its introduction - to much work to maintain, to much extra work for App developers.
Jeffrey now has a lot of work on his table because Benjamin coded a major update.
Once Jeffrey nailed that he can start all over again, since the next big update will happen sooner than later. 
Sure, Unity is a bit cheaper to make because it saves 2,5$ on a second processor, but I guess that the workload to adopt the software all the time outweighs the cost savings big time. 

VESC-Tool is progressing faster in future, and it will naturally support a wide range of different hardware configurations. It will always stay fully backward compatible.
People want to be able to use new features, upload the latest and greatest FW, be sure to have bug fixes sorted reliably through the power of the many eyes principle and the main man behind the 20K+ pages of source code. A lot of people also have different controllers in different boards and bikes and robots. In the end they want one consistent software solution to deal with all of them. 

Read more about it here:
https://vesc-project.com/Ethos
```

---
## \#22 Posted by: DerelictRobot Posted at: 2019-03-06T18:26:53.006Z Reads: 175

```
[quote="trampa, post:21, topic:86263"]
VESC based design means it runs the Vedder code, since 98% of the work is in Software and not in Hardware. Benjamin can design a new ESC within a couple of days. The software takes years to code!
[/quote]

Hear fricken hear. 

Exactly my point in that these kind of things can be reverse engineered on the hardware side in very little time at all. And exactly why I think it's strange that there's so much emphasis on trying to keep the hardware design under wraps (especially given that it's all derivative anyway).

Thank you for chiming in.
```

---
## \#23 Posted by: Deodand Posted at: 2019-03-06T19:39:32.218Z Reads: 172

```
[quote="DerelictRobot, post:22, topic:86263"]
these kind of things can be reverse engineered on the hardware side in very little time at all.
[/quote]

**Exactly, If you know what you're doing.** I consider it the entrance exam if you want to make a clone/variant of the unity. I already did and released all the challenging parts making the FW support dual motors. If they aren't even willing to put in a small amount of effort making a schematic, how good can we expect this new product they create to be? 

In your super long post, I don't really see any good motivations for why you need the schematic? We've had long discussions on the trade-offs here and I'd love to hear some other ideas on how releasing the schematics would help our customers. The main one I can think of is repair but we handle repairs pretty well as is and are more than happy to advise our customers if they want to go the DIY route. 

@trampa what's with the constant jabs in unity threads? I looked through vedder's new update some really cool stuff in there if you want to use your vesc to drive subwoofers or chain a bunch together in a quadcopter. Also some improved calibration for motors that aren't used in eskate. Really fun ideas and you can tell Vedder is super passionate about using the VESC in other platforms which is awesome. You keep quoting 20,000 lines of code though and how much better the vesc will work for eskate after the new update. But after looking through I draw the same conclusions as @Ackmaniac, the bulk of these updates doesn't really do much for our application. 

The main changes which apply to eskate are better support for dual/4wd setups over CAN-bus (**Unity did this**), improved flux-linkage detection (**Unity did this**), an automated motor detection routine to make things faster and easier (**Unity did this**), a braking fix for a bug that I found,  as well as an app that has some baseline functionality but still has a long way to go regarding bugs/dropouts etc. He did all of these in different ways from my methods but the core ideas are the same.  From the perspective of eskate, the VESC update was catching up to the ways the unity pushed forward, and not the other way around. We'll continue pioneering forward and don't need to spend too much time looking sideways as I'm passionate about the eskate application and want to create the best possible experience for our customers.
```

---
## \#24 Posted by: DerelictRobot Posted at: 2019-03-06T21:57:50.948Z Reads: 164

```
[quote="Deodand, post:23, topic:86263"]
**Exactly, If you know what you’re doing.** I consider it the entrance exam if you want to make a clone/variant of the unity. I already did and released all the challenging parts making the FW support dual motors. If they aren’t even willing to put in a small amount of effort making a schematic, how good can we expect this new product they create to be?
[/quote]

That's great that you have your own opinions, I have mine.

In **my** opinion, it's not up to **you** to determine whether or not to contribute to an open source project which you and your employer are financially benefiting from. 

[quote="Deodand, post:23, topic:86263"]
In your super long post, I don’t really see any good motivations for why you need the schematic?
[/quote]
 
I thought I made it pretty clear that I don't actually need the schematic personally. 

What motivations do I need to convince you to do right right thing?

Are you not benefiting from derivative work and now trying justify why you should not have to contribute? It doesn't work that way kid.

I'm not doing this entirely for myself, I'm doing this on good principle because not everyone has the skill set and experience backing their continued efforts towards learning that I do. 

I am making this request because you are getting paid based on an _enormous_ body of someone else's work, and your employer has openly stated he doesn't believe in Open Source and doesn't care about it.

What you are doing is moving the goalposts and justifications for as to why you don't think you should have to contribute back, and that is wrong. Furthermore you have a conflict of interest because you're currently lining your pockets off a **closed fork**, for someone who doesn't have any respect or understanding for the amount of work that goes into development like this.

If you don't understand why this is immoral, I'm not sure what to tell you there champ.

This post comes across as defensive, and ultimately you have zero ground to stand on and your stance towards this would be torn apart within a larger open source community. Go float the question elsewhere and see the response, I encourage it. 

If you do not believe you have a moral (and legal) obligation to pay it forward and give back to the community which you're now making a living off of, then you have a lot to learn beyond the under-grad levels of Electrical Engineering it takes to design something like this. 

Pretty disappointing response from you. I had hoped you came into this sport & community with a bit more open mind, and a bit less arrogance & possession over something you did a fractional amount of work on compared to those that came before you.

The idea that knowledge should be withheld is one of the very core tenets of malicious control.
```

---
## \#25 Posted by: b264 Posted at: 2019-03-06T22:23:26.586Z Reads: 154

```
[quote="onloop, post:5, topic:86263, full:true"]
We may release the schematic in the future. It’s definitely something that has been discussed internally and we may need to revisit this if we are unknowingly in breach of some license or law.

We are not experts on the law regarding this matter, so feedback from the community is appreciated.
[/quote]

The law says you must release the circuit schematics, the source code for the firmware, the source code for the GUI if derived from BLDC Tool or VESC Tool, but not the PCB gerber files or the design (aesthetics) files.
```

---
## \#26 Posted by: topcloud Posted at: 2019-03-06T22:26:24.883Z Reads: 151

```
Correct.  Watching this thread, now.
```

---
## \#27 Posted by: Deodand Posted at: 2019-03-06T22:28:26.031Z Reads: 155

```
[quote="DerelictRobot, post:24, topic:86263"]
I’m not sure what to tell you there champ
[/quote]

[quote="DerelictRobot, post:24, topic:86263"]
doesn’t work that way kid
[/quote]

[quote="DerelictRobot, post:24, topic:86263"]
someone who doesn’t have any respect
[/quote]

[quote="DerelictRobot, post:24, topic:86263"]
beyond the under-grad levels of Electrical Engineering
[/quote]

First off, can you try and remain polite and professional? Not sure why you feel the need to take such an aggressive tone, I can assure you it doesn't further your goal. It is important that people don't conflate the open-source requirements of the hardware vs. the software but I'd love to see a discussion of exactly how those apply here. For instance pretty much all vesc variants/flavours have changes within them and have no official schematics released as there is mostly just the reference schematic for the 4.12 and an old schematic of the vesc 6 before it was formally released, if this is an issue it is more widespread than an enertion and should be looked at in that context.
```

---
## \#29 Posted by: DerelictRobot Posted at: 2019-03-06T22:35:34.002Z Reads: 157

```
[quote="Deodand, post:27, topic:86263"]
First off, can you try and remain polite and professional?
[/quote]

Sorry, willful ignorance & arrogance from someone profiting off someone else's open source work tends to get me a little salty. I'll use nicer words if they offend you, but I'm not a big fan of censorship and this is a topic I'm deeply passionate about. Ignorance is no excuse on your part.

[quote="Deodand, post:27, topic:86263"]
Not sure why you feel the need to take such an aggressive tone, I can assure you it doesn’t further your goal. It is important that people don’t conflate the open-source requirements of the hardware vs. the software but I’d love to see a discussion of exactly how those apply here.
[/quote]

You clearly don't understand. And that's fine. Maybe this topic will enlighten you.

There's a difference between doing the bare minimum to meet 'legal requirements' and dragging your feet along the way, and doing something **with the intent of contribution and free sharing of knowledge**. 

How long was Enertion in violation of the OS license? Did it not taken legal pressure from Vedder himself to get them to finally release the Source Code?

They didn't do it out of good will or to benefit the community, they did it because they were finally left with no other choice.

Just how they're willing to release the original FOXBOX schematic only now, after it's no longer being sold. If you don't see that as BS, I sincerely do not know what to tell you.
```

---
## \#30 Posted by: Deodand Posted at: 2019-03-06T22:37:34.162Z Reads: 149

```
The focbox schematic has always been available actually,  under the hardware reference files download from their website. I remember looking at like a year ago or more.
```

---
## \#31 Posted by: DerelictRobot Posted at: 2019-03-06T22:39:55.889Z Reads: 150

```
[quote="Deodand, post:30, topic:86263, full:true"]
The focbox schematic has always been available actually, under the hardware reference files download from their website. I remember looking at like a year ago or more.
[/quote]

Then why could I only find v1.3/4? 

And when I requested it from Enertion they sent me a 1.7 with the same date as the day I'd requested it on.

Wouldn't it make more sense to point me to the existing link? (They didn't, they generated a new file).

Why isn't all of this just on your Enertion Github repo?
```

---
## \#32 Posted by: JohnnyMeduse Posted at: 2019-03-06T22:43:57.935Z Reads: 150

```
[quote="DerelictRobot, post:31, topic:86263"]
And when I requested it from Enertion they sent me a 1.7 with the same date as the day I’d requested it on.
[/quote]

They could send you a letter with a paper version of the schematic... and still comply to the GPL licence. 

The only thing that need to be share on a open source is the file you use and remix... If they didn't use Vedder schematic they don't need to make it open source... Look at Flipsky.. Maytech.. and other, they should be sharing there schematic since it is a remix from the original. Why aren't you putting your effor them?

Let me guess... Because they aren't Enertion... If you want the greater good of the community, you should also go after them.

But you just want to rub you dick in Jason face...
```

---
## \#33 Posted by: DerelictRobot Posted at: 2019-03-06T22:46:04.324Z Reads: 149

```
Who says I haven't requested the same of them?

[quote="JohnnyMeduse, post:32, topic:86263"]
The only thing that need to be share on a open source is the file you use and remix… If they didn’t use Vedder schematic they don’t need to make it open source…
[/quote]

You should read up on this topic before making assumptions. I encourage it. 

And please don't place words in my mouth. 

[quote="JohnnyMeduse, post:32, topic:86263"]
But you just want to rub you dick in Jason face…
[/quote]



And please leave Jason's and my own penis out of this.
```

---
## \#34 Posted by: JohnnyMeduse Posted at: 2019-03-06T22:48:16.697Z Reads: 145

```
[quote="DerelictRobot, post:33, topic:86263"]
You should read up on this topic before making assumptions. I encourage it.
[/quote]

Maybe it is you who should read more...
```

---
## \#35 Posted by: topcloud Posted at: 2019-03-06T22:53:45.651Z Reads: 145

```
How about this, guys.

@b264 is correct

@deodand could you, in good-faith, post links to the schematics, along with the source, and put this issue to rest?

To be clear: nobody here wants Enertion technology and we understand Enertion relies on Unity sales for income. 

This isn't an anti-Enertion thing; this is a pro-community thing.  

@JohnnyMeduse is also correct, there's no guarantee or SLA on this stuff.  We just expect more as the community.

Can we keep those two things separate and focus on the resolution - and avoid further escalation?
```

---
## \#36 Posted by: DerelictRobot Posted at: 2019-03-06T22:54:01.720Z Reads: 149

```
Wow. Flagging posts to censor now are we. Seriously guys? This isn't the first time this has been abused.

Do we need to call Mom in here?

My post was entirely relevant to this, I was showing an example of open source releases as I feel they should be done. 

https://www.electric-skateboard.builders/t/focbox-unity-enertions-responsibility-to-contribute-to-os/86263/28?u=derelictrobot

Censoring someone because you disagree with them only furthers my points made here. Christ. Be better than this. 

![image|690x427](upload://tiD7n0nGylYntYzwAB2JeZ5NaOt.png)
```

---
## \#37 Posted by: dareno Posted at: 2019-03-06T23:03:54.790Z Reads: 139

```
How is providing background and expertise to back up a thread off topic?
```

---
## \#38 Posted by: DerelictRobot Posted at: 2019-03-06T23:06:50.587Z Reads: 140

```
It isn't. But censorship seems to be a common theme here.
```

---
## \#28 Posted by: onloop Posted at: 2019-03-06T23:26:36.550Z Reads: 108

```
A post was split to a new topic: [I make open source robots](/t/i-make-open-source-robots/86368)
```

---
## \#39 Posted by: venom121212 Posted at: 2019-03-06T23:39:41.779Z Reads: 138

```
Can't we all get along? We need more unity :smirk:
```

---
## \#40 Posted by: banjaxxed Posted at: 2019-03-07T00:17:06.124Z Reads: 135

```
Every day guys? this stuff is destroying the quality trolling 😏
```

---
## \#41 Posted by: trampa Posted at: 2019-03-07T00:26:52.570Z Reads: 144

```
Relax everyone! This is getting pretty emotional. 
Benjamin has an ethos page up for a reason. Read through it with care and try to understand the motivation. 
The amount of work Vedder dropped into the code base is overwhelming, and without his effortless work our boards would probably still be rolling on RC-Car ESCs. He was friendly enough to share all of his efforts with the world and applied the GPL to his enormous code base and schematics. The idea behind it is to help others to gain knowledge for their own projects and allow integration of code into their own developments. Open source is all about sharing ideas and solutions to problems, so that everyone can learn from another. Spreading knowledge helps the world to get smarter and hopefully better. At least it helps to understand how thing actually work, in a time where code is taking massive control over our lives. Even this Forums software is OS! 
OS also means to be respectful, simply because developers rely on respect when the code is in the public domain. Code developers also need financial support to allow them to spend more time on writing more code. Open source doesn't necessarily translate to "free of charge for takeaway". 

If you run a fork with substantial changes, people should at least be given a chance to design their own hardware to work in combination with the changed code base. That is my opinion. 

Please remember: Without Benjamin's openness there would not have been any VESC derivate at all. No nothing to base anything on!

I will meet Benjamin on Friday night, and will ask him about his opinion. I think his opinion should be taken into account, since he spent years of coding the software that allows us to skate the way we skate today and allowed @Deodand to design a derivate of the soft- and hardware.
```

---
## \#42 Posted by: DerelictRobot Posted at: 2019-03-07T00:29:26.917Z Reads: 141

```
[quote="trampa, post:41, topic:86263"]
He was friendly enough to share all of his efforts with the world and applied the GPL to his enormous code base and schematics. The idea behind it is to help others to gain knowledge for their own projects and allow integration of code into their own developments. Open source is all about sharing ideas and solutions to problems, so that everyone can learn from another. Spreading knowledge helps the world to get smarter and hopefully better.
[/quote]

This is one of the best things you've written on these forums. 

Thanks for your insight and contributions here.
```

---
## \#43 Posted by: twan Posted at: 2019-03-07T00:36:03.128Z Reads: 136

```
Soo where I find the focbox schematic anyways. I have a burnt part that I would like to replace 😂
```

---
## \#44 Posted by: JohnnyMeduse Posted at: 2019-03-07T00:39:08.064Z Reads: 137

```
Which Parts?
```

---
## \#45 Posted by: twan Posted at: 2019-03-07T00:41:06.919Z Reads: 136

```
Well not burnt is just straight up missing lol! It's on the reverse side of the micro USB port.
```

---
## \#46 Posted by: JohnnyMeduse Posted at: 2019-03-07T00:45:07.627Z Reads: 137

```
The crystal ? (like 4 blank pads) it is an Crystal 8MHz, 10PPM same one use on regular Vesc. Here is the part number for mouser 815-ABM3B-8.0-10-1UT

or if it is one of the cap C15-C38 they are 15pF and C35 is a 2,2uF
```

---
## \#47 Posted by: twan Posted at: 2019-03-07T00:47:00.373Z Reads: 136

```
Wow thank you! No wonder why USB would not connect
```

---
## \#48 Posted by: mmaner Posted at: 2019-03-07T02:39:49.791Z Reads: 126

```
Maybe this would be put to rest if Ben himself came here and voiced his opinion instead if using a mouthpiece.
```

---
## \#49 Posted by: DerelictRobot Posted at: 2019-03-07T02:47:15.543Z Reads: 125

```
I've been told by Jason that my opinions on open source aren't welcome here, so I'm gonna sit back and let you guys handle this for now. 

CHEERS MATES!
```

---
## \#50 Posted by: mmaner Posted at: 2019-03-07T02:58:26.690Z Reads: 129

```
Censorship in this context is at best not cool and at worst malicious. Whoever flagged the post should be ashamed. 

[quote="b264, post:25, topic:86263"]
The law says you must release the circuit schematics, the source code for the firmware
[/quote]

Only if it's a VESC derivative. Enertion has claimed that the Unity is not, that issue needs to be put to bed before this issue is brought up again. 

[quote="DerelictRobot, post:24, topic:86263"]
Are you not benefiting from derivative work and now trying justify why you should not have to contribute? It doesn’t work that way kid.
[/quote]

Manners and respect. I know emotions run high especially with topics we are passionate about, but manners and respect. 

[quote="JohnnyMeduse, post:32, topic:86263"]
Let me guess… Because they aren’t Enertion… If you want the greater good of the community, you should also go after them.
[/quote]

This makes assumptions that haven't been stated by anyone and is not conducive to a profitable discussion. It is in fact argumentative, if that's the objective ok, but it didn't help anybody. 

The biggest issue I see here is people starting opinions as fact, making assumptions and treating then as facts. Kind of like this...

[quote="trampa, post:41, topic:86263"]
would probably still be rolling on RC-Car ESCs.
[/quote]

That:s marketing not fact.  The fact is there are plenty of controllers out there that do the job just fine, some better like the Arc 200. 

[quote="trampa, post:41, topic:86263"]
OS also means to be respectful, simply because developers rely on respect when the code is in the public domain.
[/quote]

That's a pretty thought, but once again not a fact. 

[quote="trampa, post:41, topic:86263"]
I think his opinion should be taken into account, since he spent years of coding the software that allows us to skate the way we skate today
[/quote]

This entire sentence is loaded with hyperbole and is the root of what's wrong with this discussion. 

I honestly don't see how anything gets done with all the bitching that goes on. The fact that this is an issue in the open is telling in itself, there's bound to have been tons of legal correspondence, if history is any guide, which apperantly hasn't done any good or the topic wouldn't be openly discussed here. 

In closing, from a user and esk8 enthusiast...  Y'all need to grow the fuck up and stop measuring your dicks in public. Your not helping the community, your actively harming it and most of us are tired of it.
```

---
## \#51 Posted by: BigZwatt Posted at: 2019-03-07T03:08:06.805Z Reads: 122

```
Yeah chaka I like tex esc.
```

---
## \#52 Posted by: SeanHacker Posted at: 2019-03-07T03:12:27.881Z Reads: 122

```
I wanted this thread to stay about opensource and what that brings to the table for EVERYONE. Seems like every time the words opensource and Enertion are mentioned, people get silenced, threatened to be banned, ect... It's pathetic and should stop. It's only hindering the progress. 

Seems like there's a few select people here that just don't get that it's beneficial for everyone involved. We can all make money if that's the end goal. Although moving FORWARD with more advanced technology is ultimately the goal in the world of opensource. Try not to forget that.
```

---
## \#53 Posted by: mishrasubhransu Posted at: 2019-03-07T03:16:35.086Z Reads: 124

```
I 100% second this. 

I find it so strange that people are trying to undermine the work that went into this and the fact that it was made opensource. I guess emotions and bias gets the best of us and logic is just kicked aside.
```

---
## \#54 Posted by: trampa Posted at: 2019-03-07T19:26:39.246Z Reads: 115

```
[quote="mmaner, post:50, topic:86263"]
Censorship in this context is at best not cool and at worst malicious. Whoever flagged the post should be ashamed.
[/quote]

Thx for these words! I don't believe in censorship as long as it's no hate speech or propaganda with bad intentions.

Hope that on www. things are handled differently.
```

---
## \#55 Posted by: mmaner Posted at: 2019-03-07T19:37:46.324Z Reads: 117

```
[quote="trampa, post:54, topic:86263"]
propaganda with bad intentions.
[/quote]

Really?  Because I can quote a never ending string of posts that are full of propaganda that you authored.  

[quote="trampa, post:54, topic:86263"]
Hope that on www. things are handled differently.
[/quote]

Speaking of propaganda, FFS.  I assume they will be handled just like they are here, as the situation arises.
```

---
## \#56 Posted by: topcloud Posted at: 2019-03-07T20:20:01.797Z Reads: 115

```
Love you like a brother Mike, and I’m asking us all to let the past go. 

Please. We all get better with time, and when we let the past rule our present the future gets real hard to see. 

I’ve asked Trampa to start sponsoring races, and they returned inmediately with a new head of Ambassadors, Matt Evans. 

Great guy, knows the track, and I’ve agreed to help develop two new female uphill racers, whom I expect will be on our Instagrams by end of Summer, if successful. 

I realize I’ve only been here since Derek invited me, and I was not part of the contention over IP in the past. 

Yet it is the past, brother.

I admire how you take up for Enertion, very much.
```

---
## \#57 Posted by: mmaner Posted at: 2019-03-07T20:50:41.164Z Reads: 114

```
[quote="topcloud, post:56, topic:86263"]
I’ve asked Trampa to start sponsoring races, and they returned inmediately with a new head of Ambassadors, Matt Evans.
[/quote]

that's awesome.  

[quote="topcloud, post:56, topic:86263"]
I admire how you take up for Enertion, very much.
[/quote]

I'm NOT taking up for Enertion, honestly I'm not.  It just seems that every time Frank quotes me its out of context or complete crap.  I swear he does it on purpose just to irritate me :slight_smile:.
```

---
## \#58 Posted by: topcloud Posted at: 2019-03-07T20:58:09.339Z Reads: 110

```
You’re the man. Mean it. -karl
```

---

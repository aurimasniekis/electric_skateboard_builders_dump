# Enertion VESC - solutions to problem

### Replies: 17 Views: 1919

## \#1 Posted by: alexmarin99 Posted at: 2016-08-30T18:43:38.761Z Reads: 162

```
Hello everyone!

So I've bought a VESC from Jason and I've received it. I've plugged it in, did all the settings and proceeded to click detect motor parameters. Red led light came on and nothing else. So I've re-checked all the wires and settings, everything was good, but it still didn't work.

So then I've contacted Enertion Support and they told me I have to buy a warranty so they can replace  the VESC... Which I don't find correct because the VESC never worked.

Anyways, what can I do? Do you have any advice?

Thank you.

Alex
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-30T18:47:32.001Z Reads: 162

```
You should have 2 months of warranty for it by default but you'll have to talk to Enertion about that. For now run detection again and go to the terminal tab and type "faults". It should list any faults you have on the VESC
```

---
## \#3 Posted by: alexmarin99 Posted at: 2016-08-30T18:48:49.455Z Reads: 159

```
This is what is written:

<img src="/uploads/db1493/original/2X/5/594e61587f628354c327d859bdb6ab822328af1c.png" width="368" height="272"><img src="/uploads/db1493/original/2X/6/6fe984d2e7138bde484835bf5f2a21868eecf870.png" width="371" height="274">
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-30T18:51:24.451Z Reads: 154

```
Sounds like a busted DRV. If so, you'll need to swap it out or get it replaced (or the whole VESC if Enertion wants to do that). Could you take a look at it and see if you see any burn marks on the DRV itself? It's the rectangle piece in the middle here

http://www.electric-skateboard.builders/uploads/db1493/original/2X/d/d8fccff96bda7a90a3cffbce2fce5ae89d1566d1.JPG
```

---
## \#5 Posted by: evoheyax Posted at: 2016-08-30T18:53:14.489Z Reads: 153

```
First, you need to check the fault code by connecting your vesc to your computer (via usb), going to the "live data" tab, and clicking "activate sampling". There's a bunch of data that will now change under the graph, and one of those says "fault code:". Tell us what that fault code is and it may be just your settings that need to be changed. A classic example is you could just be powering your vesc with a voltage outside of the range you set in the first page of settings (the min and max voltages).

If it's physically broken (which we can determine biased on the fault code), then it's nothing more than an expensive paper weight. You won't get any service unless you pay for the premium.

EDIT: you beat me to it @Jinra haha.

Yea, your pretty much screwed, buy a new one from chaka, and this will likely never happen again, and if it does, chaka repairs vesc bought from him for free or at a little charge. As a forum, we have gone through huge fights over and over about the vesc, and chaka has shown he has made changes to the vesc that seem to make it more stable/less likely to break.
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-30T18:55:04.990Z Reads: 148

```
His fault code is above ^
```

---
## \#7 Posted by: alexmarin99 Posted at: 2016-08-30T18:59:46.479Z Reads: 150

```
Yes I know where it is. I've assembled a complete VESC by myself from scratch.

There are no burn marks whatsoever on anything.
<img src="/uploads/db1493/original/2X/1/16cece6e7b550b720b1808b457d4d513e997a982.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/1/1ad5015080081137984e8c214dfadcb69a340768.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/8/85848f2fb4d06f244d323b416a763aabe6878976.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/a/a1d7734382b4f33110e8329265843997e429d782.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/e/eb8acc39fe807ea8f431b6b00829ccb2006f1c7e.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/5/5085620fa64e7d74fefd5b712078315c446927ae.jpg" width="666" height="500">

EDIT:

Some of the wrap was removed so I could take a clearer picture of the components.
I can remove all of the wrap and take other pictures if anyone wants to see more!
```

---
## \#8 Posted by: Michaelinvegas Posted at: 2016-08-30T19:01:36.399Z Reads: 140

```
@EnertionSupport pleas step in
```

---
## \#10 Posted by: Karmannghiagirl Posted at: 2016-08-30T19:50:31.018Z Reads: 133

```
honestly if i just bought vesc and it didnt work, i wouldn't just want someone to fix it, I would want the company that i bought it from to step up and help.

So nothing against you, but i bet he just wants a working vesc from enertion (which is what he paid for).
```

---
## \#11 Posted by: sl33py Posted at: 2016-08-30T19:54:00.347Z Reads: 130

```
If you've built a VESC from scratch, and @Blasto has offered to help fix - why not replace the DRV yourself?

I get what @Karmannghiagirl is saying for sure.  I'd want a working VESC from the get-go as well.  BUT shit happens and DRV chips just fail sometimes.  Instead of several days each way shipping and waiting to ride, i'd get the DRV swapped myself and be riding sooner.

Maybe @EnertionSupport can comment if this would be ok or void any "out of the box" warranty.  Which should exist if it simply doesn't work the first time connected.  14 days or whatever.
```

---
## \#12 Posted by: Cisphyx Posted at: 2016-08-30T21:11:18.281Z Reads: 108

```
I just got an Enertion VESC and had the DRV blow in under 15 minutes of use. Haven't heard back from support yet, but your post isn't giving me a lot of hope.
```

---
## \#13 Posted by: ra.rend Posted at: 2016-08-30T21:35:02.653Z Reads: 107

```
I sent mine back to be repaired. They've had it for 4 weeks now. Every week I emailed them about it. They've finally "added it to the system" yesterday. Good luck
```

---
## \#14 Posted by: Cisphyx Posted at: 2016-08-30T22:00:07.678Z Reads: 108

```
Yeah I actually ordered a bunch of DRV8302s and some various capacitors to upgrade some places on the board. I'd rather just do the repairs myself if they aren't going to send a replacement, I'd like to use it again this year.
```

---
## \#15 Posted by: onloop Posted at: 2016-08-30T22:16:22.966Z Reads: 99

```
Check this post:
http://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672

Also note. Their is a firmware bug that blows you vesc if you change the settings several times it will cause faults.

We offer a vesc-platinum this product has a 12 months replacement warranty for any fault. We send a new one out instantly. This vesc is priced very competitively and still lower than most competitors.

We also sell the vesc standard. The warranty & support is VERY limited. If you want us to do anything it will require you to return the item for review. It can take 4-6 weeks. If we need to replace parts there will be a charge and some labour charges too.

Otherwise we sell a warranty separate which can be purchased now and then we send a new vesc.

Eitherway you chose you can have your problems resolved. It's just a question of how long you are willing to wait. Faster costs more.
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-30T22:18:35.858Z Reads: 99

```
Hey Jason,

Is your factory loading the bug-free firmware now? Just a thought to save you some headaches ;)
```

---
## \#17 Posted by: onloop Posted at: 2016-08-30T22:19:35.885Z Reads: 97

```
Yes.... they have been loading it for a few weeks. 

But just incase everyone should update firmware
```

---
## \#18 Posted by: onloop Posted at: 2016-08-30T22:26:28.412Z Reads: 94

```

```

---

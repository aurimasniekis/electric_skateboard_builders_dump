# Hot air/ reflow station recommendations

### Replies: 11 Views: 1144

## \#1 Posted by: barajabali Posted at: 2017-02-13T17:14:31.583Z Reads: 102

```
We have a similar thread for soldering stations. I'm looking to build anti-spark switches.  The PCB is easily accessibly as well as the BOM parts.  The only issue i'm having is getting a hold of the right tools for the job.  Ideally i'd like to be able to make switches from scratch and potentially fix/replace mosphets on the vesc and other minor things. 

What do you guys with more 'small scale' electronics experience recommend for me? A hot air station?  reflow oven?
```

---
## \#2 Posted by: Sander Posted at: 2017-02-13T18:22:06.157Z Reads: 98

```
I recommend this Airflow Station. Been using it for a while:
<img src="/uploads/db1493/original/3X/b/8/b899ba99e4c7bf8826175bd230e51f057377c050.jpg" width="690" height="430">
Name: CSI 853B+ Digital Preheater Station with Hot Air Rework Option
Temperature Range/Hot Air: 100-480 deg C
Comes with adjustable temperature and air speed.

But if you live in a different country like mine that has 220/230VAC not 110VAC you need to find the 220/230VAC version. And ask them if they have the right socket for your wall.

[CSI 853B+ Digital Preheater Station with Hot Air Rework Option](https://www.circuitspecialists.com/csi853bplus.html) 
**Price: $129.00**

---

And you should get a pair of tweezers if you havent gotten any from before:
<img src="/uploads/db1493/original/3X/6/3/6347f8b5796005c170cbbc89351f38fb540445a0.jpg" width="300" height="300">
[Stainless Steel Anti Static Anti Magnetic Precision Tweezer Set](https://www.circuitspecialists.com/tweezer-set.html)  
**Price: $7.99**

----

This some of the Result(Keep in mind it was my first time Air Soldering):
<img src="/uploads/db1493/original/3X/7/5/7527101dea10f2bc6ed55e22ee960698a06bf3fc.jpg" width="375" height="500">

[quote="barajabali, post:1, topic:17648"]
i'd like to be able to make switches from scratch and potentially fix/replace mosphets on the vesc and other minor things.
[/quote]

[quote="barajabali, post:1, topic:17648"]
reflow oven?
[/quote]

Better with hot air station if you are going to fix/replace circuits components. Not quite possible with the Reflow Oven, would been a challenge.
```

---
## \#3 Posted by: 3sly Posted at: 2017-02-13T18:35:43.480Z Reads: 80

```
I was thinking of buying one myself. But then found out that the solder paste costs about 30 euros and is only good for max 6 months in a fridge.
```

---
## \#4 Posted by: barajabali Posted at: 2017-02-13T18:37:06.585Z Reads: 76

```
Thanks a lot man! I stumbled upon that one before .  I really appreciate the advice and all of the links !! it helps alot. 

@3sly  Which paste are you talking about?  Can you add a link to it?
```

---
## \#5 Posted by: Sander Posted at: 2017-02-13T18:42:23.723Z Reads: 76

```
Just to point this out, many people recommend this solder paste:
<img src="/uploads/db1493/original/3X/b/5/b5607c9827b68dc001b54e74e32b6b648df942d1.jpg" width="500" height="500">
[Solder Paste - 50g (Lead Free)](https://www.sparkfun.com/products/12878)
**Price: $16.95**
---
_Some of the reviews:_
Finding the right solder paste for small SMD rework applications was tricky, until I found this product. It’s easy to work with, and goes a long way.

Used it to solder all my SMD with hot air. This quantity is enough to do thousands of clean solder. use it and never revert back to awkward “classic” soldering

-----

But I can't really say anything about it yet haven't used it yet. Its chilling in my fridge :)
```

---
## \#6 Posted by: barajabali Posted at: 2017-02-13T18:45:03.215Z Reads: 72

```
Beautiful. I'm so happy I made this thread. You answered all of my questions and hopefully you engligtened people to stumble upon this in the future
```

---
## \#7 Posted by: okp Posted at: 2017-02-13T20:21:55.137Z Reads: 64

```
looks great ! what temperature did ya set the hot air station to ?
```

---
## \#8 Posted by: Sander Posted at: 2017-02-13T20:34:47.754Z Reads: 60

```
[quote="unik, post:7, topic:17648"]
what temperature did ya set the hot air station to ?
[/quote]

I mainly use 350-400C ;)
```

---
## \#9 Posted by: okp Posted at: 2017-02-13T20:40:08.123Z Reads: 58

```
how do you apply the soldering paste on the PCB ? a little needle ? 

do you use a flux pen too?
```

---
## \#10 Posted by: Sander Posted at: 2017-02-13T20:47:19.615Z Reads: 60

```
[quote="unik, post:9, topic:17648, full:true"]
how do you apply the soldering paste on the PCB ? a little needle ?

do you use a flux pen too?
[/quote]

I buy my circuits with stencil so I just apply over the stencil. If not a needle would be a great idea. Maybe the white things for your ear wax would work too? I have experienced some bridging with not using a stencil. 
[Stencil Oshpark](https://www.oshstencils.com/)

Yes I use a flux pen too. But I don't think its really necessary ;)
[Rosin Flux Pen](https://www.circuitspecialists.com/835-p.html)
```

---
## \#11 Posted by: sl33py Posted at: 2017-02-13T21:01:05.891Z Reads: 60

```
I don't use stencils yet - want to some day - but use the solder paste in syringe dispenser:

https://www.amazon.com/MG-Chemicals-Solder-Paste-Clean/dp/B00TIC895Y

So far it works great for both hot air rework and reflow oven.  Maybe slower, but the small 1.2oz/34g seems to go a long way...

I always clean w/ some denatured or rubbing alcohol before applying paste.

My recommended hotair solder station is similar to one of these:

https://www.amazon.com/Zeny-Soldering-Station-862D-Nozzles/dp/B00W1AG0FG

I have a similar one to this.  I think i got it for about $100 a few years back - best money spent on DIY in a long time!  Recommend you don't misplace/lose the small nozzles to focus hot air when doing small smd work.  You can also use kapton tape (sp?) to block/fence-off areas you don't want to heat and reflow.  Important to keep airflow down so you don't reflow components you don't want - and the lower airflow to avoid pushing those working components off their pads when replacing the defective component!  The tape can help block and hold stuff in place.

HTH - GL!
```

---

# Bypassing discharge on a 10s bms&hellip; HELP

### Replies: 21 Views: 1662

## \#1 Posted by: achatham Posted at: 2018-05-27T01:26:14.257Z Reads: 155

```
I’ve read the previous forums on other people’s setups but am still feeling like an idiot as I’m STILL not sure as how to bypass discharge on the bms. I basically have 2 5s lipos wired to the bms with a single wire connected to the B- I believe is what it is (opposite side of the charge hole on the bms in the top right corner). So if anyone can help me with this, we’d be forever friends.

If you need more info, I don’t mind posting pics, videos or whatever it takes to get the job done.
```

---
## \#2 Posted by: Emerson Posted at: 2018-05-27T02:21:33.517Z Reads: 149

```
Bypassing is really easy but can be super dangerous with lipos. I would hope you are using a vesc or focbox with proper cutoffs.

 It would help to post pics to see your setup. My guess is you will need to solder a new wire to your positive and negative terminals of your battery (positive from one lipo and negative from the other). Connect the new leads to a new xt-60 or xt-90 that goes to your ESC or anti-spark. 
 Test to verify it works then remove the old wires you have now replaced to clean it up.
```

---
## \#3 Posted by: Slak Posted at: 2018-05-27T10:55:12.098Z Reads: 130

```
Here is a schema, in french, for a 3X3S Lipo and discharge bypass by BMS build :

https://monlongboardelectrique.files.wordpress.com/2016/12/wiring-bms3.jpg

Title in black (left top) says :"BMS 9S - Charge only"
Blue box on top says : "Power supply"
Red box below says : "Fuse"

Wiring to BMS for balance leads may differ according to your BMS but you can get the whole idea of the bypass discharge thing :)

Post pictures of your BMS, wiring diagram if it was provided by seller)  and setup if you want us to have a look at it.
```

---
## \#4 Posted by: achatham Posted at: 2018-05-27T11:32:45.170Z Reads: 107

```
Ok here are a few pics of my current setup.
![image|375x500](upload://ewTYCpRcYgYbQdqO1WrPWfjc4D.jpeg)
This is my @torqueboards VESC which I love 
![image|374x500](upload://fDu2Ay9k8a70KwwesHiY5jcjF4w.jpeg)
On the left I have the negative running from the charging port to the bms C-. On the right I have my anti spark power switch negative running to the B-. The charging port positive is connected to the power switch also.
![image|374x500](upload://52kZJObSYzobTQ5HGFbek2sCbDy.jpeg)
Both lipos are connected to the bms with one (red) wire running to the B-.

Hope this helps for better direction on what I need to change to bypass discharge. Thanks
```

---
## \#5 Posted by: achatham Posted at: 2018-05-27T11:37:48.052Z Reads: 97

```
@Emerson I’ve read a lot of posts on here and other places recommending on bypassing discharge for cheap China bms’s. I have a pretty solid Vesc from torqueboards and a nice anti spark power switch from Eskating.eu that I trust more than the $10 bms.

My goal = no fires
```

---
## \#6 Posted by: Emerson Posted at: 2018-05-27T11:50:41.860Z Reads: 94

```
I hear ya, I'm currently bypassing my bms on my last build.

 Couple of questions based on the pics. What gauge wire are you currently using from your battery to your anti-spark? What's lipos are you using?
```

---
## \#7 Posted by: achatham Posted at: 2018-05-27T12:57:14.449Z Reads: 91

```
The wire going from the battery to bms to anti spark power switch is 20 awg.

The lipos are turnigy 5s 5000mah 40c each.
```

---
## \#8 Posted by: Slak Posted at: 2018-05-27T14:05:22.243Z Reads: 87

```
But there is something I don't understand :

Are you sure this is now wired for charge AND discharge ? As there is nothing connected to P- in you picture, I doubt about it.

Here is the diagram for what I think is your BMS (and here is a [link](https://fr.aliexpress.com/item/Battery-Protection-BMS-PCB-Board-For-10-Packs-36V-Li-ion-Cell-Max-40A-W-Balance/32682462334.html?spm=2114.13010608.0.0.Vk5gko) to it) :
https://ae01.alicdn.com/kf/HTB17n2bLFXXXXXWXXXXq6xXFXXXH/225409384/HTB17n2bLFXXXXXWXXXXq6xXFXXXH.jpg

I think you are already bypassing discharge. Can someone confirm, please ? @Namasaki maybe ? 

@achatham There is a lot of BMS threads in the forum, have you checked them ? Because I already saw pics of your BMS here so there is an "approuved charge only diagram" somewhere ! 

By the way, did you already ride this build wired as pictured or is it still unfinished ?
```

---
## \#9 Posted by: achatham Posted at: 2018-05-27T14:15:04.751Z Reads: 83

```
No I’m not sure it’s wired with discharge. Yes I’ve read most if not all the forums on bypassing and maybe I’m confused because I already have it set that way?!

My understanding is no connection on the p- connection on the bms is bypassing discharge.

And yes I’ve rode my board and charged once. Just scared I was going to burn the house down 😐 but if you guys confirm it looks right than I’ll feel much better.
```

---
## \#10 Posted by: Slak Posted at: 2018-05-27T14:21:37.074Z Reads: 79

```
Let's wait for someone else's confirmation but for me, it's already in "charge only" wiring mode :)

I was like you when I wired my first BMS and even now, when I do research informations for other people's BMS, I check and check them again like if this was my own case. Let's fire away from all our houses !
```

---
## \#11 Posted by: achatham Posted at: 2018-05-27T14:31:53.853Z Reads: 76

```
I’ve already fried this one being I didn’t insulate the wires good enough. Got a new one coming tomorrow and want to do this right. Thanks for the reply @Slak!
```

---
## \#12 Posted by: Slak Posted at: 2018-05-27T16:19:52.184Z Reads: 72

```
You're welcome ! And do not hesitate to put a "Solved mark" on one my good answser if I was right, would be a first for me ;)

I'm supposed to receive two of those exact BMS for me in the next week so now my homeworks on them are done, i'm ready to wire after checking for difference, just in case.
```

---
## \#13 Posted by: Emerson Posted at: 2018-05-29T20:39:20.466Z Reads: 67

```
It does look as though you are already bypassing the bms. However, 20 ga wire seems waaaaay too thin for the amps you are pulling. Those are rated for something like 5 amps continuous.
```

---
## \#14 Posted by: achatham Posted at: 2018-05-29T20:41:43.912Z Reads: 64

```
@Emerson what would you recommend? 14 gauge?

I have some larger wire. Can’t remember the size. Is it possible to go too big? Would it mess anything up?
```

---
## \#15 Posted by: Emerson Posted at: 2018-05-30T00:33:19.151Z Reads: 62

```
If it's more than 10 awg you may have an issue soldering it up. I suggest 12-14. A good note is to follow the thickness of the cables on your vesc. XT-90s work well up to 10 awg and XT-60s up to 12 awg I think. You can confirm that info witha a few Google searches.
```

---
## \#16 Posted by: achatham Posted at: 2018-05-30T01:45:30.154Z Reads: 58

```
Thanks man! Yea Im running a few xt-90 connectors and 10 awg is what I have. I'll probably end up going a little smaller like a 14.
```

---
## \#17 Posted by: Slak Posted at: 2018-05-30T22:21:27.448Z Reads: 58

```
What is your adapter current to connect to the BMS, @achatham ? 10-16AWG seems overkill if you only charge at 2-5A.
```

---
## \#18 Posted by: achatham Posted at: 2018-05-31T00:20:12.810Z Reads: 56

```
I’m using a hover board 42V charger. Is that what your wanting to know @Slak?
```

---
## \#19 Posted by: Emerson Posted at: 2018-05-31T00:24:39.804Z Reads: 56

```
Totally overkill for the bms or charging wiring. Only need the thicker wire for main current flow from battery to vesc.
```

---
## \#20 Posted by: achatham Posted at: 2018-05-31T00:28:08.931Z Reads: 55

```
Ok so you’re saying the wire going from the battery to the power switch needs to be greater than 20 awg? The power switch is connected to the Vesc.
```

---
## \#21 Posted by: Emerson Posted at: 2018-05-31T02:46:37.732Z Reads: 52

```
Battery to the anti-spark to the vesc should be thicker. Due to bypassing the bms you can use thinner wire on the balance leads and anything soldered to the bms.
```

---

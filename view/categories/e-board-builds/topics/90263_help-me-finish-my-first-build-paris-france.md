# Help me finish my first build - Paris France

### Replies: 20 Views: 419

## \#1 Posted by: JibeBigo Posted at: 2019-04-12T15:43:48.736Z Reads: 165

```
Hi guys,
I've started my first build quite some time ago and I've faced so many issues that I'm starting to get frustrated and I feel I'll never be able to finish this.
I'm still riding my chinese board to work daily (when not rainy) and the good days are coming and still no DIY done.
I'm scared I won't be able to finish it alone or that I'll end up with an unsafe (it's already not the safest transportation mode) board.
I was wondering if anyone in Paris could help me finish my board. I have a spare "smart button" flipsky, value 55€ that I'm willing to offer for anyone who would be ready to help.
So far I have the battery, enclosures, holes for it, esc connected together but I can't seem to put it all together without giving up because of a complication always coming up.
Hit me up if you can help a newbie :slight_smile:
```

---
## \#2 Posted by: Grozniy Posted at: 2019-04-12T16:10:43.307Z Reads: 157

```
Post pics here, we'll help
```

---
## \#3 Posted by: Dirt_Bag Posted at: 2019-04-13T04:08:07.590Z Reads: 138

```
you need to post a list of what parts you are working with, or this thread is useless.
```

---
## \#4 Posted by: bigben Posted at: 2019-04-13T06:09:11.802Z Reads: 132

```
At very least if you can get to the meet up in Paris it will be an interesting project for the attendee's! Perhaps we could have an event called build the newb a board??
Have you visited the site, http://www.e-sk8.fr/forum/
Like @Grozniy says, chuck some photos up and people will be able to help more.
```

---
## \#5 Posted by: ron Posted at: 2019-04-14T23:13:54.391Z Reads: 98

```
So if someone wants to help you he/she needs to know at wich point you are stuck, what you have completed so far and which components do you have.

So please post pics, describe what you have done so far and where you need help.
```

---
## \#6 Posted by: JibeBigo Posted at: 2019-04-15T08:07:13.651Z Reads: 92

```
Ok, thank you guys. I'll take pics and post asap.
The worst part is I've drilled a whole in my enclosure for the smart switch before realizing it needed to be plugged to the motors which are in the other side of the board... I bought a non smart switch from the same flipsky shop and the picture showed the same button... Thing is: it's way smaller and the hole I've drilled now needs to be filled and I don't know which material to use.
Among other issues: I suck at soldering, I have some xt90s to plug into xt60s, I don't have the tools to drill a path for my flat wires into the deck and maybe my worst enemy: my GF hates when I make a mess in the appartment :stuck_out_tongue:
```

---
## \#7 Posted by: Andy87 Posted at: 2019-04-15T10:54:43.835Z Reads: 83

```
everything not a big deal, but this...

[quote="JibeBigo, post:6, topic:90263"]
my GF hates when I make a mess in the appartment
[/quote]

... you need a workshop :smirk::joy:

but seriously

[quote="JibeBigo, post:6, topic:90263"]
I suck at soldering
[/quote]
It´s probably only the wrong solder iron or the solder not your skills ;)

[quote="JibeBigo, post:6, topic:90263"]
needs to be filled and I don’t know which material to use
[/quote]
cover it with tape and fill it up with epoxy or get kydex or similar. that shouldn´t hold you back from finishing your board.

[quote="JibeBigo, post:6, topic:90263"]
I bought a non smart switch from the same flipsky shop
[/quote]
Just forget about the smart switch and get a xt90s loop key. 
does not look that clean, but as min it will not fail on you.
```

---
## \#8 Posted by: JibeBigo Posted at: 2019-08-06T17:12:33.075Z Reads: 60

```
Hi everyone! 
I'm back ! Who thought ? (More "who cared?" haha).
After moving apartments and some projects I finally made it to the final part where I program my VESCs and plug everything in.
I dont want to mess this up.

My config is:
* 10s4p 30q cells
* 2x VESC 4.12 from 
* 2x 6355 motors from 

What should I put as values in VESC tool for it to run smooth and chill at first ?

I thought about:
* **Battery cutoff start** : 34 V (3.1 V/cell * 10 cells)
* **Battery cutoff end** : 31 V (2.8 V/cell * 10 cells)

* **Motor Type** : BLDC
* **Motor Max** : 80 A
* **Motor Min** : -35 A
* **Batt max** : 40 A
* **Batt min** : -25 A
* **Absolute max** : 130 A

What do you guys think ?

Is there anything else that I need to change (RPM, Wattage, Temperature, General settings) ?

Thanks for anyone who'll help :slight_smile:
```

---
## \#9 Posted by: TheSebas Posted at: 2019-08-06T18:11:15.816Z Reads: 52

```
Set your max ERPM to 60000
```

---
## \#10 Posted by: linsus Posted at: 2019-08-06T18:21:24.448Z Reads: 51

```
Do test runs with caution, be prepaired to tug and roll if you fall.. Your settings looks reasonable.
Come back with feedback and concerns.

Also wear a fucking helmet :innocent:
```

---
## \#11 Posted by: JibeBigo Posted at: 2019-08-06T20:11:47.396Z Reads: 49

```
Ok thanks guys ! I'm on it. Hopefully I can ride it tomorrow
```

---
## \#12 Posted by: JibeBigo Posted at: 2019-08-08T07:25:49.038Z Reads: 38

```
Well this didn't happen. I'm struggling with the programming of my vescs. I have no idea what i going on, I paired the remote, used the wizard from vesc tool but the best I managed to get is 1 motor spinning...
If anyone could help in the finishing steps for this that would be dope. 
You can make fun of me 'cause I'm an IT engineer and I can't get past the part that should be the easiest for me -__-

Whenever I run the manual motor detection, only 1 motor spins and it says "bad results" and "detection failed"...
I've tried everything...
```

---
## \#13 Posted by: bigben Posted at: 2019-08-08T09:41:35.619Z Reads: 35

```
Do you use Facebook? You could try the French Fb page or the French forum?
```

---
## \#14 Posted by: nono_fr Posted at: 2019-08-08T10:40:23.715Z Reads: 37

```
@JibeBigo va sur e-sk8.fr et sur le groupe fb affilié !
```

---
## \#15 Posted by: JibeBigo Posted at: 2019-08-08T19:31:41.672Z Reads: 27

```
J'ai posté. J'espère que j'aurai une réponse, ça mfout le seum ce truc :confused:
```

---
## \#16 Posted by: nono_fr Posted at: 2019-08-08T22:52:19.931Z Reads: 25

```
Je t'ai répondu. Si t'as Facebook, envoi ton fb en privé et je t'aiderais
```

---
## \#17 Posted by: JibeBigo Posted at: 2019-08-10T16:19:21.438Z Reads: 18

```
Thanks for everyone who helped (esp. @nono_fr ). Build is done and god, it's unnecessarily fast. Love it.
```

---
## \#18 Posted by: bigben Posted at: 2019-08-10T16:21:49.022Z Reads: 15

```
Magnifique, amuse toi bien!
```

---
## \#19 Posted by: treenutter Posted at: 2019-08-10T16:22:50.995Z Reads: 14

```
@JibeBigo - if you can, post some pics!
```

---
## \#20 Posted by: JibeBigo Posted at: 2019-08-10T16:36:53.010Z Reads: 15

```
I will once it's grip taped and completely done. Still need to adjust stuff, like that tupperware i had to use instead on the very small eboosted case for the enclosure.
```

---

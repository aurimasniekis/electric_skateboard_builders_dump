# Lipo battery connector questions * urgent*

### Replies: 11 Views: 1221

## \#1 Posted by: Mattmccrary8 Posted at: 2017-06-21T19:11:22.426Z Reads: 122

```
Ok so I run 2 5s50000mah lipos in series to make a 10s5ah pack. I carry and extra set with me so I can get more range. When I plugged my lipos into my series connector they sparked and the 4mm plugs burned on the lipos but the series connector was fine. This is where my questions come in. 

I went to a local hobby shop to see if they sold the 4mm connectors and he said "I'd never sell those garbage Chinese connectors" he told me I need to use Dean plugs. I was thinking xt60's if I was going to change? 

I then said well I didn't change them because I use a shitty b6 charger with a parrelll 4mm charging/balance board then he said that's the best way to burn my house down. So my question is, should I change the lipos to dean connectors and should I only charge one battery instead of 2 at a time?
```

---
## \#2 Posted by: Sourcecode Posted at: 2017-06-21T19:48:49.800Z Reads: 113

```
Sounds like ol mate at the hobby shop has no idea what he's talking about 😅. No need to change to deans and you can charge 2 at once no problem if it's set up correctly. Sounds like you need to make an anti spark plug tho. Do you have one?
```

---
## \#3 Posted by: Mattmccrary8 Posted at: 2017-06-21T20:10:17.951Z Reads: 106

```
I don't have one, I have an on off from torque boards. What is an anti spark plug?
```

---
## \#4 Posted by: anorak234 Posted at: 2017-06-21T20:13:49.258Z Reads: 96

```
I think xt60 is still your best bet, but use an anti spark plug if you can. Also NEVER charge in parallel with LiPo batteries - if a cell is drastically over/undercharged and you don't know it, the reader will average out with the other cell in parallel and make it look safe when it really isn't. In other words, your hobby mate was partially correct about the charging hazard except he seems to have failed to explain why. Either get two chargers, or charge them one at a time. Safety is #1 for a reason
```

---
## \#5 Posted by: Mattmccrary8 Posted at: 2017-06-21T20:16:07.764Z Reads: 82

```
I'm confused about the spark plug. I have everything TB, from my Vesc to my on off then my hxt series connector is what hooks up my batteries to my on off. Where should the spark connector be? I use an xt90 from the on off to the vesc...
```

---
## \#6 Posted by: mmaner Posted at: 2017-06-21T20:26:03.150Z Reads: 73

```
You should be ok with 4mm, but I would change to XT90 if it was me.  You can charge in series with no worries, I've been doing for almost a year now on a set of 3s 8000mah 30c lipos using a turnigy balance charger.
```

---
## \#7 Posted by: Mattmccrary8 Posted at: 2017-06-21T20:28:30.293Z Reads: 76

```
Why is everyone against a parrellel charging board?
```

---
## \#8 Posted by: mmaner Posted at: 2017-06-21T20:30:41.767Z Reads: 77

```
I dont know, I don't use them though.  I don't like the idea of carrying spare lipos around, would hate to fall and puncture one, so I permanently mount mine and build the harness I need.  At 6s you can use the MEB Charge Port method with no issues.  I use it on 2 of my boards.

http://www.electric-skateboard.builders/t/miami-electric-boards-diy-charger-how-to/4242
```

---
## \#9 Posted by: Sourcecode Posted at: 2017-06-21T20:31:38.130Z Reads: 72

```
you can charge lipo's in parallel its only unsafe if you don't understand what you're doing 😊. iv done it for years with out issue. Sometimes upto 6 packs at once.

https://youtu.be/WY194Md6KNg

Anti spark plug with a few 1w 100 ohm resistors in parallel 

http://imgur.com/mx6teDo
```

---
## \#10 Posted by: Mattmccrary8 Posted at: 2017-06-21T22:03:14.254Z Reads: 63

```
Ok I usually use the same 2 batteries in series and I charge them at the same time. I really don't want a fire or anything so what is the most fool proof way to make sure that never happens
```

---
## \#11 Posted by: anorak234 Posted at: 2017-06-23T15:47:32.691Z Reads: 48

```
In my opinion if you can find a way to charge them in series that works fine because then it basically becomes one bigger battery. You could also get a Bestech BMS (best BMSs for Lipos and arguably Li-ions). As @Sourcecode stated, if you do parallel charging safely it can successfully charge them, however I would like to point out that the lipos in the video he linked look very puffy; from my own experience I have had both Turnigy and Zippy LiPos fail on me due to parallel charging. Here's the overall picture:

<img src="/uploads/db1493/original/3X/b/6/b642942b6dfc488004fd88d5ceee992d01983eb2.jpg" width="666" height="500">

(the chart isn't perfect by any means but it should give you an idea of what charging method you may want)
```

---

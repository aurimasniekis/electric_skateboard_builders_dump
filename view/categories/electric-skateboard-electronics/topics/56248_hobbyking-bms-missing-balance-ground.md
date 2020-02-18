# Hobbyking bms missing balance ground

### Replies: 9 Views: 383

## \#1 Posted by: petter Posted at: 2018-05-21T20:11:03.922Z Reads: 90

```
So i was looking for a bms on the usual suspects, bestech ans similar. But i think they look kind of suspect and the models are pretty big for just a bms? Like 12x5 cm for 8s?

Then i looked at hobbyking and saw they had a 8s one, oh boy! Kidding aside, they have served me well in the past and it looks good and is actually very small! 6x3cm.
![received_1976323632438390|281x500](upload://faIArg1iTki2sRQwtHCwX3kb30M.jpeg)

This is also for a charge only bms, it's like 10A i think. 

There's just one thing though. There is only 8 balance wires.

Wtf hobbyking.

I mean, i guess it'll work fine since it's the ground one they have omitted but wtf!
![15269333468201204476255|375x500](upload://wrZJq4bXHrxoELT583nRPUvHWKb.jpg)
 I don't want to have to think about possible odd sideeffects from disconnecting one or the other contact!
```

---
## \#2 Posted by: L3chef Posted at: 2018-05-22T12:04:03.328Z Reads: 36

```
I like your oneplus usb cable :stuck_out_tongue:
Not all bms have a slot for the ground. Supower doesn't for example
```

---
## \#3 Posted by: pat.speed Posted at: 2018-05-22T12:09:14.861Z Reads: 33

```
Lots of bms modules don’t have ground for the balance wire as it’s not needed. Since you connect the battery negative wire directly to the board. It acts the same as the black balance wire
```

---
## \#4 Posted by: petter Posted at: 2018-05-22T12:10:20.952Z Reads: 33

```
So does anyone have any clue how this would work? 

I mean the balance leads are connected to the main positive and negative terminal of the battery, while also having a connection to each cell in between. Thats why you have (number of cells + 1) balance leads. 

But here they only have a 8 pin connector!
To clarify:
![image4493|375x500](upload://m7h1dmBqP5kvHP99i6V3ZsPl7ti.jpg)
Though if you look closely there is a small trace snaking it's way from the should be negative pin of the balance lead to the B- Pad. 

So this unit will work as it should if i connect it up as is, connecting the main battery lead and then the eight battery positive for each cell. 

But my question is, how will it work if the main connection is not made? 
I'm thinking that if it is a bad idea to only have the 8 balance leads, i'll just remove the connector and solder in the leads plus one extra to get the full nine. But i'm curious if i have to.
```

---
## \#5 Posted by: petter Posted at: 2018-05-22T12:12:12.864Z Reads: 26

```
Haha wow, no responses from yesterday and then two while i'm adding some more info. Thanks

@L3chef yeah i like it aswell but it's actually burnt out now, it's got a black stripe going up to the micro usb, getting darker each day and now it's started to fray the insulation and is not charging as fast. But it's  been used every day since the invite only era!
```

---
## \#6 Posted by: pat.speed Posted at: 2018-05-22T12:16:12.617Z Reads: 29

```
It’s all about time zones. I’m also pretty sure that is a rebranded supower/bestech bms so they might have some diagrams on their website. 

What should happen is the eight last balance leads should go the the bms plug. The first lead should be left as that is the same as connecting to b-. Well that’s how I recall it works.
```

---
## \#7 Posted by: petter Posted at: 2018-05-22T12:16:41.698Z Reads: 28

```
So for these BMSes that don't have any ground in the balance wire, what happens if you disconnect the main leads but forget to unplug the balance lead?
```

---
## \#8 Posted by: L3chef Posted at: 2018-05-22T12:17:35.114Z Reads: 27

```
@petter just curious.. Is that cable from oneplus 2? They fucked up with that cable using incorrect resistor.
```

---
## \#9 Posted by: petter Posted at: 2018-05-22T12:19:01.807Z Reads: 30

```
No, it's the original OPO one. i think it's just worn out now though

I'll go look if i find it on any of the other sites, maybe there is some more info there

Edit: Yeah, that was not very hard to find... http://bestechpower.com/296v8spcmbmspcbforli-ionli-polymerbatterypack/PCM-D124.html

also, here's the link where i bought it: https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html?___store=en_us
```

---

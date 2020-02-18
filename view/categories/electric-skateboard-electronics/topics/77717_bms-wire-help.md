# BMS wire help -

### Replies: 71 Views: 760

## \#1 Posted by: Alex753 Posted at: 2018-12-11T18:22:38.358Z Reads: 117

```
Hello !

Just received this BMS from Hobbyking : ![image|565x414](upload://7r4QxGfTjdQbmugzsQiEaJsUeJ3.jpeg) 

Why do I have only 2 wires going out of it ? 

![bms%201|690x490](upload://x9WMcPEd46tMjjMEDeK8KCTS1ev.png) 

I’m supposed to wire it like this but I have only 2 output and I don’t even know what are they !
Any idea ?
```

---
## \#2 Posted by: totalgeek9224 Posted at: 2018-12-11T18:27:40.697Z Reads: 111

```
I think those two wires are either chargeport or battery + and -. I would try to find a proper diagram of how it's supposed to be wired (if you haven't already) and if not, hopefully someone with the same bms can help you out. The big plug on the side is what the balance leads plug into
```

---
## \#3 Posted by: L3chef Posted at: 2018-12-11T18:38:21.166Z Reads: 103

```
Can you link to the bms? I think those 2 wire are a e switch or temp sensor
```

---
## \#4 Posted by: Alex753 Posted at: 2018-12-11T18:51:21.453Z Reads: 99

```
This one : https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html

Yep I know about the balance ports, i’m not at home right know but it was surprising to see only 2 wires pre welded, maybe the others one needs to be welded ...
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-11T18:53:06.780Z Reads: 96

```
![image|681x500](upload://qWVS4nF4lJg50hgGprxfKI0S5gY.jpeg) 
You mean this?
It’s the temp sensor.
You need to solder your wires to the pcb on the right terminal.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-11T18:56:59.189Z Reads: 90

```
I guess you want to use the bms for charge only right?
Than the Charger + goes directly to the battery +
The charger - goes to the bms c- and than from the batt cathode - to the battery -
```

---
## \#7 Posted by: thisguyhere Posted at: 2018-12-11T18:57:57.539Z Reads: 88

```
this is a charge only module - 4amp charge, 10amp discharge.  do not wire it for discharge.

B- is your battery negative, either P- (load) or C- (charger) is charger negative.
```

---
## \#8 Posted by: Alex753 Posted at: 2018-12-11T19:01:11.512Z Reads: 89

```
Thanks !
So the schematic that I showed over should be good ? (Without balancing wires)
Edit—
My mistake, it’s without discharge wires
```

---
## \#9 Posted by: L3chef Posted at: 2018-12-11T19:03:02.949Z Reads: 89

```
No it's wired as discharge
```

---
## \#10 Posted by: Alex753 Posted at: 2018-12-11T19:03:49.503Z Reads: 85

```
![Wiring%20diagram%20(2)|690x470](upload://2vMB5QSbTnPl3jI5zsxw59VFd3k.jpg) 

Then this one should be ok without the switch.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-11T19:05:02.256Z Reads: 84

```
Can I like my own comment?
It’s all written there 😅
```

---
## \#12 Posted by: L3chef Posted at: 2018-12-11T19:05:57.460Z Reads: 83

```
No still wired as discharge :grinning: remove P and split B- to battery and vesc
```

---
## \#13 Posted by: Alex753 Posted at: 2018-12-11T19:06:17.050Z Reads: 78

```
Haha sorry it’s easier to look with a Shematic, thank you!
```

---
## \#14 Posted by: Andy87 Posted at: 2018-12-11T19:06:19.389Z Reads: 78

```
Just like that
![image|574x500](upload://2Pi61S1QU17xUplxAzxdeezBNQE.jpeg)
```

---
## \#15 Posted by: thisguyhere Posted at: 2018-12-11T19:06:36.186Z Reads: 72

```
still wrong

![1211181105a|690x388](upload://vfCcf1YTTLBcKBIT9edX5BYwNyO.jpeg)
```

---
## \#16 Posted by: Andy87 Posted at: 2018-12-11T19:07:12.958Z Reads: 74

```
The contacts are named different on his pcb.
The p- in your drawing is c- on his pcb.
The b- I can’t see how it’s called on the pcb. Maybe b-
```

---
## \#17 Posted by: Andy87 Posted at: 2018-12-11T19:11:21.723Z Reads: 74

```
@Alex753 if you can make a picture of the top of your pcb we can say you exactly where you need to solder which wire
```

---
## \#18 Posted by: Alex753 Posted at: 2018-12-11T19:14:55.153Z Reads: 75

```
That what I was looking for, i’m not at home as said but I just got this pic 

![image|397x312](upload://cB3SRVF9i0maltugL4JSfLio0BI.jpeg) 

 Looks like I have C- , P-  and the last one I can’t really read, P or B.

Thank you very much for your help, i’ll send some better pics when i’ll Get home tomorrow if we can’t read correctly !
```

---
## \#19 Posted by: L3chef Posted at: 2018-12-11T19:20:01.234Z Reads: 73

```
It's B- wire it up as @Andy87 explained
```

---
## \#20 Posted by: Andy87 Posted at: 2018-12-11T19:22:56.258Z Reads: 75

```
I found the drawings on the hk side 😅
![image|392x500](upload://tgA3JVuRasC52nQ2Uk3ugdhlbvs.jpeg) 

So the Charger + directly to the battery +
The charger - to c- and than from the bms to the battery - how it’s shown in the drawing.
```

---
## \#21 Posted by: Alex753 Posted at: 2018-12-11T19:44:52.492Z Reads: 74

```
Honestly I don’t understand why the Balance port are connected to the - in this Hobbyking schematic.

Si i did it by myself, I should have this

![image|375x500](upload://fqE1xGZ3E5k8hSzCfnhst0fbzBK.jpeg)

Then I don’t care about my P- ? assuming that it is the discharging port so
```

---
## \#22 Posted by: Andy87 Posted at: 2018-12-11T19:49:51.294Z Reads: 70

```
You don’t use the wires for the load in the hk picture. The rest is the same like you was drawing.

And yes, just forget about the p-
```

---
## \#23 Posted by: Alex753 Posted at: 2018-12-11T19:56:29.528Z Reads: 70

```
Okay so my drawing is good.

Thank you for your help, much appreciated !
```

---
## \#24 Posted by: Alex753 Posted at: 2018-12-12T15:16:53.545Z Reads: 67

```
Hey again ! 
Restarting this thread because I have another problem, I have 8 input on my balance bms and 9 on the one that I welded for my 2x4S in serie, 

![image|666x500](upload://g36qadAnskRuEUpF5JLMLY9ZwOS.jpeg) 

The one Above was shipped with the BMS, so I guess i’ll Need to weld it to my battery balance wires, and the one below is my battery output.

I guess I won’t have to weld the positive of the battery balance right ?
```

---
## \#25 Posted by: J_Dizzle Posted at: 2018-12-12T15:51:17.340Z Reads: 61

```
That’s because you aren’t connecting to negative balance wire there. It has 8 ports for 8 positive wires. The negative balance wire is going to the B- port on your bms
```

---
## \#26 Posted by: Alex753 Posted at: 2018-12-12T16:01:21.273Z Reads: 62

```
Here is my wirings

![image|375x500](upload://hvwIoVJYc5Bw8zhvjjB48FR27AY.jpeg)
```

---
## \#27 Posted by: Alex753 Posted at: 2018-12-12T16:05:11.445Z Reads: 61

```
Just tested it with the voltmeter, it sounds like the black wire at the full left of the picture is the negative one and the 8 others are the positives, sound ok there.



Can you tell me wihich tension I should have when testing « Battery 1 » and the negative pole ? 
I don’t know If i should have 33.6 or 4.2V and I don’ wan’t to connect it the opposite way !
Thank you for your tolerance...
```

---
## \#28 Posted by: Alex753 Posted at: 2018-12-12T17:46:56.185Z Reads: 60

```
Anyone ?
10char
```

---
## \#29 Posted by: Andy87 Posted at: 2018-12-12T18:01:00.746Z Reads: 61

```
Should be like this, just for your 2 4s.
https://www.electric-skateboard.builders/t/help-12s-lipo-discharge-bypassed-bms/71243/10?u=andy87
Where the big black wire goes inside is the first battery. Where the red is going out the second battery.
Same with balance leads, you start counting on the first cell
```

---
## \#30 Posted by: Andy87 Posted at: 2018-12-12T18:11:01.667Z Reads: 63

```
Your balance - is complete from the bms.
So you need to skip the first black wire comming from the battery to the bms. The rest of the lipo wires you connect.
For the second pack the same. 
Skip the black wire and connect the other wires in the right order to your bms.
Like this
![image|581x499](upload://eA3K9SOZnwlF1AqXqVEe6ZUVAAt.jpeg)
```

---
## \#31 Posted by: Alex753 Posted at: 2018-12-12T18:34:51.342Z Reads: 61

```
Okay so basically I understand what you are explaining.
Looks strange though because one tutorial on YouTube was explaining that I needed to cut one positive wire On the balance, maybe one shematic would be way simple to see what we are talking about,

![image|375x500](upload://999dWQZ9MoJzEutggdW877VC32x.jpeg) 

Gave me a headache to drow it, i over satured the colors so you can see them easily, is it ok like this ? (I also whrote the batt numbers on the BMS !)
```

---
## \#32 Posted by: Andy87 Posted at: 2018-12-12T18:45:32.685Z Reads: 55

```
You mixed the order on your balance wires from the lipo pack.
First is the Black wire and from there count up.
In your drawing you took the red one as first and than counted up.
```

---
## \#33 Posted by: Alex753 Posted at: 2018-12-12T19:12:26.249Z Reads: 53

```
So for the left battery only here ?
```

---
## \#34 Posted by: Andy87 Posted at: 2018-12-12T19:18:32.393Z Reads: 55

```
In this order
![image|690x226](upload://sfQtlzyxf3JN8TdhQCcMvQAFoci.jpeg) 
Just you have some more wires between black and red.
Skip the black from each lipo pack and wire the rest up. The red wire is the last wire.
```

---
## \#35 Posted by: Andy87 Posted at: 2018-12-12T19:25:53.701Z Reads: 59

```
I tried to draw it up.
Hope you get it...sorry i‘m no Picasso 😅
![image|690x462](upload://fDmvMDM9CHfxnSiefCls1GQUd7n.jpeg) 

It’s already late over here and I don’t want to make a mistake, so would be nice if somebody could confirm if my drawing is also correct.
Maybe @b264 if you have a minute.
```

---
## \#36 Posted by: b264 Posted at: 2018-12-12T19:30:31.232Z Reads: 55

```
I don't see any issues with that.  If it's late and you're tired though, it may not be a good time to be hooking up lipos :slight_smile:

Put a loopkey in that + wire on the VESC though
```

---
## \#37 Posted by: Andy87 Posted at: 2018-12-12T19:38:53.173Z Reads: 54

```
Thx! Yes loopkey definitiv don’t forget 😅
```

---
## \#38 Posted by: Alex753 Posted at: 2018-12-12T19:49:17.186Z Reads: 55

```
Thank you very much guys !

Honestly it’s just perfect, i’ll have a look at this this weekend because i’m onto others things right now and you’re true.

Yup the Loopkey lol, il already have it, an lcd display and all, my board is already fully fonctional, Bms will be the final touch :smiley:
```

---
## \#39 Posted by: Andy87 Posted at: 2018-12-12T19:59:09.493Z Reads: 54

```
That’s great!
Take your time with wiring things up.
Double check everything and measure the voltage that you see it rising up in 3.6v steps.
Main leads need to be connected first than the plug for balance wires.
Ah and double check everything once again before connecting everything 😅
It’s super easy to burn up a bms...
So take your time 😉
```

---
## \#40 Posted by: Alex753 Posted at: 2018-12-13T07:59:04.230Z Reads: 54

```
And could I use some small Awg wires, like 24 to wire all of this ? 
I also have some big 12 that I used for the rest of my electronic but it’s really big to weld on the BMS ! 
I’m asking that because since the bms is wired in Parallel the output current of the batteries will always pass through the bms even if i’m Not charging the board, in this case maybe I could overheat or put too much amps on thoses wires ? (not taking about the balance wires though)

![image|281x499](upload://9gDur7fd9IkZv4wpoM5dCBTtlzL.jpeg)
```

---
## \#41 Posted by: Andy87 Posted at: 2018-12-13T08:06:14.740Z Reads: 54

```
24awg is good for 3.5a
If you have a 2a charger that would be ok, but I would go a bit higher in crosssection, like 20awg.

As you don’t connect the discharge wire on your bms there will no current flow through this wires while discharging. Only in time of charging.
```

---
## \#42 Posted by: Alex753 Posted at: 2018-12-13T08:53:24.068Z Reads: 48

```
Okay thank you, that’s why I was asking this, there is no « physical » switch to open the loop while riding it to not put my 50Amps into it.
```

---
## \#43 Posted by: Andy87 Posted at: 2018-12-13T09:00:54.461Z Reads: 50

```
as you said by your own, the bms is paralle connected.
means no current through your bms while discharging.
if the bms would be wired in series it would be different.
```

---
## \#44 Posted by: b264 Posted at: 2018-12-13T09:35:48.214Z Reads: 49

```
24AWG - 3.5A
22AWG - 7A
20AWG - 11A
14AWG - 32A
12AWG - 41A
10AWG - 55A
8AWG - 73A
&ZeroWidthSpace;
```

---
## \#45 Posted by: Alex753 Posted at: 2018-12-13T11:09:05.578Z Reads: 45

```
Yup I already saw it but I wanted to be sure that 50Amps couldn’t go through it.
```

---
## \#46 Posted by: skatardude10 Posted at: 2018-12-13T12:58:23.549Z Reads: 44

```
Good thing it sounds like you are not wiring this for discharge and instead charge only. I have this same BMS in the 6S variant, wired it in initially for discharge for what I thought was well less than a 10A load and it was constantly cutting out after a minute or two. Works wonderfully as a charge only BMS now though.
```

---
## \#47 Posted by: Alex753 Posted at: 2018-12-14T18:50:08.187Z Reads: 41

```
Lets do this :sunglasses:

![image|666x500](upload://2r2K5fGFI6QXTgjDNyYnTaaAZIG.jpeg)
```

---
## \#48 Posted by: Alex753 Posted at: 2018-12-14T20:21:21.278Z Reads: 37

```
So, everything is welded ready to connect, I tested and checked again and again everything, it should be good right now.

Before connecting everything just let me know : I have to connect firstly the batteries THEN the balance wires right ?
```

---
## \#49 Posted by: Andy87 Posted at: 2018-12-14T21:16:48.998Z Reads: 35

```
Yes first the battery and than the balance leads from first pack than the second pack.
```

---
## \#50 Posted by: Andy87 Posted at: 2018-12-14T21:20:01.468Z Reads: 32

```
Is this the actual set up?
You cut the red one of the balance wires but it should be the first black one.
If it’s in the extsntions color twisted in the order than ignor that comment.
Just have seen that the red wire is cut and isolated that’s why I want you to double check it.
```

---
## \#51 Posted by: b264 Posted at: 2018-12-14T21:23:14.323Z Reads: 32

```
Connect the negative side battery before the positive side one.
```

---
## \#52 Posted by: Indiangummy Posted at: 2018-12-14T21:53:07.910Z Reads: 33

```
@thisguyhere in you diagram does the wire that goes to B- need to be thick? since its a charge only setup can i use 22-24 awg wire? or does need to be like 10awg?
```

---
## \#53 Posted by: Alex753 Posted at: 2018-12-14T22:02:06.462Z Reads: 34

```
No don’t worry I saw the isolated red wire, i did it Wednesday but I knew I did something wrong thank’s to your shematic.

Here is what I have right now following exactly what you gave me 

![image|666x500](upload://7DAiU3xMRrNUsRO4JNGf1uFKy0V.jpeg)

(can’t be clearer with pictures but the - had been cut correctly, I connected everything and I don’t heard any noise or saw any spark so I think it should be ok.

I don’t received my 33.6V charger but I found one little 19V 1.5A from a laptop, do you think that I can already try something with it ?
I don’t think so since it’s way under 33.6V but i’m impatient :grinning:
```

---
## \#54 Posted by: Alex753 Posted at: 2018-12-14T22:05:52.757Z Reads: 30

```
Andy already replied about this, since there is no more than 4 amps, Awg22 is ok
```

---
## \#55 Posted by: Indiangummy Posted at: 2018-12-14T22:11:07.841Z Reads: 31

```
didnt see that. Thanks!
```

---
## \#56 Posted by: thisguyhere Posted at: 2018-12-14T22:17:29.468Z Reads: 32

```
Ive used 22awg wire for charge connections but then my charger is only 2amp. 

If u plan on upping your charge rate in the future, to let's say an 8amp charger, 22awg wire wont cut it. If this is the case just twist two 22awg together, that'll make like 14awg.
```

---
## \#57 Posted by: Indiangummy Posted at: 2018-12-14T22:21:03.030Z Reads: 32

```
perfect! thanks im using a 2amp charger. so i'l just do 22awg for now.
```

---
## \#58 Posted by: b264 Posted at: 2018-12-14T23:12:05.956Z Reads: 37

```
[quote="Alex753, post:53, topic:77717"]
I don’t received my 33.6V charger but I found one little 19V 1.5A from a laptop, do you think that I can already try something with it ?
[/quote]

# NO &ZeroWidthSpace;

Always use the correct charger for lithium batteries.
```

---
## \#59 Posted by: Alex753 Posted at: 2018-12-14T23:24:25.632Z Reads: 36

```
Okay thank you !

This one should be at home before the 25th : https://www.amazon.fr/gp/aw/d/B06W565W7W
```

---
## \#60 Posted by: Andy87 Posted at: 2018-12-15T04:42:13.728Z Reads: 32

```
If you have it by hand I would change the plug here to a xt90s. Would help that there is no spark when you connect the battery to the bms.
![image|680x500](upload://ndTDsYb9bs0CRR0RB0zGUVtp7iJ.jpeg) 

Like @b264 said always use the right charger.
My French is not that good bit the one you linked looks good. Important that the amps are how you want and the end voltage is the right for your 8s battery.
```

---
## \#61 Posted by: Alex753 Posted at: 2018-12-15T10:30:41.054Z Reads: 29

```
Ok Nice.
I didn’t have any more Xt90 (And Xt60 are cheaper by the way!). 
But since i wouldn’t have to unplug it so often it should be all right like this.

Okay, so I just need to wait for my charger ... thank you again for your help !
```

---
## \#62 Posted by: totalgeek9224 Posted at: 2018-12-15T11:02:10.460Z Reads: 30

```
[quote="Andy87, post:60, topic:77717"]
xt90s
[/quote]

@Alex753 note the 's' 
This model of the xt-90 has an integrated mechanism (I believe a resistor) that prevents arcs and shorts when plugging/unplugging 
This is crucial in the antispark aspect of the antispark switch :)
```

---
## \#63 Posted by: Andy87 Posted at: 2018-12-15T11:44:35.512Z Reads: 29

```
Xt60 totally enough for the charge port.
The reason why I recommend you to use the xt90s is the anti spark function, like @totalgeek9224 already said, this plug will prevent sparks in the moment you connect the battery to the bms. So no changes that your electronics of the bms will get damaged by that spark.
Here a link how they look and where to get.
Just in case you want to change it before your charger arrives.
https://s.click.aliexpress.com/e/7duGJqi
```

---
## \#64 Posted by: Alex753 Posted at: 2018-12-15T12:19:46.083Z Reads: 28

```
My charger arrived this morning, i put everything in my enclosure, attached the charging port to it and went for a ride to discharge my batteries a little bit before trying to charge them.

So I rode about 2.5Km, my batteries are at 92% (32.5V I think) and here is what I have : 

![image|375x500](upload://od6z7UY4BVPjA3FOuai4wG1pwin.jpeg) 

The charger led is still green, looks like it is not charging at all ..!
Let me check in like 30 minutes if the voltage moved up.
```

---
## \#65 Posted by: Alex753 Posted at: 2018-12-15T12:30:53.515Z Reads: 23

```
Definitely not charging, i’m Still at 32.5V.

![image|666x500](upload://tmtT4ULItciLke8pDPtxnpHNpg7.jpeg) 

Looking like this in the enclosure, lot of space and I added foam to stuck all the components, used Velcro also.
Everything isolated with thermo and hot glue, i really don’t know what could have gone wrong !
```

---
## \#66 Posted by: Andy87 Posted at: 2018-12-15T12:46:03.039Z Reads: 24

```

That’s not good to hear.
Can you disconnect the balance wires and the battery from the bms.
Than connect the charger and measure on the plug which usually connected to the battery the voltage.
If you can’t measure there anything than we have definitely a problem with your bms.
```

---
## \#67 Posted by: Alex753 Posted at: 2018-12-15T12:54:18.610Z Reads: 25

```
Nothing out of my charger port so it can be coming from that 

![image|666x500](upload://gEbb0f8BKKqpbYo8e2btHw7nxjb.jpeg) 

So I tried with another one

![image|666x500](upload://pzhi1RsLdy8IqaoXKmV6gPk6v2G.jpeg) 

I think it is definitely this, i’ll weld another one to my enclosure.
```

---
## \#68 Posted by: Andy87 Posted at: 2018-12-15T12:57:54.066Z Reads: 24

```
Let us know if it’s working!
```

---
## \#69 Posted by: Alex753 Posted at: 2018-12-15T13:12:57.574Z Reads: 23

```
Ok so new one welded cleanly, much cleanly than the previous one and current is going through it perfectly !
Now I just need to connect it to the bms
```

---
## \#70 Posted by: Alex753 Posted at: 2018-12-15T13:19:38.736Z Reads: 26

```
Ok guys I have some news 

![image|375x500](upload://6wrHShkzJZZJulpEyyl8p46HwIg.jpeg) 

IT’S WORKING DAMN PERFECTLY 

From now It will be waayyy easier to charge my board, definitely a life changing improvement haha thank you very, very much for your help !

Oh and, last question : can I let my loop key in when charging to see the battery indicator ?
```

---
## \#71 Posted by: Andy87 Posted at: 2018-12-15T14:09:09.423Z Reads: 26

```
💪👏👌
Yes you can. Shouldn’t be an issue.
```

---

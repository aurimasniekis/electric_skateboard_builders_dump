# Probably shorted VESC. How to fix?

### Replies: 19 Views: 2137

## \#1 Posted by: capfirepants Posted at: 2016-11-29T19:43:52.314Z Reads: 198

```
Hi Guys

My VESC is probably shorted. I am building my own board and was setting everything up and went for a really short (like 500 meters) ride today to test everything.
While I was riding the vesc partly stopped responding to input from the GT2B. I plugged it into the pc and monitored the signal input with BLDC. I then noticed that the red error led was flashing. I checked the error message and it returned dvr8302. I sent an email to the esk8.de guys and got a response that I should try accellerating and breaking to test the functionallity.
Since I had already unplugged my board by the time (XT90s connector) I plugged it back in. There was a small popping sound that came from the vesc and it didn't turn on any more. 

I'm now unsure if my VESC is fried - I wrote esk8.de and they told me to send it in to a company in germany that repairs vescs. Before I do that I would like to see if there is anything I can do myself to troubleshoot. 
Are there any ports I can check for resistance or continuance or something else with a multimeter to determine what is broken in the vesc?

Here are some pictures:
<img src="/uploads/db1493/original/3X/1/6/16f0a8ea845feac598c59f0c4b386615178f22de.jpg" width="375" height="499"><img src="/uploads/db1493/original/3X/b/e/be66e063f98c5e076618b3cf945b7f3d851d7bef.jpg" width="375" height="499">

Thanks for your help
```

---
## \#2 Posted by: Cisphyx Posted at: 2016-11-29T22:01:55.212Z Reads: 174

```
Blowing up the DRV is very common with the VESC. While they do offer some nice features, depending on your setup and willingness to keep throwing money at VESCs, it might be worth checking out more reliable options.
```

---
## \#3 Posted by: treenutter Posted at: 2016-11-29T22:10:10.242Z Reads: 171

```
[quote="capfirepants, post:1, topic:13913"]
it returned dvr8302
[/quote]


I don't see anything obvious from your photos. If you're getting a DRV error, the fix is to replace the DRV, either yourself or by someone who knows how (but this is DIY, so give it a shot!)

http://www.electric-skateboard.builders/t/vesc-drv8302-failures-and-repair-options/4201
```

---
## \#4 Posted by: capfirepants Posted at: 2016-11-30T06:28:23.083Z Reads: 158

```
So if the drv is smoke but the rest of the board works fine would it be normal for no lights to flash at alll or might something else be the culprit?
```

---
## \#5 Posted by: TarzanHBK Posted at: 2016-11-30T08:35:19.991Z Reads: 152

```
if you bought it from @elkick, they will take care of you ;)
```

---
## \#6 Posted by: capfirepants Posted at: 2016-11-30T14:30:10.002Z Reads: 140

```
I did, but was told it does not fit under warranty :(
```

---
## \#7 Posted by: Namasaki Posted at: 2016-11-30T14:39:32.092Z Reads: 137

```
[quote="Cisphyx, post:2, topic:13913, full:true"]
Blowing up the DRV is very common with the VESC. While they do offer some nice features, depending on your setup and willingness to keep throwing money at VESCs, it might be worth checking out more reliable options.
[/quote]
The Vesc is dependable and Drv failures are not common if you buy a quality Vesc from a reputable vendor (Chaka for example) which has the all important upgrades and you set it up correctly with respect to the erpm limit.
```

---
## \#8 Posted by: Namasaki Posted at: 2016-11-30T14:43:02.185Z Reads: 128

```
Your Red power wire may have shorted on the pins that it is resting against on the underside of the pcb. 
Check the wire for holes and burn marks
```

---
## \#9 Posted by: TarzanHBK Posted at: 2016-11-30T15:01:33.218Z Reads: 113

```
thats exactly what he did - bought from esk8.de - our EU chaka ;)

[quote="capfirepants, post:6, topic:13913"]
I did, but was told it does not fit under warranty :frowning:
[/quote]

hmm..thats the first case i heard of them not helping out... perhaps you just really did something extremly wrong, otherwise they normally help you out.
```

---
## \#10 Posted by: Cisphyx Posted at: 2016-11-30T15:21:31.928Z Reads: 114

```
[quote="Namasaki, post:7, topic:13913, full:true"]
[quote="Cisphyx, post:2, topic:13913, full:true"]
Blowing up the DRV is very common with the VESC. While they do offer some nice features, depending on your setup and willingness to keep throwing money at VESCs, it might be worth checking out more reliable options.
[/quote]
The Vesc is dependable and Drv failures are not common if you buy a quality Vesc from a reputable vendor (Chaka for example) which has the all important upgrades and you set it up correctly with respect to the erpm limit.
[/quote]

I've yet to have a VESC last more than a couple weeks, including one from Chaka, even with conservative settings. My 12S ESC on the other hand, while not quite as smooth as a VESC, has handled some serious abuse with no issues whatsoever.  

The VESC is great if you know what you're doing and are willing to deal with repairs, but I think this forum tends to over-recommend it to people who are expecting a more straightforward piece of equipment.
```

---
## \#11 Posted by: capfirepants Posted at: 2016-11-30T15:24:13.831Z Reads: 99

```
Well yeah, he said that I can send the VESC in to a guy in dortmund which can fix it. He will then let me know if it's a warranty case or not and if yes, they will pay for the fix. @Namasaki I've checked the power wires, there is no short there. I've re-inspected the whole vesc under good lighting and sadly didn't find anything. I'm not "stupid" with electronics, had conservative settings on the vesc and it still blew... I feel a bit f** 'cause I didn't really use it much nor aggressivly but it still broke.

@Cisphyx Care to recommend the ESC you're talking about? I'm still thinking if I should get it fixed only to have it break again when I get it back or not.
```

---
## \#12 Posted by: TarzanHBK Posted at: 2016-11-30T15:31:02.084Z Reads: 96

```
then of course let them fix it! Send it!
```

---
## \#13 Posted by: capfirepants Posted at: 2016-11-30T15:32:26.263Z Reads: 91

```
Alright - will do that. I'll keep you posted!
```

---
## \#14 Posted by: Namasaki Posted at: 2016-11-30T16:34:50.050Z Reads: 91

```
I have 2 Vescs from Ollinboards (Chaka) that I've been running hard for months with no issues at all. 
10s voltage 190kv motors. Well within the erpm limit. 
I tried hobby escs before and my experience with them was less efficiency which equated to less performance and more heat. ( I literally burned one of my 12s Escs up climbing hills) There power chips are tiny compared to the Vesc and have a greater tendency to overheat. 
Also the brakes on hobby Escs are a joke compared to the Vesc.
```

---
## \#15 Posted by: Namasaki Posted at: 2016-11-30T16:37:54.491Z Reads: 90

```
I'm not familiar with es8.de
Are they using the same upgrades as Chaka?
```

---
## \#16 Posted by: TarzanHBK Posted at: 2016-12-01T07:17:16.503Z Reads: 85

```
yep. They know what they´re doing and also provide warranty
```

---
## \#17 Posted by: capfirepants Posted at: 2016-12-01T15:42:35.132Z Reads: 84

```
I'm very interested if it will apply in my case... We'll find out in a few days.
```

---
## \#18 Posted by: evoheyax Posted at: 2016-12-01T17:37:29.417Z Reads: 81

```
I've ha 2 enertion vescs crap out (one came broken) and 8 chaka vescs now without a single issue. I run FOC, high amps, 12s, pretty much all the abuses everyone talks about. Switch between back and forth between FOC to BLDC to FOC back to BLDC before, without a single issue. They are extremely solid vescs.

I would be surprised if es8.de did all of chaka's upgrades. He does the little things, like using a UV pigment to make sure the coats he adds to the final board for protection is perfect and he didn't miss any spots.

@Cisphyx Did you send your chaka vesc back for repairs? That's one of the beauties with chaka vescs.

And yes, the community does highly recommend, maybe even over recommend the vesc. But IMO, a person new to eskateboards are more likely to blow up hobby grade escs than the vesc, due to their limited abilities for configuration (for example, using things like high or very high for a setting called acceleration instead of a numerical amp limit), and they usually don't have many, if any protections on other electronics. The vesc can protect itself from overheating, batteries from over discharging, motors from blowing up, and more. When you really get down to the details, the vesc, even with the chances of blowing up, is still better IMO than any hobby grade esc.
```

---
## \#19 Posted by: Mike_Lemon Posted at: 2018-09-10T22:11:01.560Z Reads: 30

```
Hi, 

I'm coming from the future...

Any other options than the VESC?
```

---

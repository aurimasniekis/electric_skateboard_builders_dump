# E-switch problem

### Replies: 51 Views: 2476

## \#1 Posted by: Bloop Posted at: 2017-06-10T19:45:26.942Z Reads: 216

```
Hi maybe a stupid question but can someone make it clear for me?
 
I have this bms -> http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D223V1.html

with an e-switch .. well now when i have it ON i get 37V from my battery. when i close it im still getting 37V. What is going wrong?
<img src="/uploads/db1493/original/3X/e/a/eac56bed60636aaa794def0c3243f7b71fb3a7c7.png" width="666" height="500">

This is how i have it connected (2nd img with the xt90 loop key.

Please  help
```

---
## \#2 Posted by: Tobi Posted at: 2017-06-11T04:01:53.954Z Reads: 189

```
why do you are using loop key if your bms has a switch ?
i wired it like image 1 with same bms and it worked perfectly fine.

just use the e - switch to break the loop
```

---
## \#3 Posted by: Bloop Posted at: 2017-06-11T05:24:11.249Z Reads: 186

```
@Tobi can you show me the switch or idk.. i have a regular switch and as i said is not working.. both when is on/off im getting 37v on my output

Also the loop key is to disconnect the vesc while charging
```

---
## \#4 Posted by: Namasaki Posted at: 2017-06-11T06:24:23.405Z Reads: 182

```
Using the loop key to disengage the vesc should not cause a problem. You have it wired correctly in diagram 2.
So, are you saying that your board is on all the time with the switch off or on?
If yes, then check the wiring for the e-switch and make sure the wires are not shorted together.
they could be touching together where they are soldered into the pcb or there could be a solder bridge there. The solder points for those wires are very close together.
If that looks good, follow the path of the wires all the way to the physical switch and see if they are touching together where the insulation is bare.
If that all checks, disconnect the wires from the physical switch and check it with a multimeter to make sure it's opening and closing correctly.

BTW, where are you measuring the output?
```

---
## \#5 Posted by: Bloop Posted at: 2017-06-11T06:39:17.564Z Reads: 159

```
Yes the board is on all the time. with the swtich on or off im still getting power. Im measureing it right before it gets into the vesc. Right after the loop key and just before the Vesc.

I didnt test the switch connections on the bms yes since they are sealed from manufacture with a white stuff i will check that out.
```

---
## \#6 Posted by: Namasaki Posted at: 2017-06-11T06:44:22.414Z Reads: 154

```
remove the white stuff if you have to to check them.
But first, try just disconnecting the white wires from the physical switch and see if the board is off
```

---
## \#7 Posted by: Bloop Posted at: 2017-06-16T07:26:30.496Z Reads: 140

```
@Namasaki i checked the switch and is working just fine.. i tested on the back pads where the switch connect to the BMS and when i off is no connected and when is on is connected ...


Altho im still getting 35V on output everytime even with it on or off
```

---
## \#8 Posted by: Bloop Posted at: 2017-06-16T07:30:34.839Z Reads: 141

```
<img src="/uploads/db1493/original/3X/d/3/d30052ede01b088acee0a3c81893ab8c9a6955ff.jpg" width="666" height="500">
```

---
## \#9 Posted by: Namasaki Posted at: 2017-06-16T13:12:30.929Z Reads: 135

```
Did you try disconnecting the physical switch completely and checking output voltage?
```

---
## \#10 Posted by: Bloop Posted at: 2017-06-16T13:25:02.237Z Reads: 134

```
no but i ignored the switch and connected everything for a test and i have no idea why but now it works perfectly.... i measured the tension in the morning and 5days ago and it was 35V whatever the switch position...


Now it works but i have no idea why :\ 

Thank you for your help tho. Really appreciate it.
```

---
## \#11 Posted by: Namasaki Posted at: 2017-06-16T14:18:18.712Z Reads: 130

```
I think you have a funky physical switch. 
That is why I suggested removing the switch completely to see if the bms was at fault or the switch.
```

---
## \#12 Posted by: pjotr47 Posted at: 2017-07-08T21:19:13.921Z Reads: 130

```
Dear Bloop,
I have the same thing with a [BMS](http://www.bestechpower.com/37v10spcmbmspcbforli-ionli-polymerbatterypack/PCM-D336.html) from bestech. What did you do for fix it? I use now a antispark just as you. I really want to use the e switch.
```

---
## \#13 Posted by: Bloop Posted at: 2017-07-09T04:50:04.162Z Reads: 132

```
well not really sure what was the problem.. but the things i did was:

1. cleaned the white thingy around the e switch wires.
2. stick everything on board
3. then i turned off the e switched added the antispark and it was working. then turned on the e switch and got power. tirned off the switch wait 5- 10 sec for the capacitors to diacharge then the board was off.

Something else i found out. I use the bms both for charge and discharge. And even for discharge you need to have the balance leads connected otherwise kt wont work.


Maybe add some picture or your circuit we could help you that way @pjotr47
```

---
## \#14 Posted by: Namasaki Posted at: 2017-07-09T05:22:48.567Z Reads: 120

```
@pjotr47 
That's right, the Bestech will not turn on unless the balance wires are connected.
I would say, if your bms is not turning off, the first thing is to disconnect the physical switch and once thats eliminated and not the problem, Then the problem is likely where the white wires attach to the pcb. If they're shorting together or if there is a solder bridge between the mounting holes, The bms will stay on.
```

---
## \#15 Posted by: pjotr47 Posted at: 2017-07-09T11:56:19.980Z Reads: 117

```
I have tested my BMS more times. I have soldered the wires off the bms, so the BMS must turn off but the BMS stays on and drop +-5volt of a 42volt battery. When i connected the 2 switch holes the voltage go to 42volt. I have also tested the temperature sensor (connected the 2 solder holes) but the voltage drop also to 37volts... This evening have i some time to test an go i take a picture...
```

---
## \#16 Posted by: Bloop Posted at: 2017-07-09T12:30:49.251Z Reads: 115

```
Well if you disconnect the switch at all you still get 42V ?? cause if that.s the case then might be a problem with the bms.. 

If not then connect the switch back and test again. If you still get 42V with the switch off (again be carefull with that capacitor let it discarge) then try another switch.

When i turn on my eboard i set the switch on off then connect the loop key and then i set the switch on 

do some more testings on that
```

---
## \#17 Posted by: Namasaki Posted at: 2017-07-09T16:46:27.320Z Reads: 107

```
Did you get your bms directly from Bestech?
```

---
## \#18 Posted by: ekitesurfer Posted at: 2017-07-11T17:08:50.799Z Reads: 102

```
Try checking voltage with vesc connected.
```

---
## \#19 Posted by: pjotr47 Posted at: 2017-07-12T08:50:51.979Z Reads: 101

```
OK today I go test that. I have also contact witch bestech I hope that they also can help me.
```

---
## \#20 Posted by: pjotr47 Posted at: 2017-07-12T08:51:55.939Z Reads: 102

```
Yes, I have contacted bestech and I must take pictures for them...
```

---
## \#21 Posted by: Namasaki Posted at: 2017-07-12T11:26:15.941Z Reads: 89

```
Even with the Vesc connected it takes several seconds for the voltage to drain down

@ekitesurfer was having the same issue with his until he connected the Vesc after which it works fine.
```

---
## \#22 Posted by: pjotr47 Posted at: 2017-07-17T13:54:45.263Z Reads: 87

```
Youre right, I have connected the vesc and the voltage drain down, but not to 0volt but to 3volt... Is 3volt normal?_
```

---
## \#23 Posted by: Namasaki Posted at: 2017-07-17T14:39:42.504Z Reads: 86

```
Yes. 2-3v is normal
```

---
## \#24 Posted by: Bloop Posted at: 2017-07-17T15:07:41.494Z Reads: 87

```
Yes is normal. I will check mine too when i get back. But when i switch it off my vesc is off so is all i need :D 

Glad you solved your problem pjotr
```

---
## \#25 Posted by: Bloop Posted at: 2017-08-19T21:28:33.345Z Reads: 85

```
Hey i bring back this post with some new questions. I read that the bms e-switch should be on during the charging ... but my board is charging with the e-switch on and off.. 

Is this normal ??

Also it happened that if i leave the board with the e-switch off and the loop key connected, when i turn the switch on the board wont turn on.. i.ll have to disconnect the loop key and reconnect it. 

Any idea with this???
Thank you
```

---
## \#26 Posted by: Namasaki Posted at: 2017-08-19T21:34:18.757Z Reads: 85

```
The instructions for the bms say that the E-switch should be on while charging. That means that it should be on.
If you don't turn it on, them maybe the bms won't balance your pack properly or protect it from shorts or overcharging.

So if you ignore the instructions and something gets damaged, it's on you.
```

---
## \#27 Posted by: Bloop Posted at: 2017-08-19T21:37:03.819Z Reads: 82

```
Oh i see.. it was strange for me because a few days ago i forgot to turn it on and thought it will not charge unless it is On. but i guess it make sense what you saying here. 

And yeah i dont want to ruin it but was something unexpected for me hehe.

Thanks.
```

---
## \#28 Posted by: marcmt88 Posted at: 2017-10-04T21:41:55.569Z Reads: 68

```
I measured about 9V across the switch and fuse.  Is that right?  I was expecting to get 36V since it's connected to 10s4P battery.  I have a 12V switch that would not work when wired to the bms e-switch.  Where did I go wrong?  Thanks for the input.

https://www.electric-skateboard.builders/uploads/db1493/original/3X/d/3/d30052ede01b088acee0a3c81893ab8c9a6955ff.jpg
```

---
## \#29 Posted by: Bloop Posted at: 2017-10-04T21:49:11.311Z Reads: 65

```
You wont get battery voltage on switch tho. Through switch will go less curren than the main battery cables.

Something strange that i saw tho is that when i have the vesc connected the switch is working just fine. On-37V off 0V

But if i remove the vesc and only connect my multimeter the eswitch is not working and is always on On 37V off 37V
```

---
## \#30 Posted by: marcmt88 Posted at: 2017-10-04T21:52:10.199Z Reads: 63

```
...so it would not be able to power a 12V switch that I have?  What kind of switch do you have?
```

---
## \#31 Posted by: Bloop Posted at: 2017-10-04T21:54:07.750Z Reads: 63

```
12v switch you mean the one you connected to the bms wite wires ? That is the maximum voltage that the switch can handle more then that and it will short. So the 12V one should be just good
```

---
## \#32 Posted by: Bloop Posted at: 2017-10-04T21:54:48.946Z Reads: 62

```
What is the rest of your setup ?? how did you connect everything else . and what is not working for you?
```

---
## \#33 Posted by: Namasaki Posted at: 2017-10-04T22:07:09.432Z Reads: 63

```
[quote="Bloop, post:29, topic:25044"]
But if i remove the vesc and only connect my multimeter the eswitch is not working and is always on On 37V off 37V
[/quote]
 
The switch works wether your vesc is connected or not. 
The reason it appears to not work is that when the vesc is disconnected, there is nothing to drain the residual voltage down. 
When the Vesc is connected, it's Caps drain the residual voltage down
```

---
## \#34 Posted by: Namasaki Posted at: 2017-10-04T22:09:46.253Z Reads: 60

```
Did you mean the 12v switch is not turning the bms on?
```

---
## \#35 Posted by: marcmt88 Posted at: 2017-10-04T23:02:12.386Z Reads: 61

```
My set up is similar to diagram #2 as Bloop with XT90s.  Currently I have everything connected between the battery and the BMS except VESCs.  I connected my 12V switch (Ulincos Latching Pushbutton Switch ON/OFF with Blue LED)  to the BMS 2-white e-switch wires...push to turn on but blue LED did not lit up.  How can you check whether the bms is on?  Thanks.
```

---
## \#36 Posted by: Namasaki Posted at: 2017-10-04T23:04:59.680Z Reads: 70

```
The 2 white wires are not meant to supply voltage for a switch light
```

---
## \#37 Posted by: Bloop Posted at: 2017-10-04T23:09:37.451Z Reads: 69

```
As @Namasaki said.. the eswitch will only turn on and off the bms.. 

the button led will need the 3th pin connected too -> something like this 
https://www.oznium.com/images/wiring_diagrams/led_rocker_switch_diagram.jpg

But id suggest you dont worry about the led.. just on/off and see if the vesc is working.
```

---
## \#38 Posted by: marcmt88 Posted at: 2017-10-04T23:11:01.065Z Reads: 60

```
when the switch is connected to the bms e switch, How do I check whether the switch is turning the bms on?
```

---
## \#39 Posted by: marcmt88 Posted at: 2017-10-04T23:15:38.400Z Reads: 56

```
No way to check bms on or off unless VESC is connected?
```

---
## \#40 Posted by: Namasaki Posted at: 2017-10-04T23:15:41.462Z Reads: 57

```
What @Bloop said,
Connect the vesc and turn the bms on. The vesc should turn on.
You must have the balance wires connected though, or the bms will not turn on.
```

---
## \#41 Posted by: marcmt88 Posted at: 2017-10-04T23:20:41.094Z Reads: 57

```
OK, thanks for your help.  Will give it a try.  Separate question:  how then can the integrated LED on the switch turns on?
```

---
## \#42 Posted by: Namasaki Posted at: 2017-10-04T23:38:05.383Z Reads: 60

```
You would need to use a different switch and supply it with 5v from another source.
On my builds I use this switch and supply the led with 5v from an empty channel on my receiver.
https://www.amazon.com/gp/product/B00YS25ZEM/ref=oh_aui_detailpage_o04_s00?ie=UTF8&psc=1

You need a switch like this because you have to keep the voltage for the led isolated from the white wires.
This is how I wired it
blue and green to white wires from bms
red and black wires to open channel on receiver.

<img src="/uploads/db1493/original/3X/9/e/9e2edbc28fb5352964adb360259354903560671e.jpeg" width="690" height="387">

<img src="/uploads/db1493/original/3X/2/8/28663c15b3bcd91c4a968578861296b9f255ff7b.png" width="506" height="500">
```

---
## \#43 Posted by: marcmt88 Posted at: 2017-10-04T23:49:01.564Z Reads: 58

```
Ok, VESCs turn on when connected.  Thanks again Namasaki and Bloop for your help.  Need to get myself one of those switch.
```

---
## \#44 Posted by: Namasaki Posted at: 2017-10-04T23:52:32.806Z Reads: 57

```
The switch turns the bms on which powers the vesc which powers the receiver which powers the led in the switch.
It happens so fast that the led lights as soon as you push the button.
```

---
## \#45 Posted by: marcmt88 Posted at: 2017-10-05T00:33:45.894Z Reads: 56

```
I have this switch.  Is there a way to wire similar to the one you suggested?

<img src="/uploads/db1493/original/3X/4/f/4feca692cc87a069b89e4e704b00c81a5c9e3338.jpg" width="500" height="500">
```

---
## \#46 Posted by: Namasaki Posted at: 2017-10-05T00:43:30.173Z Reads: 58

```
Give me a minute and I'll make a diagram for it

<img src="/uploads/db1493/original/3X/b/1/b12c06698a02a1d3999916a17a4b80e75fc2c4b2.png" width="690" height="394">
```

---
## \#47 Posted by: marcmt88 Posted at: 2017-10-05T01:06:32.143Z Reads: 58

```
YOU ARE AWESOME!!! I will give it a try.  Thank you so much!!!
```

---
## \#48 Posted by: marcmt88 Posted at: 2017-10-25T16:49:41.356Z Reads: 58

```
Running into a little problem connecting + and - to the receiver, On power up VESC received power but LED did not light up.  I contact Miami Electric; they said "The remote only has one channel.  It has 2 sets of 3-pin connections so you can connect two VESC or a BEC and an ESC without using an adapter."  Does this mean no way to tap power from the receiver to power the LED switch?  Would this be safe or even possible then to tap power from the VESC to power the LED?
Thanks in advance.
 
<img src="/uploads/db1493/original/3X/0/a/0afe23fd7cf580e53bbfed4346c2f7e4ecfe8427.jpg" width="375" height="500">
```

---
## \#49 Posted by: Namasaki Posted at: 2017-10-25T21:44:57.575Z Reads: 53

```
I dont think it would be a problem but I can't say for sure.
```

---
## \#50 Posted by: SpartanFrench Posted at: 2018-04-21T23:18:45.183Z Reads: 39

```
Hi guys,

Digging an old post but I have kind of the same problem. My BMS used to have an E-switch button that worked great.
Suddenly, my E-switch LED button stop working but I was still able to use my board.

Then, I decide to replace my button and that's when I realised that my switch don't do anything.
I removed the switch completly but my BMS and VESC stay on.

I mesure Voltage between the two wire coming from the BMS to the switch and I got nothing : 0V

What could I do ?
```

---
## \#51 Posted by: SpartanFrench Posted at: 2018-04-21T23:26:14.442Z Reads: 39

```
![front BMS|690x388](upload://tVNOqiXYxgiFiauD3D2kID4vN9D.jpg)![Back BMS|281x500](upload://3GCkalikhqJPQ0aorGwJyn2fi74.jpg)
```

---

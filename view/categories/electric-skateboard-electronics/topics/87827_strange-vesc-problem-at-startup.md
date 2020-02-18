# Strange VESC Problem at Startup

### Replies: 48 Views: 488

## \#1 Posted by: RyuX Posted at: 2019-03-21T11:53:32.667Z Reads: 121

```
Dear Members

I need your advice - my board has a weird behavior since a couple of weeks.
Whenever I start the board and want to throttle it will stop the throttle.
I will throttle again and it will stop for another 3-4 times and then suddenly it will work.

The VESC will print the following errors.
Anyone had a similar issue ?

![image|200x500](upload://2BYMHGhHD8glyHKgXep1XMsHsPH.png) 

Thanks for your help.
```

---
## \#3 Posted by: RyuX Posted at: 2019-03-21T12:12:42.654Z Reads: 103

```
But my board works after one minute.. its only the startup phase
```

---
## \#4 Posted by: Sn4pz Posted at: 2019-03-21T12:13:52.053Z Reads: 100

```
Any way to get live data? Metr?
```

---
## \#5 Posted by: RyuX Posted at: 2019-03-21T12:17:55.274Z Reads: 100

```
I could try to record it with the metr app. Never used metr app for live data though. Could it be that the Hall sensor is giving up on me ?
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-03-21T12:41:55.615Z Reads: 92

```
Just get meter data and report back, it could be anything really
```

---
## \#7 Posted by: RyuX Posted at: 2019-03-21T12:47:40.272Z Reads: 88

```
Will do and then supply the screenshot. Thanks
```

---
## \#8 Posted by: trampa Posted at: 2019-03-21T12:56:00.968Z Reads: 82

```
What FW are you running?
```

---
## \#9 Posted by: AlanZhou Posted at: 2019-03-21T13:24:06.241Z Reads: 81

```
I don't think it's fried as I've been taught that drv fualt is like a check engine light on your car, it could be number of things but not exactly the drv

Or the drv is just fried...
```

---
## \#10 Posted by: Mich21050 Posted at: 2019-03-21T13:53:54.601Z Reads: 75

```
@AlanZhou you are right. I was in school and just jumped to conclusion's a bit to fast. 

Maybe the wizard himself could be helpful? :slight_smile: @JohnnyMeduse
```

---
## \#11 Posted by: Mich21050 Posted at: 2019-03-21T14:09:23.593Z Reads: 77

```
Ok so after taking a closer look at Vedder's schematic I think that you could test if the DRV8302 is still working if you just measure the output voltage at your PWM cable... :slight_smile: 

If you have a multimeter just check if your remote receives power... :slight_smile:

Someone, please correct me if I'm wrong.

[quote="Sn4pz, post:12, topic:87827, full:true"]
We dont even know what VESC hes talking about, I mean it can be guess based on previous posts but ???

Gotta provide information
[/quote]
I was just assuming that he's talking about a 4.12.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-03-21T14:09:42.873Z Reads: 73

```
We dont even know what VESC hes talking about, I mean it can be guess based on previous posts but ???

Gotta provide information
```

---
## \#13 Posted by: Sn4pz Posted at: 2019-03-21T14:11:02.253Z Reads: 73

```
dude how is your reply ABOVE my post :o LOL
```

---
## \#14 Posted by: RyuX Posted at: 2019-03-21T14:11:31.314Z Reads: 74

```
It is a maytech Vesc.. HW is 4.10 I think.
```

---
## \#15 Posted by: Mich21050 Posted at: 2019-03-21T14:11:48.856Z Reads: 70

```
I ninja edited my original post... :joy:
```

---
## \#16 Posted by: Sn4pz Posted at: 2019-03-21T14:12:05.523Z Reads: 69

```
Ah yes, maybe email them to ask for their schematic? If theyll give it out :man_shrugging:
```

---
## \#17 Posted by: RyuX Posted at: 2019-03-21T14:12:20.843Z Reads: 70

```
So it couldn't be a sensor issue ?
I replaced the Hall sensor of my motor one year ago..
```

---
## \#18 Posted by: Sn4pz Posted at: 2019-03-21T14:12:42.174Z Reads: 72

```
I didnt know you could change reply mid edit :thinking: I've never been able to do that before 

Oh well :joy:
```

---
## \#19 Posted by: Mich21050 Posted at: 2019-03-21T14:13:31.610Z Reads: 74

```
I don't think so. Do you have a other vesc you could try it with? You could also try running it sensorless? (Wohnst du in Wien? Dann könnte ich dir eventuell helfen) :slight_smile:
```

---
## \#20 Posted by: Sn4pz Posted at: 2019-03-21T14:14:28.497Z Reads: 72

```
It could be anything man, maybe the silicone in some computer chip just took a poo

who knows :man_shrugging:

Your best bet is the wizard @JohnnyMeduse or @ThermalM16 for vesc repair, just remember that soldering a vesc requires precision... if you attempt it on your own be ready to take your time lol
```

---
## \#21 Posted by: RyuX Posted at: 2019-03-21T14:16:23.672Z Reads: 71

```
I already replaced a DRV8302 on another VESC... however I don't really want to change it if I don't have to. With my hot air station I tend to fry them sometimes because my Temp is not reliably stable.

I think if the board runs after one minute I can'T imagine that the DRV8302 is fried.
It might be something else - but I will try unsensored mode tonight and see what happens
```

---
## \#22 Posted by: Sn4pz Posted at: 2019-03-21T14:18:18.416Z Reads: 66

```
post pictures man, sometimes when a 8032 dies it shows physical signs of stress or literally just a hole in it lol

It could be an easy diagnosis
```

---
## \#23 Posted by: RyuX Posted at: 2019-03-21T14:19:09.620Z Reads: 67

```
I have a heatsink on it :P to cover holes
```

---
## \#24 Posted by: Sn4pz Posted at: 2019-03-21T14:20:50.602Z Reads: 66

```
maybe your heatsink jiggled and couldnt direct the heat off enough anymore. Seriously check it lol
```

---
## \#25 Posted by: RyuX Posted at: 2019-03-21T14:21:45.968Z Reads: 67

```
will do.. however for an IC to get a hole it takes quite something and I think it would not work after one minute if it had a hole in it :D but you never know
```

---
## \#26 Posted by: RyuX Posted at: 2019-03-22T07:17:13.662Z Reads: 60

```
![Screenshot_20190322-080702_metr|281x500](upload://a4Jgj4DqLAC57svuc1bY9slKJWS.jpeg) ![Screenshot_20190322-080653_metr|281x500](upload://dJlhTy7L22LABqoXlirL9PEE8vF.jpeg) 

Here are the screenshots.. after the first error I throttled again and didn't have a problem the whole trip.. not sure what to make out of this
```

---
## \#27 Posted by: RyuX Posted at: 2019-03-22T09:53:34.017Z Reads: 53

```
Will do some Sensorless rides today.. I somehow have the feeling it has to do with the sensor maybe. Will keep you posted
```

---
## \#28 Posted by: RyuX Posted at: 2019-03-22T10:11:24.432Z Reads: 53

```
It's not the sensor.
Sensorless ride with the same results.. a couple of cutouts when starting the ride, after that no issues![Screenshot_20190322-111002_metr|281x500](upload://ghLa64Dvnd5CmE2IsWxA5ecpKZ0.jpeg) ![Screenshot_20190322-111014_metr|281x500](upload://cobPSVlVgnemHpM0vfoYWA09uH9.jpeg)
```

---
## \#29 Posted by: banjaxxed Posted at: 2019-03-22T18:12:05.690Z Reads: 48

```
Drv chips you normally can see physical damage, easy to check, but do make sure the right f/w is applied per trampa’s post
```

---
## \#30 Posted by: RyuX Posted at: 2019-03-22T18:16:21.029Z Reads: 47

```
I am using the Ackmaniac 3.100 - I tried flashing it again but didn't change much.
I mean the board is usable - I just wonder what it could be all of a sudden :slight_smile:
```

---
## \#31 Posted by: banjaxxed Posted at: 2019-03-22T18:49:16.684Z Reads: 47

```
Look for a small spot of damage, sometimes it kind of still works like you are experiencing but still fuuuucked

Check the legs too, a loose leg is no good, a high quality pic close up in focus here may help
```

---
## \#32 Posted by: trampa Posted at: 2019-03-22T18:49:32.195Z Reads: 48

```
Maybe a GND loop. Y-PPM, cruise control via  one receiver on two ESCs, motor cable with wiggle waggl to GND....
```

---
## \#33 Posted by: banjaxxed Posted at: 2019-03-22T18:51:20.773Z Reads: 48

```
Is it one you repaired?
```

---
## \#34 Posted by: RyuX Posted at: 2019-03-22T18:55:39.274Z Reads: 48

```
No actually it is a new one. It did this after around 1 week of first using it.
I mean if it was really fucked - why is it only not working when first starting the board and only for around 1-4 throttles ?

Makes no sense to me - all the cables have proper isolation. Only one ground line has been used from the BMS.

so really strange. Also I never really go hard on my board and it is heatsinked from the beginning.
```

---
## \#35 Posted by: banjaxxed Posted at: 2019-03-22T19:51:52.450Z Reads: 46

```
I'd deffo inspect the drv, maybe even as far to hit it up with hot air and reseat.

It's a cheap 4.10 iirc so QA could be the problem, consider returning it if under warranty

Edit: older maytech 4.10 known to be a bit dodge especially when subjected to FOC, unlike the newer clone they knocked out

Probably something you had but didn't use so maybe no warranty, probably time to give the pcb a full looking over concentrating on the drv of course. If the drv ground pad has a tenuous solder link...maybe but you can't see it of course. On start it has a problem but then the heat of operating temp 'fixes' the problem
```

---
## \#36 Posted by: trampa Posted at: 2019-03-22T19:57:26.472Z Reads: 45

```
[quote="RyuX, post:34, topic:87827"]
Only one ground line has been used from the BMS.
[/quote]

What does that mean?
```

---
## \#37 Posted by: JohnnyMeduse Posted at: 2019-03-22T22:28:07.826Z Reads: 36

```
[quote="RyuX, post:14, topic:87827, full:true"]
It is a maytech Vesc… HW is 4.10 I think.
[/quote]

It is really important to know what is the hardware version of your esc the difference between a 4.10 and 4.12 could lead to similar issue on startup . Also are you in bldc or Foc? Could you post some setting? Maybe some picture of your connection could be helpful as well?
```

---
## \#39 Posted by: RyuX Posted at: 2019-03-23T00:06:33.815Z Reads: 37

```
I will remove my enclosure tomorrow and have a look at the PCB

I am in BLDC

Parameters:

![image|373x332](upload://fU1D5r5a9LFvWWWQr9ufsL0w4hu.png) 
![image|690x335](upload://vuzNSrgL4qf1yHdikOuaqDKzbD5.png) 
![image|567x242](upload://5XaGnh0cMx8fnWXLYhnZ6GDzAbn.png) 
![image|539x323](upload://im8NpK2zNFber4MXxYr3p3TS7qt.png)
```

---
## \#40 Posted by: JohnnyMeduse Posted at: 2019-03-23T02:17:03.846Z Reads: 37

```
[quote="RyuX, post:39, topic:87827"]
I will remove my enclosure tomorrow and have a look at the PCB
[/quote]

Thank,  It is going to help you figure out your issue.

Also, did you try different Firmware, I woild suggest to try 2.18 (I know it is an old firmware, but on some setup I’ve seen it work better for older Vesc)
```

---
## \#41 Posted by: RyuX Posted at: 2019-03-23T08:38:39.829Z Reads: 34

```
I reflowed the DRV8302, also did the c18 cap mod.
Let's see if this helps
![20190323_084710|281x500](upload://klVPMdUvzPiPfE4WWD6Auxup1BA.jpeg)

The residue you see is only the white silikon adhesive (from the heatsink)
```

---
## \#42 Posted by: RyuX Posted at: 2019-03-23T08:54:17.849Z Reads: 31

```
Also on some sidenote:

Yesterday I had to go around 20km from the city back to my home with my longboard - I decided that this would be a good test.

So it was quite cold outside and it took almost 10 minutes until the cutouts stopped - but after that I completed the hole 1 hour ride without any issues. Thats why I also think reflowing the DRV might help because this behavior sounds like cold solder joint of sorts.

So let's see what the tests today will bring forward.
```

---
## \#43 Posted by: RyuX Posted at: 2019-03-23T13:11:44.779Z Reads: 28

```
After reflowing the DRV two times with some high quality flux and changing C18 from 2.2uF to 4.7uF I had a great fun ride for the first time in a very long time.
Not even one strange behavior, everything just working as it should. 

So I hope that was the problem all along..

https://metr.at/r/sAVxV

I recorded it.
![Screenshot_20190323-140613_metr|281x500](upload://dHHQpSmZgTsRocfVmBB7yuaRQ6l.jpeg)
```

---
## \#44 Posted by: banjaxxed Posted at: 2019-03-23T14:15:40.789Z Reads: 26

```
Nice ending
```

---
## \#45 Posted by: RyuX Posted at: 2019-03-23T15:39:12.508Z Reads: 23

```
There is almost nothing that can't be fixed with a good amount of flux and heat :stuck_out_tongue:
```

---
## \#46 Posted by: banjaxxed Posted at: 2019-03-23T15:43:23.372Z Reads: 22

```
A bad DRV ground anyways
```

---
## \#47 Posted by: RyuX Posted at: 2019-03-25T12:31:33.048Z Reads: 18

```
Another question - Don't want to open a new thread..
So I replaced the DRV Chip on my old vesc. However I get this weird behavior and a DRV Error.
The GND Pin is properly soldered and all the other pins look good as well

The duty cycle is jumping around and the temperature is wrong

![image|690x373](upload://mgTP3oNMT6AG5knp9Na4bsC833x.png)

Side note: I only use a test power supply with 18V at the moment since I got no battery to test (and the power supply can be Current limited so its always safer to test it with this supply in case of short circuits)
```

---
## \#48 Posted by: RyuX Posted at: 2019-03-25T15:20:02.243Z Reads: 17

```
Ah well.. a good 30 minute ultrasonic cleaning got rid of the problem I think..

![image|690x379](upload://xNVe3EEbjuZDNr1VqRwlkXU1Jmv.png)

EDIT: When trying motor detection it will drop a DRV Error (the Current will go up to 7A and then to -7A but the motor will not spin).

Any ideas ?
```

---
## \#49 Posted by: RyuX Posted at: 2019-03-25T16:03:18.231Z Reads: 14

```
Motor detection is working now.. However when I try to start the motor with the Arrow keys sometimes it works - other times the RED LED will flash and I will get a DRV Error.

![image|414x500](upload://kTumJ2Q8RJlvwbN2WTIqFXPvFcG.png)
```

---
## \#50 Posted by: RyuX Posted at: 2019-03-25T16:37:54.777Z Reads: 13

```
OK its working now.

Had to properly reflow all the IRFS7530 - seems some connections got bad when reflowing the DRV
```

---

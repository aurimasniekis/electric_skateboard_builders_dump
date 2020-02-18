# Enertion remote randomly disconnecting?

### Replies: 19 Views: 2321

## \#1 Posted by: michaelcpg Posted at: 2016-04-27T02:27:38.751Z Reads: 141

```
Hey guys,

I got my first board running over the weekend and so far it's been a tonne of fun. I'm using all Enertion parts except for the deck so it's essentially the exact same setup as a Raptor Mono. 

I have one fairly major issue with the board though, the remote has a habit of randomly disconnecting from the board and the only way I can get it too reconnect is to turn off both the board and remote and then turn them back on a few seconds later. I'm assuming it could be an issue with either the remote or the VESC (maybe the space cell's BMS?) but I'd be interested to see if anyone else has had the same thing happen with their board?

The VESC is setup in BLDC mode with Enertion's recommended current and voltage cut off settings. Other than that, the only settings I've changed are in 'App Configuration > PPM' where I have the control mode set to 'Current no reverse with brake' and have made changes to 'Minimum pulsewidth' and 'Maximum pulsewidth'.

As I mentioned in the title, this seems to happen randomly rather than just when I'm applying heavy braking or acceleration.

I've found that @onloop has made a thread for changing the channel for the remote so I might give that a go but I'd be interested to see if there's anything else that could be causing this issue. So far it hasn't been a major problem as it's thankfully only happened when I'm not going particularly fast but it's enough of an issue that it makes me feel unsafe to ride the board at higher speeds.
```

---
## \#2 Posted by: Dedbny Posted at: 2016-04-27T08:57:06.647Z Reads: 122

```
Definately trry the different channel.
```

---
## \#3 Posted by: michaelcpg Posted at: 2016-04-28T08:05:51.720Z Reads: 104

```
I've tried channel 2, 6 and 9 but with no luck... :pensive:
```

---
## \#4 Posted by: onloop Posted at: 2016-04-28T08:12:21.722Z Reads: 105

```


photos of the wireing inside board please.
```

---
## \#5 Posted by: michaelcpg Posted at: 2016-04-28T08:21:35.786Z Reads: 103

```
Here you go @onloop

<img src="/uploads/db1493/original/2X/9/965284658db566d7ba75963a31c842686a872ac4.jpg" width="689" height="390">

The connections between the receiver and VESC had electrical tape around them to help stop vibrations from disconnecting the wires, so I'm hoping that shouldn't be an issue...
```

---
## \#6 Posted by: onloop Posted at: 2016-04-28T08:25:26.873Z Reads: 102

```
what is that box made from>?

have you tried the receiver in another position?
```

---
## \#7 Posted by: michaelcpg Posted at: 2016-04-28T08:27:38.448Z Reads: 102

```
I'm not sure exactly. It's the bottom of a large plastic toolbox that I've cut out.

Although I haven't tried the receiver in a different position I have tried controlling the board from around 5 meters away without any issue.
```

---
## \#8 Posted by: onloop Posted at: 2016-04-28T08:31:50.933Z Reads: 100

```
so the receiver works? just sometimes doesn't?

you have any other ESC or another RX/tX combo? you need to try some trouble shooting
```

---
## \#9 Posted by: michaelcpg Posted at: 2016-04-28T08:34:24.088Z Reads: 99

```
Yea most of the time the receiver has been fine, up until the last few days it's only cut out very rarely. I've probably done over 50km of riding so far. 

I'm completely new to eBoards/RC places/drones etc so don't have anything to test with other than what I've bought from you sorry.
```

---
## \#10 Posted by: onloop Posted at: 2016-04-28T08:40:38.330Z Reads: 97

```
these are the potential problems

1. the RX or TX is faulty. try another one
2. the wire running between the RX & VESC is a problem. try swapping it OR try the other channel of the RX
3. the VESC has a hardware fault. try another ESC
4. the vesc has a software issue. reload firmware/change some settings.


once we establish to problem we can offer some more assistance, maybe by another cheap RX/TX combo... it's a good idea to have a spare anyway.

from my experience with the enertion remote, it works or it doesn't. intermittent errors are hard to solve.
```

---
## \#11 Posted by: Luke Posted at: 2016-04-29T23:39:23.460Z Reads: 82

```
@michaelcpg I also live in wellington, and was wanting to make a board exactly like you but I was worried about getting up the hills in Brooklyn with just 1 motor. Would you be keen to meet up so I can see how you have set your board up and how you've overcome most of your issues ? I dont have any experience with E-boards but would prefer to build over buy if I can.
```

---
## \#12 Posted by: michaelcpg Posted at: 2016-04-30T00:02:39.102Z Reads: 82

```
Yea man we should be able to sort something out, send me a pm with your contact details, Facebook would probably be easiest, and we can organise something. Although I haven't done any riding on the Brooklyn hills yet, based on my current experience, the main road from town up to Brooklyn would probably be fine on a single Enertion 6374 motor, I wouldn't be so sure about the road on the hill between Brooklyn and Aro Valley. If you're planning on going on a lot of steep hills you'll probably be better off getting two motors, not just for the extra torque going up the hill but also for the extra traction going down hill.
```

---
## \#13 Posted by: Dedbny Posted at: 2016-04-30T23:34:08.380Z Reads: 78

```
Any luck with resolving your remote droP out issues. Could it be a loose connection with receiver and vesc. Alot of vibration while riding can losen things. If it not resolve it sounds like you have to do trouble shooting to work out whaf component might be the issue.

Could if be getting interrance from sone other bluetooth device. Probably unlikely. Know when I had the numchuck remote and some lady with her car alarm button on messed up my control. Lost control at speed and went down.
```

---
## \#14 Posted by: Luke Posted at: 2016-05-01T01:24:02.684Z Reads: 73

```
Pretty sure he fixed it by plugging in the receiver into the alternate plug option, not sure how it works but I saw the board working fine yesterday!
```

---
## \#15 Posted by: michaelcpg Posted at: 2016-05-01T02:16:19.460Z Reads: 73

```
Thanks for all the help guys. As @luke mentioned, it seems to be running fine now. I pulled the board apart the other night and made a few minor changes but I suspect what fixed it was the fact that I connected the servo wire to the other set of pins on the receiver so I'm guessing maybe the connection on the other pins are dodgy?

I've done a few test rides since the change and so far I've only had the board cut out on me once. In this particular case I expect that the cutout was more likely due to the fact that I was braking quite heavily at the time while travelling down a fairly steep hill, which is still a little concerning.

Short of adding more cells to my battery to convert it from a 10s3p pack to a 10s4p pack (which I might look at doing eventually anyway), does anyone have any other tips on how to ensure I get more reliable braking on steeper hills?
```

---
## \#16 Posted by: barajabali Posted at: 2016-05-01T03:15:33.504Z Reads: 62

```
could it have been that the remote wasnt charged ? 

Usually its the simple stuff. did you charge your remote since it fixed itself?
```

---
## \#17 Posted by: Dedbny Posted at: 2016-05-01T03:32:28.034Z Reads: 61

```
Dual motors should help with braking.
```

---
## \#18 Posted by: michaelcpg Posted at: 2016-05-01T03:36:50.971Z Reads: 61

```
@barajabali To be completely honest I couldn't tell you for certain whether or not this could've been the case, but I don't remember charging the remote at all in the hour or so when I tested the board while it was having issues and after I'd opened it up and swapped the servo wire to the other connector. Any idea how long these remotes are supposed to last between charges anyway?

Thanks @Dedbny, I think another Enertion 6374 motor for a dual diagonal setup will be my next purchase at this stage.
```

---
## \#19 Posted by: barajabali Posted at: 2016-05-01T04:00:58.814Z Reads: 58

```
no im not sure how long they last.. i use the GT2B remote. 

and whats important is that the problem went away!
```

---

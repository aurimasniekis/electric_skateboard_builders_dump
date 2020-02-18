# Mislabeled FOCBOX

### Replies: 42 Views: 2872

## \#1 Posted by: flywithgriff Posted at: 2017-08-17T01:26:41.138Z Reads: 389

```
I am in the process of adding extensions to my motors for running foc. However, the label for the sensor wire connector on the FOCBOX is a different order than the pcb!

FOCBOX: 5V, H3, H2, H1, T, GND
PCB: 5V, T, H3, H2, H1, T, GND

These are brand new FOCBOX so I assume this should not be an issue but would like to make sure.
```

---
## \#2 Posted by: mmaner Posted at: 2017-08-17T01:34:30.303Z Reads: 383

```
I'm interested in this as well.  This is what I've found so far...

MOTOR SIDE  >>  JST-ZH 6 pin 1.5mm pitch
VESC SIDE   >>  JST-PH 6 pin 2.0mm pitch

* Motor HAL Sensor Cable

Pin 1 (BLACK)   =  Ground
Pin 2 (BLUE)    =  Phase C(3)
Pin 3 (YELLOW)  =  Phase B(2)
Pin 4 (WHITE)   =  Phase A(1)
Pin 5 (GREEN)   =  Temp Control
Pin 6 (RED)     =  + 5.0v =/- 10%
```

---
## \#3 Posted by: scepterr Posted at: 2017-08-17T01:37:50.734Z Reads: 349

```
@flywithgriff follow PCB order, stickers are messed up...awesome QA right :laughing:
```

---
## \#4 Posted by: flywithgriff Posted at: 2017-08-17T01:40:14.544Z Reads: 325

```
@EnertionSupport is this legitimately an issue? Are the stickers seriously wrong? I have found another thread where this was an issue on the previous vesc-x. New stickers and still mislabeled? I assume you will have a reassuring reply for this!
```

---
## \#5 Posted by: scepterr Posted at: 2017-08-17T01:42:05.790Z Reads: 312

```
https://enertionboards.zendesk.com/hc/en-us/articles/115000952453-Pin-map-on-motor-sensor-on-the-PCB-does-not-match-the-sticker
```

---
## \#6 Posted by: SilentException Posted at: 2017-08-17T01:44:18.821Z Reads: 301

```
http://www.electric-skateboard.builders/t/new-improved-focbox-official-thread/11102/431

Yup, the issue was already reported and confirmed by Enertion in linked post.
```

---
## \#7 Posted by: JLabs Posted at: 2017-08-17T01:44:27.271Z Reads: 284

```
Yes they are @Jinra noticed this on the latest batch of the FOCBOX.
```

---
## \#8 Posted by: flywithgriff Posted at: 2017-08-17T01:44:56.002Z Reads: 274

```
And yet they don't care enough to fix the issue... awesome.
```

---
## \#9 Posted by: flywithgriff Posted at: 2017-08-17T01:45:36.497Z Reads: 272

```
Just to be clear. Follow the order on the PCB and ignore the sticker, correct?
```

---
## \#10 Posted by: JLabs Posted at: 2017-08-17T01:45:54.347Z Reads: 267

```
Im pretty sure that the next batch should have it right, enertion support was notified (should be wrong in the first place).

Yes ignore the sticker..
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-08-17T01:50:03.240Z Reads: 261

```
@JLabs this is the connector on the BKB 190kv 6374. Is the missing wire for the temp?

 <img src="/uploads/db1493/original/3X/9/6/96f2621f9e60c4263980b0fadf3bb0476bdb236f.jpg" width="375" height="500">
```

---
## \#12 Posted by: JLabs Posted at: 2017-08-17T02:11:04.828Z Reads: 250

```
Red and Black are power with the other 3 being sensors. So yes you are correct about the temp not being included
```

---
## \#13 Posted by: flywithgriff Posted at: 2017-08-17T02:12:30.621Z Reads: 242

```
And the order of sensor wires matter or no?
```

---
## \#14 Posted by: JLabs Posted at: 2017-08-17T02:13:31.847Z Reads: 242

```
Hmm im not sure if the VESC auto detects that or not.. I would think so.. Im gonna half to phone a friend for that.
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-08-17T02:15:15.885Z Reads: 238

```
Ok cool deal. I can just match the order on the manufactured connector on the motor.
```

---
## \#16 Posted by: SeanHacker Posted at: 2017-08-17T02:25:03.580Z Reads: 235

```
Phase wire order doesn't matter if you're using a VESC. ;)
```

---
## \#17 Posted by: JLabs Posted at: 2017-08-17T02:27:49.751Z Reads: 234

```
Hes referring to the sensor wires, which im pretty sure dont matter but I cant be totally sure
```

---
## \#18 Posted by: Jinra Posted at: 2017-08-17T03:32:04.063Z Reads: 227

```
They don't matter, you run detection and it figures it out. The order is important for hobby escs
```

---
## \#19 Posted by: adrianenertion Posted at: 2017-08-17T03:36:04.786Z Reads: 227

```
Hi guys,

Our apologies for this. We did contact our factory regarding this issue, but they still shipped with incorrect stickers. You can read about it here: 

https://enertionboards.zendesk.com/hc/en-us/articles/115000952453-Pin-map-on-motor-sensor-on-the-PCB-does-not-match-the-sticker

If you are still having concerns after reading this, please feel free to contact our 24/7 support team to try to assist you further.

Kind regards,
```

---
## \#20 Posted by: flywithgriff Posted at: 2017-08-17T03:36:24.847Z Reads: 220

```
Awesome! So as long as the 5V and GND are in place and the T is empty all is good.
```

---
## \#21 Posted by: JLabs Posted at: 2017-08-17T04:00:15.043Z Reads: 208

```
Yes, exactly
```

---
## \#22 Posted by: torqueboards Posted at: 2017-08-18T10:02:04.784Z Reads: 186

```
@Jinra - Ditto at what Jinra mentioned.. for VESC doesn't matter the order typically only specifically for RC Sensored ESCs would it matter. VESC will auto detect.
```

---
## \#23 Posted by: XTLA Posted at: 2017-08-26T14:22:10.576Z Reads: 172

```
Hi guys, i have same type of motor sensored wire with @flywithgriff and the motor sensor also have no temp wire. The connector wire seems had different color order too but theres white wire for temp i quess. Sud i just ignored the connector wire color as long as the motor wire go with rite order with the focbox, is that correct? Or i need to reorder the connector wire and do i need to remove the temp wire on the connector since the motor wire also don't have? Thanks for the advice 😊

<img src="/uploads/db1493/original/3X/0/7/0744075f8d6af66719008ff399342b0f62816e41.JPG" width="499" height="499">
```

---
## \#24 Posted by: flywithgriff Posted at: 2017-08-26T14:55:48.898Z Reads: 156

```
Reordering the wires in the new connector is a choice. You don't have to but I'm a bit OCD so I did! Make sure the red and black wires are in the two ends to match the FOCBOX sticker. The T opening stays empty and the other three wires are sensor wires that can be in any order. I just did a conversion last night and will post pics in a bit for you.
```

---
## \#25 Posted by: XTLA Posted at: 2017-08-26T15:00:29.611Z Reads: 154

```
Honestly i'm a bit ocd 2 😁, I'll be following this thread, thanks for your help.
```

---
## \#26 Posted by: flywithgriff Posted at: 2017-08-26T15:53:51.948Z Reads: 156

```
This is the correct wiring order! The sticker is wrong. As long as the red, black, and open space are in this position the other three sensor wire order does not matter.
<img src="/uploads/db1493/original/3X/1/7/1773a85b9d0b0d263c6475d55f3dfd92e064d5ca.JPG" width="500" height="500">
```

---
## \#27 Posted by: XTLA Posted at: 2017-08-26T15:56:35.685Z Reads: 145

```
Do you re-order the connector wire color? And also remove the T wire?
```

---
## \#28 Posted by: flywithgriff Posted at: 2017-08-26T15:57:37.044Z Reads: 145

```
I did, I ordered it to match the motor and the connector on my other FOCBOX.
```

---
## \#29 Posted by: XTLA Posted at: 2017-08-26T16:01:39.717Z Reads: 143

```
Is it work? How if im not re-ordering and leave the T wire conected to the focbox eventho its not conected to the motor sensor? Was wondering about that
```

---
## \#30 Posted by: flywithgriff Posted at: 2017-08-26T16:13:51.442Z Reads: 145

```
Yes it works. You do not have to re-order the wires. However, if you do not re-order them you should ignore the colors and make sure the order is correct with how you attach them to the motor sensor wires.
```

---
## \#31 Posted by: XTLA Posted at: 2017-08-26T16:19:07.974Z Reads: 145

```
Thanks for such infos, thats all i need to know.
```

---
## \#32 Posted by: Gynpe Posted at: 2017-10-10T10:03:42.486Z Reads: 141

```
Hey guys, I have a question regarding this issue.

And its that I have an APS 170KV motor, and it has 6 wires for the sensors, and the thing is... In this thread I'm not supposed to be connecting the T on the focbox (Which is in H3 on the sticker) but Bruno from APS is telling me to connect the wires as they are.

And he also tells me that there is no TEMP wire on that motor.

So, right now I'm connected as this thread states, without the T... Should I Just connect them all?

And how do I know if its working properly??
```

---
## \#33 Posted by: longhairedboy Posted at: 2017-10-10T12:06:32.102Z Reads: 129

```
i wonder if the batch i just ordered still have the wrong stickers.
```

---
## \#34 Posted by: egzplicit Posted at: 2017-10-10T12:08:14.409Z Reads: 129

```
They don’t. I got two focboxes a few weeks ago and the labelling is correct now
```

---
## \#35 Posted by: banjaxxed Posted at: 2017-10-10T15:26:38.279Z Reads: 126

```
Bruno will probably have wired them the right way which ignores what is on the sticker
```

---
## \#36 Posted by: Mikenopolis Posted at: 2017-10-10T18:25:28.989Z Reads: 120

```
I would assume that the sticker doesn't matter as the PCB is correct and matches whatever comes out from the motor's sensor JST connector.
```

---
## \#37 Posted by: Gynpe Posted at: 2017-10-12T00:44:28.263Z Reads: 110

```
I ended up connecting the 6 cables coming out of the motor, and notice nothing.

Is there anyway to know if the sensors are working properly?
```

---
## \#38 Posted by: banjaxxed Posted at: 2017-10-13T07:09:56.975Z Reads: 102

```
Vesc tool shows sensors
```

---
## \#39 Posted by: maxbicyclemax Posted at: 2018-12-21T20:16:15.546Z Reads: 55

```
So do Focbox’s read temperature if the motor has a heat sensor?
```

---
## \#40 Posted by: barajabali Posted at: 2018-12-21T20:45:48.742Z Reads: 48

```
The focbox unity can. I believe the old Focbox could too yes.
```

---
## \#41 Posted by: JohnnyMeduse Posted at: 2018-12-21T21:16:19.725Z Reads: 40

```
But it require the newest firmware 3.xx, from either Vedder or Ackmaniac.
```

---
## \#42 Posted by: barajabali Posted at: 2018-12-21T21:17:56.341Z Reads: 40

```
Thanks for the info!
```

---

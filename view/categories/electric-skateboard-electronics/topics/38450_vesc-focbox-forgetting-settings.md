# VESC/FocBox &ldquo;forgetting&rdquo; settings?

### Replies: 14 Views: 884

## \#1 Posted by: Mikenopolis Posted at: 2017-11-15T22:34:42.211Z Reads: 156

```
Is this a thing?
 
I finally replaced my FocBox (running sensored FOC) the other day night, rode it around for about 3 miles. I was able to start from a stand still with no issues.

Today I decided to ride it a bit more during my lunch break because I want to make sure my last vesc was faulty in the last two blow ups I had and that it was not the motor's fault. I noticed right off the bat that I was unable to start from a stand still! Kickstarting works.

Got back to the office and opened up the board, no blinking red light (PHEW). I checked all the setting in both vesc and noticed that the replaced one had it as sensored, but none of the hall sensors values were filled in, it was all 255. I remember measuring and applying...which is why I was able to start from a stop right? 

Has this ever happened to anyone? where the setting reverted back or something after powering off?
```

---
## \#2 Posted by: Martinsp Posted at: 2017-11-15T23:25:43.752Z Reads: 140

```
A very summilar think has happened to me when I configured my VESCs for foc sensored and after successful tests in the basement I powered the board off as usuall and went outside and after powering the board on on the street it had some values reset so I was not able to ride but other than that I have not had this problem. It is very rare, including mine this is the third time I have seen this happen so I don't think that it is a thing...
```

---
## \#3 Posted by: E1Allen Posted at: 2017-11-16T07:15:21.102Z Reads: 119

```
I've had my FocBox reset the settings as well
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2017-11-16T08:02:01.065Z Reads: 108

```
@Mikenopolis i think your vesc has attracted a disease  Alzheimer's,funny because my TB esc my settings were once reverted as well,but i didint touch the board for like a week,so i dont know if it had anything to do with that.After that never had it happen to me 5 months going strong.
```

---
## \#5 Posted by: Mikenopolis Posted at: 2017-11-16T08:40:43.493Z Reads: 105

```
Glad to see I'm not the only one. I reflashed the vesc and started over again. The only thing I can think of is me messing with the settings using an iPhone app and Bluetooth module (HM-10), but it was working after I using that. Rode my board 8 mile this evening and seems fine. Fingers crossed
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-11-16T15:32:51.511Z Reads: 91

```
Do you push your board while the VESC is switched off sometimes?
```

---
## \#7 Posted by: TarzanHBK Posted at: 2017-11-16T15:38:59.345Z Reads: 86

```
you mean it´s possible to erase it´s flash memory with little push-currents, that turns power on and off?
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-11-16T15:42:12.785Z Reads: 86

```
I have nothing that proofs it but since i only push the board while the VESC is switched on i never had that issue again. When the VESC starts it trys to read the settings. And when it looses power by doing that over and over again the EEPROM might corrupts that address and reads the default settings instead.
But it also could be another reason.
```

---
## \#9 Posted by: Mikenopolis Posted at: 2017-11-16T16:08:11.165Z Reads: 83

```
Interesting. I never push this board when off. Plus build is still in FOC testing stages, I thought I had it working last week after a 3 mile test, then the FocBox threw a fault. Replaced the vesc and tested it for a bit. Thought it was working after a short test ride, next day my setting FOC tab's setting we're back to default and unsensored. Learned my lesson, not going to call this board done until I put at least 50 miles in. 40 more to go.
```

---
## \#10 Posted by: TarzanHBK Posted at: 2017-11-16T16:12:14.746Z Reads: 80

```
Hmm okok.. sounds logical.
Might be interesting trying to recreate that to give a general rule when vesc looses settings
```

---
## \#11 Posted by: Zertax Posted at: 2018-09-12T13:16:58.195Z Reads: 48

```
I just got a similar problem my vesc seems to forget all configuration when turned off. It works fine to ride If i configur it and ride but when i turn it off for a while  and then on again it seems to have forgetten all the setting.

Edit vesc 4.12
```

---
## \#12 Posted by: Pimousse Posted at: 2018-09-12T13:26:33.733Z Reads: 44

```
Same happened to a guy on the french forum.
The VESC "forgot" cut off settings. He screwed brand new batteries up. :neutral_face:
```

---
## \#13 Posted by: Zertax Posted at: 2018-09-12T13:48:57.988Z Reads: 41

```
but this seems to reset all settings
```

---
## \#14 Posted by: Zertax Posted at: 2018-09-12T14:11:47.261Z Reads: 33

```
seems to reset itself after i plug it out of the computer and then batteries, is the their a battery on the vesc which can break?
```

---

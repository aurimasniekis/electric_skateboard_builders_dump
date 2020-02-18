# Bricked FOCBOX and ST-LINK

### Replies: 16 Views: 1446

## \#1 Posted by: RiGo Posted at: 2018-02-08T11:20:04.199Z Reads: 216

```
I'm trying to fix a bricked FOCBOX (uploaded incorrect firmware) by connecting to it using an ST-LINK to upload the firmware that way.

All the connections are correct but for some reason I can't connect to it in the ST-LINK utility.

I just keep getting a "Cannot connect to target" error.

Has anyone successfully connected to a FOCBOX using an ST-LINK? If so, could you please share how you did it?
```

---
## \#2 Posted by: TarzanHBK Posted at: 2018-02-08T11:23:07.591Z Reads: 214

```
Don´t you have to replace something if you fack up the firmware this way @JohnnyMeduse?
```

---
## \#3 Posted by: Surfer Posted at: 2018-02-08T11:45:14.551Z Reads: 203

```
Did you try to reset the st32? On the pin 7
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2018-02-08T13:44:53.265Z Reads: 183

```
Well if you can't connect a St-Link there not much to do except changing the MCU. :worried:
```

---
## \#5 Posted by: Surfer Posted at: 2018-02-08T14:33:41.116Z Reads: 175

```
Yes there the option to reset it, and it connects again, tested.
I was flashing new firmware and the computer shot down in the middle of the flashing, I couldn't connect anything, no usb, no st-link, the only way to connect again was grounding the pin 7 for a moment, after that I could connect again to the st-link. 
This is what I did:
https://youtu.be/jEz0C2bT2M0
```

---
## \#6 Posted by: TarzanHBK Posted at: 2018-02-08T14:35:22.970Z Reads: 170

```
Alright, so what exactly do you do?
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-02-08T14:37:40.340Z Reads: 163

```
are you a soft shell or hard shell kinda guy?
```

---
## \#8 Posted by: JohnnyMeduse Posted at: 2018-02-08T15:08:34.224Z Reads: 152

```
I’m the kind of guy that will rather pass 2 minutes changing a MCU than 30 min try to save it 😉🤪🤪
```

---
## \#9 Posted by: GrecoMan Posted at: 2018-02-08T15:15:31.444Z Reads: 153

```
LOL

i’m talkin bout tacos. hard or soft?

don’t turn that into something it isn’t 😉
```

---
## \#10 Posted by: RiGo Posted at: 2018-02-08T21:58:58.439Z Reads: 134

```
I should add that I have this problem with my other (non-bricked, functioning) FOCBOXES as well.

That's why I'm wondering if anyone has managed to successfully connect to a FOCBOX using an ST-LINK like this one:

[img]https://www.sunrom.com/img/p/958/958_800.jpg[/img]
```

---
## \#11 Posted by: Martinsp Posted at: 2018-02-08T22:10:35.267Z Reads: 131

```
I use seemingly the same ST-link, just a green one. Are you sure about the connections? You did not mention that you soldered on a header that is used to connect the ST-link. I dont think that VESC-X and FOCBOXES come with them soldered on already. 

Does the FOCBOX turn on? I mean do any LEDs come on? There should be at least one LED on even with no MCU soldered on so if there are no LEDs on, you have a short somewhere which means bigger problem than firmware mismatch.
```

---
## \#12 Posted by: RiGo Posted at: 2018-02-08T22:17:59.281Z Reads: 125

```
Yeah, I soldered on a header. I have checked and double checked the connection order and I'm positive it's correct. I have tried powering the FOCBOX without using the 3.3V connection as well as using the 3.3V connection without powering the FOCBOX.

The bricked one has a blue LED. With the rest, the other LEDs come on as well.

![IMG_5824|666x500](upload://pgSP2b03t99VjWWe2VMAbqfCkBv.jpg)
```

---
## \#13 Posted by: Martinsp Posted at: 2018-02-08T22:27:54.580Z Reads: 122

```
If you have sucessfuly used the ST-link before than this does not apply but if this is the first time doing this, try connecting all 6 pins because in case you have a V1 marked as V2 you will need all 6. For real V2 ST-links you only need 4. Just to narrow down the problems since you said you can not connect to the other FOCBOX either.

EDIT: I uploaded an incorrect FW to VESC 4.12 once and it was turning on and connecting to BLDC-tool it would stay on 95% duty cycle all the time. I replaced the MCU which solved the issue so that might be the solution for you too. I am just not sure if the problem is in the FOCBOX since you can not connect to the other one either.
```

---
## \#14 Posted by: RiGo Posted at: 2018-02-09T00:04:42.341Z Reads: 115

```
Thanks, I'll try connecting the 6th pin.
```

---
## \#15 Posted by: SOICDIP Posted at: 2018-02-09T02:04:32.684Z Reads: 110

```
https://www.electric-skateboard.builders/uploads/db1493/original/3X/b/1/b11ef34bedcad3ed7b3cce2bfd47b662ac7b4aa5.jpg

Double check your header pinout.

![image|179x117](upload://3kGss73ra1oYKxkvozE2njZ74bS.png)
```

---
## \#16 Posted by: Eboosted Posted at: 2018-09-14T04:43:18.466Z Reads: 60

```
[quote="RiGo, post:14, topic:45864, full:true"]
Thanks, I’ll try connecting the 6th pin.
[/quote]

@RiGo did you ever connect  the ST Link to the FocBox? did you wired the 6th pin?
```

---

# Upgrading Raptor 2 battery from 10s to 12s?

### Replies: 11 Views: 384

## \#1 Posted by: Eboosted Posted at: 2018-12-17T05:19:37.382Z Reads: 139

```
Has anyone upgraded the battery of the Raptor 2 from 10s to 12s yet successfully? 

Or things might start blowing? 

I'd only need to upgrade the BMS and battery
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-12-17T05:33:18.445Z Reads: 137

```
Well, focboxs run happily at 12s, the unity was tested at 14s and it worked (not a great idea), so id assume itd be just fine...? I'm sure there are people planning 12 and 13s builds with the r spec drive kit?
```

---
## \#3 Posted by: barajabali Posted at: 2018-12-17T05:35:33.422Z Reads: 133

```
You’d need to upgrade the bms, switch, lcd, battery/charger (12s3p) 

Then you’d need to change the settings once the firmware/ run different firmware 

Motors can handle it and so can the focboxes!
```

---
## \#4 Posted by: Deodand Posted at: 2018-12-17T17:56:47.591Z Reads: 84

```
The switch would be fine


**EDIT**: Only on a 2.1, the switch for the raptor 2 is on the BMS. 

and I think the LCD might even be able to be switched into a mode that supports 12s but I'm not sure, @Blasto do you have any idea on the LCD? Yeah Just lose a bit of that safety margin on over-voltage but should be fine. 

My 2.1 already goes a bit over 30 mph with the 90mm, imagine 97mm with 12s... you're looking at near 40 mph top speed. Scary stuff.
```

---
## \#5 Posted by: barajabali Posted at: 2018-12-17T17:58:10.320Z Reads: 82

```
[quote="Deodand, post:4, topic:78228"]
I think the LCD might even be able to be switched into a mode that supports 12s
[/quote]
There isnt a button to switch modes on this LCD.

Nvm saw your edit.
```

---
## \#6 Posted by: Deodand Posted at: 2018-12-17T18:01:27.454Z Reads: 78

```
I think the pads for the button might still be there... Haven't fiddled here is the back of my old LCD from a raptor 2. Probably some way to do it but maybe more work than it's worth. 

![IMG_20181217_095935|690x316](upload://8vzHriBDNUOVccdrKTjIvWkWVaI.jpeg)
```

---
## \#7 Posted by: Blasto Posted at: 2018-12-17T18:04:23.755Z Reads: 77

```
I think you need to hold this button at power up to access the voltage inputs

![image|668x390](upload://mxR6xm0tK9TqzocujuZrsY2n3hF.jpeg)
```

---
## \#8 Posted by: barajabali Posted at: 2018-12-17T18:10:31.443Z Reads: 71

```
The button doesn't exist on production Etrays

I'm sure it would work if you shorted the pads.
```

---
## \#9 Posted by: Deodand Posted at: 2018-12-17T18:16:07.931Z Reads: 71

```
This thing is off an early raptor 2 so maybe they quit populating it, but yeah just shorting the pads with a bit of metal would do the trick... maybe plug it in to a lower voltage current limited power supply when you do it though. Don't want to short your battery on accident and blow the thing up.
```

---
## \#10 Posted by: Surfer Posted at: 2018-12-17T19:06:47.161Z Reads: 63

```
And how about the charger? I think is based on the kingpan design, should be good up to 12s or more, I have to test it!!
```

---
## \#11 Posted by: barajabali Posted at: 2018-12-17T19:11:31.276Z Reads: 60

```
Do you mean opening the charger and changing the voltage and amp output? 

Its prob possible but I wouldn't do it. Charger is sealed shut. Let me know if you decide to open it take pictures lol
```

---

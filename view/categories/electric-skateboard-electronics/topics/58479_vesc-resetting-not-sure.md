# Vesc Resetting? Not sure

### Replies: 9 Views: 230

## \#1 Posted by: Ebisane9 Posted at: 2018-06-11T02:12:36.244Z Reads: 50

```
Okay. So this new problem just developed.
I set up my vescs, everything working fine; no drv error; no problem.
I close it up, and suddenly it doesn’t spin the motor. I connect back to Vesc tool and it spins up. I think the ppm fields are resetting somehow. Anyone ever experienced this?

Please let me know what info y’all need to diagnose
```

---
## \#2 Posted by: CarlCollins Posted at: 2018-06-11T02:14:34.371Z Reads: 50

```
@Ebisane9

Are you sure you write settings each time when you set it up?
```

---
## \#3 Posted by: Ebisane9 Posted at: 2018-06-11T02:19:28.683Z Reads: 46

```
Yeah! I used the wizard. The other motor i set up is working fine with no problems :/.
```

---
## \#4 Posted by: CarlCollins Posted at: 2018-06-11T02:20:46.343Z Reads: 41

```
try checking the cables, if there is any loose connection.
try writing the settings twice
```

---
## \#5 Posted by: Ebisane9 Posted at: 2018-06-11T02:22:57.658Z Reads: 32

```
Okay I’ll try, the weird thing is. When I’m done programming and i unplug, it works fine. I even power cycle it and it’s fine. Then i closed the enclosure and it suddenly wasn’t fine. I’m using split ppm for the two motors and one of them responds fine while the other one suddenly doesn’t...
```

---
## \#6 Posted by: JLabs Posted at: 2018-06-11T02:25:08.635Z Reads: 33

```
I just set up a Build today, when I used the wizard it didn’t store the values for the PPM. Call me quick if you want
```

---
## \#7 Posted by: CarlCollins Posted at: 2018-06-11T02:32:20.566Z Reads: 30

```
@Ebisane9
Follow the wizard and write the values manually
```

---
## \#8 Posted by: Ebisane9 Posted at: 2018-06-11T02:35:22.991Z Reads: 28

```
Thanks @CarlCollins @JLabs.
Jared I’ll hit you up since we’re texting already. Will update thread for anyone who might run into this in the future!
```

---
## \#9 Posted by: Ebisane9 Posted at: 2018-06-12T03:01:04.047Z Reads: 16

```
HEHE! Thanks to @Jlabs on the phone we were able to diagnose the problem. We were  bit stumped till we started pushing shit into the vescs and realized the receiver pin had a cold solder due to vibrations no doubt. Bummer but not bummer, NO fried vesc = Happy esk8r. I'm swamped for work during the week but have friday off so will be a quick 15 second solder job and i should be up on the road. Ordered some heatshrink as well.
```

---

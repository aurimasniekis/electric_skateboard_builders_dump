# Setting up my ESK8 VESC - FOCBOX

### Replies: 13 Views: 383

## \#1 Posted by: MarcShane Posted at: 2018-08-19T17:40:48.747Z Reads: 135

```
I finally have most or all of my parts to begin my build.  Is anyone free to walk me through setting up the correct BLDC settings for my components.   I can set up a teleconference tonight and we can review the settings together.  Let me know if anyone has some free timelater this evening.  

Chris
```

---
## \#2 Posted by: Spatt Posted at: 2018-08-19T19:44:53.071Z Reads: 121

```
If you post here more info about how many motors,motor type, info about battery lipo or li ion (xSyP) someone surely will help you easily. 
You should also decide if you want to run in foc mode or bldc. I don’t remember sincerly if in bldc tool there is the ? Symbol next to every conf but for sure in vesc tool there is one and it’s very usefull to well understand everything. Btw welcome to this awesome hobby.
```

---
## \#3 Posted by: Acido Posted at: 2018-08-19T19:46:50.103Z Reads: 113

```
you can make this a lot easier by listing the specs of your battery and motors
theres a lot of threads on motor detection too
its pretty easy if you read a little bit, better to learn how it works than to let someone make it for you, you will need it in the future for sure
```

---
## \#4 Posted by: L3chef Posted at: 2018-08-19T19:53:50.064Z Reads: 105

```
Basically the new vesc tool does this for you with the "wizard setup"
```

---
## \#5 Posted by: MarcShane Posted at: 2018-08-20T16:21:20.314Z Reads: 74

```
Ok -  i have tried to do it myself and cannot even get the focbox to connect to the PC.  Not connected.  I tried hitting the refresh and connect buttons on the application...  Any other advice ?
```

---
## \#6 Posted by: MarcShane Posted at: 2018-08-20T16:32:15.418Z Reads: 70

```
Tried checking for new port
```

---
## \#7 Posted by: L3chef Posted at: 2018-08-20T17:26:53.090Z Reads: 67

```
What power source do you have for the vesc?
Usually when the vesc doesn't connect it's either the usb cable or the drivers on your computer
```

---
## \#8 Posted by: AlexBE Posted at: 2018-08-20T23:52:17.892Z Reads: 59

```
FOCBOX can be fussy with which USB cable you use. Try another few.
```

---
## \#9 Posted by: Spatt Posted at: 2018-08-20T23:53:08.782Z Reads: 59

```
Make sure that the usb cable it’s inside the port of the focbox because some microusb are larger than the hole and it’s not a good contact for data transfer...
```

---
## \#10 Posted by: HillRipper21 Posted at: 2018-08-21T00:03:39.761Z Reads: 56

```
Use a stronger, thicker micro-usb cable. The one that came with my focbox didn't work either, i used one of my own.
```

---
## \#11 Posted by: briman05 Posted at: 2018-08-21T01:58:19.824Z Reads: 49

```
You have to use a usb data cable and not just a charging cable ie the one that comes with a nanox if you have a ps4 the remote charging usb will work with it.
```

---
## \#12 Posted by: MarcShane Posted at: 2018-08-21T03:06:09.843Z Reads: 43

```
It was the usb cord.  I originally used the mini usb from the nano x remote.  It did not work, tried another that I had and whella!!  I used the following video to set up my Foc box.  https://youtu.be/dxDXUrk-7ek
```

---
## \#13 Posted by: briman05 Posted at: 2018-08-21T03:30:52.509Z Reads: 42

```
Yep figured it was the usb I had that same thing happen
```

---

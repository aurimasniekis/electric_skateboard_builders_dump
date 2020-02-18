# BLDC Tool not recognising my VESC - &ldquo;No Firmware Read Response&rdquo;

### Replies: 11 Views: 2563

## \#1 Posted by: Dougieman1001 Posted at: 2017-05-29T22:07:18.363Z Reads: 228

```
Hey,
I've come to configure my VESC for some fine tuning but am having a problem... 
Here is what I have done:
I first turn on the board and wait for the light to stop blinking on the VESC.
Next I open the BLDC tool and then plug in the VESC. 
On the Drop down menu for COM(s) Only COM1 shows up. 
I click connect. For a breif moment, it says connected then comes up with "No Firmware Read Response" and then says not-connected. 
I downloaded and installed COMs drivers (http://www.st.com/en/development-tools/stsw-stm32102.html) and tried again.
Nada. 

(I'm using Enertion's VESC-X)
Any suggestions/help? I have literally no idea..

Thanks
```

---
## \#2 Posted by: Blasto Posted at: 2017-05-29T22:31:28.471Z Reads: 226

```
try another usb cable. micro usb's often are for charging only.
```

---
## \#3 Posted by: Dougieman1001 Posted at: 2017-05-29T22:42:57.707Z Reads: 219

```
Alright I will tomorrow, good point never even crossed my mind! :joy:
```

---
## \#4 Posted by: Jebe Posted at: 2017-05-29T23:13:20.462Z Reads: 200

```
and check the comms port you're using
```

---
## \#5 Posted by: Dougieman1001 Posted at: 2017-05-30T19:58:28.335Z Reads: 183

```
What do you mean?
It only comes up with the one option - COM1
```

---
## \#6 Posted by: Jebe Posted at: 2017-05-30T20:38:35.917Z Reads: 175

```
Unplug the usb, plug into a different usb port. Should make an audible sound. Sounds like the lead
```

---
## \#7 Posted by: Dougieman1001 Posted at: 2017-05-30T20:42:54.559Z Reads: 172

```
Yeah, I have. No sounds, I've tried 5 leads now and none of them are working. I mainly only use Micro USB for charging things, dont own an android etc so I never had the need for a data cable..
```

---
## \#8 Posted by: Jebe Posted at: 2017-05-30T20:45:13.487Z Reads: 166

```
5 is a bit coincidental. Rebooted pc? What power source are you using for vesc? Might be lower than the low voltage cut off limit
```

---
## \#9 Posted by: Dougieman1001 Posted at: 2017-05-30T20:48:39.338Z Reads: 160

```
Two fully charged 5s lipos in series so 10S. Ill reboot my pc and check though
```

---
## \#10 Posted by: Jebe Posted at: 2017-05-30T21:19:28.506Z Reads: 155

```
Try one battery.
```

---
## \#11 Posted by: Dougieman1001 Posted at: 2017-05-30T21:30:27.787Z Reads: 150

```
I got it, it was the cable(s) :joy: 
I ended up using a micro usb cable from my amazon echo which worked xD 
Alls good. Thanks though
```

---

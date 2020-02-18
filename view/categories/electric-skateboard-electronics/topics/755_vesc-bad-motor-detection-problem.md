# VESC &ldquo;bad motor detection&rdquo; problem

### Replies: 10 Views: 3163

## \#1 Posted by: Moja Posted at: 2015-12-19T10:05:34.780Z Reads: 216

```
 After assembling 2 brand new VESC's one of the VESC's is having trouble running the motor. When I try to detect the motor parameters I get the error "Bad detection results received".
 
I have tried running the same motor through my other VESC which is working fine and It has no problems. I have tried multiple VESC firmware versions through multiple versions of BLDC tool and still nothing. This leads me to believe the problem is hardware related on the VESC. The green and blue lights are illuminated and I have re soldered the wires to assure there are no shorts or bad connections. 

 When I try to detect the motors or drive them I get short sudden
jolts in the motor every few seconds. 

 - I am running 2x 4.10 VESC's with the 2.4 BLDC tool with the 2.3    firmware loaded.
 - Running 2 Enertion R-spec motors
 - I am using a Nyko Kama nunchuck 

Here is the dialogue I get when I try to detect the motors:

<img src="/uploads/db1493/original/2X/6/6f81e07bf4514cda5f3f6214b6c0376983e1d76c.png" width="690" height="361">
```

---
## \#2 Posted by: lowGuido Posted at: 2015-12-19T10:13:55.738Z Reads: 199

```
have you tried re flashing the firmware? 
edit sorry I re read what you had said and you have tried that. 
disregard...

I had similar issue and latest firmware flash fixed it.
```

---
## \#3 Posted by: sk8ace Posted at: 2015-12-19T10:19:09.596Z Reads: 198

```
Mine was working fine but now I'm getting "drv8302" fault code in the Realtime Data tab, along with Failed Detection. 
If you go to the Realtime Data tab and click on "Active sampling" at the bottom left, what error does it show for you when you hit Up on the Nyko Kama controller? Mine now shows "drv8302"
```

---
## \#4 Posted by: Blasto Posted at: 2015-12-19T12:41:19.735Z Reads: 197

```
Can you take pics of your vesc causing troubles?

I've often seen, and done myself is bridge the middle pin on the fets, it caused similar issues.
```

---
## \#5 Posted by: chaka Posted at: 2015-12-19T16:43:45.564Z Reads: 184

```
Check the DRV pins for bridging, also check the fets left leg for bridging.  If R28 is cold jointed it would cause these symptoms too.

Best case scenario is a poor battery or motor connection.

Lets see some high resolution photos!
```

---
## \#6 Posted by: Moja Posted at: 2015-12-23T01:28:22.058Z Reads: 173

```
Thanks for the troubleshoot tips, on the road for a few weeks, I'll try and get some images up as soon as I get the chance.
```

---
## \#7 Posted by: Moja Posted at: 2015-12-23T01:33:15.617Z Reads: 170

```
I need a clear schematic that outlines what each component is called, Im nor sure what the components mentioned above are. Links would be appreciated.
```

---
## \#8 Posted by: elkick Posted at: 2015-12-23T12:14:32.084Z Reads: 170

```
Have a look in the BOM under https://github.com/vedderb/bldc-hardware. All parts are assigned to specific locations on the PCB.
```

---
## \#9 Posted by: dogeatgod Posted at: 2016-01-29T09:54:57.892Z Reads: 155

```
@Moja did you resolve your issue?
I have similar, although all was working fine when running 2.5, updated firmware to 2.8 and then got message 'bad detection result received' on motor detection, reverted to 2.5 and issue remains. VESC 4.10
```

---
## \#10 Posted by: Vermontstig Posted at: 2016-10-24T05:18:21.542Z Reads: 80

```
How did you fix your problem I have the same issue.
```

---

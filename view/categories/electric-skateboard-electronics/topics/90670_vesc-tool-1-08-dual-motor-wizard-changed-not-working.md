# VESC Tool 1.08 Dual Motor Wizard Changed. Not working

### Replies: 8 Views: 555

## \#1 Posted by: captclearleft Posted at: 2019-04-15T22:17:50.076Z Reads: 95

```
Hello, 
Relative to using two separate VESC 4.12 VESCs.
I could use some help here.  I am trying to set up a new dual motor setup, but can't seem to get through the new tool (Vesc Tool 1.08).  The old VESC Tool was super easy.  This wizard is not as intuitive...  

![app_settings_can_1|690x457](upload://AbdbSH0tZGNsBr5DUaq7AYN0d9W.png) 

I tried setting the Master first, and selecting this VESC as the VESC the input is connected to.  Then setting up the other VESC I would do the opposite.  No, Luck.  I am not sure how to get the two VESCs to communicate...  

Thanks in advance.
```

---
## \#2 Posted by: Schwiedessen Posted at: 2019-05-24T14:56:45.549Z Reads: 68

```
Hey,  I am facing the same trouble!
Could you fix it and if yes, how?
```

---
## \#3 Posted by: captclearleft Posted at: 2019-05-24T15:22:05.422Z Reads: 63

```
Ok. let me look. Yes.  The fix was little odd.  Standby
```

---
## \#4 Posted by: captclearleft Posted at: 2019-05-24T16:07:53.726Z Reads: 62

```
OK, The way I believe I got it to work (using **PPM** remote).. No guarantees. Do this at your own risk. 

NOTE: Make sure you are all up to date on your firmware.  The VESC firmware should be the same.

First:
- Power OFF the VESCs and Unplug the can-bus cable (DO NOT HAVE THE TWO VESCs connected to each other).
- Run the motor setup on the Master VESC 
- Run the Remote (Input Setup Wizard) Setup on the Master VESC 

  ---> After Master VESC Setup, Change the "Multiple VESCs over CAN-bus" to TRUE (under App Settings, PPM). Or, whatever input you are using...

- DO NOT PLUG IN CAN-BUS CABLE
- Setup the Slave VESC, Motor setup
- I think I plugged in the receiver, and Setup the remote(Input Setup Wizard) as well. Not sure it's necessary.  After the wizard is done (if you use the wizard).
- Under "App Settings", "General" "App to Use = No App"
- Under "App Settings", "General" "Can Status Message Mode = CAN_STATUS_1" (I think that is what I used).

Now.  After all is unplugged.  Turn everything off.  Plug receiver into Master VESC, plug in the CAN-BUS cable.  

Skateboard safely supported so that the wheels can spin freely without damaging anything or anyone.

Turn on remote, turn on Skateboard.

Test it.  The wheels should spin close to the same as you press the throttle.  Mine were not exact.  One always spooled a little before the other. 

If this does not work.  Unplug can-bus cable.  maybe set the  "Can Status Message Mode = CAN_STATUS_1" on the Master...  Or change it too CAN_STATUS_1_2 on the salve...  Or a combination of those...  Not sure.    

Let me know if any of that works.
```

---
## \#5 Posted by: Sn4pz Posted at: 2019-05-24T21:33:15.871Z Reads: 54

```
[quote="captclearleft, post:4, topic:90670"]
Unplug the can-bus cable(DO NOT HAVE THE TWO VESCs connected to each other).
[/quote]


remember to turn your board off before unplugging your canbus cable, otherwise you can end up with bricked VESCs :+1:
```

---
## \#6 Posted by: Schwiedessen Posted at: 2019-05-25T12:55:27.286Z Reads: 49

```
tnx,  the thing is that I am using dual FSESC 6.6 PLUS
No, internal canbus!
I am lost at this point...
```

---
## \#7 Posted by: captclearleft Posted at: 2019-05-25T13:35:57.107Z Reads: 47

```
Ok, Sorry about that.  Ya. This problem was with connecting two separate units.
There has to be a TON of tutorials on setting up the new DUAL VESC 6's...  
Please post a link here when you find it.  I found this with a quick Google Search:

https://www.youtube.com/watch?v=VPhExzFXeQo
```

---
## \#8 Posted by: Cieszyn Posted at: 2019-06-05T04:12:06.651Z Reads: 34

```
I have the same issue. If you go to 5:20 at your video you'll see when connecting the second vesc you dont configure anything - it pairs it to the master vesc. Probably the vesc tool from your video is 0.95
 
On new vesc tool (as in the picture provided above) with slave vesc you still have to configure the input and it doesnt work. You can control only the master motor.

BTW it works on vesc tool 0.95, you have to downgrade.
```

---

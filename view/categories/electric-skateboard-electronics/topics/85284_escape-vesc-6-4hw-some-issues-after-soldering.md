# ESCape (VESC 6.4HW) some issues after soldering

### Replies: 16 Views: 462

## \#1 Posted by: ron Posted at: 2019-02-25T00:02:58.770Z Reads: 137

```
Hi there all.

I hope someone can help me regarding my two not properly working ESCapes.

I have soldered 4 of the ESCAPE Boards and on 2 on them I have a Problem. 
I just wanted to ask if someone could give me a hint how to determine the failing/failed part(s) .

Im first focusing on one of them which seems to power on (blue solid LED).

**ESCAPE1:**

* POWER through PowerSupply: BLUE LED is on
* Power through USB (With R1 bridged): BLUE LED is on
- Measuring 5.1V on the 5V pins of the JST Connectors
- Nothing stinks or gets hot
- Connected and Powered through STLINK: BLue LED is ON but STlink dosen't recognize the STM Chip

So. When I connect the VESC to the PowerSupply @12V/0.8A the BLUE LED is turning on but there is no Current draw seen on the Power Supply. When I connect my VESC 4.12 (Which are working) to the POWER Supply it draws about 0.5A@12V.
Also when I turn on the VESC through the PowerSupply @12V/0.8A and connect it through USB (R1 not populated/bridged) I dont see any COM device in the HardwareManager of Windows. Shouldn't there occur a virtual COM Device when connecting through USB while Powered through PowerSupply.?
All the Pins on the STM and the DRV are looking good and seem to be connected. In that matter I desoldered the DRV and the STM (Reflow/Resolder Station) and removed all of the solder from the Pads on the PCB and resoldered them with flux. But the same Problem still remains.

Either the STM or the DRV are faulty or somewhat damaged or somewhere on the PCB a component is damaged.

Do you have any suggestions on where to look for and what to measure to determine the where the issue is located. 
Would appreciate any help.

![DSC04945|503x500](upload://yOcBPpCAuygzIAapMaD3pCq5VZm.jpeg) ![DSC04946|494x500](upload://6eiykUiFbOMliGhPAxabXlUvtmX.jpeg) 


**ESCAPE2:**

This one is behaving like this:
- Power through Power Supply with 12V@0.8A NONE of the LEDs are lit up.
- Connecting it over USB to PC while powered up over the PowerSupply dosen't change anything (R1 NOT populated). So no connection to Windows.
- On the 5V pins of the JST Connectors I measure about 1.1V instead of 5.1V when powered over PowerSupply
- Powering the ESCAPE through ONLY USB with Populated/bridged R1 -> Blue LED lights up and I can measure 5.1V on the 5V pins of the JST Connectors. But still no Data Connection to Windows, so no COM Port recognized.
- Connecting through only STLINK: Blue LED is On and I can Program the Bootloader and Firmware. So the STM32 is recognized properly.
-When Powering through Power Supply no Current is drawn.

I also resoldered the STM and the DRV Chip but it didn't change anything regarding the failure.

So something in the PowerSupply Chain should be messed up? I don't know where to start looking. I thought first to look at the Parts for the PowerSupply but don't know where to measure. I think I should measure the MosFets between Drain/Source/Gate to see if they are damaged?!

![ESCAPE_VESC2_1|514x500](upload://gCYj65fllJ6cjG2HUamo7EuKv26.jpeg) ![ESCAPE_VESC2_2|508x500](upload://ia9wlKPwhgS7zruxxWnETXtpXtM.jpeg) 


And on both Boards there are no issues seen on visual inspection. Besides the Flux not cleaned/removed  entirely.



**BTW:** Could I clean the VESC fully populated in an ultrasonic bath with 99% Isopropanol without the Crystal and other components taking damage?


Would be nice if someone could help me figuring this out... Thank you in advance.

Greetings from Germany!
Ron
```

---
## \#2 Posted by: mynamesmatt Posted at: 2019-02-25T10:36:57.372Z Reads: 88

```
@JohnnyMeduse you got any idea what could be the issue here.? we gotta boi in need
```

---
## \#3 Posted by: JohnnyMeduse Posted at: 2019-02-25T13:50:24.493Z Reads: 84

```
Hi,

I don't know the type of flux you use, but I've seen lots of problems caused by too much flux. The first thing to try, I suggest to maybe clean then. I usually use heat, Isopropyl and flux remover, I'd never try an ultrasonic bath but yeah, it should work. 

Also, you don't need R1.

Regards
JF
```

---
## \#4 Posted by: Surfer Posted at: 2019-02-25T15:12:51.368Z Reads: 75

```
The drv in the first vesc is clearly blow
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2019-02-25T15:28:33.077Z Reads: 73

```
It is not burn mark. It is flux residues.
```

---
## \#6 Posted by: AlanZhou Posted at: 2019-02-25T16:31:56.677Z Reads: 71

```
Bridged solder?

![ESCAPE_VESC2_2__01|508x500](upload://9QWniZ1JTZsM8tKK1ZOtLQmNSmO.jpeg)
```

---
## \#7 Posted by: ron Posted at: 2019-02-25T16:40:24.091Z Reads: 64

```
Yepp. These are all Bridges/connected to one pad as intended by the PCB/Boardlayout.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-02-25T16:41:41.675Z Reads: 63

```
Wtf..... Pads are not soupposed to be bridged are they??? Or am I dumb, it's a drv I'm mind blown
```

---
## \#9 Posted by: ron Posted at: 2019-02-25T16:45:58.179Z Reads: 62

```
Yepp it's flux.. 

Before resolder and solder the DRV and STM chip back I didn't use any flux and after using flux the failure didn't change so either the uCs are defective or somewhere else on the board something is defective. 

I'll try to get the flux off as best as I can. 

So any hints about where to look at with this failures described above.

Thanks in advance for your help :slight_smile: . Appreciate it... 

Should I reflow the Components/Board to see if something changes? Maybe there is somewhere a cold solder joint.

Greetings from Germany
Ron
```

---
## \#10 Posted by: ron Posted at: 2019-02-25T16:47:53.866Z Reads: 58

```
In this case some of the Pads are intended to be bridged or better said, connected to one trace on the PCB .
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2019-02-25T16:48:33.729Z Reads: 57

```
Yes those pads are suppose to be bridge
```

---
## \#12 Posted by: AlanZhou Posted at: 2019-02-25T16:48:44.970Z Reads: 61

```
Germany? My Google somehow showed me this.
![Screenshot_20190225-114922|245x500](upload://9cPa58lRaQcexsRqeHbGXUxTkDS.jpeg)
```

---
## \#13 Posted by: ron Posted at: 2019-02-25T16:50:36.050Z Reads: 60

```
🤣🤣🤣🤣


Man, don't blow my cover off..
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2019-02-25T16:51:10.952Z Reads: 58

```
[quote="ron, post:9, topic:85284"]
So any hints about where to look at with this failures described above.
[/quote]

Maybe check at the Chrystal part of the circuit. Make sure you put the 15pF at the right place
```

---
## \#15 Posted by: ron Posted at: 2019-02-25T16:52:01.450Z Reads: 58

```
Will do that.. :)
```

---
## \#16 Posted by: ZmasteR Posted at: 2019-03-24T13:12:53.348Z Reads: 41

```
Up, got quite the same issue.
Did you find a solution ?
```

---

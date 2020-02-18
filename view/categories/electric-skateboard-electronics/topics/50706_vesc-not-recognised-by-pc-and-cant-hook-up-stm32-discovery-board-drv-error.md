# VESC not recognised by pc, and can&rsquo;t hook up stm32 discovery board (DRV error)

### Replies: 16 Views: 554

## \#1 Posted by: zblad Posted at: 2018-03-30T19:54:17.749Z Reads: 54

```
My VESC was connecting to my pc just fine until today.  My other VESC will still connect so I know its not my laptop.  I grabbed my discovery board and the instant I plug the VESC into it I get a blue light,  But my other VESC can connect to it fine.  Its almost like its shorted out but I am not really sure where to look for the short or how it would have even happen.  Is there any components on the VESC that could cause this behavior.
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-30T20:11:16.355Z Reads: 46

```
Strange.. blue light usually means no bootloader. Are you running dual?
```

---
## \#3 Posted by: zblad Posted at: 2018-03-30T20:22:14.429Z Reads: 42

```
I am so I measured voltage across the ground and pin 1 in this picture and I get 5.5 volts not sure why.  I am hoping the mcu isn't shot but I am leaning towards it is.

![pinout|277x188](upload://elvFZ04MpYracNfxlkobAnRFXX3.png)
```

---
## \#4 Posted by: RedEagle Posted at: 2018-03-30T20:28:14.015Z Reads: 35

```
Which connector is that?
```

---
## \#5 Posted by: zblad Posted at: 2018-03-30T20:31:43.772Z Reads: 35

```
its the one you hook the stm32 discover board too...  Program / Debug
```

---
## \#6 Posted by: RedEagle Posted at: 2018-03-30T20:34:49.695Z Reads: 35

```
Looks like you have a direct short to ground from the 3.3v line. Fried MCU and possibly DRV too. I would check the 5v rail and do a continuity test across the board.
```

---
## \#7 Posted by: zblad Posted at: 2018-03-30T20:45:25.959Z Reads: 35

```
so I found a tiny ball of solder where my remote plugs into.  I picked the ball out and it connects to my pc no problem now which is good.... But my motor wont spin up so I think your right about the drv which sucks but its not the first one I have had to replace.
```

---
## \#8 Posted by: RedEagle Posted at: 2018-03-30T20:47:11.373Z Reads: 34

```
Not spinning as in with remote or arrow keys? Have you typed faults in terminal? Any faults show up?
```

---
## \#9 Posted by: zblad Posted at: 2018-03-30T20:59:54.273Z Reads: 31

```
alright so now I got the motor to spin up but it spins fast then stops and says detection failed.  I am using the new vesc tool so I'm not 100% sure how to get the faults but I'm guessing its going to be a drv fault but why does it spin up a little?
```

---
## \#10 Posted by: RedEagle Posted at: 2018-03-30T21:01:54.513Z Reads: 30

```
On the left you'll see VESC Terminal. Click on it and type faults in the box.
```

---
## \#11 Posted by: zblad Posted at: 2018-03-30T21:08:11.235Z Reads: 29

```
Also my led doesn't blink red when I power it on.  Usually when you power it up isn't it suppose to flash like 2 or 3 times?
```

---
## \#12 Posted by: zblad Posted at: 2018-03-30T21:09:09.733Z Reads: 30

```
Fault : FAULT_CODE_DRV

Current : -1.4

Current filtered : -1.3

Voltage : 33.67

Duty : 0.006

RPM : 2.2

Tacho : 7

Cycles running : 1

TIM duty : 310

TIM val samp : 155

TIM current samp : 26250

TIM top : 52190

Comm step : 4

Temperature : 25.75


Fault : FAULT_CODE_DRV

Current : 0.6

Current filtered : 0.3

Voltage : 33.64

Duty : 0.006

RPM : 2.9

Tacho : 8

Cycles running : 1

TIM duty : 310

TIM val samp : 155

TIM current samp : 26250

TIM top : 52190

Comm step : 5

Temperature : 25.70
```

---
## \#13 Posted by: RedEagle Posted at: 2018-03-30T21:13:27.076Z Reads: 29

```
[quote="zblad, post:12, topic:50706"]
Fault : FAULT_CODE_DRV
[/quote]

Well, I think you know what that means..
```

---
## \#14 Posted by: zblad Posted at: 2018-03-30T21:14:05.232Z Reads: 29

```
I was hoping it was a bad solder joint but o well digikey is here in town so Monday ill get a new one and try replacing it :(
```

---
## \#15 Posted by: RedEagle Posted at: 2018-03-30T21:17:51.068Z Reads: 29

```
Good luck. If you can't replace it yourself you can either send it to @JohnnyMeduse (US) or @Martinsp (EU).

I also found a guy willing to do DRV repairs (EU).

https://www.electric-skateboard.builders/t/eu-local-drv-repair-service/
```

---
## \#16 Posted by: RedEagle Posted at: 2018-03-30T21:32:48.236Z Reads: 25

```
I've gone ahead and changed the title to be easier to find for people with the same problem. Maybe it's a good idea to mark this thread as solved?
```

---

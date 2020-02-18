# Question about vx1 remote and focbox unity

### Replies: 33 Views: 589

## \#1 Posted by: Shawnl55 Posted at: 2019-10-08T02:25:33.713Z Reads: 137

```
Hi, if i get the vx1 remote from flipsky, and i have a focbox unity, do i choose vesc 4, vesc 6, or non vesc receiver for the unity? Also for the unity, what do i put for max braking regen current and max braking current? I know these r noobish questions but i just wanna check. Thanks!
```

---
## \#2 Posted by: skatardude10 Posted at: 2019-10-08T02:53:06.420Z Reads: 136

```
I believe the Unity is based off Vesc 4. I'd order that and even if you don't do UART control you can still use the PPM cable with the unity to connect via the non-vesc remote setup (ppm). Someone correct me if I'm wrong. And the only difference between vesc4 and vesc6 is two of the cables are swapped on the UART connection, so worst case scenario you order the wrong one and you would just need to cut two cables and swap them or pop 2 of the crimped connectors out and swap them.
```

---
## \#3 Posted by: Shawnl55 Posted at: 2019-10-08T03:09:06.216Z Reads: 125

```
Well i dont wanna get the wrong one or it might blow out my reciever.
```

---
## \#4 Posted by: Shawnl55 Posted at: 2019-10-08T03:13:12.246Z Reads: 121

```
Btw do u know if in the focbox unity app, for motor calibration, should the max braking current be the same or less as the max motor current? I have max motor current on the max amps my motor can handle.
```

---
## \#5 Posted by: Kalitapaws Posted at: 2019-10-08T14:35:22.994Z Reads: 106

```
Buy VESC4 version as @skatardude10 suggested. Once it arrives cross check the cables and make sure they match with your unity pin out card and the VX1’s wiring diagram in the little pamphlet. 

I modified my connector cuz I ordered vesc6 like a dummy but switch cables around and it works great. 👌
```

---
## \#6 Posted by: itsrow Posted at: 2019-10-08T15:19:49.843Z Reads: 103

```
I got the VESC 4 and lined my cables up, tried switching TX and RX couple times to no avail.  Any advice for setup?  Remote pairs with receiver fine, just cant seem to get VESC to read the receiver.
```

---
## \#7 Posted by: Kalitapaws Posted at: 2019-10-08T15:40:05.118Z Reads: 99

```
That’s odd. 

Have you finished set up on the app with remote? You have to finish making sure all settings are done and also make sure you are selecting UART in the UI.
```

---
## \#8 Posted by: itsrow Posted at: 2019-10-08T15:44:28.403Z Reads: 97

```
And set baudrate to 115200mhz
```

---
## \#9 Posted by: Ben.Nexus Posted at: 2019-10-08T15:45:59.308Z Reads: 90

```
Unity and VX1 UART doesn't really work, just use PPM. You lose basically nothing.
```

---
## \#10 Posted by: Kalitapaws Posted at: 2019-10-08T16:07:21.243Z Reads: 89

```
I’ll let you know once I get my computer. I’m using 9-something but I don’t remember at the top of my head.
```

---
## \#11 Posted by: Shawnl55 Posted at: 2019-10-08T16:10:05.623Z Reads: 89

```
What does baudrate do?
```

---
## \#12 Posted by: itsrow Posted at: 2019-10-08T16:41:55.126Z Reads: 84

```
I believe it just sets where the VESC is listening for inputs / outputs, similar to for frequency for remotes.
```

---
## \#13 Posted by: itsrow Posted at: 2019-10-08T16:42:15.751Z Reads: 83

```
I'm not even using a unity, just can't seem to get it to work :(.
```

---
## \#14 Posted by: Ben.Nexus Posted at: 2019-10-08T16:54:37.023Z Reads: 79

```
Can you show us images of the way you have it wired?
Have you tried using PPM?
```

---
## \#15 Posted by: itsrow Posted at: 2019-10-08T17:25:32.640Z Reads: 77

```
Im starting to think the VESC itself is fried, failed motor detection, no inputs of any kind and DRV failures oh god why :(
```

---
## \#16 Posted by: Ben.Nexus Posted at: 2019-10-08T17:45:42.193Z Reads: 76

```
Are your phase wires shorting? Or disconnected?
```

---
## \#17 Posted by: Crashmaster Posted at: 2019-10-08T18:33:26.544Z Reads: 77

```
I'm using a Non Vesc Vx1 in PPM mode on my Unity. I had a Vesc6 Vx1 it binded but would not connect to the Unity In PPM. So I bought the Non Vesc and it worked.
```

---
## \#18 Posted by: skatardude10 Posted at: 2019-10-08T22:50:27.982Z Reads: 71

```
baudrate is the communication rate/speed.
```

---
## \#19 Posted by: Shawnl55 Posted at: 2019-10-09T01:06:12.948Z Reads: 64

```
So im pairing the focbox with a metroboard battery. The battery has its own power switch and the focbox has its own power switch, is it ok to just not connect the battery switch and just use the focbox switch?
```

---
## \#20 Posted by: Shawnl55 Posted at: 2019-10-09T02:28:55.360Z Reads: 65

```
If i get vesc 4 receiver, will i select the uart mode in the focbox? And am i still able to use ppm mode for vesc4 receiver?
```

---
## \#21 Posted by: Kalitapaws Posted at: 2019-10-09T02:56:47.529Z Reads: 58

```
You should be able to use both. Not at the same time though I don’t think.
```

---
## \#22 Posted by: Shawnl55 Posted at: 2019-10-09T16:15:33.116Z Reads: 54

```
So i know theres a extra wire from the receiver that goes to the positive wire of the battery that reads the percent in the battery to show on the remote. How would this work if everything is in the focbox, does the focbox read the battery and send it to the remote?
```

---
## \#23 Posted by: Kalitapaws Posted at: 2019-10-09T20:41:05.610Z Reads: 55

```
No, you still want to connect that extra wire straight to the positive battery lead. :) 

Some remotes can do that however I believe, but at least the VX1 requires you to solder that to the battery positive from the battery going to the focbox.
```

---
## \#24 Posted by: Ben.Nexus Posted at: 2019-10-09T21:17:50.321Z Reads: 52

```
Yes, you do need to wire it into a positive lead. But you can use the AUX power on the unity.
```

---
## \#25 Posted by: Kalitapaws Posted at: 2019-10-09T22:03:31.971Z Reads: 51

```
oh! this I had no idea, its good to know. I just wired mine in haha.
```

---
## \#27 Posted by: Shawnl55 Posted at: 2019-10-11T18:42:34.182Z Reads: 42

```
For uart mode on the focbox, which baud would i choose for the vx1 vesc4 receiver?
```

---
## \#28 Posted by: PixelBot Posted at: 2019-11-07T14:41:20.789Z Reads: 35

```
Why is the extra wire needed?  Just for Battery indicator?  My VX1 works just fine with the 3 wire PPM harness.
```

---
## \#29 Posted by: flipskytech01 Posted at: 2019-11-09T09:53:49.948Z Reads: 30

```
Please choose the non vesc, PPM mode. The remote and receiver are the same, and the only difference among them are wires. VESC4 UART wires with 7 pins plug; VESC6 UART wire with 8 pins plug; non vesc comes with a PPM wire and a blue dupont wire connecting receiver "V" and battery "+" for skateboard battery status. 
For Unity, if using the UART mode, it's not smooth to use the slide turnon with high current motor. So, it's better to choose the PPM mode for Unity.
Before using the PPM mode, please do parameters setup. For UART mode, no need to do parameters setup, you can use it directly after the receiver and remote paried succesfully.
```

---
## \#31 Posted by: Shawnl55 Posted at: 2019-11-10T22:07:00.589Z Reads: 25

```
What is slide turn on?
```

---
## \#32 Posted by: Shawnl55 Posted at: 2019-11-10T22:08:00.478Z Reads: 25

```
For vesc4 UART and PPM mode, wiring the “V” receiver to the positive AUX JST-Ph 2-pin on the unity is ok right?
```

---
## \#33 Posted by: flipskytech01 Posted at: 2019-11-12T03:57:50.891Z Reads: 23

```
The unity can support slide turnon, and you can set via the tool
```

---
## \#34 Posted by: flipskytech01 Posted at: 2019-11-12T03:59:32.237Z Reads: 24

```
Please solder the V with battery "+" for skateboard battery status. You can review the diagram via our company website. Thanks
```

---
## \#35 Posted by: JuanMontero Posted at: 2020-02-10T23:37:54.985Z Reads: 8

```
Thanks for the detailed info. Then with the VX1 I won’t be able to use the slide turnon? Can you give more info on it please? I’m looking to buy a new remote to replace my broken nano x. VX1 looks nice but I love the slide turn on feature on my unity.
Thanks
```

---

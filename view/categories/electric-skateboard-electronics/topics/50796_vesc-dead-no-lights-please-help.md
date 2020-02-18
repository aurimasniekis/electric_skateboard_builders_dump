# VESC Dead (no lights) please help

### Replies: 16 Views: 935

## \#1 Posted by: RyuX Posted at: 2018-03-31T19:38:59.182Z Reads: 129

```
Dear Community.

When testing out a Bluetooth module on the UART Port somehow Ground and RX Shorted and I saw a little spark.
From that time on the VESC was dead.
The voltage on the PPM Receiver Module is still there. But the VESC itself will not show any LEDs.
Any hints on where to start troubleshooting ?
I can solder SMDs and troubleshoot but here I don't really know where to start - i also didn't see any fuses only many small Capacitors and resistors.
Please help :frowning:
```

---
## \#2 Posted by: FabianOdermatt Posted at: 2018-03-31T19:45:10.126Z Reads: 127

```
 [Here](https://github.com/vedderb/bldc-hardware/blob/master/design/BLDC_4.pdf)'s the schematics.
As far as I know the DRV feeds the LEDs, but I'm not sure tho.
```

---
## \#3 Posted by: RyuX Posted at: 2018-03-31T19:54:55.048Z Reads: 122

```
Hey thanks. I just checked.. The DRV has 48Vs on the PVDD pins. The STM32F4 however has no voltage on the VDD pins.
So I guess I will have a look at the supply line there :frowning:
```

---
## \#4 Posted by: RyuX Posted at: 2018-03-31T20:13:46.861Z Reads: 110

```
On the STM32F4 supply circuit GND and VDD are shorted. I will now remove all the capacitors but I think maybe the STM32F4 is dead. Is there anyone able to sell me a flashed STM32F4 with the firmware ? Man... what a bad day today :frowning:
```

---
## \#5 Posted by: MannyM0E Posted at: 2018-03-31T22:05:19.109Z Reads: 94

```
Samethig kinda happened with me too. But I just sent it to @ThermalM16 for repair
```

---
## \#6 Posted by: RyuX Posted at: 2018-03-31T22:07:37.219Z Reads: 92

```
I live in Austria / Europe - so I don't want to send it around the world. I will try to get a STM32F4 and try to load a bootloader on it. I am pretty sure the MCU is cooked :(
```

---
## \#7 Posted by: RyuX Posted at: 2018-04-01T07:56:57.552Z Reads: 74

```
Just a quick update - i desoldered the STM32F4 Chip and it seems that the short circuit from GND to VDD is now gone.. so the MCU is broken for sure.
It seems that short circuit also destroyed my BMS (it was a smart BMS).

So this little 0,1 sec short circuit will be costing me some serious bucks and long waiting time :disappointed_relieved:
```

---
## \#8 Posted by: RyuX Posted at: 2018-04-01T08:20:33.219Z Reads: 71

```
So i ordered a new STM32F405RGT6 now and a STLink V2. So hopefully I can flash the bootloader on it and revive the VESC again.
Also I will have to figure out how to get a flashed ATMEGA328P for the BMS - which might be hard as it's not open source.
I am really shocked how fragile everything is. But i surely learnt from that.
I will keep you guys updated on any progress of course

![20180401_101038|690x388](upload://gU9vsazwKUJc2IWoxiOa53zWlHn.jpg)![20180401_101021|281x500](upload://4cB7ljNGVF9r2Afqc0oWi7Sd8B.jpg)
```

---
## \#9 Posted by: RyuX Posted at: 2018-04-01T19:25:48.043Z Reads: 58

```
Small Update:
After desoldering the STM32F405 I connected the VESC again.
It seems I have +3,3V and +5V Voltage rail working - which means the 3V regulator and the DRV should be still good.
So replacing the STM32F4 should theoretically work when i can figure out how to properly get the bootloader and everything on there.
Fingers crossed..![IMG_20180401_212052|690x388](upload://fs49mZs8w0mmzIy3O5jXoLqQrkv.jpg)![IMG_20180401_212122|690x388](upload://mAqNlEur0Qlzjj9Lc47U624izSK.jpg)
```

---
## \#10 Posted by: RyuX Posted at: 2018-04-04T19:20:58.626Z Reads: 48

```
Short Update..
Got the STM32F405 from Mouser and replaced it.

I also changed the three Caps on on the Power Line to some Nichicon 1000uF.
Now waiting for the STLink V2 and hopefully I can connect and flash the bootloader.


![20180404_211609|281x500](upload://c2oOocV6TRBz468ZCdFGz22CYfU.jpg)![20180404_211621|281x500](upload://6ufQ4ytxwUnrzJM0M0SlgotkMrS.jpg)![20180404_190001|281x500](upload://9vqXsSc9g9Th6mmrG7kT9Deljuk.jpg)![20180404_211700|281x500](upload://ox6B3rRbBAn6NG85GETp1Q3O3WM.jpg)
```

---
## \#11 Posted by: Bjork3n Posted at: 2018-04-04T19:23:22.881Z Reads: 47

```
You can flash bootloader with vesc tool. 
No need for stlink :slight_smile:
```

---
## \#12 Posted by: RyuX Posted at: 2018-04-04T20:03:56.809Z Reads: 46

```
I am pretty sure that an Empty STM32F4 can not be connected VIA Usb directly without it already having a bootloader on it .. Or am I completely wrong ?
```

---
## \#13 Posted by: RedEagle Posted at: 2018-04-04T20:07:16.130Z Reads: 44

```
Why not try it and find out : )
```

---
## \#14 Posted by: Bjork3n Posted at: 2018-04-04T20:08:15.594Z Reads: 44

```
Don't know about that. 
I had maytech vesc that didn't come with  bootloader and used the vesc tool to install it with usb
```

---
## \#15 Posted by: RyuX Posted at: 2018-04-04T20:15:41.574Z Reads: 45

```
Not working here.. the STM32F4 is not recognized by usb at least on my board
```

---
## \#16 Posted by: RedEagle Posted at: 2018-04-04T20:21:13.687Z Reads: 43

```
Every time you plug a usb device in a pc you should hear a sound. If you don't hear it I guess st link is the way to go.
```

---

# HM-10 just blinks, no bluetooth signal

### Replies: 18 Views: 1362

## \#1 Posted by: denton Posted at: 2018-09-03T20:21:22.787Z Reads: 125

```
I am requesting some help with an issue I have had with the HM-10 Bluetooth module. 
It has worked a few times in the past but then just stopped working all together.
now it just blinks the red LED and is nowhere to be found looking for a bluetooth signal.

I have replaced the module 3 different times and the same issue repeats across all three modules.
I checked the wiring, because I was originally using a plug to go into the UART connector. 
So to ensure it isn't the plug I soldered in the wires directly just to try it out.
![IMG_2139-1|375x500](upload://pho4pSXh4Y25cUtqOvw3caJ2CKa.jpeg)![IMG_2140-1|375x500](upload://fPeJlYHlQl1vdXWPW36hZFnQi8a.jpeg)

Here is the SUPER shotty connections. I just threw it together really fast... so no judgment he said judging it anyway. 

I have the VESC settings at PPM & UART and set to 9600.
![38%20PM|690x453](upload://3Oo2VxQxC1HfNaffia3b6Xygcpd.png)![44%20PM|690x453](upload://pT7dWgDb3MV9XhK6mPdPRIiBP9N.png)

this is where I am at a loss. Is there a firmware issue? A bad UART port on my VESC? 
I bet there is something super simple here that I am just not aware of, so I turn to the experts.
Thanks for your help.
```

---
## \#2 Posted by: danielz Posted at: 2018-09-03T22:01:14.168Z Reads: 109

```
mine just quit too, so i googled the main chip cc2541 and it absolute max voltage was something like 3.9v, ive been using 5v! on the supply. so i assume its that that gradually killed mine. Ordered some resistors to create a voltage divider on the vesc tx pin, and ill use 3.3v for supply.
```

---
## \#3 Posted by: denton Posted at: 2018-09-04T03:08:52.484Z Reads: 108

```
let me know if that works!
I might try that soon, I need to order a new module.
```

---
## \#4 Posted by: Nordle Posted at: 2018-09-04T07:25:08.567Z Reads: 104

```
make a picture showing the pinout from the HM10 **with labeling**. because or you have another hm10 than me, or your wiring is completely wrong...
```

---
## \#5 Posted by: rey8801 Posted at: 2018-09-04T08:41:13.569Z Reads: 101

```
I think his wiring is correct the 5V wire in the black one and then follow from there GND / TX and RX. Where do you see it wrong?
Anyhow how does the module show up on your phone? Try to check this app "Serail Bluetooth Terminal" if you can connect. If you do not see your module at all with your phone and you are running Android Oreo, then try with an older phone. With Oreo they change the BLE connection and most of the clone modules do not work anymore.
```

---
## \#6 Posted by: Nordle Posted at: 2018-09-04T09:06:45.163Z Reads: 102

```
![image|678x245](upload://dFNvFkVhJDHaf8kAwRsRWjeP9xp.jpeg)

his red wire goes from hm10_vcc to tx_vesc pin?
```

---
## \#7 Posted by: rey8801 Posted at: 2018-09-04T09:12:07.047Z Reads: 100

```
i think he has like this one ![image|678x345](upload://rBLI4aUWsAFSwJyqniIx3KKimk0.jpg)
Where actually the pin layouts are mirrored
```

---
## \#8 Posted by: denton Posted at: 2018-09-04T13:38:38.721Z Reads: 92

```
Here is the update of how I have it wired in with the reference photo photoshopped in.

![update|375x500](upload://hcbKDVgUnYjeuUyO3J14mleQzDR.jpg)
```

---
## \#9 Posted by: rey8801 Posted at: 2018-09-04T13:39:58.046Z Reads: 87

```
Can you post the back of your module you should have what the pin are. Like vcc, gnd ecc
```

---
## \#10 Posted by: denton Posted at: 2018-09-04T13:41:30.167Z Reads: 87

```
not until later on tonight, it is currently hot glued to the board at my apartment. 
I will grab a picture of the other modules later on if I can at lunch.
```

---
## \#11 Posted by: danielz Posted at: 2018-09-04T16:37:58.784Z Reads: 85

```
i bought a logic level converter instead now, and for reference mine is a genuine hm-10
```

---
## \#12 Posted by: Lionpuncher Posted at: 2018-09-04T19:24:46.493Z Reads: 79

```
That looks like a dsd bt module from Amazon?
I couldn't get that one to work either. I believe it's a clone module.
```

---
## \#13 Posted by: denton Posted at: 2018-09-06T00:25:36.875Z Reads: 77

```
Here is what all three of them look like. 
![image|375x500](upload://7fRvDlLMzGcRTPp8w9ZSQvmIu8B.jpeg)
```

---
## \#14 Posted by: Andy87 Posted at: 2018-09-06T05:15:29.893Z Reads: 81

```
Did you try to find the module with a BLE scanner?
I had issues with my first module too.
Was searched for it with a BLE scanner and after I could connect always.

Make sure the bt signal is not used in a other app. Could be an issue too.

This modules where working rock solid for me.
iOS and Android and cheap too

http://s.aliexpress.com/mIviqeUn
```

---
## \#15 Posted by: rey8801 Posted at: 2018-09-06T05:27:36.133Z Reads: 78

```
The wiring is correct. You are using a clone which is fine, only problem is to get it work with Android 8.x. I have tried a lot of modules since I am selling them and the module @Andy87 suggested is a clone too but has a different firmware compare the one you have that I think is a CC2541 clone. Anyhow the Bt05 clone usually work with Oreo although I have some that doesn't dipenda of old they are and which firmare they have installed. If you want to be really sure I advice to flash the original HM10 firmware on your clone https://forum.arduino.cc/index.php?topic=393655.0 then they became 100% compatible and they show up as HM10 on your phone. No problem anymore. That what I susally do with my modules.
```

---
## \#16 Posted by: danielz Posted at: 2018-09-07T19:03:22.258Z Reads: 70

```
Mine wasnt dead in the end as i thought, must be either vesc firmware or phones firmware has changed. Neither vesc shows any data on either of the hm-10s (Genuine units) Annoying.
```

---
## \#17 Posted by: denton Posted at: 2018-09-07T19:30:07.661Z Reads: 70

```
I have an iPhone and it may be an OS update that changed it, but it was working just fine a few months ago with the VESC firmware that was on it. The VESC is up to date. However I don't have a clue on how to check the firmware on the Bt05 which is what would show up in the Eskate App. 

So what is my next course of action?
```

---
## \#18 Posted by: danielz Posted at: 2018-09-29T12:50:17.744Z Reads: 64

```
It was the most recent firmware!!! vesctool 0.95. I downgraded with 0.91 and bam it all works again. I repeated the test. For whatever reason data isnt being sent on the latest firmware. Im using vesc 4.10 and genuine keyes hm-10s.
```

---

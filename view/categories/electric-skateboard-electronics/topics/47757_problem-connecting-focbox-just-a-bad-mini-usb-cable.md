# Problem connecting focbox. Just a bad mini usb cable :sunglasses:

### Replies: 20 Views: 696

## \#1 Posted by: stormboard1 Posted at: 2018-02-28T15:43:17.762Z Reads: 133

```
Finished my battery last night just went to try check the Vesc and went plug it in heard a pop..polarities are correct and xt90s is fully pushed in..![image|375x500](upload://2wE6XVEBygAPTrN5hxPh1HbZxHx.jpeg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-02-28T15:55:59.981Z Reads: 123

```
A pop from the FOCBOX? wasnt it the spark sound?
Also, were the phase wires connected to something? Maybe they touched and the pop was a FET/DRV. 
try opening it up and see if there is anything visibly burned
```

---
## \#3 Posted by: stormboard1 Posted at: 2018-02-28T16:00:33.212Z Reads: 117

```
I didn’t realise I need the loopkey out it was plugged in so current rushed to the xt60 connector and there’s a lil chat mark on the xt60 from the loop key side here
![image|375x500](upload://8UasKaUjPWrHgqod2X34LcYGb01.jpeg)
```

---
## \#4 Posted by: Martinsp Posted at: 2018-02-28T16:02:33.672Z Reads: 110

```
Oh, so it was the spark that you heard? I think that it should work because before i found out about antispark plugs and switches my switch was disconnecting connectors :D
```

---
## \#5 Posted by: stormboard1 Posted at: 2018-02-28T16:22:57.659Z Reads: 105

```
Spark and it synged the xt60 from the loopkey that connects to the xt60 on the focbox you can see it in the pic above was just a pop as it just touched
```

---
## \#6 Posted by: stormboard1 Posted at: 2018-02-28T16:32:35.141Z Reads: 102

```
Does my motor need be connected before I plug in the loop key just to check the Vesc..have the motor wires insulated with electrical tape on the Vesc (gotta change the bullet connectors
```

---
## \#7 Posted by: MLT34 Posted at: 2018-02-28T16:39:32.360Z Reads: 98

```
The pop from a spark is normal, its the capacitors charging up rapidly. Not great for the connectors if you do it repeatedly, which is why an antispark switch or antispark connector is recommened. But if your polarities are correct and everything still works, it was just a dramatic spark and popping noise.
```

---
## \#8 Posted by: stormboard1 Posted at: 2018-02-28T17:23:35.379Z Reads: 91

```
Do I need my motor connected to connect the focbox then loop key(won’t make that mistake again😂)
```

---
## \#9 Posted by: Deckoz Posted at: 2018-02-28T17:37:43.142Z Reads: 90

```
No... You can program the focbox excluding motor detection without the motor plugged in.

You need bldc tool as the focbox comes stock with 2.18

Other wise if your using vesc tool or ack firmware you will need to flash before you can connect and read.
```

---
## \#10 Posted by: stormboard1 Posted at: 2018-02-28T18:01:10.331Z Reads: 81

```
Nice one how do I flash it?
```

---
## \#11 Posted by: Deckoz Posted at: 2018-02-28T18:05:32.218Z Reads: 76

```
Connect in the tool you want to use and go-to the firmware tab...
```

---
## \#12 Posted by: stormboard1 Posted at: 2018-02-28T18:23:46.944Z Reads: 69

```
I’m in the bldc tool but says not connected is that because the motors not connected ya
```

---
## \#13 Posted by: Deckoz Posted at: 2018-02-28T18:25:39.509Z Reads: 67

```
No.

You need to select the com port that the vesc is connected to. Then click connect. 

Motors not connected have nothing to do with the "not connected" in the lower right.
```

---
## \#14 Posted by: stormboard1 Posted at: 2018-02-28T18:33:03.565Z Reads: 69

```
No com port just a blank drop down menu that doesn’t drop down![image|375x500](upload://2M5R0ESFm6rt22UeNem62ahB1gL.jpg)
```

---
## \#15 Posted by: Deckoz Posted at: 2018-02-28T18:33:28.891Z Reads: 66

```
You need to install the STM32 drivers then...
```

---
## \#16 Posted by: stormboard1 Posted at: 2018-02-28T18:41:53.579Z Reads: 63

```
Where are they
```

---
## \#17 Posted by: Deckoz Posted at: 2018-02-28T18:44:12.246Z Reads: 65

```
Windows Mac or Linux?
```

---
## \#18 Posted by: stormboard1 Posted at: 2018-02-28T18:48:34.803Z Reads: 66

```
Windows 10 bro
```

---
## \#19 Posted by: Deckoz Posted at: 2018-02-28T18:48:48.692Z Reads: 67

```
http://www.st.com/web/en/catalog/tools/PF257938
```

---
## \#20 Posted by: stormboard1 Posted at: 2018-02-28T21:46:19.774Z Reads: 56

```
Was just a bad usb cable🙌🏻
```

---

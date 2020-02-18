# Broken focbox no lights

### Replies: 21 Views: 850

## \#1 Posted by: Bloop Posted at: 2018-05-10T20:56:51.963Z Reads: 162

```
Hey i have 2 focboxes with problems..
A few months ago i used them and only one would detect on BLDC tool the other one wouldnt. Both of them worked in rest i could connect the motor and remote and spin the motor but one of them would not detect on pc.

Today i tried to connect them again and none of them would even turn on .. no lights would turn when connect them to the battery. 

Who could give me a few idea of what can i try and do to understand what is wrong with them ?? 

Thank you.
```

---
## \#2 Posted by: Bloop Posted at: 2018-05-11T05:36:49.379Z Reads: 129

```
Anyone in uk that repairs focboxes ??
```

---
## \#3 Posted by: bigben Posted at: 2018-05-11T05:41:06.127Z Reads: 125

```
@EnertionSupport might be able to help or @Martinsp does repairs I think?
```

---
## \#4 Posted by: Scoo_B_SK8 Posted at: 2018-05-11T06:29:40.062Z Reads: 122

```
Have you opened them up at all to see any obvious signs?...
-DRV chip
-Fets + thermal pads ... no clear film
-Voltage regulator (Logic)
```

---
## \#5 Posted by: ARetardedPillow Posted at: 2018-05-11T07:13:32.500Z Reads: 113

```
Do you have pictures of how they are connected?
```

---
## \#6 Posted by: Bloop Posted at: 2018-05-11T07:27:56.893Z Reads: 106

```
Yeah i opened them couldnt see anything weird :-?? nothing burnt no idea. I will take some pictures when i can.

@ARetardedPillow How they are connected ?? i just connected the battery to the vesc ?? what do you mean?
```

---
## \#7 Posted by: ARetardedPillow Posted at: 2018-05-11T07:34:42.274Z Reads: 106

```
Like pictures of the solder joint and stuff, just making sure that the solder joint is nice and sturdy and they're not connected in reverse polarity. Also check the joints of the phase wires and etc.
```

---
## \#8 Posted by: Martinsp Posted at: 2018-05-11T07:59:37.559Z Reads: 104

```
Pictures may be useful. As for solder joints, check if there is voltage on the last connector on focbox, if there is and the focbox does not show any signs of life, measure voltage on the ppm connector between red and black. There will most probably be 0V which would point to internal hardware failure.
Would you be able to send us a picture of the PCB? Ideally of both focboxes and both sides maybe there are some signs of what happened 

I do repair vescs, I am located in Slovakia. More info can be found here or pm if you have any questions. http://electricskateboard.repair/index.php?id_product=12&controller=product 

Thank you @bigben for the mention. 

Martin.
```

---
## \#9 Posted by: Bloop Posted at: 2018-05-11T12:04:53.595Z Reads: 95

```
![52 PM|282x500](upload://jM68RIgg8spI1rzeEefQjCHwsYj.jpeg)![04 PM|282x500](upload://qvk8H5Uo0gl0KOm26DxIsIb0trX.jpeg)![29 PM|282x500](upload://gnsPLtywUVHmQHU7kmrUkWdUtky.jpeg)![13 PM|282x500](upload://w6Njv53i7h22dcwzZ9eYNUsHKwk.jpeg)
```

---
## \#10 Posted by: Martinsp Posted at: 2018-05-11T12:09:06.240Z Reads: 92

```
Thank you.
Can you please check the CAN chip on the firs picture (small, 8 legs next to PPM wires) that the two black dots are not burn marks? They seem like burn marks, that would most probably be shorting the 5V line on your FOCBOX preventing it from turning on.

If the dots are burn marks, I would assume that the VESCs were connecting using CAN and the fault would be most probably same on both VESCs

There dont seem to be any obvious burn marks on the other pictures
```

---
## \#11 Posted by: Bloop Posted at: 2018-05-11T12:11:13.443Z Reads: 91

```
The PPM is 5V hmm
```

---
## \#12 Posted by: Martinsp Posted at: 2018-05-11T12:12:09.227Z Reads: 88

```
on the focbox with the dots/burn marks?
So you are also getting the blue LED?
```

---
## \#13 Posted by: Bloop Posted at: 2018-05-11T12:19:13.247Z Reads: 85

```
yeah the one with burn marks im getting 5v on ppm but no led. No blue or red led are turning on when connected :-?? ...
```

---
## \#14 Posted by: Bloop Posted at: 2018-05-11T12:21:19.752Z Reads: 84

```
Ah sorry is not 5v on ppm.. is fluctuating between 2 an 5... my bad x.x
```

---
## \#15 Posted by: Martinsp Posted at: 2018-05-11T12:25:15.136Z Reads: 84

```
Hmm that would be a short somewhere, there may be a problem with the DRV that is supposed to create the 5V and it is causing the fluctuation or there is something shorting it in a way.

If you want to try to repair them yourself, I would start with the CAN chip, it is the easiest to desolder and if the VESCs were connected via CAN it is pretty likely the problem. Not 100% but it is possible.
```

---
## \#16 Posted by: Bloop Posted at: 2018-05-11T12:28:04.976Z Reads: 82

```
I understand. Yeah i had someone playing with it over CAN too.. so is likely. 
Can you tell me what the chip is called or where could i find it. 

Also any idea what could be the cause of it not being recognized by the pc ? I wasnt able to read it on BLDC tool so i couldnt program it.
```

---
## \#17 Posted by: Martinsp Posted at: 2018-05-11T12:33:43.113Z Reads: 80

```
Well if the VESC is not turning on the PC does not see anything connected. The PC only recognizes the VESC after it boots (after the initial red LED flashes)

The chip can be found here based in UK http://uk.farnell.com/texas-instruments/sn65hvd232d/ic-can-transceiver-1mbps-8soic/dp/1103107?st=SN65HVD232D
```

---
## \#18 Posted by: Bloop Posted at: 2018-05-11T12:40:17.036Z Reads: 78

```
Yeah ofc i mean before the CAN got burnt. When it was working and i managed to spin the motors etc i still could not connect it to my laptop.
```

---
## \#19 Posted by: CarlCollins Posted at: 2018-05-12T06:49:31.068Z Reads: 63

```
@Bloop

Have you contacted Enertion Support?
I think we can handle this for you.
Please email at support@enertionboards.com 
Also let us know from where you purchased them.
```

---
## \#20 Posted by: Bloop Posted at: 2018-05-12T07:05:47.859Z Reads: 57

```
Hey @CarlCollins I got them from someone on forum and dont have waranty + had really bad experience with enertion support + late shipping and not in AU so idk feels a bit too complicated..

Thank you.
```

---
## \#21 Posted by: CarlCollins Posted at: 2018-05-12T07:14:29.106Z Reads: 55

```
@Bloop

If you purchased it from reseller then we will be able to solve it.
Please contact support. I hope this time your experience will not be bad :slight_smile:
```

---

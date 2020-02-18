# 10S5P battery pack with BMS wont charge

### Replies: 39 Views: 2310

## \#1 Posted by: nikoli280 Posted at: 2017-10-16T17:34:48.053Z Reads: 171

```
Hi everyone. I finally got my Battery pack with BMS finished. The Spagetti cables reads the right voltages from 3.7 and up to 37.

But when i attach the 42V battery charger to the BMS. The light on the battery charger goes from green to red and then turns off then tries the same again. It is clear that the voltage is cut by some sort of protection. Either by the BMS or the power supply. I mostly think its the power supply. 

I dont know what can cause this. The cables are correctly installed and voltages read right.

When i installed the BMS i firstly tried to solder the battery negative leads directly to the BMS. It gave a spark and a black mark around the spot. I tried to see for damage or hot components or smell. But nothing i could find was suspicious. So i just assumed it was a connection spark.

Can it maybe have fried the BMS with the spark? Does not seem right but i cant see any other reason why it wont work,

I have had the whole battery connected now and nothing gets hot or smells. 

lookinh forward to hearing your advice.

<img src="/uploads/db1493/original/3X/9/0/90ae1b49c2d073050664b282306bda77f79f68e0.jpg" width="375" height="500"><img src="/uploads/db1493/original/3X/c/d/cd85a89f36e493e406d8446dd9a0481d2d5d64ac.jpg" width="375" height="500">
```

---
## \#2 Posted by: willpark16 Posted at: 2017-10-16T17:57:22.576Z Reads: 153

```
How did you wire your battery?
```

---
## \#3 Posted by: nikoli280 Posted at: 2017-10-16T18:08:41.914Z Reads: 150

```
5 LG H4 in standard parrelel packs and then with a single positive and negative cable then i connected the BMS leads cable to each of the red positives and connected the packs of 5 to each other, which after i could see a total voltage of 36V
```

---
## \#4 Posted by: willpark16 Posted at: 2017-10-16T18:12:40.707Z Reads: 145

```
That would be 5s10p
```

---
## \#5 Posted by: willpark16 Posted at: 2017-10-16T18:13:51.318Z Reads: 145

```
Show me photos of how you actually wired it
```

---
## \#6 Posted by: nikoli280 Posted at: 2017-10-16T18:26:37.099Z Reads: 139

```
<img src="/uploads/db1493/original/3X/6/f/6f2bd3f1f3af93139d19438fe282af7c1ea26fcf.jpg" width="690" height="209">
```

---
## \#7 Posted by: willpark16 Posted at: 2017-10-16T18:31:47.907Z Reads: 138

```
You might have attached your balance leads in reverse
```

---
## \#8 Posted by: pennyboard Posted at: 2017-10-16T18:34:01.122Z Reads: 137

```
Looks like 10s5p to me. 

@nikoli280 what brand of bms are using? It's possible you fried it with that spark.
```

---
## \#9 Posted by: willpark16 Posted at: 2017-10-16T18:35:05.397Z Reads: 136

```
Diagram wasn't uploaded
```

---
## \#10 Posted by: nikoli280 Posted at: 2017-10-16T18:36:23.747Z Reads: 135

```
This is the BMS

http://www.batterysupports.com/lion-lipo-nbsp-36v-nbsp-10s-c-32_41.html
```

---
## \#11 Posted by: nikoli280 Posted at: 2017-10-16T18:37:32.127Z Reads: 130

```
I just think it is wiered that i get a correct voltage reading at the end after BMS, if that could be possible then i dont see that the BMS could be the problem. please correct me if im wrong.
```

---
## \#12 Posted by: nikoli280 Posted at: 2017-10-16T19:29:24.346Z Reads: 126

```
Does anyone have a possible solution. This bugs me the hell out.
```

---
## \#13 Posted by: Fiori Posted at: 2017-10-16T19:38:09.369Z Reads: 122

```
I would check your BMS wiring as willpark said. You may have your balance leads reversed. You can attempt to see if you can manually charge the battery by bypassing the bms as well.
```

---
## \#14 Posted by: nikoli280 Posted at: 2017-10-16T19:43:58.078Z Reads: 113

```
I have checked the cables and they seem right. starting from right to left i get 3.6V 7.2 and so on up to 36V
```

---
## \#15 Posted by: Jumpman Posted at: 2017-10-16T19:58:23.968Z Reads: 108

```
On the link above it seems to indicate the wiring should be from right to left, unfortunately.
```

---
## \#16 Posted by: nikoli280 Posted at: 2017-10-16T20:11:48.441Z Reads: 107

```
Yes sorry i typed wrong. my configuration is from right to left.
```

---
## \#17 Posted by: Fiori Posted at: 2017-10-17T05:14:18.492Z Reads: 98

```
It seems odd that you would get a spark when connecting the negative battery cable.....Did you do that while the balance connector was plugged into the bms?

Can you tell me the voltage at these two wires? Also, in the picture, is that the top or bottom of the connector(when plugged in)? I

edit: looks like the top i just want to make sure

<img src="/uploads/db1493/original/3X/e/f/ef36001a665d08788c2b2a9de94a37ac9a867f22.jpg" width="423" height="500">
```

---
## \#18 Posted by: nikoli280 Posted at: 2017-10-17T05:47:29.965Z Reads: 90

```
I only got the spark when I was trying to solder the negative lead from the battery directly to the BMS. In the instant the soldering iron touched I got a spark. 

Then I decided to make small plugs from the BMS and after that I could connect and disconnect the battery negative leads from the battery without spark
```

---
## \#19 Posted by: nikoli280 Posted at: 2017-10-17T05:48:45.417Z Reads: 89

```
Is the 2 plugs the end of each side of the Ballance cable? If it is then I get 36V. Which should be fine right
```

---
## \#20 Posted by: Fiori Posted at: 2017-10-17T05:52:23.279Z Reads: 92

```
> I only got the spark when I was trying to solder the negative lead from the battery directly to the BMS. In the instant the soldering iron touched I got a spark.

Was the 11 pin bms connector plugged into the BMS prior to you soldering the negative cable?

> Is the 2 plugs the end of each side of the Ballance cable? If it is then I get 36V. Which should be fine right

I need the voltage at the green point, and the voltage at the purple point in the photo I posted
```

---
## \#21 Posted by: nikoli280 Posted at: 2017-10-17T06:02:49.137Z Reads: 88

```
The Ballance connector was not connected when soldering.

Can you show me on this picture where I need to check?<img src="/uploads/db1493/original/3X/1/5/1579c64c861af0bb0e822617c2f825d6a5b0d236.jpg" width="536" height="444">
```

---
## \#22 Posted by: Fiori Posted at: 2017-10-17T06:05:08.370Z Reads: 85

```
I can show you on that picture, but I purposely used the picture you provided to ensure we are measuring the correct spot
```

---
## \#23 Posted by: nikoli280 Posted at: 2017-10-17T06:18:07.240Z Reads: 81

```
Yes but I can't see where to measure because of the shrink wrap. And I can not just measure the wires since all the leads are positive.
```

---
## \#24 Posted by: nikoli280 Posted at: 2017-10-17T06:19:17.164Z Reads: 82

```
Sorry they are not positive. They are between a positive and negative
```

---
## \#25 Posted by: Fiori Posted at: 2017-10-17T06:20:04.602Z Reads: 81

```
you can probe the pin easily, and then put your negative lead straight to the battery negative cable.
```

---
## \#26 Posted by: nikoli280 Posted at: 2017-10-17T06:27:09.762Z Reads: 77

```
Yeah okay. That I have done. 

When I have connected the probe to the first pin from the right. And the other to the negative I get a voltage of 3.6 

When I connect to the negative and then the last pin I get 36V. 

So it should work. I have done a test all the way through were I got. 

1. 3.6V
2. 7.2V
3. 10.8V 

And so on
```

---
## \#27 Posted by: egzplicit Posted at: 2017-10-17T07:54:44.788Z Reads: 72

```
I don’t understand how can you get a spark when connecting the negative wire to the BMS while the balance leads and everything else is disconnected. It’s not a complete circuit so unless you had other stuff connected, it should not spark.

When I hooked my BMS I did the same, I soldered the b- from the BMS to the minus of the battery. Then  c- to the charging socket. Then measured all pins from the balancing connector to make sure everything is ok. Then plugged it into the BMS and proceeded to charge the pack.
```

---
## \#28 Posted by: egzplicit Posted at: 2017-10-17T07:58:24.669Z Reads: 71

```
Maybe try measuring from b- on the BMS to last pin on the balancing port. You should see 36v.
```

---
## \#29 Posted by: nikoli280 Posted at: 2017-10-17T08:30:00.909Z Reads: 68

```
I do see 36v. I thought first that the spark was a simple connection spark. But I'm not sure
```

---
## \#30 Posted by: egzplicit Posted at: 2017-10-17T08:44:40.480Z Reads: 66

```
Then maybe the BMS is dead. You can't get sparks on incomplete circuits so some other wires must have been connected or something. Maybe it's time to test a new bms...
```

---
## \#31 Posted by: nikoli280 Posted at: 2017-10-17T16:49:09.653Z Reads: 60

```
Okay now i tried again with no diffrence. But when i unplugged the BMS i took out the negative leads first. Nothign happened. Dont you guys think that is why it does not work? When a BMS has connected the 10 leads alone it is said to burn out on the website.

So if nothing happens now then it must have happended before therefore the bms is broken?
```

---
## \#32 Posted by: psychotiller Posted at: 2017-10-17T20:03:56.981Z Reads: 52

```
Here's my take, Something was wrong when you encountered the spark. Then when you implemented the plug, and got no spark the second time, the damage was already done. You don't get a spark now because whatever short you created while wiring the bms is fried. The spark was the first indication of a problem. Read, Replace, Repeat.
```

---
## \#33 Posted by: nikoli280 Posted at: 2017-10-17T20:24:03.989Z Reads: 49

```
Sound right. Now i just have to make sure that i dont make the spark again. Do you know if it is possible to make the spark with the negative wire from the battery pack and the BMS and the soldering iron`?
```

---
## \#34 Posted by: psychotiller Posted at: 2017-10-17T20:28:53.431Z Reads: 49

```
I would say only if something else is connected incorrectly.
```

---
## \#35 Posted by: nikoli280 Posted at: 2017-10-17T20:37:37.112Z Reads: 50

```
Do you have a smart idea of how to test. 

I can use the ground and positive to get a total of 35.6v Which is what i want.

I can measure on the Ground of the pack and then measure each of the cables in the balance cable to get.

1. 3.6V 
2. 7.2V
3. 10.8V

And so on. So that seems to be in order.
```

---
## \#36 Posted by: psychotiller Posted at: 2017-10-17T20:46:42.125Z Reads: 46

```
Not specifically...you shouldn't be seeing sparks though while connecting a bms
```

---
## \#37 Posted by: Fiori Posted at: 2017-10-17T21:17:07.082Z Reads: 45

```
What everyone here is saying, is that you should not have power at that bms for any reason unless the balance plug is connected, or your wiring is incorrect in some way. The only way that BMS receives power is those balance leads. If you got a spark, then there was either power at your BMS, or power at your negative cable(eg incorrect wiring, positive lead instead of negative ect...). 

For that spark to have occurred, you would have HAD to have power at the bms, or you were connecting the positive lead of your battery instead of the negative. There is no other possible way for that lead to spark. Unless your solder iron has in internal short(highly unlikely).
```

---
## \#38 Posted by: nikoli280 Posted at: 2017-10-17T21:47:15.391Z Reads: 49

```
Okay but if I make a voltage check with red probe on positive and black probe on negative I get 35.6V but I reverse I get -35.6V that indicates that the cables are rightfully installed right?
```

---
## \#39 Posted by: Fiori Posted at: 2017-10-17T21:49:10.756Z Reads: 46

```
Correct.

10 chars
```

---

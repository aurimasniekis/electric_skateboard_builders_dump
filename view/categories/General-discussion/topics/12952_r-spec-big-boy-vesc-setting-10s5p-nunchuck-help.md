# R-SPEC big boy &#124; VESC setting &#124; 10s5p &#124; nunchuck &#124; help

### Replies: 9 Views: 1254

## \#1 Posted by: kyo Posted at: 2016-11-13T02:58:03.615Z Reads: 160

```
I am setting my vesc atm. Would u eboarder out there with exp give me advice or some figure pleass?

<img src="/uploads/db1493/original/3X/3/d/3d62dc8bcb9b17afd868308eeed93ae2a86979b9.JPG" width="666" height="500">

Here are my setting with bldc

<img src="/uploads/db1493/original/3X/1/e/1e2d334dac928027fcaa875dc7e7fc28f41f7527.JPG" width="666" height="499">
```

---
## \#2 Posted by: Blasto Posted at: 2016-11-13T03:16:02.093Z Reads: 150

```
my setup w 10S4P & R-spec big boy. Leave your max input voltage at 57V, lower your max batt
<img src="/uploads/db1493/original/3X/c/3/c315dd988069d1929a513b9cf2d597f485fa85f9.png" width="690" height="454">

for more reference

http://www.electric-skateboard.builders/t/the-mule-i-mono-r-spec-big-boy-i-10s4p-i-zenit-freeride-deck-i-vesc-x-i-foc-enabled/11238?u=blasto
```

---
## \#3 Posted by: kyo Posted at: 2016-11-13T04:00:19.886Z Reads: 132

```
Thanks so much, one quick question: the brake is kinda hash, i mean its kinda strong. Is there a placenin bldc tool that i can configure the brake?
```

---
## \#4 Posted by: Jinra Posted at: 2016-11-13T04:02:32.866Z Reads: 127

```
motor min is your brake, lower it to 30-40 for softer braking.
```

---
## \#5 Posted by: Plumb77 Posted at: 2017-02-04T11:51:35.209Z Reads: 85

```
Wondering if I would be able to use these same settings I have a 10s3p with a 6374 190kv motor
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-02-04T12:12:48.603Z Reads: 85

```
You don't use a lot of the capacity of your battery. So you should set the battery cutoff start to 30 and the cutoff end to 28. With those settings you are still on the safe side.
For the 10S3P the battery min should be reduced to -12 and you should do another motor detection if not only the battery changed.
```

---
## \#7 Posted by: Eboostin Posted at: 2017-02-04T17:17:08.814Z Reads: 72

```
I thought 3V (30V on 10S) a cell was the recommended cutoff
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-02-04T17:22:22.575Z Reads: 70

```
For the most Li-Ion cells you could go down to 2.5V a cell. But from 2.8V till 2.5V there is not much energy left and the voltage sag is quite huge. So i recommend to set the cutoff start to 3.0V and the end to 2.8 so that the voltage will be in between and never lower than 2.8V to be on the safe side. But to set the cutoff start higher than 3.0V doesn't make much sense because then you reduce the power already too early.
I need to test a start of 2.9V and end 2.8V. Maybe that even works without issues. But weather is too bad at the moment.

But for a LiPo battery the start should be at 3.6V and end at 3.4V. OF if you want to go low then 3.5V and 3.3V.
```

---
## \#9 Posted by: Plumb77 Posted at: 2017-02-04T18:02:06.145Z Reads: 64

```
Interesting would I be asking to much if I could maybe PM you so I am going to be setting up my first build today or tomorrow. I've read the VESC set up guide in the forum and it is a little confusing. I by no means don't need to maximize the settings for speed just want a reliable set up with Regen braking. I'm using 10s3p with built in BMS 25r Samsung cells. Enertion 4.12 vesc.
```

---

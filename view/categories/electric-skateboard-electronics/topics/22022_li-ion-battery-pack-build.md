# Li-ion battery pack build

### Replies: 17 Views: 1403

## \#1 Posted by: Idobartal Posted at: 2017-04-29T09:34:15.754Z Reads: 262

```
I have INR18650 cells... should i maka 2 batteries of 6s3p of 6000mah ? or 2 batteries of 5s4p 8000mah? What should i build ?I have the sk3 turnigy 168 kv and a maytech vesc
```

---
## \#2 Posted by: bartroosen12 Posted at: 2017-04-29T09:55:39.873Z Reads: 260

```
6S3P always better
```

---
## \#3 Posted by: Idobartal Posted at: 2017-04-29T11:24:14.856Z Reads: 248

```
Is it ok to connect two 6sp3 in series to make a 12s3p battery for this setup right?
```

---
## \#4 Posted by: bartroosen12 Posted at: 2017-04-29T16:16:21.371Z Reads: 227

```
Yeah of course even better, your esc can handle 12S?
```

---
## \#5 Posted by: saul Posted at: 2017-04-29T16:19:21.825Z Reads: 218

```
10s4p has a bit more capacity. 
12s3p if you want extra speed.
```

---
## \#6 Posted by: Alan_Smithee Posted at: 2017-04-29T18:02:27.549Z Reads: 198

```
[quote="Idobartal, post:1, topic:22022"]
INR18650
[/quote]

what cells exactly? INR18650.. is not enough to identify your cells.
```

---
## \#7 Posted by: Idobartal Posted at: 2017-04-30T00:05:54.351Z Reads: 169

```
Maytech VESC, up to 12s...
```

---
## \#8 Posted by: Idobartal Posted at: 2017-04-30T00:07:02.201Z Reads: 171

```
Can you please explain the calculation of these factors ?
 I have a 2000mah cells...
```

---
## \#9 Posted by: Iam319 Posted at: 2017-04-30T04:59:23.996Z Reads: 163

```
I have a 10s2p battery setup with 2200 mAh batteries. if I am right in how i calculated it, I should have 162.8 Watt hours. would someone check my work to make sure Im not drastically over or underestimating the capabilities of my batteries?
```

---
## \#10 Posted by: saul Posted at: 2017-04-30T06:56:32.743Z Reads: 158

```
[quote="Idobartal, post:8, topic:22022, full:true"]
Can you please explain the calculation of these factors ? I have a 2000mah cells...
[/quote]

umm math? 10*4  = 40 cells. 12*3 = 36 cells. 10s4p has 4 more cells = more capacity.
12s3p has higher voltage, so more rpm. 
2ah cells are really small. and probably can't produce enough amps. dont expect great performace either way..
```

---
## \#11 Posted by: Idobartal Posted at: 2017-04-30T11:32:22.758Z Reads: 136

```
Thx again, i know the math but im not sure about the meaning...
12s3p has more voltage 
And 10s4p has more amps (6000mah vs 8000mah)
Right?

Technologically speaking, what define that the 12s3p drains faster ? And how come less amps give more rpm ? Thx again
```

---
## \#12 Posted by: Alan_Smithee Posted at: 2017-04-30T18:13:58.016Z Reads: 127

```
since you're not telling us what cells exactly you use, I'm going to assume its either samsung 20R (22A discharge) or 20Q (15A discharge) cells. 
So with 3S you could draw 66A/45A and with 4S you could draw 88A/60A.
I'd definitely go with 4S, since its not only more capacity but it will also run the cells not as close to their limits which will drastically improve their life expectancy (number of cycles).

I run a 10S6P battery (because I have only 10A cells) with a sk3 192kv motor. Top speed is 36km/h on rather small 70mm wheels right now. so on 10s your 168kv motor should have more torque (mine is already pretty good) and similar or better speeds if you use larger wheels like 90mm which would be recommended anyway.
```

---
## \#13 Posted by: Idobartal Posted at: 2017-04-30T19:01:03.197Z Reads: 126

```
Sorry about the delay, the cells are from an electric bike battery (friends bike was stolen without the battery, the bike wes new and so is the battery)

I dont see any brand on the cells, but they are 2000mah.
```

---
## \#14 Posted by: OskarCastrone Posted at: 2017-04-30T19:56:08.825Z Reads: 120

```
I would not recommend using those cells then. They are probably some cheap chinese cells then... maybe tou could take a picture of them to show us? 

Batteries for electric bikes is usually not capable of supplying as many amps as needed for an eskate... These cells can probably only deliver about 5-10a each. 

I would highly recommend that you do some more research on which cells you have got your hands on before continueing using them.
```

---
## \#15 Posted by: Alan_Smithee Posted at: 2017-04-30T22:11:37.071Z Reads: 119

```
[this spreadsheet I made should help you to identify your cells.](https://docs.google.com/spreadsheets/d/1fYjDxxCJXfm2wdpGWCaOUGq8V8TOEgsnplHQa4YQpRQ/edit#gid=0)

we really have to know what cells they are. if they are indeed chinese ones (which is not automatically bad) 10S4P might not be enough to supply the current needed,
```

---
## \#16 Posted by: Idobartal Posted at: 2017-05-01T09:47:20.226Z Reads: 108

```
i don't know why you are giving me such a worried response... I already built a 6s3p battery out of these and it work great... these are the cells <img src="/uploads/db1493/original/3X/0/8/080b4316c49495631ba1353ed68e67bfc7a0b1a2.JPG" width="375" height="500">
```

---
## \#17 Posted by: Alan_Smithee Posted at: 2017-05-12T16:29:03.406Z Reads: 92

```
here's the datasheet: http://www.batteryspace.com/prod-specs/6321.pdf

as you can see, they are rated for a max. output of 6A. at 3p thats 18A. Thats around 400Watts of constant power your pack can provide. An SK3 should draw more than that on average. That means, If your not super light and are exclusively riding on flat asphalt, you are killing your batteries while still not at the performance your other components could deliver. if you don't have some kind of over current protection, like fuses your cells may eventually overheat and vent/catch fire.

just saying.

btw.. that does your speed and range looks like? 168kv seems pretty low for 6S, and with that motor and battery setup, do you get more than 5km out of it?
```

---

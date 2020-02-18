# Using FOCBOX 65K ERPM

### Replies: 19 Views: 1593

## \#1 Posted by: onepunchboard Posted at: 2017-08-25T18:49:49.299Z Reads: 197

```
So,,, I know everyone freaks out on 60k erpm.
But I use 10s5a, sk3 260kv (265kv in reality), and if I limit @ 60k, it bottle necks my battery and speed by 7k erpm. 

So, I raised to 65k erpm cuz focbox possibly has less noise, and faster fet than original 4.12

I free spin it and no problem, and I don't think I can hit that number any time soon, but useful on busy road knowin that u can move a side as quick as car

Theoretical speed is 70khm, I 've hit 51kmh so far, couldn't find any longer road to test yet.

Braking is bit of an issue at this speed tho, either too much stress on belts, or bad braking.

Anyways, I'm successfully using 65K erpm. tho I can't  validate this as I need to reach 70khm which probably not possible on flat due to lack of torque and air resistance.

Bottom line: going over 60k is not only inefficient but not necessary.
```

---
## \#2 Posted by: karma Posted at: 2017-08-25T19:51:31.153Z Reads: 182

```
You are using a single motor and 9mm belt width to break at 51? Scary...
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-08-25T20:05:46.954Z Reads: 172

```
I changed some stuff of course. now I'm using 15/36 15mm belt single 97mm
```

---
## \#4 Posted by: Titoxd10001 Posted at: 2017-08-25T20:24:31.006Z Reads: 168

```
According to that ratio you'd have to go 66kph to reach 60k erpm
```

---
## \#5 Posted by: Cobber Posted at: 2017-08-25T20:32:36.533Z Reads: 163

```
find a good space with run off, go WOT, you know for science, and let us know what happens :innocent:
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-08-25T20:37:06.993Z Reads: 160

```
oh is it? I must miss something in my calculations.  tnx
```

---
## \#7 Posted by: onepunchboard Posted at: 2017-08-25T20:38:11.927Z Reads: 152

```
for sure. I will to put this thing to the limit😆
```

---
## \#8 Posted by: scepterr Posted at: 2017-08-25T20:47:23.611Z Reads: 150

```
A focbox is a vesc4, is a vesc4, is a vesc4. Did I mention it's a vesc4? Lol It'll die just like the rest, might just take a couple extra miles.
```

---
## \#9 Posted by: Titoxd10001 Posted at: 2017-08-25T20:54:35.368Z Reads: 147

```
Yeah. A forum member created this to figure speed in erpm

https://scottkellum.github.io/Esk8-RPM-finder/
```

---
## \#10 Posted by: onepunchboard Posted at: 2017-08-25T20:59:27.323Z Reads: 143

```
have u tired urself? lol? 
I'm just curious if it will indeed die. cuz the limit is  based on experience. i heard safe limit is up to 70k absolute safe is 60k.
```

---
## \#11 Posted by: onepunchboard Posted at: 2017-08-25T21:02:31.770Z Reads: 136

```
tnx I will reach 70khm according to this. but probably won't  due to air resistance Unless I go really steep hill.
```

---
## \#12 Posted by: scepterr Posted at: 2017-08-25T23:43:48.562Z Reads: 118

```
All I'm saying is don't rely on the focbox being more capable than a "standard" vesc4. It has no functionality beyond that of 4.12.
```

---
## \#13 Posted by: onepunchboard Posted at: 2017-08-25T23:49:04.911Z Reads: 112

```
Okay, i acknowledged.
```

---
## \#14 Posted by: scepterr Posted at: 2017-08-25T23:51:26.916Z Reads: 106

```
If you fry it I'll fix it for less than $80 :wink:
```

---
## \#15 Posted by: onepunchboard Posted at: 2017-08-25T23:54:10.028Z Reads: 106

```
Tnx for offer😃 but I I live in canada. if that's okay
```

---
## \#16 Posted by: scepterr Posted at: 2017-08-25T23:56:00.231Z Reads: 107

```
I'm in NYC :slight_smile:
```

---
## \#17 Posted by: JohnnyMeduse Posted at: 2017-08-26T00:12:59.765Z Reads: 108

```
80$ WTF it is like stealing people  

ShamelessPlug

https://drvwizard.com/

BTW @onepunchboard Don't always listen to other The FocBox is a improve version of the 4.12....

Actually I've try it in FOC over 85k erpm on a e-bike, but since it was unofficial, I won't recommand it after more testing.
```

---
## \#18 Posted by: onepunchboard Posted at: 2017-08-26T00:17:44.230Z Reads: 107

```
oh Johnny, I know I heard about u. I know the prices NW haha. he probably joking around cuz enertion's Warrent... I still doubt it will die on 65k. people beating this vesc a lot. specially for many bikers.
```

---
## \#19 Posted by: onepunchboard Posted at: 2017-10-03T15:20:27.303Z Reads: 68

```
Here is Update,

My DRV is not fried still, But, with 65k erpm, the motor hits 70k+ time to time, when I loose traction over cracks.

This either, goes ABS over so I up the abs then, DRVfault(Temporary and does not show up in terminal)

So I changed back too 60k erpm, cuz it starts to becoming safety concerns,

I think the sudden increase of rpm loose counting from the vesc,

Bottom line: gradual increase of erpm seems to work fine in FOCBOX. However real life testing shows it's not very stable.

Now I'm :cry:
```

---

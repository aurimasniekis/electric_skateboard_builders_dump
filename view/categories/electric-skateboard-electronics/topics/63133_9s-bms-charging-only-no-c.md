# 9s bms(charging only) no C-?

### Replies: 7 Views: 241

## \#1 Posted by: MannyM0E Posted at: 2018-07-28T06:54:07.284Z Reads: 50

```
Hey everyone. I'm at the finally stage of building my dad his emtb and also my first emtb build as well. I have given him my 9s lipo batteries and rest of my old stuff so he can build something. So here's my question. I'm familiar with 10s BMS but my dad has a 9s and bought this BMS from eBay, but I can't find where the C- would be at, there's only B- and P- .Can someone please help me out here, I hella want my dad to have a board already so we can ride tomorrow. And input will help thanks everyone

https://www.ebay.com/p/Balance-BMS-PCM-21a-W-temp-Switch-for-9s-33-3v-Li-ion-Li-po-Battery-9s21w001/2218166250?iid=221809130907&_trksid=p2349624.m4097.l9055
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-07-28T07:03:05.637Z Reads: 49

```
this may be a bms with auto charging and discharging on the same ports 😊
```

---
## \#3 Posted by: MannyM0E Posted at: 2018-07-28T07:06:16.671Z Reads: 47

```
Yes but if I connect to the P- that'll active the discharge that's only 21a which I'm trying to bypass. How can I bypass discharge
```

---
## \#4 Posted by: Sender Posted at: 2018-07-28T09:29:08.548Z Reads: 41

```
Thats not how it works, pack positive goes to charge port positive, BMS P- goes to charge port negative.

To bypass, set it up like that and just have your main pack - and pack + going straight to the motor controller or switch or whatever you are doing.  Thus "bypassing" discharge. If you wanted to use it with discharge you would use the other p- terminal on the BMS going to the motor controller instead of straight from the pack.

![s-l400-1|400x324](upload://2ERImsYEFuGJFzs2Hwugia7wjnZ.jpg)
```

---
## \#5 Posted by: mmaner Posted at: 2018-07-28T12:56:52.308Z Reads: 35

```
This ⬆️ &nbsp; &nbsp;
```

---
## \#6 Posted by: MannyM0E Posted at: 2018-07-29T01:40:25.760Z Reads: 20

```
@Sender  @mmaner hell yea guys that did the job. Appreciate the inputs, Idk what I would without this site lol 😂 You guys are amazing now my dad can enjoy his board and hopefully he'll love to build more with me
```

---
## \#7 Posted by: randomawol Posted at: 2018-08-29T02:23:12.372Z Reads: 16

```
How would someone hook a charge port into this while bypassing the bms for discharge or is that not possible?
```

---

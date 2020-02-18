# Does Using Lower Max Motor Amps Improve Range?

### Replies: 6 Views: 243

## \#1 Posted by: AdamE3399 Posted at: 2018-12-26T22:52:28.021Z Reads: 99

```
So I recently finished my dual 6364 motor build with 15mm belts as my third board, I choose to build this board to improve on my single 6374 motor board on 12s which gave an insane top speed of 60kmh but has pretty bad torque and if you were going fast and you belt broke it would scare the living shit out of you. So I build a dual motor build to improve torque and reduce belt breaking and belt slippage and both boards are using turnigy 5000mah 20c lipos and my single motor board seems to get 15 to 20km range especially if I ride slower like 30 kmh, though the new board seems to get only half the range. I was under the impression that dual motors meant that your board used less power on start up due to splitting the work load which I would have compensated for the loss of power using dual motors but that doesn't seem to be the case. When I use this esk8 calculator https://calc.3dservisas.eu/ and enter in all the specs it also shows that one board will get 14km whereas the dual motor board will only get 7km of range.

So I was wondering if there was a way to improve the range on this board by adjusting vesc settings e.g motor max current or batt max, or If I just have to live with it.
Thanks in advanced for any responses
```

---
## \#2 Posted by: pat.speed Posted at: 2018-12-26T23:43:08.755Z Reads: 89

```
Two motors does not use more or less than a single. Yes, there my be some complicated crap to say one uses more than the other but roughly they use the same power. I get about 20km riding a dual 6355 on 12s5000mah lipos. I’m not sure how you ride but it must be fast or something is quite inefficient.

Also if you want to save battery motor amps won’t help much, try adjusting battery amps
```

---
## \#3 Posted by: AdamE3399 Posted at: 2018-12-27T00:08:08.623Z Reads: 82

```
Alright, thanks for the response, I always thought that using dual wasn't more inefficient, its just weird that this calculator says so https://calc.3dservisas.eu/ , and I guess it could be because I have dual I do accelerate reasonably faster.
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-12-27T00:12:00.247Z Reads: 76

```
I agree with @pat.speed. Lower Battery Max. I used to be able to push an 8-10 mile limit (at 40A per vesc) out to 20+ miles by lowering battery max alone to 20A per vesc.

Setting watt limits is another way to do it and get consistent power across a charge. Say 200W per vesc, go far.
```

---
## \#5 Posted by: pat.speed Posted at: 2018-12-27T00:12:56.496Z Reads: 70

```
Yeah the calc is messed up in that aspect, then range thing is weird
```

---
## \#6 Posted by: AdamE3399 Posted at: 2018-12-27T00:31:55.725Z Reads: 65

```
alright ill try lowering batt max to 20A and see how that goes, thanks for the help
```

---

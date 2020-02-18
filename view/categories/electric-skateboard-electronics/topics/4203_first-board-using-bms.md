# First board using bms

### Replies: 21 Views: 2402

## \#1 Posted by: barajabali Posted at: 2016-06-03T20:35:56.194Z Reads: 176

```
So for my mountain board build I've decided to use a bms instead of my regular balance chargers just for convenience since it's a 10s8p pack it's pretty big and I want to just plug it in and walk away. 

I have pictures of what I think I can use I'm using 80samsung 25R cells.

Of these four items what charger and bms combo would you use? 

<img src="/uploads/db1493/original/2X/e/eee703d61d4929929b28f00b18da9f3758835785.png" width="281" height="500"><img src="/uploads/db1493/original/2X/c/c7c63656cc019caf0c817592b0995d3ae29c5095.png" width="281" height="500"><img src="/uploads/db1493/original/2X/c/c5ce061a5345dfbb72d5d69eff10232d3a1e4311.png" width="281" height="500">
```

---
## \#2 Posted by: ArmandR Posted at: 2016-06-03T20:42:50.528Z Reads: 157

```
Are you using lipos?
```

---
## \#3 Posted by: Jinra Posted at: 2016-06-03T20:44:24.172Z Reads: 153

```
@ArmandR He said he's using Samsung 25R's

If I were to make a pack I'd buy pretty much the same BMS's you listed. You have a max output of 160A, but you should check how much amperage your motors are rated for. I bet you'd be fine with the 100A BMS.

PS. 10s8P is insane, 840wh at full charge!
```

---
## \#4 Posted by: Michaelinvegas Posted at: 2016-06-03T20:44:54.682Z Reads: 150

```
[quote="barajabali, post:1, topic:4203"]
80samsung 25R cells.
[/quote]

Hey @ArmandR 👆🏻
```

---
## \#5 Posted by: barajabali Posted at: 2016-06-03T20:49:08.625Z Reads: 140

```
I'm using 2 of enertions 6372 190kv motors. Not the small 6355's. They're gonna need some monster batteries! 

Okay the charger price it's kind of extreme in difference which would you go for?
```

---
## \#6 Posted by: barajabali Posted at: 2016-06-03T20:50:39.409Z Reads: 134

```
I don't need the 150amp bms because my esc's are only rated to 120 so I'd prefer my bms to fail before my esc's do. 

Which charger would you guys go for? Is the 5a vs 2a worth the price jump
```

---
## \#7 Posted by: Jinra Posted at: 2016-06-03T20:54:31.116Z Reads: 134

```
I'd get the cheaper charger simply because fast charging tends to reduce cell life a bit and the fan on the fast charger is probably loud as hell. If I'm going to be charging up 840wh I'd probably end up leaving it plugged in overnight anyway.
```

---
## \#8 Posted by: ArmandR Posted at: 2016-06-03T20:55:53.882Z Reads: 128

```
Sorry :slight_smile:
```

---
## \#9 Posted by: barajabali Posted at: 2016-06-03T20:56:07.092Z Reads: 125

```
True. So I think I'm gonna go with the 100amp bms and the 2a charger. 

Thank god I got away with the cheaper stuff lol
```

---
## \#10 Posted by: Michaelinvegas Posted at: 2016-06-03T20:58:07.018Z Reads: 127

```
Lol...it's funny...all good...

I do shit like that too lol
```

---
## \#11 Posted by: XIII Posted at: 2016-06-03T21:13:48.866Z Reads: 137

```
Hi , 

I'm gonna make your flatpack's 10s 10000mah lipo's 10C

so searching for a BMS aswell. 
Can i get away with a 60A BMS or should i opt for the 100A BMS aswell? 

ESC is rated for 120A aswell.

And how do you know if the bms has a on/off switch like the SPACE cell? 
It's not listed ...
```

---
## \#12 Posted by: barajabali Posted at: 2016-06-03T21:16:02.627Z Reads: 133

```
Wel I'm using 100amp bms because this is goin on a mountain board which is going to produce higher than average amps. 

I think you can get away with a 60-80 amp bms on a regular board depending if it's dual drive or single. 

And good question about the on off switch. Not sure

Maybe  @longhairedboy knows
```

---
## \#13 Posted by: lox897 Posted at: 2016-06-03T22:44:51.166Z Reads: 124

```
I don't think any of the batterysupport BMS come with soft switches. Some Bestech ones do though.
```

---
## \#14 Posted by: barajabali Posted at: 2016-06-03T22:45:56.872Z Reads: 125

```
Hmm I don't mind just putting a breaker switch on it that's what I always do
```

---
## \#15 Posted by: lox897 Posted at: 2016-06-03T22:48:48.199Z Reads: 123

```
I don't know why people like the BMS switches so much. Unless they bypass the BMS when you need more amps, I would just go with a loop key.
```

---
## \#16 Posted by: squad Posted at: 2016-06-03T23:26:07.053Z Reads: 119

```
Just keep in mind You're going with two motors and two of 120A rated ESCs, that means, with 100A BMS each motor can get only 50A continous. Just my 50c, I like to use much higher rated components than necessary ;)
```

---
## \#17 Posted by: barajabali Posted at: 2016-06-03T23:27:27.567Z Reads: 121

```
True! I haven't considered that fact. Maybe I will just go with the 150 amp bms. It's only a few dollars more anyhow.
```

---
## \#18 Posted by: XIII Posted at: 2016-06-04T08:36:34.685Z Reads: 110

```
Do you place your loop key between the batteries and the BMS , or between the BMS and the ESC ?
```

---
## \#19 Posted by: lox897 Posted at: 2016-06-04T11:04:03.417Z Reads: 102

```
I would place it on the ESC cables. That way it doesn't drain the batteries power.
```

---
## \#20 Posted by: XIII Posted at: 2016-06-04T11:36:00.907Z Reads: 98

```
So the BMS will constantly be on and drain power?
```

---
## \#21 Posted by: lox897 Posted at: 2016-06-04T11:49:31.124Z Reads: 97

```
Sorry. I thought you were talking about a voltage meter. The loop key is just placed between the bms cables and the esc.
```

---

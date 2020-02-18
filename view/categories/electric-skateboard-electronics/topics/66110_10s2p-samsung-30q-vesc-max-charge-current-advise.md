# 10s2p samsung 30q vesc max. charge current advise

### Replies: 12 Views: 653

## \#1 Posted by: flozilla Posted at: 2018-08-26T09:35:28.899Z Reads: 194

```
Hello,

I cannot seem to find information about what is a save setting that gives me the most possible brake force while keeping my battery unharmed.

Atm, I have the charge current set to 8A. But this feels a bit too little for dynamic riding.

I am under the impression that for these cells and the 10s2p configuration the maximum charge current should not exceed 12A.
So dialing the vesc setting to 11A would be save?

Can someone maybe has made experience and can confirm this? 
Any objections to my impressions?

Many thanks in advance!
```

---
## \#2 Posted by: xilw3r Posted at: 2018-08-26T10:05:25.832Z Reads: 189

```
Where did you see the suggestion for maximum charge current in 2p to be 12A ?

https://eu.nkon.nl/sk/k/30q.pdf

Well it is shown that the maximum charge current should be 4A, but this is for continuous charge current. During braking it can be considered to be a pulsed charging. In reality, you can set pulsed charging for 2C without any issues, so 6A per cell or 12A total. Just dont do full power braking for a long time :slight_smile:
Personally I would even set braking current to 15A and just be mindful of my actions. If it is needed in an extreme situation it can save your skin
```

---
## \#3 Posted by: flozilla Posted at: 2018-08-26T10:15:04.798Z Reads: 174

```
Thanks @xilw3r for your quick answer!
I drew the 12A max charge exactely from that common rule of max charge 2C for 2P... 

My question concerns braking to stop or when descending. 
Here  I dont want to harm my cells since they cost money which i already spent alot of lately 😁.

Will crank the vesc settings up to 11A for now to see how this will slow me down. 

Thanks again.
```

---
## \#4 Posted by: pat.speed Posted at: 2018-08-26T10:20:21.646Z Reads: 162

```
You can also try upping the motor min setting
```

---
## \#5 Posted by: flozilla Posted at: 2018-08-26T11:42:08.654Z Reads: 157

```
Hah! That means the difference would go up in heat? 
Gotta check my settings again. (Man i am looking forward to affording the metr module 😁)

Then I would have to heatsink the vescs' mosfets right?
```

---
## \#6 Posted by: pat.speed Posted at: 2018-08-26T12:00:58.810Z Reads: 155

```
I don’t think it will make a noticeable difference. I have mine set on -45 although that’s on a dual board and I only weight 60kg
```

---
## \#7 Posted by: flozilla Posted at: 2018-08-26T20:12:36.016Z Reads: 133

```
Aha! My Motor Current Max Brake was set to -20A already... Will put Battery Current Max Regen to -11A and Motor Current Max Brake to -30A and see what happens.![1535314202618625579690|375x500](upload://hvE8kOAXCkLu1aklRQHgzee8Twp.jpg)Only issue is that in my box its really crammed. So I am a bit anxious about high temeratures.

I am about 82. Working on that issue too 😓
```

---
## \#8 Posted by: flozilla Posted at: 2018-08-26T20:17:58.697Z Reads: 123

```
Also set Mosfet Temps cutoff start to 50°C and End to 54°C to check out if I even get there or if i can stop shitting my pants...

Man do I want that bt monitor!
```

---
## \#9 Posted by: dareno Posted at: 2018-08-27T00:40:34.057Z Reads: 108

```
[quote="flozilla, post:7, topic:66110"]
I am about 82.
[/quote]

Shit dude thats awesome  I'm 45 and feel too old for this shit :stuck_out_tongue_winking_eye:
```

---
## \#10 Posted by: xilw3r Posted at: 2018-08-27T06:27:51.761Z Reads: 94

```
I completely forgot lol. Yes set your motor brake current to a higher value. Shit dude, im running -50A on the motor and -15 on the battery. It definitely is not all going to heat as far as i can tell, its way more complicated with all those magic pixies. But its all good, it seems. You can definitely go for -40 on motor and see what happens.

Im a damn 90kg fat ass too.. but my mommy tells im pretty.
```

---
## \#11 Posted by: moon Posted at: 2019-05-25T03:04:49.403Z Reads: 42

```
You're not old sir:)
```

---
## \#12 Posted by: dareno Posted at: 2019-05-25T04:32:51.970Z Reads: 39

```
Ah 45.   I remember those 4 years
```

---

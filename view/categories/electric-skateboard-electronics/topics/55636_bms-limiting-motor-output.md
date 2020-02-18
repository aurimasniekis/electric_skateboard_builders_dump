# BMS limiting motor output?

### Replies: 15 Views: 796

## \#1 Posted by: Alon Posted at: 2018-05-16T09:41:22.148Z Reads: 105

```
Hi there everyone,
I have a question regarding Amp limit caused by the BMS. 
I'm at the stage of ordering parts for my first board.
I already ordered and received the motor - Turnigy SK3 6374 192kv which is rated as max 80Amp.
Battery will be a 10s4p LG hg2 (20 Amps continuous each). 
The BMS will most likely be:
https://m.banggood.com/37V-42V-10S-45A-Li-ion-Battery-Protection-Board-BMS-PCB-System-p-1177351.html?rmmds=search
Which is rated as 45 Amps continuous (ignore for the fact that it is supposed to withstand 100A instantaneous discharge). 
Now:
-The motor max 80 Amps
-The battery is 4p so is capable of 80 Amps
-The BMS is 45 Amps

Does this mean that the BMS will limit the whole system and I will only be able to run 45 Amps? 

Thanks for your help!
```

---
## \#2 Posted by: Alon Posted at: 2018-05-16T09:43:13.187Z Reads: 100

```
Forgot to mention, the controller will be a standard 4.12 vesc. Most likely Maytech or TB.
```

---
## \#3 Posted by: JonathanLau1983 Posted at: 2018-05-16T09:58:52.464Z Reads: 96

```
You'll want to restrict current on the Vesc. BMS over discharge current will likely just cut out leaving you powerless. Vesc max current will simply reduce your top acceleration and top speed if I'm not mistaken.
```

---
## \#4 Posted by: Alon Posted at: 2018-05-16T10:21:05.701Z Reads: 94

```
If I understand you correctly, you mean that in the current setup the BMS will cut at 45A, and if I want to prevent this from happening I need to disable over-discharge protection? 
If so how do I do that? Do I need to modify the BMS in some way?
```

---
## \#5 Posted by: JonathanLau1983 Posted at: 2018-05-16T10:39:53.113Z Reads: 85

```
You need to limit it on the Vesc.
Disabling the BMS over discharge current will just make it blow instead.
```

---
## \#6 Posted by: Acido Posted at: 2018-05-16T13:17:01.027Z Reads: 57

```
you do not want to go over 50A on those vescs
```

---
## \#7 Posted by: Acido Posted at: 2018-05-16T13:17:27.260Z Reads: 55

```
also that is not possible as i know
```

---
## \#8 Posted by: Alon Posted at: 2018-05-16T13:25:23.919Z Reads: 55

```
But does thes BMS limit me to 45A in this current setup?
```

---
## \#9 Posted by: Acido Posted at: 2018-05-16T13:27:17.909Z Reads: 54

```
unless you bypass discharge it will limit it
but since your going with those vescs, you do not need a better bms
```

---
## \#10 Posted by: Slak Posted at: 2018-05-16T15:44:50.258Z Reads: 47

```
We're only talking about 5A, no big deal then :) No problem if you set 45A as Battmax in your VESC config (which would be limited to 50A anyway). You wouldn't maybe not see the difference brought by those 5A.
```

---
## \#11 Posted by: JonathanLau1983 Posted at: 2018-05-16T16:34:28.688Z Reads: 44

```
Question really is what happens if the Vesc attempts to pull over 45A.
Will it simply only allow 45A through, of cut out if over 45A is pulled.
```

---
## \#12 Posted by: Namasaki Posted at: 2018-05-16T17:40:55.447Z Reads: 43

```
[quote="Alon, post:8, topic:55636, full:true"]
But does thes BMS limit me to 45A in this current setup?
[/quote]

You need to get the specs of the bms to be sure what its parameters are.
If it's max continuous current is 45a and it's max peak current is 100a then it's over current detection should be set around 100a. 
Meaning that drawing more than 45a continuously will not shut the bms down but drawing more than 45a continuously could cause it to overheat and that could cause it to shut down if it has over temp protection. 
If it doesn't have over temp protection then overheating it could cause permanent  failure.
If your building a single drive street board with vesc, the 45a bms will probably be ok.
```

---
## \#13 Posted by: Namasaki Posted at: 2018-05-16T17:45:05.873Z Reads: 42

```
[quote="JonathanLau1983, post:11, topic:55636, full:true"]
Question really is what happens if the Vesc attempts to pull over 45A.

Will it simply only allow 45A through, of cut out if over 45A is pulled.
[/quote]

The bms will not limit the current to 45a or cut out unless the over discharge current detection is reached.
It will just start to overheat.
```

---
## \#14 Posted by: Alon Posted at: 2018-05-17T11:45:22.089Z Reads: 32

```
Thanks to everyone for your help!
Just to be sure that I understand correctly. Lets say the whole system is rated at 80A except for the BMS whyich is 45A. Does this mean its effecively a 45A system? And the max amps the motor will see is 45A?
@Namasaki
```

---
## \#15 Posted by: Namasaki Posted at: 2018-05-17T17:14:58.623Z Reads: 25

```
Yes and no. 
You can set the motor max at 80a and the battery max at 45a
The motor current is normally higher than battery current. 
For example

![image|281x499](upload://xswYSUAMuvJhY0GAyQL7zea5yUL.jpg)
```

---

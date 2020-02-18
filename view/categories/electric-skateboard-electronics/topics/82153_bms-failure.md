# Bms failure ? —-

### Replies: 24 Views: 332

## \#1 Posted by: Alex753 Posted at: 2019-01-26T14:18:28.799Z Reads: 86

```
Hey ! 

So I rode my board for about 100miles since the beginning of the build and I experienced last evening a strange thing, I plugged my board with my banana plug as usual to my Hobbyking 8S bms, (Without opening my enclosure), everything worked well, red led as usual, charging.

I left the board for like 10 minutes and the led turned to green like if it was fully charged.
Since I was at only 50% when I plugged it i was supprised because it’s usually not this quick, I turned on the board and I was at 32.5V, so about 80% battery and it won’t charge anymore.

I though about a weld spot which could go off because of the vibrations so I removed the enclosure and everything was surprisely ok.

Then I tested the charger directly at the output because my board electronics were looking good and I had a correct 33.6V, so the charger shouldn’t be the issue.

After that I plugged my voltmeter directly onto my board charging port (And it’s danregous af omg), touched the two poles by mistake and created a sympatic spark, I though I burned the bms at this time. Then I plugged back the charger to see if everything was still ok and it was charging again, I left it again for like 30 minutes and it charged up to 100% without problem like before.

What happened ? It’s really strange that shorting the charging port solved the problem so I’m asking you to be sure that I havn’t got any problem !

Have a nice week end guys!
```

---
## \#2 Posted by: b264 Posted at: 2019-01-26T14:22:36.570Z Reads: 76

```
Put [a fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) on your charge port
```

---
## \#3 Posted by: b264 Posted at: 2019-01-26T14:24:09.214Z Reads: 76

```
Do you have photos?  Which BMS is it?  Does the battery voltage change if you flex it?  Are there burn marks anywhere?  Can you pull apart any solder joints?  Did you try a new charge jack?
```

---
## \#4 Posted by: Alex753 Posted at: 2019-01-26T14:43:26.068Z Reads: 76

```
Of course thanks for your help, so it’s this exact BMS plugged in charge only https://hobbyking.com/en_us/8s-li-ion-pcm-charge-4a-discharge-10a.html

Battery voltage stay the same, wired with AWG14, XT60, here is how it look like 

Board charging,

![image|666x500](upload://rXlC332VeMZoDT6C13ogfD3c5O4.jpeg)  

![image|666x500](upload://tmLaUPMJwpP7SqhZbdJjVYRbKlA.jpeg) 

All the stuff in the battery enclosure, compact but current is passing and batteries are not compressed too much.

Solder joint are good but I can still change the charging port if needed because I used this kind of low Voltage/Amps electrician stuff ![](http://www.travaux-electrique.fr/wp-content/uploads/2016/10/Choisir-et-utiliser-un-domino-%C3%A9lectrique.jpg)

There is actually some little burn marks inside of the charging port but they must be coming from last evening shorting, looking like this 

![image|375x500](upload://2SHjlwaE8dnSlSWF6Rz6hcWygcR.jpeg) 

Didn’t tried to change the charging port because I don’t have the time rn, I still have some of them if needed tho but since this one is working it might be ok.

What do the fuse could do on my issue by the way ?
```

---
## \#5 Posted by: Alex753 Posted at: 2019-01-26T14:46:42.992Z Reads: 66

```
The most important thing is to actually know what happened and to be sure about if it can happen again, it’s my main commuter to College so ...!
```

---
## \#6 Posted by: Sebike Posted at: 2019-01-26T14:47:03.384Z Reads: 65

```
A fuse can save you from burning down your house in case of a short in the charge port.
```

---
## \#7 Posted by: Alex753 Posted at: 2019-01-26T14:48:34.646Z Reads: 64

```
Well that seems to be interesting :thinking:

So I just need something higher than the current passing through the Bms charging port ? Right now I have 33.6V and 1.5Amps
```

---
## \#8 Posted by: Sebike Posted at: 2019-01-26T14:52:26.586Z Reads: 61

```
It should be rated for more volts and amps than what you are charging with, yes.. So, a 5-10A fuse  should be fine.
```

---
## \#9 Posted by: b264 Posted at: 2019-01-26T14:57:30.796Z Reads: 56

```
[This fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) is perfect, and cheap, and small
```

---
## \#10 Posted by: Alex753 Posted at: 2019-01-26T15:04:05.948Z Reads: 48

```
20€ Shipping, but thank you, i know what to buy now !
```

---
## \#11 Posted by: b264 Posted at: 2019-01-26T15:04:41.697Z Reads: 47

```
Look for a similar device then on your side of the pond ;-)

(and link it here so others can find it)
```

---
## \#12 Posted by: Alex753 Posted at: 2019-01-26T15:06:42.511Z Reads: 44

```
Yup that’s what I was about to do, there is lots of little electronic store where I could find this.

Then have you got any idea about what happened last time while charging the board ? 
The fuse would protect but not prevent any issue !
```

---
## \#13 Posted by: Friskies Posted at: 2019-01-26T15:07:53.523Z Reads: 46

```
It sounds like your BMS read one of the P groups as fully charged and shut the charging circuit off. You probably have a P group with a loose cell in it or a bad connection.

So basically you probably have a bad connection in the pack somewhere and just picking it up and moving it around fixed It.
```

---
## \#14 Posted by: Alex753 Posted at: 2019-01-26T15:24:02.051Z Reads: 44

```
I’m in 8S1P so if a cell die I would have a voltage loose and I wouldn’t have 33.6V fully charged, so it’s not this but a bad connection seems logic to me, than’s guys !
```

---
## \#15 Posted by: b264 Posted at: 2019-01-26T16:03:27.559Z Reads: 43

```
It could be a bad connection on the BMS itself, not in the pack series connections, and so it would still read full voltage on the pack output.

@Friskies is right, look where your balance leads connect to BMS
```

---
## \#16 Posted by: Benjamin899 Posted at: 2019-01-26T17:27:39.776Z Reads: 34

```
maybe a stupid question, but how can a charge port short?
```

---
## \#17 Posted by: Alex753 Posted at: 2019-01-26T17:28:42.503Z Reads: 32

```
Touching the two poles with water or anything other that is conductive.
```

---
## \#18 Posted by: Benjamin899 Posted at: 2019-01-26T17:30:32.654Z Reads: 34

```
mmhkay, okay i always encase open spots like that with hotglue.
```

---
## \#19 Posted by: Sebike Posted at: 2019-01-26T17:34:55.728Z Reads: 33

```
It happened recently to someone on this forum. 

Charger port shorted as the charger was plugged in. The contacts melted into each other.. Scary! I believe the port was already slightly damaged, so maybe the positive pin was pushed towards the negative outer body as the plug was pushed in.
```

---
## \#20 Posted by: Alex753 Posted at: 2019-01-26T17:36:40.162Z Reads: 34

```
You can’t actually because it’s directly where you plug your charger, that’s why you must have a fuse (Not like me !)
```

---
## \#21 Posted by: Benjamin899 Posted at: 2019-01-26T17:39:04.486Z Reads: 29

```
thanks, noted
```

---
## \#22 Posted by: Alex753 Posted at: 2019-01-26T17:39:44.086Z Reads: 29

```
Yeah I saw it but how is it even possible ? 
Charger is designed to not short !
```

---
## \#23 Posted by: Sebike Posted at: 2019-01-26T17:41:26.559Z Reads: 29

```
If something breaks, it breaks. Most charge ports we use are pretty cheap and built accordingly..

Edit Not talking about the charger here, but the jack on your board.
```

---
## \#24 Posted by: Alex753 Posted at: 2019-01-26T18:00:42.231Z Reads: 26

```
Oh yeah that’s true, the little part coming out can easily break for sure.

Benjamin have a look at this picture I posted above,

![image|375x500](upload://2SHjlwaE8dnSlSWF6Rz6hcWygcR.jpeg) 

If the part that is coming out of the port and the internal one touch themselves, it’ll short.
```

---

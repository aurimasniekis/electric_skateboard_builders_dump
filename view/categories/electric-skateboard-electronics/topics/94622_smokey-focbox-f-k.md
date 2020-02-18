# Smokey Focbox&hellip;&hellip; F%@K!

### Replies: 31 Views: 507

## \#1 Posted by: DringDingle Posted at: 2019-05-22T13:19:20.640Z Reads: 227

```
Rage. 
Hoping someone can tell me what I did wrong. 
Or tell me it's fixable....

Sequence of events...

I just got finished running a motor detection on my 6374 and got the hall sensors working (another storey but it's fine) 

Turned everything off. Plugged the canbus cable back in, (other focbox was already configured, set as the slave and all G .... I had previously had everything running) 

Plugged in. Throttled up. Perfect. Motors in sync, no cogging (previously mentioned storey), lookin sexy as fuck.

Power up again, then gave it a bit of brake. And then smoke..... (From the master)

Other deets
- All the other focbox settings were default I didn't mess with anything 99% sure on that.
- 12s5p 30q battery. Charged to about 46v. 
- the slave focbox still worked / other motor spun. (While still connected to the master even though it wasn't working) 
- off an on again - nothin. Just sits there with the blue light. 


Anyone know what's fried looking at these pics? 
I'd never opened it up so I can't spot the difference..... (Also not that electronically savvy)

![IMG_20190522_204401|281x500](upload://dUaeag3WedNNd9VpQtWRnP0VFGC.jpeg) 
![IMG_20190522_204432|690x388](upload://y1hNVZn4fSTaGQ1KNoUJlaq06HE.jpeg) 

Needless to say ... I'm pretty bummed. Been putting this together for about 10 months and it's my first build. 😢
```

---
## \#2 Posted by: yelnats8j Posted at: 2019-05-22T13:23:22.503Z Reads: 209

```
Can you take pictures of the capacitors?

Also this doesnt look so good?
![20190522_092323|243x500](upload://rsYNreHcqnbMPZY0Chzsp9AUWXm.jpeg)

@JohnnyMeduse
```

---
## \#3 Posted by: DringDingle Posted at: 2019-05-22T13:24:06.382Z Reads: 201

```
On the ends? Ya will do. 

Yeah thought as much.... Dunno what it is though.
```

---
## \#4 Posted by: pjotr47 Posted at: 2019-05-22T13:24:12.927Z Reads: 199

```
Oh that is a cheap fix. Looks like only a burned drv chip
```

---
## \#5 Posted by: yelnats8j Posted at: 2019-05-22T13:25:39.955Z Reads: 193

```
Thats what I was thinking but, when my esc went up in smoke it was also the capictors so just want to check.
```

---
## \#6 Posted by: pjotr47 Posted at: 2019-05-22T13:26:59.610Z Reads: 193

```
Yeps you can kill multiple comments on the vesc. 

Where do you live @DringDingle? There are vesc repair guys on the forum
```

---
## \#7 Posted by: DringDingle Posted at: 2019-05-22T13:27:01.314Z Reads: 191

```
![IMG_20190522_212536|690x388](upload://qAA4v91XUz9JW06yMyb5pyd9VFa.jpeg) ![IMG_20190522_212513|690x388](upload://44Tyg4KLmPONX5ERoNsOJcI2Me9.jpeg) ![IMG_20190522_212505|690x388](upload://eIgIHqJEUH9cRq6WR09UyECv6VH.jpeg)
```

---
## \#8 Posted by: yelnats8j Posted at: 2019-05-22T13:28:25.253Z Reads: 180

```
Looks like a DRV problem thats it.

Its only like a 50$ fix so not that bad.
```

---
## \#9 Posted by: DringDingle Posted at: 2019-05-22T13:29:01.491Z Reads: 178

```
Taking it back out of its case.... It does 'smell' like the problem is on the underside. Hilarious as it sounds it was noticeable after taking the underside cover off again ha.
```

---
## \#10 Posted by: DringDingle Posted at: 2019-05-22T13:29:17.677Z Reads: 175

```
Australia. More specifically western Australia
```

---
## \#11 Posted by: DringDingle Posted at: 2019-05-22T13:30:02.056Z Reads: 172

```
Awesome. I suppose..... More to the point what caused it to happen?
```

---
## \#12 Posted by: yelnats8j Posted at: 2019-05-22T13:33:02.248Z Reads: 165

```
@dareno did you ever find someone to repair your VESC?
```

---
## \#13 Posted by: dareno Posted at: 2019-05-22T13:34:59.220Z Reads: 162

```
I do all my own vesc repairs.


None of which have been successful.
```

---
## \#14 Posted by: DringDingle Posted at: 2019-05-22T13:36:59.155Z Reads: 159

```
@dareno I'm pretty sure I was reading your thread not long ago about you frying something :open_mouth:

I hope I haven't just done the exact thing you have after reading the thread
```

---
## \#15 Posted by: dareno Posted at: 2019-05-22T13:39:33.360Z Reads: 155

```
I have a fry kitchen.
```

---
## \#16 Posted by: dareno Posted at: 2019-05-22T13:50:20.567Z Reads: 151

```
There is no where and I mean no where you can get esk8 related esc's repaired here.  I have tried.  Can bus well then you can snip off the chips but DRV's well no.   If you find an Aussie wizard then share.
```

---
## \#17 Posted by: taz Posted at: 2019-05-22T13:52:20.985Z Reads: 150

```
The irony in that Australia, the home of the Focbox, has nobody to repair them is not lost on me :grinning:
```

---
## \#18 Posted by: dareno Posted at: 2019-05-22T13:54:44.377Z Reads: 147

```
We don't get domestic shipping either.   Fuck you @onloop.  Look after the minors.   :sunglasses:
```

---
## \#19 Posted by: DringDingle Posted at: 2019-05-22T13:57:57.971Z Reads: 143

```
Bought these late November last year.... What are the chances I'll get it replaced you think? Seeing as they have never been 'used' 

(I didn't buy the replacement warranty... Welp)
```

---
## \#20 Posted by: deucesdown Posted at: 2019-05-22T14:33:30.690Z Reads: 130

```
Have you tried a phone repair shop? They ought to have all the equipment.
```

---
## \#21 Posted by: KaramQ Posted at: 2019-05-22T14:53:24.468Z Reads: 122

```
[quote="yelnats8j, post:8, topic:94622"]
Its only like a 50$ fix
[/quote]
Money don’t grow on trees, aren’t you like 15?
```

---
## \#22 Posted by: pjotr47 Posted at: 2019-05-22T14:55:28.675Z Reads: 120

```
50dollar is not the deal breaker on a whole board. 

He only wants to tell the problem could have been worse
```

---
## \#23 Posted by: baxter Posted at: 2019-05-22T16:26:56.605Z Reads: 113

```
I suppose because its an Australian company, it should be obliged to comply with Australian consumer law?

https://www.accc.gov.au/consumers/consumer-rights-guarantees/repair-replace-refund
```

---
## \#24 Posted by: taz Posted at: 2019-05-22T16:29:09.355Z Reads: 111

```
The question is are you buying from an Australian company?

Maybe this is one of the reasons they have no local shipping.
```

---
## \#25 Posted by: Bcoad Posted at: 2019-05-23T01:01:57.762Z Reads: 97

```
I was wondering the same thing when i ordered unity and saw options to buy warranty. I thought why buy I'm an aus customer this is an aus company warranty is always included in aus. So didnt get extra warranty. Search enertion abn they seam to say its an Australian private company.
```

---
## \#26 Posted by: DringDingle Posted at: 2019-05-23T04:04:50.876Z Reads: 84

```
Can anyone shed light on why the drv chips blow?
```

---
## \#27 Posted by: Sn4pz Posted at: 2019-05-23T04:08:07.594Z Reads: 83

```
I think a major factor is voltage. They're only capable of handling 60v, and occasionally (obv depending on setup) spikes above that occur
```

---
## \#28 Posted by: J0ker3366 Posted at: 2019-05-23T04:13:42.820Z Reads: 82

```
They hate us.
```

---
## \#29 Posted by: Narnash Posted at: 2019-05-23T09:04:13.297Z Reads: 68

```
Any Laptop/phone repair buisness that is worthy to be called **repair buisness** should be capable to replace a DRV8302 for small money. At least if you provide the part and state that you cover the labor and risk (that the repair fails if more than the DRV is done). 

It's a 5-15$ chip and maybe 20 min of work + flux, a hot air station and maybe a 
magnifying glass/
microscope thats it.
```

---
## \#30 Posted by: mikenyc Posted at: 2019-05-23T10:43:54.052Z Reads: 51

```
lol maybe in 2 years
```

---
## \#31 Posted by: DringDingle Posted at: 2019-05-24T06:40:39.852Z Reads: 29

```
I'll give it a go thanks!
```

---

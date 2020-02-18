# Calculating Max Amps from Lipo C Rating

### Replies: 25 Views: 393

## \#1 Posted by: MaxMalouf Posted at: 2018-08-23T00:16:32.336Z Reads: 107

```
Hi, 
A little bit of a newbie question here,
 
I have 10x 1s lipo batteries with a C rating of 20C. (https://hobbyking.com/en_us/turnigy-5000mah-1s-20c-lipoly-single-cell.html)
I have these 10 batteries linked up in a 10s1p setup and wanted to calculate how many amps continuous this pack can do.

I found a website with a calculator, however, it gave me a continuous amps rating of 100amps! surely my 10mm thick pack cannot do 100amps continuous..... right?

Just wanted to know what to set my VESC to, to not harm my battery. 
Thanks, Max.
```

---
## \#2 Posted by: Winfly Posted at: 2018-08-23T00:19:26.034Z Reads: 101

```
Actually it can. Max continuous current = lipo capacity * C rating

5Ah * 20C = 100 A

That's like how C rating is defined. And high current rating is  one of the advantage of using lipo instead of li-ion cells
```

---
## \#3 Posted by: NickTheDude Posted at: 2018-08-23T00:23:01.235Z Reads: 97

```
Sadly there doesn't seem to be any standard for measuring C rating so most manufacturers vastly overstate them. I think most peoplr assume they're capable of half of what they say they are.
```

---
## \#4 Posted by: PatRocks Posted at: 2018-08-23T00:40:56.362Z Reads: 87

```
This is one of my favorite topics, and IMO, one of the most important subjects concerning Lipolys.
The statement made by @NickTheDude is (sadly) quite accurate. 

For the best sources of information about lipo batteries, I recommend the various rc-hobby forums, as they often have been around for several years more than this one. Additionally, they tend to use lipo batteries exclusively for the power to weigh superiority. Not that this forum lacks in scientific talent by any means, but the rc-hobby groups seem to attract more, as not every geek is thrilled about skateboarding. I really mean no disrespect to our forum, but it’s good to look around for an enhanced degree of perspective. My go-to is rc-groups forum. 

There is a tool that does exactly that, it's called the "Wayne Giles ESR meter "
```

---
## \#5 Posted by: MaxMalouf Posted at: 2018-08-23T01:07:13.534Z Reads: 77

```
Haha, Okay thanks guys, I'll set it to around 30-40 amps to be safe?
```

---
## \#6 Posted by: PatRocks Posted at: 2018-08-23T02:05:45.651Z Reads: 75

```
Can you measure the voltage of the pack under load? That is how you determine the pack resistance and come to a reasonable safe discharge rate
```

---
## \#7 Posted by: MaxMalouf Posted at: 2018-08-23T02:35:30.938Z Reads: 70

```
I'll have to use my bluetooth module for that, I'll look into it.
```

---
## \#8 Posted by: NickTheDude Posted at: 2018-08-23T03:54:23.074Z Reads: 67

```
Assuming you're going single motor, yeah 30-40 amps should be no problem. If you're going dual 25ish should probably be your max.
```

---
## \#9 Posted by: Namasaki Posted at: 2018-08-23T04:11:06.108Z Reads: 65

```
The Problem with 5ah 20C batteries is the voltage will sag under load so be careful when you get down to 50% charge because you could over discharge the battery very easily with voltage sag.
```

---
## \#10 Posted by: MaxMalouf Posted at: 2018-08-23T04:27:40.511Z Reads: 60

```
@Namasaki Does the VESC not cut out when the battery voltage is too low?
```

---
## \#11 Posted by: MaxMalouf Posted at: 2018-08-23T04:30:05.207Z Reads: 60

```
yeah I'm going dual motor. I think 20 amps each is sufficient, they are only the 90mm Maytech hubs.
```

---
## \#12 Posted by: Andy87 Posted at: 2018-08-23T04:32:33.131Z Reads: 61

```
You should also look into the point of how much your vesc can handle.
Don’t know which esc you have but usually they rated between  40-60a bat constant max.
So in a single set up 80a would probably also fry your drv.
```

---
## \#13 Posted by: MaxMalouf Posted at: 2018-08-23T04:35:26.711Z Reads: 58

```
I am planning on doing 20a bat max per VESC. I should be pretty safe...hopefully.
```

---
## \#14 Posted by: Namasaki Posted at: 2018-08-23T05:18:49.260Z Reads: 55

```
[quote="MaxMalouf, post:10, topic:65776"]
Does the VESC not cut out when the battery voltage is too low?
[/quote]

Yes it does but you’ll want to set it conservatively for Lipo cells
```

---
## \#15 Posted by: PatRocks Posted at: 2018-08-23T05:29:07.406Z Reads: 55

```
To elaborate on what @Namasaki is saying, those cells will sag individually at different rates because they will have different internal resistance. There are no two cells that are perfectly identical in their efficiencies, so one will be the best, and one will be the weakest. The difference between each may be small or large and the only way to know is either through precision measurements, or careful observation. There's a lot to consider when using lipos, fortunately however, there's a lot of information out there to help you find understanding. 

The V-esc can read pack level voltage, but it cannot measure cell level voltage. The safest approach is to become intimately aware of each cell's behavior and not push them to their potential until you **know** the weakest link

Edit: if you don't find answers to your questions here, check out rcgroups, endless sphere, or many of the other forums out there, and you will
```

---
## \#16 Posted by: TowerCrisis Posted at: 2018-08-23T05:32:35.640Z Reads: 52

```
I'm using these same cells in a 1p config. Haven't had experience with vesc undervoltage, is it a hard cut or will it just throttle down and decrease power until voltage stops sagging?


And @MaxMalouf I had a 10S2P pack with those same cells. I was easily pulling peaks of 50 amps on it when I really gunned it from a start. No noticeable voltage sag, even at near empty capacity.

But I've heard these cells vary frequently by batch.
```

---
## \#17 Posted by: Namasaki Posted at: 2018-08-23T10:57:41.080Z Reads: 50

```
The Vesc has a soft and hard back off strategy. 
Low voltage start is soft
Low voltage end is hard

Even my 5ah 60c Lipos sag some under load. 
You can bet that 5ah 20c Lipos  will sag under load even in a 2p configuration. 
How much will depend on several factors. 
It’s not that noticeable to the rider but it’s there and you’ll see it if you monitor your voltage with an inline meter while riding.
```

---
## \#18 Posted by: MaxMalouf Posted at: 2018-08-24T01:10:17.834Z Reads: 46

```
@Namasaki What should i set the cutoff voltage at to be safe? 31v for a 10s?
```

---
## \#19 Posted by: Namasaki Posted at: 2018-08-24T01:24:05.449Z Reads: 46

```
For 10s Lipo pack I would set the 

Battery cutoff start at 36v
Battery cutoff end at 34v
You don't ever want your Lipo cells to drop below 3v
Setting your cutoff at 31v would be very risky.
This is if you are not monitoring your voltage while riding.

I set my start at 34v and my end at 32v but I constantly monitor battery voltage by an inline volt meter mounted through the top of my board and usually stop when it hits 36v and I never go below 34v.
I also use a high amp bms that monitors individual cell voltages and prevents me from discharging any cell below 3v.
```

---
## \#20 Posted by: MaxMalouf Posted at: 2018-08-24T01:25:55.126Z Reads: 47

```
ah geez okay, thanks for the advice
```

---
## \#21 Posted by: Namasaki Posted at: 2018-08-24T01:29:14.268Z Reads: 47

```
Please read again, I updated my post
```

---
## \#22 Posted by: MaxMalouf Posted at: 2018-08-24T01:31:25.196Z Reads: 44

```
Yeah I use a BMS as well, I am thinking of putting in a Bluetooth Module and monitoring the voltage that way.
```

---
## \#23 Posted by: Namasaki Posted at: 2018-08-24T01:38:41.535Z Reads: 43

```
I have the metr bluetooth module and app but it doesn't report accurate battery voltage.
I contacted metr about it and they told me that it's because the Vesc V4 doesn't report voltage accurately.
The best way is with an inline meter mounted on top of the deck or through the deck like this:

![JPG|375x500](upload://4VKYoZb5OZPue6Xp2NgtyEtZpvr.jpeg)

![JPG|375x500](upload://tAOcFfrg5FcRNQXwdQRYAk7NF6P.jpeg)
```

---
## \#24 Posted by: MaxMalouf Posted at: 2018-08-24T03:27:54.167Z Reads: 41

```
Nice! That looks super clean.
```

---
## \#25 Posted by: Cobber Posted at: 2018-08-24T06:18:42.851Z Reads: 39

```
I play the voltage game even more conservatively.

All my lipos are 60/65c & I use a soft cutoff of 3.7v and hard at 3.5v.
I also only charge to 4.15v.

<img src="https://www.electric-skateboard.builders/uploads/db1493/optimized/3X/e/1/e1a8a6e15c04883958d10290ffa0d33751d3ab81_1_670x500.jpg" alt="image"/>

https://www.electric-skateboard.builders/t/lowest-safe-lipo-voltage-under-load/58095/3?u=cobber
```

---

# Acceptable drift between cells

### Replies: 40 Views: 539

## \#1 Posted by: Ishayc Posted at: 2018-08-03T19:15:56.373Z Reads: 164

```
Hi,

After a ride, most of my 10 cells battery stay within 0.05v from each other, but 2 cells differs by almost 0.2v.
I was wondering, what you guys thinks is an acceptable drift between cells before starting to worry?
My battery is Lithium Ion, 10s8p and the cells are 18650 Samsung 26j.

Thanks,
Ishay
```

---
## \#2 Posted by: Hummie Posted at: 2018-08-03T19:17:22.665Z Reads: 160

```
what cells and how many are there total?  just ten?  lipo?  ion?  iron?  if you have a couple in parallel be nice to know what is really going on in the p group and maybe one is ruining it.   bummer having cells in p stuck together so you cant know which is bum
```

---
## \#3 Posted by: wafflejock Posted at: 2018-08-03T19:26:55.795Z Reads: 150

```
Depends on how deeply you're draining them I wouldn't consider .2V drift to be that bad if you have cells at 3.4V and 3.6V, if you are at 3.7V on the top and 3.5V at the bottom would be more of a concern since at 3.7-3.8V you still have a large percentage of the battery power available but at 3.6 and lower it is less than half of the full charge in the cell.  Basically you want to be able to pull the same mAh from all the cells that are in series so that no given battery in series is ever below/past the voltage cliff on discharge.
```

---
## \#4 Posted by: Ishayc Posted at: 2018-08-03T19:35:08.410Z Reads: 143

```
Edited, Thanks.
Yes, It's a real pain to check the batteries in the P group especially after isolating the cells like crazy with a ton of electric tape and hot glue.
```

---
## \#5 Posted by: Ishayc Posted at: 2018-08-03T19:36:58.961Z Reads: 136

```
After draining the battery to 87% I had a drift of 0.14v.
The highest cell was at 4.05 and the lowest one at 3.91.
I get to 3.6 volts per cell only when squeezing the throttle because this battery is 21ah and the rage is crazy.
```

---
## \#6 Posted by: Fatos Posted at: 2018-08-03T19:42:46.533Z Reads: 131

```
I would start to get concerned actually. Since you have 8paralell cells it sounds like you most likely have one bad cell in each of those 2 groups.
You have a voltage drop of around 12-15% or 1/8. Not scientific proving but its an indication. 

I would charge them one by one one and se if you se the same after som riding. Just. To make sure that it isn't the bms.
You should at least investigate the pack in my opinion. 
Again this is what I think, but in the end its your call :)
```

---
## \#7 Posted by: Ishayc Posted at: 2018-08-03T19:46:41.086Z Reads: 116

```
I'm afraid it's not possible to charge them one by one.
What the max drift(estimation) before the battery is dead? or until it goes puff on me.
```

---
## \#8 Posted by: Fatos Posted at: 2018-08-03T19:53:25.233Z Reads: 109

```
Because you do have 8p it means that the problem is not so visible. Say you have lost one cell that means 1/8 of capacity for that row. Around 12.5%. As you can see it already sounds the way your pack is behaving. I'd you have 10s2p that would be 50% and directly dangerous.
This problem will grow with time since those two rows will have to work harder so it won't gett better. I personally would not sleep well  without fixing that :(.
Say Tesla car has over 60 cells in parallel that is not a big problem,but in your case it could be.

It is always possible to charge the rows one by one. Takes some skilles but it is possible. Or you could check if all the cells are getting fully charged after a long charging time.
```

---
## \#9 Posted by: Fatos Posted at: 2018-08-03T19:56:24.107Z Reads: 103

```
And please dont take only my word, there are more experienced guys who might have better clue than me. And maby prove my suspocion wrong.
```

---
## \#10 Posted by: Ishayc Posted at: 2018-08-03T20:04:53.185Z Reads: 98

```
I get your point.
Im now charging the battery and waiting for the BMS to kick in to see if it helps.
```

---
## \#11 Posted by: Fatos Posted at: 2018-08-03T20:08:17.622Z Reads: 93

```
Charing the pack to full might take time :). Deppening on the bms you have. But you would be able to see if it kicks inn.
```

---
## \#12 Posted by: michaelcpg Posted at: 2018-08-04T07:53:31.250Z Reads: 84

```
Would be interested to know what cells you're using. I've got a 10S9P pack that I've been using daily for several months now without balancing and they're all still within less than 0.01V of each other
```

---
## \#13 Posted by: Ishayc Posted at: 2018-08-04T08:19:21.821Z Reads: 79

```
Really? Sounds weird that they don’t drift at all without balancing.
I’m using Samsung 26j.
```

---
## \#14 Posted by: Ackmaniac Posted at: 2018-08-04T10:52:16.508Z Reads: 73

```
Normally good Li-Ion cells don't drift much. 0.2 is definitely too much and I do agree that it seems you lost a cell of your pack. And why do you use 26J. Did you harvest them from laptop batteries?
```

---
## \#15 Posted by: Ishayc Posted at: 2018-08-04T11:41:55.178Z Reads: 69

```
That’s what I was afraid of.
Not from a laptop, but I got the cells for almost free.

I’m using Bestech BMS and I think it does not balalnce the cells anymore. Does it have a way to know one of the cells in the P group is dead?
```

---
## \#16 Posted by: wafflejock Posted at: 2018-08-04T15:09:33.057Z Reads: 63

```
No the BMS has no way to measure that all the cells in parallel are at the same voltage. You'd have to disassemble the p groups and test the IR (internal resistance) or esr(equivalent seried resistance) to determine which cells are bad.

Also just to note I was talking numbers for lipos for liion the whole voltage scale is slid down a bit but same idea holds true.
```

---
## \#17 Posted by: strattos Posted at: 2018-08-04T15:24:31.404Z Reads: 60

```
![Capture%20_2018-08-04-09-19-28|297x500](upload://kViqRlmEJkjcXwMgcSaQMzINM0T.png)

Cells should all drift at a similar rate over their lifespan. Your bms is more there to monitor cells than it is to "balance charge". I have yet to have any balancing turn on.
```

---
## \#18 Posted by: Ishayc Posted at: 2018-08-04T15:35:37.316Z Reads: 53

```
lol my cells are not balanced at all compare to yours.
btw, what is this app calls?
```

---
## \#19 Posted by: strattos Posted at: 2018-08-04T15:41:51.057Z Reads: 58

```
Xiao xiang bms ![Capture%20_2018-08-04-09-36-20|297x500](upload://vpL5roemurnQN7gIWPuYyMofYSJ.jpg)

It's limited to those Chinese Bluetooth BMS's from what I understand. The pack is fairly new still maybe a dozen full cycles so I'll report back once I've got more cycles on it.
```

---
## \#20 Posted by: Acido Posted at: 2018-08-04T15:55:49.196Z Reads: 55

```
The less drift the better, when your pack is fully charged leave it at least 20minutes to balance itself out, each time
```

---
## \#21 Posted by: strattos Posted at: 2018-08-04T16:11:45.218Z Reads: 54

```
It's set up to static balance so it'll balance as soon as the cells vary by more than 0.01V

My BMS has had yet to activate its balancing circuit, which is how any well designed pack should be Imo. If you are constantly having to balance your cells something is probably wrong Imo.
```

---
## \#22 Posted by: Chase Posted at: 2018-08-04T17:23:55.632Z Reads: 50

```
Badass app. I’m such a noob I didn’t even know about these Bluetooth bms you speak of.
```

---
## \#23 Posted by: strattos Posted at: 2018-08-04T17:37:33.673Z Reads: 50

```
I'm honestly surprised you don't see them more often there's maybe half a dozen ppl using them that I've seen.

Using charge only 10$ BMS's scare me lol. 

I was originally gonna run BMS less before I found these.
```

---
## \#24 Posted by: Acido Posted at: 2018-08-04T17:39:47.942Z Reads: 49

```
On any bestech bms that is used the most on here, balancing starts as soon as one of the cells hit 4.2 

I do not know any bms that is balancing all the time can you link me one?
```

---
## \#25 Posted by: strattos Posted at: 2018-08-04T17:42:23.867Z Reads: 46

```
Ohhhh boy I got create a thread for this shit lol https://m.aliexpress.com/item/32827750823.html?pid=808_0000_0201&spm=a2g0n.search-amp.list.32827750823&aff_trace_key=63c1f9c951c34dbe8b96f4548590dce1-1525552980071-09079-7M7IEmQnY&aff_short_key=7M7IEmQnY&aff_platform=msite
![Capture%20_2018-08-04-11-41-27|297x500](upload://bLXTu66gOX555ZIrX91Lazdu301.png)

Those are just the basic settings available for the app the pc app let's you change about 20x more settings lol
```

---
## \#27 Posted by: strattos Posted at: 2018-08-04T17:47:38.069Z Reads: 46

```
This is the 12s version I used well it was from a different seller 
 http://s.aliexpress.com/zU7B3yiM Same kinda idea it's all based off of these designs from 
https://www.lithiumbatterypcb.com/3s-to-30s-lithium-ion-pcb/

They are the original designer as far as I can tell and have customizable options for ordering whatever you could need.
```

---
## \#28 Posted by: Chase Posted at: 2018-08-04T18:03:01.947Z Reads: 46

```
Wow thanks. I don’t know how I overlooked these when searching. I’m looking at a high discharge and it looks like this might work.

https://m.aliexpress.com/item/32847165991.html?spm=a2g0n.store-products.0.0.11d05f5ayHAEEy
```

---
## \#29 Posted by: strattos Posted at: 2018-08-04T18:03:25.770Z Reads: 48

```
Just so everyone knows there is no iPhone app currently so android only.
```

---
## \#30 Posted by: strattos Posted at: 2018-08-04T18:05:29.559Z Reads: 48

```
Those are even a step up in some ways supporting whatever battery config you want. But they are quite large /pricy. You can get up to 100Amp discharge BMS's of the same style I added a link to my previous comment of the exact one I'm currently using.

Tho I'm only using the 80Amp model
```

---
## \#31 Posted by: Chase Posted at: 2018-08-04T19:17:47.857Z Reads: 46

```
Cool thanks. Just bought one. By the way are these antennas?

![image|333x500](upload://luaKUZOCkj3djg1Dr7Lorr3LztB.jpeg)
```

---
## \#32 Posted by: sebaszz Posted at: 2018-08-04T19:22:47.674Z Reads: 45

```
there is

only not from the supplier but made by someone else

![image|281x499](upload://iGfCeHDA97c20h7zLbUp1KH2DdM.png)
```

---
## \#33 Posted by: Chase Posted at: 2018-08-04T19:46:18.363Z Reads: 42

```
Awesome. How do we get it?
```

---
## \#34 Posted by: strattos Posted at: 2018-08-04T20:01:19.286Z Reads: 42

```
Damn what bms/app is that.

As far as I know someone could write a much better app for this and it shouldn't be to hard for android but good to know someone made an iPhone version.
```

---
## \#35 Posted by: strattos Posted at: 2018-08-04T20:02:09.966Z Reads: 43

```
They are temperature sensors!
```

---
## \#36 Posted by: sebaszz Posted at: 2018-08-04T20:17:12.770Z Reads: 43

```
[https://itunes.apple.com/nl/app/xiaoxiang-bms/id1375405426?mt=8](https://itunes.apple.com/nl/app/xiaoxiang-bms/id1375405426?mt=8)
```

---
## \#37 Posted by: Andy87 Posted at: 2018-08-04T21:13:14.269Z Reads: 37

```
Just found this one
http://s.aliexpress.com/VZfymUJJ
A bit more expensive but works from 8-24s and up to 300a.
```

---
## \#38 Posted by: strattos Posted at: 2018-08-04T21:15:14.812Z Reads: 36

```
Lmao what do you need 300A bms for? thats the real question.
```

---
## \#39 Posted by: Andy87 Posted at: 2018-08-04T21:18:07.423Z Reads: 35

```
Nu who knows 😂😂😂 if I wanna fly to the moon...
No, seriously, if I wanna go quad mountain board I need as min the opportunity to go 150a.
300 is over the top but one day with 24s...😂🚀
Need to find the right esc for it🤔
```

---
## \#40 Posted by: Trdolan03 Posted at: 2018-11-25T17:21:57.221Z Reads: 26

```
[quote="Andy87, post:39, topic:63740"]
Need to find the right esc for it🤔
[/quote]

@Kug3lis  10 char
```

---
## \#41 Posted by: Andy87 Posted at: 2018-11-25T17:25:41.813Z Reads: 25

```
Or 
https://vesc-project.com/node/339
Still not 300a but I can live with it 😬😂🤪
```

---

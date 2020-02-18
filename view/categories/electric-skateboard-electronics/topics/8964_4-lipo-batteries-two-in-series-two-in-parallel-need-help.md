# 4 LiPo batteries. Two in series. Two in parallel (Need Help)

### Replies: 21 Views: 6010

## \#1 Posted by: Tijmen Posted at: 2016-09-05T09:00:36.907Z Reads: 320

```
Hey guys. Currently running my longboard on two 3S 8000mAh batteries wired in series.

I'd like to add 2 more batteries in parallel to double my capacity. I'd like to keep the batteries in the box when charging, so I need help with a diagram that'd include the wiring of the batteries and especially their balance leads, so that all I have to do is plug the batteries into my charger, along with a 6S balance lead which would then charge all 4 batteries.

Is this possible? Is it also possible to add only 1 battery and run 2 in series and one simply added to increase capacity?
```

---
## \#2 Posted by: kovjanos Posted at: 2016-09-05T10:58:04.143Z Reads: 305

```
It's just the battery config, add switches to separate battery for charging. Make sure cells are on the same charge level before connecting them (otherwise balance current could hurt your cells).

Although it would be possible to add  1x6S to a (3+3)S to get 6S2P, the cells could be so different that discharging would lead to more cell-balancing and you would not have the expected capacity and could shorten the life of the cells. 
<img src="/uploads/db1493/original/2X/c/c85fc2da7110e78f75cc56acd42615ae50558e27.png" width="412" height="331">
```

---
## \#3 Posted by: benwong Posted at: 2016-11-21T08:28:47.590Z Reads: 247

```
<img src="/uploads/db1493/original/3X/7/f/7fd04e5119b25085cb33c56bcea84ab0f63c7ce3.png" width="690" height="403">

this diagram works? 
same as title, 2 in series and 2 in parallel.
```

---
## \#4 Posted by: TarzanHBK Posted at: 2016-11-21T10:17:07.546Z Reads: 238

```
no you can´t cheat on physics ;)

you have to wire the 3. and 4. battery in series to get another 8s 5000mah pack and after that connect them in parallel to get 8s 10000mah.

Don´t wire different batteries together like a 4s and a 8s parallel.
```

---
## \#5 Posted by: lox897 Posted at: 2016-11-21T10:18:16.772Z Reads: 226

```
Put 2 batteries in parallel and the other two in parallel. Then connect those in series
```

---
## \#6 Posted by: benwong Posted at: 2016-11-21T13:13:37.647Z Reads: 217

```
okay, @TarzanHBK @lox897  thanks for your advise~~
```

---
## \#7 Posted by: charliek Posted at: 2016-12-15T05:11:13.777Z Reads: 203

```
Would connecting 2  x 3s 5000mah battery in series be same with connecting 2 x 6s 2500mah battery in parallel?
```

---
## \#8 Posted by: Tijmen Posted at: 2016-12-15T11:53:53.558Z Reads: 189

```
2x3S 5000mAh in series would be 6S 5000mAh
2x6S 2500mAh in parallel would be 6S 5000mAh
So yes I think it'd be the same
```

---
## \#9 Posted by: SirBo Posted at: 2017-09-26T20:24:28.014Z Reads: 147

```
Just wondering if it makes any difference if you wire 2 bats in series first and then connect them in parallel, or the other way around. When you just look on the maths, it doesn't change anything. But is it better for any reason to do it in the way you suggested? Just wondering and try to understand what i'm doing :slight_smile:

regards
```

---
## \#10 Posted by: MysticalDork Posted at: 2017-09-26T20:27:41.091Z Reads: 145

```
No difference, just which is easier to wire physically. If you go with two full series packs, and then wire them in parallel, you'll end up with a ton of balance leads to mess with. If you wire the cells in parallel and then in series, it makes it simpler to wire. Of course, lipo packs are already in series, so it's kinda a moot point either way
```

---
## \#11 Posted by: lox897 Posted at: 2017-09-27T12:56:04.213Z Reads: 130

```
Incorrect @MysticalDork

Here is a quote from @chaka 
“I want to add that in the "real world" connecting the cells in parallel first makes for a much more stable pack with lower voltage sag. This may not make sense on paper but real world testing has shown this to be true. My only concern with building a pack like this is if on cell shorts it will take the whole pack with it if the internal fuse fails.”

On @whitepony ‘s endless sphere thread from ages ago. It will also help to prevent thermal runaway if cells first balance themselves then connect to other cells.

I am no expert on this but I’m sure @chaka an explain it way better
```

---
## \#12 Posted by: TarzanHBK Posted at: 2017-09-27T13:35:04.367Z Reads: 128

```
i can second that.
There are a lot of lipos available with cells in paralell - 2s2p for example. A parallel group works as one unit. So get them as closest as possible together with the smallest possible resistance (wire lenght) and you will have a much more stable cell unit which balance itself.
After that, you can start with a serial connection.

Ameri..Parallel first - Serial second! :monkey:
```

---
## \#13 Posted by: MysticalDork Posted at: 2017-09-27T14:42:17.356Z Reads: 121

```
Isn't that what I just said, however ineloquently? Parallel first, series after. You can do it the other way but it's more of a pain.
```

---
## \#14 Posted by: lox897 Posted at: 2017-09-27T18:05:26.676Z Reads: 113

```
Yes sorry, I should’ve said that your reason wasn’t the most important and not that you were incorrect.
```

---
## \#15 Posted by: tojo Posted at: 2018-06-22T20:34:25.371Z Reads: 78

```
Hi guys! 
I have questions on the topic if you don't mind!
I have a 6s battery pack  (2x3S in series) since 2 month, can i add 2X3s in parralel to double the range (with two new and two old) ? If yes How i wire the BMS two, I use the same or i put another 6S BMS ? 

Thanks in advance!!
```

---
## \#16 Posted by: Tijmen Posted at: 2018-06-25T07:48:49.585Z Reads: 75

```
I would definitely not recommend adding old batteries with new ones. You'll definitely run into issues down the line.
Much better to just get all new ones entirely
```

---
## \#17 Posted by: David.c Posted at: 2020-01-06T10:03:04.056Z Reads: 18

```
Hi! 

Sorry for digging up an old post, hope you don’t mind. 

I’m currently putting together my first Electric Longboard.


If I were to purchase 4 of  Turnigy 4000mAh 4S 30C Lipo Pack w/XT-60 (2 series + 2 Parallel) should I get a decent amount of range? Single motor 6374 Torque ESC BLDC, I know a lot more comes into factor but rough estimate. 

The EV app calculator suggested I should get around 50km...
```

---
## \#18 Posted by: Tijmen Posted at: 2020-01-06T20:03:52.132Z Reads: 18

```
Hey David!

Actually fun to see an old post dug up like this to see how far I've come with this hobby! With your desired config you'll get 8S 8000mAh (8S 8Ah). 8Ah is fairly ok but it definitely won't be a long range monster. You'll always need to be aware of how much power you have and to be a bit conservative with the throttle and speed. That said, that's very doable and actually makes for a relaxed ride rather than some insane monster on wheels. You're not gonna get 50km though that's for sure. On my 12Ah dual 6374 build I get around 30km. That's not conservative riding though but still. Gives you a bit of an idea.

You do need to make sure you have an ESC that works with 8S. Also keep in mind that lower voltages are less efficient. 8Ah at 12S will get you further than 8Ah at 8S. I did however run 6S for a long time and it served me great so no complaints there. Good luck!
```

---
## \#19 Posted by: Fosterqc Posted at: 2020-01-06T21:31:03.126Z Reads: 18

```
Haha I used those 4Ah 30C packs from hobbyking. They were fast but a cell died in under 10 rides. Li-ion for esk8 unless you really know how to use lipos.
```

---
## \#20 Posted by: David.c Posted at: 2020-01-08T11:18:34.423Z Reads: 13

```
Thanks for the info! Where did you purchase your battery from or did you build it? 30km is perfect for me!
```

---
## \#21 Posted by: Tijmen Posted at: 2020-01-08T11:31:36.776Z Reads: 12

```
The 12Ah battery? I build my own 18650 packs. It's a 10S4P VTC6 pack for 120A continues output although a pack with 30Q's is just as good. I do definitely recommend 18650 over lipo though for eskates because of the amount of vibration and abuse the boards can go through.
```

---

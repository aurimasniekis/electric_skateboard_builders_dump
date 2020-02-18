# Making my own battery from 18650 cells

### Replies: 18 Views: 750

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-05-18T08:00:33.109Z Reads: 167

```
So my batteries are over a year old now and starting to show performance issues so I thought I'd replace them sometime soon. I always wanted to make my own battery, so I did some research and I found those 18650 cells that are used to make electric bike batteries.
Did anyone here make a battery for his board from those cells? are they reliable?
Also, I'm not sure how I would go about connecting them, if I connect 9 cells in series, each cell 3000mAh, then I'll have a 9s 3000mAh pack? if I want 6000mAh do I need to make two 9s 3000mAh packs and connect them in parallel?
Sorry if I'm asking dumb questions, I don't really know much about this subject.
Thanks
Edit:
Will [these](https://www.aliexpress.com/item/NEW-Dolidada-100-original-3-7-V-3000-MAH-18650-battery-for-us18650-Sony-VTC6-30A/32850710277.html?spm=2114.search0104.3.10.77f069bffFy6Sb&ws_ab_test=searchweb0_0,searchweb201602_3_10152_10151_10065_10344_10068_5722815_10342_10343_10340_5722915_10341_5722615_10696_10084_10083_10618_10307_5722715_5711215_10059_308_100031_10103_10624_10623_10622_5711315_5722515_10621_10620,searchweb201603_25,ppcSwitch_5&algo_expid=4b68a6c6-8394-4de1-a984-7068505796cb-1&algo_pvid=4b68a6c6-8394-4de1-a984-7068505796cb&priceBeautifyAB=0) work?
```

---
## \#2 Posted by: karma Posted at: 2018-05-18T08:05:30.390Z Reads: 159

```
If you look around a bit on the forum you will see that alot of people use the 18650 for their batteries. They are the sweet spot for size and power for eBoards. My recomendation, only buy cells from trusted vendors and the cell alot of people including me use is the Samsung 30Q (3000mAh and 15A cont. )
```

---
## \#3 Posted by: karma Posted at: 2018-05-18T08:06:17.952Z Reads: 156

```
Your assumptions of creating a 9S 6000mAh is correct. I recomend you watch some videos on youtuve by Michag Toll (channel: ebikeschool) to get some info on how to build a battery. He also has a good book if that’s more of your taste.
```

---
## \#4 Posted by: Sebike Posted at: 2018-05-18T08:06:37.379Z Reads: 145

```
Use. Search. Will. Find. Plenty. Info. 😊
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-05-18T08:07:34.038Z Reads: 140

```
Thanks, I'll look for the samsungs
```

---
## \#6 Posted by: b264 Posted at: 2018-05-18T08:52:55.902Z Reads: 134

```
Also if you put your location on your profile folks can help you better.  Depending on where you are, it can change EVERYTHING about cell pricing.
```

---
## \#7 Posted by: ShakeNBake7000 Posted at: 2018-05-18T09:20:47.090Z Reads: 123

```
Oh alright, I'll check, I'm from Israel, probably buy it online and not here because everything is expensive here.
```

---
## \#8 Posted by: ShakeNBake7000 Posted at: 2018-05-18T09:27:19.867Z Reads: 123

```
I just remembered I had a few years old electric bike battery, I took it apart and it had 40 of the 22650 3.7v 2500mAh cells, can't seem to find the discharge but considering it was used in a ebike battery it should be fine right? I think it's worth a shot since I already have the cells.
![26 PM|375x500](upload://xJL3OepXevW7pyFQtD4fz9ax6lU.jpeg)
```

---
## \#9 Posted by: JonathanLau1983 Posted at: 2018-05-18T09:39:29.001Z Reads: 117

```
Anything printed on the cells?
```

---
## \#10 Posted by: ShakeNBake7000 Posted at: 2018-05-18T09:40:51.363Z Reads: 120

```
Yeah.
![26 PM (1)|666x500](upload://d3qWmeuFYlyNjjJ6iJRAAZ8XsZw.jpeg)
Sorry its on the side
```

---
## \#11 Posted by: JonathanLau1983 Posted at: 2018-05-18T09:54:22.412Z Reads: 114

```
If they're anything like these ones then the outlooks not good.

Max continously discharge: 3C   (this would make it 7.5A a cell times 4 in parallel = 22.5A)
Max instant (30s) discharge: 5C ( = 37.5A peak)

What board you looking to put them on? Hub or belt drive?

https://www.alibaba.com/product-detail/Headway-li-ion-battery-22650-2_499002546.html
```

---
## \#12 Posted by: ShakeNBake7000 Posted at: 2018-05-18T09:55:32.758Z Reads: 112

```
Using one belt drive motor, that means it needs high amps and its not enough?
For some reason the reply isn't working.
@JonathanLau1983
```

---
## \#13 Posted by: JonathanLau1983 Posted at: 2018-05-18T10:20:11.966Z Reads: 108

```
Yeah, most belt drives will pull beyond these numbers. So you'll see massive lag during acceleration.

You'd be better off starting from scratch.
```

---
## \#14 Posted by: ShakeNBake7000 Posted at: 2018-05-18T10:22:33.248Z Reads: 109

```
[quote="JonathanLau1983, post:13, topic:55870"]
You’d be better off starting from scratch.
[/quote]

Alright, thanks for the help
```

---
## \#15 Posted by: b264 Posted at: 2018-05-18T17:21:32.747Z Reads: 89

```
[quote="ShakeNBake7000, post:7, topic:55870"]
probably buy it online
[/quote]

Get Samsung 30Q flat top cells from http://ru.nkon.nl
```

---
## \#16 Posted by: ShakeNBake7000 Posted at: 2018-05-19T14:00:41.841Z Reads: 65

```
Wow thanks it's out of stock but its way cheaper than what I found, need to check shipping to see if its not too expensive
```

---
## \#17 Posted by: b264 Posted at: 2018-05-19T17:16:22.801Z Reads: 58

```
They will come back in stock soon.  Set up a stock alert
```

---
## \#18 Posted by: Tampaesk8er Posted at: 2018-06-09T19:20:33.584Z Reads: 36

```
Here is a great video for you, its funny, this video was made cause i brought the idea to him. At the end of the video, he announces the winner to his book about 18650 batteries and i was the winner to his giveaway. His name is Micah Toll and he's from Tel Aviv and you can even buy the batteries from him, he knows his stuff and the book is great by the way.

https://youtu.be/1D90heZ8z4s
```

---

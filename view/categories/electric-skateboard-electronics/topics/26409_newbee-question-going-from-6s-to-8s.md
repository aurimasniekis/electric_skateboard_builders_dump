# Newbee question. Going from 6s to 8s

### Replies: 10 Views: 583

## \#1 Posted by: Silverline Posted at: 2017-06-29T19:52:58.972Z Reads: 86

```
Hallo...

I have this skateboard kit : https://www.elxskate.com/collections/all/products/x1-electric-skateboard-kit
And i have updated the ESC to an VESC....

At the moment i`m running the board with a 6s 5000mAh lipo battery (following the info from the site)
But I've been thinking of, if I would get longer distance, if i upgrade my currently battery to a 8s 5000mah battery instead ?

I have not much info about the motor unfortunately, besides it`s 1200watt, and my motor pulley is 20T and wheel pulley 60T.

I love my board, but whant a little more distance if possible. 

Hope for some help :-)
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-29T20:25:59.834Z Reads: 83

```
Increasing voltage will help with top speed and electrical efficiency to some degree and does increase the overall power in the pack but when you're looking at capacity increase really you just need more Ah (current available over time).  One issue with bumping the voltage could be if the motor can't handle it but otherwise should be fine increasing the voltage.  Another possible problem is if the kv of the motor is too high (above 260kv from what I've been hearing) then you can run into issues with the max eRPM for the VESC to turn the motor and can blow the DRV chip if you don't throttle that value, but I don't think you get into the upper limits of that unless it's a combo high kv motor and high voltage battery.
```

---
## \#3 Posted by: Challlsss Posted at: 2017-06-29T20:28:10.488Z Reads: 77

```
A good idea would be to add another 6S in parallel. This would essentially double your range
```

---
## \#4 Posted by: Silverline Posted at: 2017-06-29T20:32:20.981Z Reads: 73

```
Thanks guys...

So what i´m hearing you guys says, is that with 8s 5000mah , i will not have any noticeable increase in range. I was hoping, that the less current draw i would have over the motor, when increasing the voltage, would give me some more range. But maybe it`s better with some more capacity overall, and stay on 6s..

Sadly the only thing i know about the motor is that it`s 1200watt. I have asked the seller, and he dont know. I know it`s a chinese board.
```

---
## \#5 Posted by: Challlsss Posted at: 2017-06-29T20:34:27.233Z Reads: 64

```
you will have a increase in range. But you will probably ride your board harder and that will decrease your range
```

---
## \#6 Posted by: Smorto Posted at: 2017-06-29T20:38:15.210Z Reads: 59

```
Like everyone has said, with higher voltage you will have more Wh and thus more range. However, at @Challlsss mentioned, you will probably ride the board faster which will actually decrease your range. The best option is to add another 6s battery in parallel as @Challlsss mentioned as well.
```

---
## \#7 Posted by: Silverline Posted at: 2017-06-29T20:50:02.311Z Reads: 52

```
Thanks guys...

I will do that.
```

---
## \#8 Posted by: Challlsss Posted at: 2017-06-29T20:51:23.839Z Reads: 50

```
Oh btw that is exactly what I am doing right now to my build. So if something goes horribly wrong I'll be sure to let you know haha ;)
```

---
## \#9 Posted by: Silverline Posted at: 2017-06-29T21:12:52.892Z Reads: 47

```
Ha ha

What batteries are you using ? I'm using 2x 3s 5000mah in series. But i have problems with fitting the batteries inside the 'container' thats why i came Up with the 8s thing, because hobbyking is selling single lipo pacs 1s5000mah, and 8pcs would fit perfect... So now i need to figuring out how to fit two 6s in parallel inside :-/
Maybe  i just wait and se what you come Up with 😎
```

---
## \#10 Posted by: Challlsss Posted at: 2017-06-30T14:12:57.831Z Reads: 19

```
I have 4x 3SX 5000mAh in a 2S2P configuration. I am building a new enclosure for them.
```

---

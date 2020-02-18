# 8WD! eight wheel drive

### Replies: 8 Views: 1137

## \#1 Posted by: okay Posted at: 2017-06-04T01:07:25.219Z Reads: 236

```
Cheers everyone! I Was wondering if I could have tandum trucks and have hub motors on everyone? Now before you start typing, I know that this is crazy and unrealistic. Could you guys run some numbers and figure out how mant lipos I would need? Also could you figure out how fast this could go and horsepower? Pricepoint?
```

---
## \#2 Posted by: Smorto Posted at: 2017-06-04T01:58:50.537Z Reads: 223

```
Let me begin by saying that I am not expert on any of this ant can't answer most of your questions. Just so you know though, your top speed will stay (relatively) the same weather you have 2 hub motors, or 8. To calculate how many "lipos" you will need we need to know a few things. What type of hub motors you are using, your weight, riding conditions, and the types of "lipos" you ar referring too. This will be a sight if it ever happens though! :slight_smile:.
```

---
## \#3 Posted by: NickTheDude Posted at: 2017-06-04T03:40:11.562Z Reads: 205

```
Yes! Do it for science! 

First of all, this would be absurdly expensive, 8 VESCs alone would cost almost a grand. However, if you wanted to do it... I'd shoot for around 4000W because 500W per motor seems reasonable for hub motors. If you were using VESCs I'd go 10S cause that seems to be the sweet spot.

500W / 37V = ~14A

So you'd need to tune your 8 VESCs for 14A each. Then you'd need a battery that can discharge enough current.

14A * 8 = 112A

You'd need to be able to discharge 112A continuous. Assuming you were using a 10S 8000mAh lipo, you would want one with a C rating around 30C because they often overstate the C rating and assuming it is half of whats stated is a safe bet. 8000mAh at 15C is 120A, which should be enough.

Then you'd just have to find hub motors that can reliably handle 500W, which shouldn't be too hard, then you're good to go!

All that being said, 4000W from 8 motors isn't actually that much and if you found motors that could handle more watts you could get a higher discharge battery and probably hit somewhere around 6000-8000 watts if you wanted to.

BTW 1000W is about 1.35 horsepower.
```

---
## \#4 Posted by: saul Posted at: 2017-06-04T06:38:14.589Z Reads: 163

```
I had a similar thought a while back. tandum trucks came up right away, then tank treads!
https://www.electric-skateboard.builders/t/ultimate-overkill-8-motor-awd-concept/11594
```

---
## \#5 Posted by: High-roller Posted at: 2017-06-04T06:59:49.025Z Reads: 154

```
Considering that this now exists:
https://www.electric-skateboard.builders/t/tank-track-board/23332/53
I'd say that if you have the budget and the drive to make it- go for it! If you prove that it can be done, maybe others will follow.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2017-06-04T13:19:00.922Z Reads: 106

```
A 4WD would be more than enough as long as you don't weight more than 200 kilos and it would be doable by costs and enclosure size for the components. I could modify my board for example to a 10S8P battery and by that i have the space for 4 more VESC's. Actually when i think about it there would be space to fit 8 VESC then by stacking them.
Then take the Enertion R-SPEC Ghost motors which can easily output 1500 watts and more each. Then you would have already 6000 watts which would be very hard to handle. 
But then you also would need different power output settings because the front wheels would loose traction easily. But with my firmware mod you can program different ratios for the front and backwheels. So 1500 watts for the back and 1000 for the front would make more sense which still outputs 5000 watts in total. (more than enough for a street board)
```

---
## \#7 Posted by: evoheyax Posted at: 2017-06-04T18:48:14.786Z Reads: 66

```
Why do you need to adjust power output for the front and back?

I've never had the front slip on me even once. And I don't use traction control. I run each little hummie motor a little over 1000 watts each, so 4000 watts total.

Not trying to argue, just want to understand your perspective better :slight_smile:
```

---
## \#8 Posted by: Ackmaniac Posted at: 2017-06-04T18:55:55.572Z Reads: 65

```
When i drive backwards with my board in reverse then the wheels easily loose traction. But i also ride with 80 motor amps. And for braking it would be useful the other way round. Instead of slipping back wheels you can brake harder at the front. For a car it is the same principle. Front wheels can brake harder than back wheels. Roughly it is a ratio of 70/30.
```

---

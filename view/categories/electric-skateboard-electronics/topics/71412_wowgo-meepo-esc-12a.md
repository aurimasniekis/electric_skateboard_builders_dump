# Wowgo/meepo esc 12A

### Replies: 12 Views: 1052

## \#1 Posted by: ramon Posted at: 2018-10-16T18:02:22.025Z Reads: 132

```
Why is it that my wowgo has more torque with this esc:
[https://es.aliexpress.com/store/product/NEW-version-2-4G-transmitter-esk8-24V-36V-single-dual-motor-drive-controller-brushless-hub-motor/3151014_32918075083.html?spm=a219c.search0104.3.131.5098222csFwsut&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_318_10547_319_10548_10696_450_10084_10083_10618_452_535_534_533_10307_10820_532_10301_10821_10303_204_10059_10884_10887_100031_320_10103_5727015_448_449_5727515,searchweb201603_60,ppcSwitch_0&algo_expid=6a540567-5360-4766-ad85-9b7d50ad7e83-18&algo_pvid=6a540567-5360-4766-ad85-9b7d50ad7e83&transAbTest=ae803_5](https://es.aliexpress.com/store/product/NEW-version-2-4G-transmitter-esk8-24V-36V-single-dual-motor-drive-controller-brushless-hub-motor/3151014_32918075083.html?spm=a219c.search0104.3.131.5098222csFwsut&ws_ab_test=searchweb0_0,searchweb201602_2_10065_10068_318_10547_319_10548_10696_450_10084_10083_10618_452_535_534_533_10307_10820_532_10301_10821_10303_204_10059_10884_10887_100031_320_10103_5727015_448_449_5727515,searchweb201603_60,ppcSwitch_0&algo_expid=6a540567-5360-4766-ad85-9b7d50ad7e83-18&algo_pvid=6a540567-5360-4766-ad85-9b7d50ad7e83&transAbTest=ae803_5) 
which is 12A than my DIY board which is using a vesc which is supposed to handle up top 150A?
Am I missing something? Even if its 12A per motor it still only 24A peak compared to the 150A vesc peak
```

---
## \#2 Posted by: Sn4pz Posted at: 2018-10-16T18:03:50.628Z Reads: 127

```
just because its rated for it doesnt mean it hits it.... seems like you need this:

https://www.electric-skateboard.builders/search

What battery do you have?

its very likely you dont have your settings dialed in right
```

---
## \#3 Posted by: ramon Posted at: 2018-10-16T18:08:41.760Z Reads: 125

```
I have 6S1P lipo ( 2*3s 5000mah in series) with 35c each, so its supposed to be able to handle a 175A discharge on paper. And I've tried multiple settings (up to 50A battery discharge) on BLDC, right now it has been over a year since I used my DIY board for the last time, but I was thinking to turning it into a 2WD offroad board.

(batterys have always been charged with a balance charger and the motor is rated for up to 3KW)
```

---
## \#4 Posted by: Sn4pz Posted at: 2018-10-16T18:15:07.388Z Reads: 111

```
unfortunately, as far as I understand, lipo batteries are commonly 'mislabled', and are rated for more amps that they can carry. So thats a possibility(what brand, maybe link it?) 

Unforunately what you actually bought is a chinese ESC, so theres no programming that you can do to change it :( 

Also im not too sure about voltages, because a 10s system is 36v, but that is compatible with 24v and 36v.... is 24v 6s?
```

---
## \#5 Posted by: ramon Posted at: 2018-10-16T18:21:44.463Z Reads: 104

```
I have two boards, my diy board is using an enertion 2015 vesc programable with BLDC tool, but my wowgo is using that chinese non-programable esc (but its still producing more torque). So my question  was why is my expensive single drive vesc producing less torque than a cheap chinese dual drive esc.

Battery misslabeling is an option since my diy board batteries were from hobbyking, but even with that, I dont think that if they're misslabeled and rated for 175 amps they wil draw less than the 24 amps that my chinese esc peaks.

The only thing which comes to my mind is to try my expensive meepo battery on my expensive vesc and motor
```

---
## \#6 Posted by: Sn4pz Posted at: 2018-10-16T18:26:57.833Z Reads: 92

```
Not sure how versed you are with the bldc tool but maybe your motor max is off? As far as I know that setting deals with torque....

I doubt your meepo battery with do anything different. 

im kinda stumped, im sure its simple enough though. Post bldc settings?

not to mention, the jump between single and dual motor is large.... could be that your first build just doesnt cut it? :man_shrugging:
```

---
## \#7 Posted by: Sn4pz Posted at: 2018-10-16T18:29:38.389Z Reads: 79

```
additionally motor kv is important. what kv is your bldc motor?
```

---
## \#8 Posted by: Jmding Posted at: 2018-10-16T18:41:48.782Z Reads: 79

```
Your power is low because your voltage is 60 percent what wowgo uses. Even though your current is high, the lack of voltage means your power is low. And you likely have very tall gearing to compensate for that low power. Hence your torque is low
```

---
## \#9 Posted by: bartroosen12 Posted at: 2018-10-16T18:47:14.426Z Reads: 80

```
I got the ownboard kit with the same esc as the wowgo and it draws max 18A, so 9A per motor.
In your alliexpress links is stated "current: 12A"
So I guess that's 12A per motor so 24A in total.
That should definitely feel more powerfull than your wowgo esc.
I've heard that the banshee preditor board also has 24A and feels much more powerfull than ownboard/wowgo.
Wowgo has a more smooth throttle curve while this alliexpress esc has a more 'agressive' curve.

And yeah your 6S setup should be able to pull 40A to get roughly the same power.
Also 1 motor makes a difference and you got only 6S1P so 1 cell has to be able to give 40A so you will get some beautifull voltage sag which also reduces the power and speed

So that can be pretty normal that the chinese esc is performing better
```

---
## \#10 Posted by: wowgoboard Posted at: 2018-10-19T07:34:18.410Z Reads: 61

```
Hi guys,  It is reasonable that Wowgo ESC is customized to 18 A ，because the 24 A will crate much more heat and load to the motor and battery, although it would cause problem in a short time, but maybe after a long time, it will affect the life time of board, and the 18 A could also crate a very big torque to fit lots of roads, so it's a good balance,  many customers said their Wowgo board works very good after they use it for  a long time, that's because we consider every details before we made it, our goal is not only make the good quality electric skateboard, but also consider everything which will increase the riding feeling of the riders and make it durable. We think we can do it better in electric skateboard, that's why we are in the market, thanks
```

---
## \#11 Posted by: Jmding Posted at: 2018-10-19T14:54:44.121Z Reads: 52

```
Hello Wowgo! Welcome to the forum! It's great to have some representation from the consumer brands on here. There's a lot we can learn from each other. You should consider starting a thread in the general discussion area announcing yourself. I'm sure lots of people have feedback or product ideas they would like to suggest if they knew you were on here! 

Does reliability of this ESC drop off significantly after 18A? How does 20A perform long term (as an example)? 18A probably makes a lot of sense for your customers, it is well known that your product is more refined and cohesive than many of its competitors. Please don't take the the statement that the ESC is "only" 18A as accusatory, it is just that this forum is full of adrenaline junkies that run dual setups with 150 at the motors and 3:1 gearing on top of that! That's why you very few people here use Chinese hub motor components, just a different audience altogether. .
```

---
## \#12 Posted by: Jmding Posted at: 2018-10-19T15:22:12.055Z Reads: 42

```
@ramon
double check your VESC configuration?  What motor_current value did you set in VESCTool?  Battery_current isn't enough, if your battery_current = 1000A but your motor_current = 1A, the motors will only ever experience 1A of current.

Its possible that the Chinese ESCs allow temporary high currents, whereas the VESC will prevent you from ever going over your motor_current value.  If that's the case, you might set your motor_current to, say, 2x higher and just make sure not to sit at more than 50% throttle for more than 10 seconds at a time.
```

---

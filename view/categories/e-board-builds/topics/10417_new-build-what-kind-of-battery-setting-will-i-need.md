# New Build - What kind of battery setting will I need?

### Replies: 35 Views: 2837

## \#1 Posted by: r0ymanesco Posted at: 2016-09-30T14:55:10.993Z Reads: 177

```
I'm currently doing research to begin my first eBoard build and I have a couple of questions. So I'm thinking of using two 3S 5200mAh 10C (20C Peak) 11.1V batteries and the r-spec motor from enertion. However I can't decide if I should put the batteries in series or in parallel. From what I understand, if I put the batteries in series, I would have an output voltage of 22.2V which would be enough to start the motor (14 - 44V Max) but would hinder its performance since the nominal output current for the battery is only 10C ( 10C x 5.2A = 52A and 2400W / 22.2V = 108A so the battery cannot output enough current). On the other hand, if I put them in parallel, I could output enough current ( 10C x 10.4A = 104A) but my output voltage (11.1V) would not be sufficient to start the motor (14 - 44V Max). The obvious solution to this problem would be to get more batteries and have two pairs of two batteries in series then connect them in parallel but that would increase the cost quite a bit so my main question is would it be possible to use this motor with just two batteries that I mentioned or do I HAVE to get more batteries to solve this issue. Thanks in advance.
```

---
## \#2 Posted by: JLabs Posted at: 2016-09-30T14:57:29.201Z Reads: 167

```
Running 3s is a little low.  I'd recommend getting 3s 20c batteries an putting them in series.
```

---
## \#3 Posted by: r0ymanesco Posted at: 2016-09-30T15:01:46.206Z Reads: 161

```
Thanks for the reply, I have thought about that but when I went on hobbyking to look at batteries, I can't seem to find a 5000mAh 20C battery that has a TX60 connector which I need to use the VESC from enertion. Most of them come with 5.5mm bullet connectors but hobbyking doesn't sell 5.5mm bullet connector to TX60 adaptors. Is there a way to get around that or will I have to make my own adaptor? Thanks
```

---
## \#4 Posted by: JLabs Posted at: 2016-09-30T15:30:18.900Z Reads: 140

```
No problem! Yes, you can just cut the connect off and solder on an XT60. I would not recommend this if you have never soldered before or have a small soldering iron.
```

---
## \#5 Posted by: r0ymanesco Posted at: 2016-09-30T15:43:38.225Z Reads: 127

```
Ok great, soldering is not really a problem for me so this solution should work out. I do have another question. What kind of range do you think putting two 5000mAh 20C batteries in series would give me ( I weigh 53 kg)? I want to be able to ride for at least 5km, would this setup be able to achieve this range? Thanks in advance.
```

---
## \#6 Posted by: 2-alex-2 Posted at: 2016-09-30T15:49:01.530Z Reads: 123

```
I'm running 3x2s 5000mah in series to get 6s which is what you would be looking at minimum. I also run a 245kv single motor with 16-32t gearing which roughly I'm getting 9km out of a charge. This is mainly on flat ground with only a short up hill so depending on the terrain your running on will determine how far you will get.
```

---
## \#7 Posted by: r0ymanesco Posted at: 2016-09-30T15:50:42.805Z Reads: 117

```
Ok thanks for the suggestion. Would you say that 3x2s 5000mah is better than 2x3s 5000mah setup?
```

---
## \#8 Posted by: 2-alex-2 Posted at: 2016-09-30T15:57:21.274Z Reads: 119

```
No wouldn't make any difference if they are same c rating. Just I run a drop through deck and needed to be as thin as I can. How much would two new 3s cost you as there are pre built options available.
```

---
## \#9 Posted by: JLabs Posted at: 2016-09-30T15:59:21.034Z Reads: 114

```
2x3s is better. Your not going to want to charge all of those batteries.
```

---
## \#10 Posted by: r0ymanesco Posted at: 2016-09-30T16:01:06.567Z Reads: 117

```
From what I can see 2x3s 5000mah is going to be around 36 GBP and I will also have to buy TX60 connectors to solder them on which costs around 3 GBP. Can you link me to pre built options? Thank you
```

---
## \#11 Posted by: 2-alex-2 Posted at: 2016-09-30T16:01:10.447Z Reads: 110

```
I charge mine as one 6s so no extra time in that
```

---
## \#12 Posted by: 2-alex-2 Posted at: 2016-09-30T16:02:24.009Z Reads: 111

```
http://alienpowersystem.com/shop/batteries/alien-6s-10000mah-35c-lipo-battery-flat-configuration-size-a/

This is a prebuilt option but also double the mah with 10000mah so lot more but everything is done. Where in U.K. Are you.
```

---
## \#13 Posted by: r0ymanesco Posted at: 2016-09-30T16:06:32.536Z Reads: 114

```
I live in London. This looks really impressive but is considerably more expensive than what I had in mind. Thanks for the suggestion anyway. Speaking of which, what kind of charger do you use? I've been looking at this one http://www.hobbyking.com/hobbyking/store/__103697__HobbyKing_C3_50W_Charger_Discharger_AC_DC_UK_Plug_UK_Warehouse_.html which looks good enough but I'm not sure if it's the best I can get. Also are BMS necessary? If so will this one which seems to be both an indicator and a manager work ok ( http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=43590 ) ? Thanks in advance and sorry for the long question.
```

---
## \#14 Posted by: 2-alex-2 Posted at: 2016-09-30T16:09:57.480Z Reads: 96

```
Yea mine cost me like £40 for the 3 and mine are 35c just more work involved in wiring them together. Ok there are some on here that are in London I'm further up north in Cumbria.
```

---
## \#15 Posted by: r0ymanesco Posted at: 2016-09-30T16:12:19.741Z Reads: 102

```
Yea I figured putting more work in wiring them up should save me some money. Speaking of which, what kind of charger do you use? I've been looking at this one http://www.hobbyking.com/hobbyking/store/__103697__HobbyKing_C3_50W_Charger_Discharger_AC_DC_UK_Plug_UK_Warehouse_.html which looks good enough but I'm not sure if it's the best I can get. Also are BMS necessary? If so will this one ( http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=43590 ) which seems to be both an indicator and a manager work ok?  Thanks in advance and sorry for the long question.
```

---
## \#16 Posted by: 2-alex-2 Posted at: 2016-09-30T16:15:10.575Z Reads: 102

```
That charger seem OK similar to the bmax 6 ac that others use. As for bms it's not necessary if you are going to use one of these charger you just have to be carful with the voltage and not running them to low so my esc has a cutoff of 3.4v per cell so x6=20.4v and I now run a volt meter on my board. And as long as you balance charge them with that charger the levels should stay good. 

<img src="/uploads/db1493/original/3X/6/e/6e821e2e4ff95b5ca1a9bce186d66142030e4b8f.jpg" width="666" height="500">
```

---
## \#17 Posted by: r0ymanesco Posted at: 2016-09-30T16:20:09.209Z Reads: 90

```
Ok I see. Can you link me to the volt metre you're using? Also, how do you decide on the cutoff voltage? Thanks
```

---
## \#18 Posted by: 2-alex-2 Posted at: 2016-09-30T16:24:28.862Z Reads: 94

```
Will get a link just on eBay 
https://www.ebay.co.uk/itm/331724469467 

The cutoff is what's been researched by a lot of people from Rc community, when the voltage drop to low they can get damaged and possibly catch fire which is why you need to take lots of care with lipo when discharging and charging.
```

---
## \#19 Posted by: sl33py Posted at: 2016-09-30T16:25:20.657Z Reads: 90

```
I think you have some good suggestions and options already, but wanted to clarify the C rating of the batteries.  I wouldn't go below a 100a ability of the batteries (my minimum) as most are marketing from the company and totally unreliable and likely incorrect.  So an example is the 3s 5000mAh 20c (20c * 5Ah = 100a).  The better they can provide, or the more in parallel to lessen the load - the less voltage sag - and if you don't heavily draw (=heat) the batteries they will also last longer.

I also recommend DIY w/ two 3s for 6s.  I usually get the thinnest (C dimensions on HK) batteries i can find - and with only 3s you can get some super thin ones around 20-25mm.  Nice and stealthy!

Cutoff voltage - i set mine to 3.6v because with a little bit of sag you can pull them lower and i don't want to damage my cells.  Also get a lipo alarm to yell when you hit that voltage - vs just relying on the ESC to let you know, or by feel.

GL!
```

---
## \#20 Posted by: r0ymanesco Posted at: 2016-09-30T16:39:48.203Z Reads: 89

```
Thanks for the additional info. I'm guessing to be safe getting two 3s 5000mAh 25C would be best?
```

---
## \#21 Posted by: 2-alex-2 Posted at: 2016-09-30T16:42:12.177Z Reads: 77

```
If you could get 30c is the ideal and what I run and have no issues but I am looking to upgrade and get that pre build 10000mah or find some decently prices 3s 10000mah to get more mileage as get 6 miles at the moment but would love more.
```

---
## \#22 Posted by: Namasaki Posted at: 2016-10-01T07:06:31.210Z Reads: 80

```
I read through the post quickly so I might have missed it but did anyone mention that you'll need some sort of anti spark solution?
And I would recommend that you get the highest C rating you can. It really makes a difference in performance and range using 60c packs over 20c
It might seem like over kill but really it's not. 
Even with a 300a battery, there will be some voltage drop under load.
```

---
## \#23 Posted by: r0ymanesco Posted at: 2016-10-02T10:17:48.582Z Reads: 78

```
I thought the C rating just determines highest discharge rate of the battery and it depends on the motor to pull the necessary current from the battery? I might be wrong since I'm new at this.
```

---
## \#24 Posted by: Namasaki Posted at: 2016-10-02T18:43:10.832Z Reads: 76

```
You are correct. The motor draws the current. 
If your using a standard RC Esc, the throttle controls the amount of voltage supplied to the motor and the amount of current will be determined by the amount of load placed on the motor.
If your using a Vesc in current control mode, full voltage is supplied constantly while the Vesc limits the amount of current the motor can draw. 
More throttle=more current. 
Now, you are also correct concerning the C rating of the battery. The C rating X mah = max constant discharge rate. 
There is however one other important factor. That is Voltage sag. The more current you draw from the battery and the closer you get to the max discharge rate, the more the voltage drops. Reducing power and range.
The reduction of range is a factor that I have just recently discovered testing various batteries on flat and hilly conditions. And the science to back it up is this. Voltage X Capacity /G = Range
The value of G was 22 with my 145kv hub motors
The value of G was 18 with my 230kv belt drive with 16/36 gears
So as your voltage drops, your range is decreased.
This is why you want your max discharge rate to be as high as you can get it.
There are two ways to achieve this.
Some have used multi rotor packs with very high capacity and low C rating.
I chose lower capacity with very high C rating. 5000mah X 60c for 300a discharge rate.
Higher C rated Lipos tend to have lower internal resistance which makes them more efficient and less prone to heat.
```

---
## \#25 Posted by: sl33py Posted at: 2016-10-02T19:38:58.815Z Reads: 71

```
[quote="Namasaki, post:24, topic:10417"]
There is however one other important factor. That is Voltage sag. The more current you draw from the battery and the closer you get to the max discharge rate, the more the voltage drops.
[/quote]


Great post @Namasaki!  @r0ymanesco - listen to what he's saying here.  If you look at some of the battery tests (mooch is amazing for these) you can see the voltage sag he mentions.

The big impact to range on sag is both heat and reduced battery capacity (you get less than the claimed xxxxmAh's).

here's a good example:
[img]http://i.imgur.com/dfXpV5Q.png[/img]
It's a LOT of squiggly lines... but the things to look at are the big "sag" on the far left as you try to pull more and more amps from this 18650 - and the corresponding poor capacity ( 1000mAh capacity @ 20a discharge of a 3100mAh cell!) when you pull too much amps from a cell.  This is an extreme example, but really illustrates performance at different discharge rates.  The heavier you draw a cell the more heat it generates - losing energy to heat is likely a huge reason for the poor capacity.

HTH!
```

---
## \#26 Posted by: r0ymanesco Posted at: 2016-10-02T20:19:23.409Z Reads: 63

```
I see, thanks @Namasaki and @sl33py Great info, I will try to get the highest C rating I can afford.
```

---
## \#27 Posted by: Namasaki Posted at: 2016-10-02T20:30:26.983Z Reads: 64

```
How did you get that meter to read voltage instead of percentage?
```

---
## \#28 Posted by: Namasaki Posted at: 2016-10-02T20:51:00.196Z Reads: 69

```
I use these 2s packs in series. Its a simple setup and keeps the battery low profile.
For 6s you would only need 3 and you could charge them all at once with a 6s balance charger or put more in series and use an onboard BMS as I did and charge with a laptop charger.
http://www.hobbyking.com/hobbyking/store/uh_viewitem.asp?idproduct=52279
<img src="/uploads/db1493/original/3X/6/a/6a9dce26a72053009a414050a84576274ee79823.png" width="364" height="500">
```

---
## \#29 Posted by: r0ymanesco Posted at: 2016-10-02T20:52:35.607Z Reads: 66

```
Great, given that this is tried and tested, I will be getting three of these then. Cheers :slight_smile:
```

---
## \#30 Posted by: Namasaki Posted at: 2016-10-02T20:58:39.747Z Reads: 72

```
So far I am really stoked with the performance of these batteries and the hard case is a huge plus. 
Check out my build thread here:
http://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
When buying on Hobbyking.com, create or log in to your account first.
They tend to give better prices when your logged in.
You should get these batteries for $25.79 ea.
If there showing a higher price, sit on the page until they pop up a discount offer.
Service has been great buying for Hobby king west warehouse lately. Their delivery time is really fast!
<img src="/uploads/db1493/original/3X/e/a/ea0fa2f9c6f8575ad7a0ceb68527ebb3e7c55782.png" width="690" height="388">
```

---
## \#31 Posted by: 2-alex-2 Posted at: 2016-10-02T21:53:32.988Z Reads: 72

```
Button on the back changes it
```

---
## \#32 Posted by: vadimkovalev99 Posted at: 2017-06-15T09:33:26.760Z Reads: 37

```
okay this much science made me smile :D you really sound like you know this stuff man i wish i could be thesame. i just forgot half the stuff i read :P
```

---
## \#33 Posted by: rizwanar Posted at: 2017-10-15T07:58:24.796Z Reads: 29

```
Is it possible to use a single lipo battery with 35c 6s 4200mah
```

---
## \#34 Posted by: rizwanar Posted at: 2017-10-15T08:01:03.961Z Reads: 30

```
Is it possible to use a single lipo battery with 6s 20c and 4200mah battery for electric skaye board
```

---
## \#35 Posted by: Namasaki Posted at: 2017-10-15T14:10:40.973Z Reads: 30

```
If you want to run 6s it is recommended to not use a Vesc because of high current. This is what I've heard, I haven't personally tried a Vesc with less than 10s. 
As for the battery, get something that will handle high current and yield long range like this:

http://www.smc-racing.net/index.php?route=product/product&path=67_119&product_id=467
```

---

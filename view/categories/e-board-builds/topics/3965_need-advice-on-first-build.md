# Need advice on first build

### Replies: 11 Views: 1398

## \#1 Posted by: HakuG Posted at: 2016-05-29T05:33:26.222Z Reads: 101

```
Hi everyone!

Thanks for everyone who answered questions in my previous thread. It really helped me today when I was deciding on parts.

Deck:
[Bamboo Longboard](http://www.amazon.com/SCSK8-Bamboo-kicktail-Longboard-Skateboard/dp/B004URTVBI/ref=sr_1_1?s=sporting-goods&ie=UTF8&qid=1464487389&sr=8-1&keywords=blank+longboard+deck)

Trucks and Wheels: 
[83mm Wheels with 180mm trucks](http://www.amazon.com/Longboard-Trucks-Flywheels-Owlsome-Bearings/dp/B01B08HCLA/ref=sr_1_4?ie=UTF8&qid=1464487701&sr=8-4&keywords=83mm+wheels)

Motor Mount:
Built myself (Advice from those who have done this with CNC mills or whatever is greatly appreciated)

Drive Train 
[38 Teeth Large Pulley](http://shop.sdp-si.com/catalog/product/?id=A_6A55M014DF1506)
[14 Teeth Small Pulley](http://shop.sdp-si.com/catalog/product/?id=A_6A55M038NF1512)
[60 Teeth Belt](http://shop.sdp-si.com/catalog/product/?id=A_6R55M060150)

Motor
[SK3_6354_260kv Brushless Outrunner Motor](http://www.hobbyking.com/hobbyking/store/__18127__Turnigy_Aerodrive_SK3_6354_260kv_Brushless_Outrunner_Motor.html) (Alternatives welcome. These are currently in backorder =/)

ESC
**I could really use someone's help between deciding between this [Turnigy one](http://www.hobbyking.com/hobbyking/store/__17982__Turnigy_dlux_120A_HV_Brushless_Speed_Controller_OPTO_.html) and this [HobbyKing YEP one](http://www.hobbyking.com/hobbyking/store/__20696__HobbyKing_YEP_120A_HV_4_14S_Brushless_Speed_Controller_OPTO.html)**

Remote

Bluetooth Arduino (Also wouldn't mind someone who's hooked up their phone to this)

Batteries
[3 x 3S LiPo Batteries](http://www.amazon.com/ZIPPY-Flightmax-5000mAh-3S1P-20C/dp/B0072ADJ4K/ref=sr_1_4?ie=UTF8&qid=1464490651&sr=8-4&keywords=3S+5000mah+20C+lipo+battery)

Enclosure
Not quite sure yet, but probably just a walmart box

Charger and Power Supply
**I would also love some help as to which chargers to get and how to hook it up. People keep talking about "balance charging", but I'm rather clueless to what that means and how I can set that up.**

Thanks,
Harnek
```

---
## \#2 Posted by: Jinra Posted at: 2016-05-29T06:01:37.557Z Reads: 85

```
You may want to get a larger motor (perhaps 6372) if you're going single drive for the additional power for hills. Balance charging is the process of balancing out your cells while charging. The [Imax B6](http://www.hobbyking.com/hobbyking/store/RC_PRODUCT_SEARCH.asp?strSearch=imax+b6) is a pretty popular lipo balance charger. You'll want to balance charge to avoid overcharging certain cells in a series.
```

---
## \#3 Posted by: karma Posted at: 2016-05-29T09:27:35.384Z Reads: 80

```
I agree, I use the Imax B6 V2 and it's great. With the [V2](http://www.hobbyking.com/hobbyking/store/RC_PRODUCT_SEARCH.asp?strSearch=Imax+b6+V2) you don't need a power supply, just plug it into the wall. 

If you want to learn about how balance chargers work and why you should use them, check [this](https://www.youtube.com/watch?v=wIbHLacozFo) video out.
```

---
## \#4 Posted by: karma Posted at: 2016-05-29T09:38:31.381Z Reads: 77

```
I think your motor has a high KV rating and will result in a high top speed when running on 9S. ([calculated](http://toddy616.blogspot.se/2013/07/electric-skateboard-calculator.html) with this) I would say go for a lower kv motor to get more torque, maybe 200 or 220. [These](http://www.ollinboardcompany.com/category/brushless-motors) motors from chaka seems nice, haven't tried them yet but they should do wonders. The [r-spec motors](product/torqueboards-12s-120a-car-esc-opto-hv/) from enertion is also a beast. 

If your budget is over $100 for an ESC I would say go for a[ tested ESC](product/single-motor-120a-6s-esc/) like torqueboards. Remember to pick a programming card if you want to tweak the settings! If you are really interested in tweaking with your ESC you could get a [VESC](http://www.ollinboardcompany.com/product/vedder-s-speed-controller) but it might be over your budget.
```

---
## \#5 Posted by: HakuG Posted at: 2016-05-29T17:14:30.680Z Reads: 65

```
I think the tested ESC one doesn't handle higher voltages tho, right? the VESC was a little too pricey for my budget =/ and the VESC on enertion boards won't be coming in until Julyish, so I'm kinda hesitant.
```

---
## \#6 Posted by: karma Posted at: 2016-05-29T18:19:00.133Z Reads: 60

```
Oh right you were running 3 x 3S, I updated the link to the right one, check it out.
```

---
## \#7 Posted by: jakobnator Posted at: 2016-05-29T22:32:45.697Z Reads: 55

```
I have a very similar build
http://www.electric-skateboard.builders/t/basic-bamboo-scsk8-bamboo-kicktail-yocaher-trucks-turnigy-6364-245kv-custom-welded-6s-3sx2-zippy-fvt-esc/1669

The mount was pretty difficult to get just right considering how expensive CNC can be. When welding the mount it is difficult on those trucks to get perfectly square because they aren't cylindrical and they are tapered. 

For the ESC, honestly just get the VESC I tried the chinese RC Car ESCs but if your going to spend the money just get the one that is made for eboards.
```

---
## \#8 Posted by: HakuG Posted at: 2016-05-29T22:59:41.955Z Reads: 53

```
How was the board you used? Also, you said you 3-D printed the belt, but did you also do the same with the pulleys?
```

---
## \#9 Posted by: HakuG Posted at: 2016-05-29T23:25:54.316Z Reads: 55

```
Also, one question about chargers, @karma
Say I use a 10S4P battery. Although the V2 power supply says I can only go up until 6S, because each cell is around 2.5S and I plan on charging it in parallel, will it still function? 

Thanks,
Harnek
```

---
## \#10 Posted by: jakobnator Posted at: 2016-05-29T23:40:09.828Z Reads: 52

```
Board is great, one or two of the plys isn't bamboo so it has some stiffness, but it flexes a bit under my weight (245 lbs). I 3D printed the drive gear because I couldn't for the life of me drill the holes perfectly centered to make a metal one. ABS gears work great no visible wear as of now. The motor gear is metal, and the belt is from that website you are looking at pullies from. Honestly you can save money by buying the smaller pulley and belt on ebay.
```

---
## \#11 Posted by: karma Posted at: 2016-05-30T08:07:41.591Z Reads: 41

```
Since I assume that you are going to connect the batteries with 4mm bullet connectors and not  solder/weld the packs together you can charge them separately. Watch [this](https://www.youtube.com/watch?v=w8ijfcjU-rc) video for charging a LiPo battery with the Imax B6. You can also parallell charge the batteries with a  [paraboard](http://www.hobbyking.com/hobbyking/store/__14856__HobbyKing_Parallel_charging_Board_for_6_packs_2_6S_XT_60_.html) if the batteries have the same capacity & cell count. Hope this makes sense.
```

---

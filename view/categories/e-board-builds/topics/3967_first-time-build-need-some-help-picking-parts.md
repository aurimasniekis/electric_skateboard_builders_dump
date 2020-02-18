# First time build! Need some help picking parts

### Replies: 14 Views: 1429

## \#1 Posted by: NickTheDude Posted at: 2016-05-29T07:52:53.090Z Reads: 112

```
Hey guys, this is my first time building anything like this, and prior to the couple days of researching I've done, I have no experience or knowledge of ESC's motors, batteries and the like. However, after much thought and research I've come up with this list.

2x [5000mAh S4 25C Compact Batteries](http://www.hobbyking.com/hobbyking/store/__21371__ZIPPY_Compact_5000mAh_4S_25C_Lipo_Pack.html)
1x [6374 192kV Motor](http://www.hobbyking.com/hobbyking/store/__18129__Turnigy_Aerodrive_SK3_6374_192kv_Brushless_Outrunner_Motor.html)
1x [2.4Ghz Transmitter/Receiver](http://www.hobbyking.com/hobbyking/store/__44693__Quanum_2_4Ghz_3ch_Pistol_Grip_Tx_Rx_System.html)
1x [Turnigy Sentilon V4 100A Speed Controller](http://www.hobbyking.com/hobbyking/store/__38787__Turnigy_Sentilon_V4_100A_5_12s_HV_Bulletproof_Speed_Controller_w_RPM_Sensor.html)


And from what I understand I am going to need a BEC with the ESC as well. I'm planning on 3D printing 36T/16T pulleys, buying a belt and making my own mount. The board I'm using is a [Madrid P-Cock](https://images-na.ssl-images-amazon.com/images/I/61eNW-hOo5L._SL1000_.jpg) and it is pretty low to the ground so I will have to mount the motor so that it sticks out the back.

That's my plan, if I've missed anything please let me know and I would love to hear any suggestions. Thanks!
```

---
## \#2 Posted by: karma Posted at: 2016-05-29T09:26:33.529Z Reads: 108

```
The batteries and motor seem good. If you want an alternative I would look at [these](http://www.ollinboardcompany.com/category/brushless-motors) motors from chaka (ollinboardcompay). I would strongly recommend not using that transmitter because I have heard some bad reviews on it, seems to break within a weak of use. I would either go with the [Wiiciever and Nyko Kama combo](product-category/wireless-wii-nunchuck/) or the [GT2B](product/torqueboards-2-4ghz-mini-remote-controller/). I have never seen someone use that ESC and would suggest you get[ this one](product/torqueboards-12s-120a-car-esc-opto-hv/) instead. You will  need a [separate UBEC](product/12s-ubec/)/SBEC. Would suggest picking up a programming card so that you can tweak the settings. You'll also need a balance charger to charge your batteries, like [this](http://www.hobbyking.com/hobbyking/store/__58285__IMAX_B6AC_V2_Professional_Balance_Charger_Discharger.html) one.
```

---
## \#3 Posted by: Michaelinvegas Posted at: 2016-05-29T09:55:04.739Z Reads: 105

```
Let me add to @karma...

It looks like ur running 8s ... 

I would check this thread for an 8s or more esc 

http://www.electric-skateboard.builders/t/new-builder-list-of-known-and-commonly-used-parts/2983?u=michaelinvegas

Electronic Speed Controllers

VESC 50a 12s
DIY's 120a 12s
FVT 120a 6s
FVT 180a 6s
Castle Mamba Monster2 6s
Castle XL2 8s
Hobywing EzRun MAX8 6s
Hobywing EzRun MAX5 200a 8s
Hobywing EzRun MAX6 160a 8s
Hobbywing XeRun XR8 Plus 6s

This one I think is for a helicopter or plane

[quote="NickTheDude, post:1, topic:3967"]
1x Turnigy Sentilon V4 100A Speed Controller
[/quote]
```

---
## \#4 Posted by: karma Posted at: 2016-05-29T10:54:03.748Z Reads: 80

```
Thanks for pointing that out! Thought it said 3S for some reason... Updated my post.
```

---
## \#5 Posted by: NickTheDude Posted at: 2016-05-29T17:06:47.634Z Reads: 72

```
Thanks guys! So the issues is that I live in Canada and I'm trying to keep this as cheap as possible, so I'd like to be able to order all my parts from one source to avoid extra shipping costs and the VESC is very expensive on top of that. So, I looked through the hobbyking catalog for an ESC that would work with my setup but I can't seem to find a car ESC that suits my needs, could you guys take a look? Otherwise do you know of any hobbyking alternatives that I could find an ESC and parts similar to the ones listed? Thanks!
```

---
## \#6 Posted by: HakuG Posted at: 2016-05-29T17:11:59.229Z Reads: 69

```
I think these two fit the specs:
[120A Turnigy](http://www.hobbyking.com/hobbyking/store/__17982__Turnigy_dlux_120A_HV_Brushless_Speed_Controller_OPTO_.html)

and

[120A HobbyKing YEP](http://www.hobbyking.com/hobbyking/store/__20696__HobbyKing_YEP_120A_HV_4_14S_Brushless_Speed_Controller_OPTO.html)

But I'd love a confirmation
```

---
## \#7 Posted by: NickTheDude Posted at: 2016-05-29T17:21:48.676Z Reads: 69

```
That's what I was thinking as well, but apparently their meant for RC planes/helicopters. Can these be programmed to be used with a longboard?
```

---
## \#8 Posted by: Jinra Posted at: 2016-05-29T18:27:59.954Z Reads: 65

```
you probably don't want to print motor pulleys, wheel should be fine.
```

---
## \#9 Posted by: Michaelinvegas Posted at: 2016-05-29T18:31:34.320Z Reads: 69

```
I'd use caution picking out an esc that no one has tried ... Especially if it's your first build....try to stick with known products first to avoid added expense in getting the wrong esc and wasting time waiting to get the right thing....

Finding a compatible esc for 6s is easy....the trick is finding ESCs that are 7s to 12s that will work for our application....they do have ESCs for cars that are 12s but you are looking at the $150-$200 range for these types of ESCs.... Best so far seems to be vesc and the TB or carvon ESCs that can handle up to 12s

The majority of the ESCs that are 12s are for helicopters, planes and boats
```

---
## \#10 Posted by: NickTheDude Posted at: 2016-05-29T23:13:24.435Z Reads: 67

```
Okay, so I've revised my plan a little bit, I've decided to go with a 6354 260kV motor so that I could potentially upgrade to a dual motor setup in the future if I want to, it also brings the cost down a little. With this I'll go with 2 4S batteries in series and a 36:14 ratio. This should theoretically give me a top speed of around 30mph. So, does anyone have experience with the 54mm motors? Are they low on torque? Would I be able to fit 2 64mm motors beside eachother on a 180mm paris truck? Also, if I got an ESC rated for 2S-6S, what kind of effect would it have with a 8S setup? [This is the one](http://www.hobbyking.com/hobbyking/store/__77144__HobbyKing_174_8482_X_Car_Beast_Series_ESC_1_8_Scale_120A.html) I was thinking of getting. Thanks again for all the help guys.
```

---
## \#11 Posted by: Michaelinvegas Posted at: 2016-05-29T23:28:13.126Z Reads: 60

```
KV numbers will tell the torque...not the size of the motor
```

---
## \#12 Posted by: NickTheDude Posted at: 2016-05-29T23:41:42.578Z Reads: 59

```
So what exactly does having a longer motor do?
```

---
## \#13 Posted by: Namasaki Posted at: 2016-05-29T23:44:50.123Z Reads: 58

```
Hey Nick, in case your new to Hobby King. I have a good tip for you. Go to the item you want and just sit on the page until they pop up a discount offer window. It may take a little while but they do it and you'll save some money.
It's also a good idea to create an account so that you can track your order on their site.
```

---
## \#14 Posted by: NickTheDude Posted at: 2016-05-30T00:21:22.194Z Reads: 56

```
Alright, since the only 8S car ESC on hobbyking is 125$ without the BEC and programming card I think I will go with 2 3S batteries in series, the ESC i linked a couple posts above and a 6354 260kV motor with a 2:1 ratio which should give me the same top speed but less torque. Because of this I'll likely go for dual motors in the future if need be, but right now this is looking like the way to go on my budget.

Also, I was wondering if something like a 1.6:1 gear ratio with dual 260kV motors and 6S batteries would be a good setup. Since I would be getting more torque from the dual motors would it make sense to alter the gear ratio like that in order to get higher top speed?
```

---

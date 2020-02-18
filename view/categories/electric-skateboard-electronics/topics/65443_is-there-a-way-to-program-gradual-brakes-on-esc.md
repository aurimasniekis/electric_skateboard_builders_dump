# Is there a way to program gradual brakes on ESC?

### Replies: 7 Views: 893

## \#1 Posted by: freddyfred01 Posted at: 2018-08-20T07:33:47.185Z Reads: 109

```
I have a HobbyWing Skywalker 80A UBEC ESC but the braking is extremely sudden and only comes on when power is not applied. Ideally I would like to coast with no power on and push the trigger up to brake. The motor also seems to jump very suddenly in rpm at about half throttle. Is this because of the ESC or transmitter.
If anyone could help that'd be great thanks.

Motor:
https://www.ebay.com.au/itm/270KV-N5065-5065-Brushless-Motor-For-DIY-Electric-Skateboard-Scooter-Multicopter/292136737913?hash=item4404b4dc79:g:7cEAAOSwbc5awdn1
ESC:
https://www.ebay.com.au/itm/Hobbywing-QSKYWALKER-80A-ESC-Speed-Controller-with-BEC-for-Multicopter-N6E0/112973277761?epid=3013225999&hash=item1a4dbb6a41:g:5FMAAOSwfEVaxEWo
Transmitter/receiver:
https://www.ebay.com.au/itm/2-4GHz-Receiver-Binding-Plug-Radio-Remote-Controller-For-Electric-Skateboard-NEW/173252792888?epid=14017556542&hash=item2856abd238:g:P6kAAOSwWxNaxHSo
```

---
## \#2 Posted by: bigben Posted at: 2018-08-20T07:49:12.891Z Reads: 95

```
Likely to be the esc. There are a lot of more reasonable VESC type controllers out there now.
I'd invest in one of those and steer clear of escs that aren't made for this. One esc I and others have had some success with is the FVT150.
```

---
## \#3 Posted by: slick Posted at: 2018-08-20T12:38:50.712Z Reads: 70

```
It sounds like your ESC has drag brakes. I found this program card but your ESC does not seem to have programmable brake options.

http://www.hobbywing.com/goods.php?id=373&filter_attr=

Maybe theres a LCD program box for your ESC than will enable you to adjust brakes. If I were you and I hate to sound like any other VESC user in the forum _but_ I suggest you get yourself a VESC of your choice since it´s the safer option. I used an ESC with *only* drag brakes and it´s not that fun. No coasting and worse - pretty dangerous since you cant apply braking force proportionaly. 

Even the cheapest VESC-variant is better than what you currently have...more important is the safty of proper working brakes.
```

---
## \#4 Posted by: freddyfred01 Posted at: 2018-08-20T12:58:13.118Z Reads: 56

```
Yeah that sounds right. If only has an on/off for brakes.
What’s the cheapest suitable VESC for my 6S board that you would recommend. I’m not too familiar with VESCs so I went with a cheap 30AUD ESC.
I’m on a very tight budget and I’m Australia 
Thanks so much for you help
```

---
## \#5 Posted by: slick Posted at: 2018-08-20T13:39:47.868Z Reads: 51

```
Sure, no problem.

the cheapest one I know of and own is the one from Hobbyking. I´ve been running on it on FOC since day 1 with no problems. I´ve tried an SK3 5065 280kv and 236kv - both with no problems at all. Plus, it has a 1 year warranty - so you´re covered pretty well (especially when you´re on a budget). And of course - China aint so far away...so you should´nt be waiting too long for your VESC.

Once you have the VESC it´s important to configure it via PC. You´ll have to download the **[VESC TOOL](https://vesc-project.com/vesc_tool)** (you´ll need an account on thier site first) to configure your setup (motor, 
remote control...etc) You´ll only need to do this once until you change anything in your setp. If you do change anything, you´ll have to configure your new setup before you hit the road.

I recommend you read the VESC thread in the forum while you´re waiting...it´s a lot to digest but you´ll get it soon enough...
```

---
## \#6 Posted by: freddyfred01 Posted at: 2018-08-21T07:17:05.051Z Reads: 31

```
[quote="slick, post:5, topic:65443"]
SK3 5065 280kv
[/quote]

Would you be able to link me one. I’ve had trouble searching them and only found them for $100AUD + which is way too expensive for me. Something around $60AUD would be suitable.
Thanks again
```

---
## \#7 Posted by: slick Posted at: 2018-08-21T07:29:47.001Z Reads: 31

```
sk3 5065 275kv
https://hobbyking.com/de_de/turnigy-aerodrive-sk3-5065-275kv-brushless-outrunner-motor.html?___store=de_de

this was the one i meant. im light at 72kg and it has decent performance with 3:1 and 2.4:1 gearing. i had it running on 8s lipo.
```

---

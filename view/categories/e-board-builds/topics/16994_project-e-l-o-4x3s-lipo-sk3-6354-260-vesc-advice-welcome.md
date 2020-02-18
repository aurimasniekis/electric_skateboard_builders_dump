# Project E.L.O - &#124; 4x3s LiPo &#124; SK3 6354-260 &#124; VESC? &#124; -Advice welcome-

### Replies: 19 Views: 2769

## \#1 Posted by: Tenho2 Posted at: 2017-01-31T20:58:58.842Z Reads: 188

```
Hi!

I'm building my first electric skateboard and before starting the real build blog i wanted to ask some advice from the wiser guys in here. :slight_smile:

My plan is to make a skateboard with  a nice (15km+/9.32ml) range, i dont care for the top speed that much atleast for now.
I can always change the gearing/motor/ or something if, say a top speed of 20km/h(12.42ml) doesn't feel quite enough.

The parts i have picked for my project, and which i actually could use some advice are as follows:

-Motor- Turnigy Aerodrive SK3 - 6354-260kv
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6354-260kv-brushless-outrunner-motor.html

-Battery- 4 X Turnigy 5000mAh 3S 20C Lipo Pack - making 6s 10 000 mAh total
https://hobbyking.com/en_us/turnigy-5000mah-3s-20c-lipo-pack.html-Controller

-Radio- Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System - smallest i could find in the price range
https://hobbyking.com/en_us/quanum-2-4ghz-3ch-pistol-grip-tx-rx-system.html

-VESC-

-Drive system- I'm trying to find the cheapest wheels(maybe 70 or 80mm) and the cheapest motormount and pulley's combo from eBay. Motormount and pulley set's as a combo go for about 20-25€ and a set of wheels about the same.

Edit: Scratch the cheap motormount idea, they are all for 50xx series motors and will not fit the 6354 series motor i was planning.
Would 50xx series motor have enough torque?
They are a bit cheaper at Hobbyking


Should i go with maybe a slighty lower kv motor? I'm currently about 80kg(176.36 pounds), i'm trying to lose a few kilogram's, but let's not trust it will actually happen before summer. :slight_smile:
 
VESC - Are they all the same? Some advertise having double thickness in the traces and there is the new X model which has 60A of continous current capasity, but those are a bit too expensive.

http://www.michobby.com/product/vedder-vesc-speed-controller/
https://www.proto-boards.com/product-page/vesc-speed-controller
http://www.hellray.de/vesc/

If i remember correctly these are the two cheapest options available from european vendors + the cheapest i have found from anywhere. Cheapest complete one that is, I found some half way done but i would really want to hand solder tiny SMD chip's 0805 size components are ok, but haven't done smaller than that.
Are all of these equal to each other or is one better that the other in some other way than price too?

The specs are same in all of them but, maybe if someone has some experience from one of these?
I do understand that buying the cheapest chinese one might not be the safest bet but still.
Even with the tax and customs duty it comes about 50€ cheaper than the one from germany (which i actually almost bought already)


Am i taking a big risk going with a 6s battery over an 8s?

I was originally going to buy just an ESC
HobbyKing® ™ X-Car Beast Series ESC 1:8 Scale 120A
https://hobbyking.com/en_us/hobbykingr-tm-x-car-beast-series-esc-1-8-scale-120a.html

But after doing my research i have come to the conclusion  VESC is far superior to a normal RC car ESC?
Is the regenerative braking in VESC something that really is usefull and extends your range or is it just more of an novelty feature? I know it depends on the "hilliness", but still.

Going for the car ESC would save me about 70-120€, that's a lot of ice cream and hotdog's while riding my new electric board around the town...

For the power switch i was going to use XT90 antispark connectors, like many have here.
Fusing? I have only seen fuse's used with the anti spark switch.
Finding a good rubber cover for the exposed XT in the bottom of the board seem's suprisingly hard.

I'm adding a few more features and options to the board, but since this build log hasn't "officially started" yet i'm not going into too much detail about those.
Everything together (motor, battery pack's, radio, VESC, some XT90 connectors, some with anti spark and some 10 AWG silicon wire the total is 400-450€, wouldn't really want to go much more than that.

Thank you very much if you actually took the time and read all the way thru!
Special thanks to everyone who has some advice to my setup! 

Greetings!
Tenho2
Finland
```

---
## \#2 Posted by: Smorto Posted at: 2017-01-31T21:05:46.231Z Reads: 156

```
[quote="Tenho2, post:1, topic:16994"]
-Radio- Quanum 2.4Ghz 3ch Pistol Grip Tx & Rx System
[/quote]


First thing I see is getting a GT2B for around the same price. The Quanum seems to drop out sometimes while the GT2B is rock solid. I would also recommend a lower kv motor maybe something around 200 but that is just my opinion. You are also missing trucks, Caliber II 50 degrees are the norm around here. Another benefit of the VESC is that if you treat it well it will outlast and far outperform any hobby ESC. Just a thought. Thats all I can see for now, good luck in your build.
```

---
## \#3 Posted by: Tenho2 Posted at: 2017-01-31T21:15:40.926Z Reads: 155

```
Thank you for the advice Smorto!

I too have heard some mixed reviews from the Quanum, only reason i'm considering it is the size and looks since i don't have a 3D printed to make the modded case for the GT2B. But the fact that pretty much everyone is using the GT2B radio might tell i should too. :slight_smile:

I'm trying to find something with a slightly lower kv and think about it for sure.
I'm not sure if the 264kv motor has enough torque to haul my fat bum.

I'm propably going to use my old Fox trucks and my Powel Minilogo deck if i dont find a decent longboard second hand.

I have heard some horror stories about VESC's burning, but ofcourse i realize that could surely happen to the hobby ESC too. Hobby ESC's are just a bit more affordable to burn. In some case's.

Thank you again for the advice, i'll look in to it and do some more research. :)

Greetings!
Tenho2
```

---
## \#4 Posted by: Smorto Posted at: 2017-01-31T21:33:10.236Z Reads: 145

```
No problem. Trust me, getting the GT2B and having it be a bit ugly but being safe is much better than getting the quanam and ending up with a nasty injury :slight_smile:.  I'd say 90% of the VESCs burning is due to user error or not knowing the limits, if you get a quality VESC and treat it correctly it should not burn. I don't know about those trucks but if you can get the motor mount to fit to them them great.
```

---
## \#5 Posted by: okp Posted at: 2017-01-31T21:56:12.875Z Reads: 137

```
We also have VESCs and are in Paris :slight_smile: 

http://www.unikboards.com/en/boutique/vesc-v/

you should go for a GT2B with my mod :slight_smile:

happy building!
```

---
## \#6 Posted by: Tenho2 Posted at: 2017-01-31T22:26:07.295Z Reads: 120

```
That is very much true. No fun having a cool skateboard when your yaw is in two pieces. :)

Dab of electric glue will do miracles. :)
```

---
## \#7 Posted by: Smorto Posted at: 2017-01-31T22:37:35.655Z Reads: 121

```
What do you mean about the electric glue?
```

---
## \#8 Posted by: Tenho2 Posted at: 2017-01-31T22:38:23.250Z Reads: 129

```
Hi!

Thanks for the advice! :slight_smile:
I believe i did visit your shop few hours ago dont know why i didn't mention it as a an option. :) 
I'm sorry for that.
Are you going to run an amazing discount on VESC's soon? ;)

Was it the 3D printed case mod that everyone seems to use? I have read and seen pictures from those. Didn't find one from the store thought?
Well my eyes are pretty much useless after 10 hours of looking into my laptop's screen. :D
```

---
## \#9 Posted by: Tenho2 Posted at: 2017-01-31T22:38:49.223Z Reads: 128

```
Tig welding. :)
```

---
## \#10 Posted by: Smorto Posted at: 2017-01-31T22:40:30.983Z Reads: 127

```
Im still confused lol, what will you be big welding an why?
```

---
## \#11 Posted by: Tenho2 Posted at: 2017-01-31T22:43:28.185Z Reads: 131

```
T not a B. ;)
https://m.youtube.com/watch?v=K3NTAuDjuYA

I mean welding the motormount to the truck. :)
```

---
## \#12 Posted by: Smorto Posted at: 2017-01-31T22:46:06.672Z Reads: 128

```
Ahhhh I see thought you were still talking about the quanam remote lol. Hahaha about the "big welding" it auto corrected.
```

---
## \#13 Posted by: Tenho2 Posted at: 2017-01-31T22:49:51.296Z Reads: 122

```
Oh! :smiley:
Well i should have made myself more  clearer.
Pretty tired after researching parts for my skateboard the whole day. :D
```

---
## \#14 Posted by: Tenho2 Posted at: 2017-02-02T16:16:25.551Z Reads: 94

```
Ok. I have done a bit more research and i might go with this motor instead of the 260kv.
https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6364-190kv-brushless-outrunner-motor.html

Now i just need to find a motormount, which is a lot harder than i thought. Maybe i'll just craft my own from a block of aluminium.

Also i might go with sprocket's and chain instead of the more commonly used pulley's and belt setup.

Greetings!
Tenho2
```

---
## \#15 Posted by: Tuomalar Posted at: 2017-02-02T16:24:50.457Z Reads: 90

```
What trucks you're going to use? 

Ps. Moro
```

---
## \#16 Posted by: Tenho2 Posted at: 2017-02-02T16:54:14.395Z Reads: 86

```
No moro moro! :slight_smile:

I'm propably going to use a pair of old Fox trukcs i have on my skateboard. The axle support is Perttu much round so i have to weld the motormount to keep it in place. Or i find a used longboard since my skateboard has 50mm wheels that have some wear already and to be able to use even 70mm wheels i might need spacer's anyway.

Market's for used longboards ain't that great at the moment so one option i have been considering also is to get the cheapest trucks and wheels combo from eBay around 40€.

Greetings!
Tenho2
```

---
## \#17 Posted by: Tenho2 Posted at: 2017-02-07T10:17:05.960Z Reads: 73

```
Small updates.

GT2B controller is out of the equation, atleast for now. The shipping costs only would be 50$ from the Hong Kong warehouse plus tax and custom fee's.

Most of the other parts are also unavailable from the EU warehouse of Hobby King so I need to wait them to restock.

Does anyone know where to get a motormount for the 6354 series motor? All the cheap one's in eBay are for 50xx motors.
I might need to make it myself.
Or would 50xx series motor have enough torque?
I have seen many people use them so maybe that's an alternative.

Greetings!
Tenho2
```

---
## \#18 Posted by: Tuomalar Posted at: 2017-02-07T10:47:38.781Z Reads: 71

```
I do have 2 enertion lookalike motor mounts from groupbuy. Located in Finland.
```

---
## \#19 Posted by: Tenho2 Posted at: 2017-02-07T12:29:52.753Z Reads: 68

```
Superb! I'm sending you a pm. :slight_smile:

Greetings!
Tenho2
```

---

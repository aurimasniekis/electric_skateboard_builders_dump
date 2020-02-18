# Help! College Student First Electric Longboard Build

### Replies: 20 Views: 371

## \#1 Posted by: FlyingPoptart Posted at: 2019-12-26T14:31:13.413Z Reads: 87

```
Hello everyone, I'm new at this forum. I heard about electric longboarding and, as I need to figure out if I want to continue learning electrical engineering (and also getting an electric longboard of my own),  I decided I wanted to build my own. I'm a student going to university (if anyone else goes to UMass Amherst, hi) so I have pretty specific needs, namely that I will prioritize weight and cost over top speed and range. I would be happy with a top speed of 15 mph--anything higher and I would be a danger to myself and my classmates. Furthermore, there is one hill on campus notorious for how steep it is, so I also want to prioritize hill climbing abilities.

My ultimate goal is to convert my foldable boardup longboard into an electric version.

----- Parts -----

I did a lot of research and wanted to get feedback on whether the parts I want to use.

Although I don't have much experience, I want to create my own battery. I wish to use these cells in a 6s3p combination with this BMS.
https://eu.nkon.nl/rechargeable/li-ion/18650-size/samsung-inr-18650-30q-3000mah.html
https://www.aliexpress.com/item/32955184179.html?spm=a2g0o.productlist.0.0.4aa67cd81IiQ4L&algo_pvid=090f9fd8-622e-4c4f-98e4-bba965369788&algo_expid=090f9fd8-622e-4c4f-98e4-bba965369788-1&btsid=914e531d-c74f-4f8d-bb52-0f9308d112af&ws_ab_test=searchweb0_0,searchweb201602_5,searchweb201603_53

I also want to use two of these motors. I found it really cheap on taobao. Here's the link but it's in Chinese, so I translated and copy and pasted the specs here.
https://item.taobao.com/item.htm?spm=a1z0d.7625083.1998302264.5.5c5f4e69kk4ENj&id=558189099368
6354 Dimensions:
Output shaft diameter: 10mm
Shaft: Flat shaft
output shaft length: 30mm
weight: 554g
KV: 180KV
Power: 1500W
Voltage: 24V
No-load speed: 4350 rpm
No-load current: 1.1A
Number of Poles: 14
Torque: 4N / m

I'm assuming that this truck would be able to fit two of these motors in a dual motor setup.
https://www.amazon.com/Caliber-Trucks-Cal-44%C2%B0-Longboard/dp/B00NY426YW

I plan to use this charger
https:///collections/battery-chargers/products/6s-epower-pack-4a-charger#description

My VESC will be two of these. I know lots of people use dual ESCs, but I'm afraid I'll burn one out by accident, so this kinda gives me two chances at screwing up rather than one.
https://flipsky.net/collections/electronic-products/products/mini-fsesc4-20-50a-base-on-vesc-widely-used-in-eskateboard-escooter-ebike

Although there are a few more parts I need to decide on, I figure these are the biggest ones and the ones that I should be most concerned about. 

----- Questions -----

My first biggest question (apologizes if this was already answered, I just had to make sure), is selecting the right current for the BMS. I read somewhere that the BMS should have be rated at half the maximum discharge rate of the battery so the battery doesn't wear down fast, so considering three Samsung 30q batteries with a discharge rate of 15A each, that adds up to 45A total discharge rate, meaning that my BMS should be rated at around 20A. Is that correct?

Second, different 6354 BLDC motors have ratings between 1500W and 2500W. Does that number indicate maximum power output?

Third, what does the shaft length of a motor mean? Some manufacturers offer the choice between 8mm and 10mm but I'm not sure what the difference is and if I should choose one over the other.

Fourth, I wanted to know if the built in heat sink in the VESC would be enough to keep the VESC cool assuming I 3D print an enclosure with no windows (I still need to do some research on the materials for that). 

Fifth, is dual 6354 motors enough for hill climbing? I would like someone to check me on my physics Assuming a total load of 90kg with my board, my backpack, and myself, 100mm wheels and 25% hill grade, the torque to keep me at a constant velocity would be F * r = sin(arctan(.25))*m*g*(d/2), which is 10.7 N*m. Torque is the rotational analogue of acceleration, so the approximate 5 N*m of torque fudge factor would theoretically be able to push me up the hill from a dead stop. To go up a hill at 8 m/s, the power delivered by my motors need to be F * v = sin(arctan(.25))*m*g*|v|, giving me 1711W. 
Assuming that this website below is right in calculating the maximum torque, I have enough torque to push me up the hill with some fudge factor left over. Furthermore, 1711W dissipated across two 1500 watt motors (totaling 3000w) should be enough to keep me going up the hill at a decent velocity. This means that my setup should be enough to push me up that hill. Is my physics and line of thinking right?
https://calc.3dservisas.eu/?Tc8xD8IgEAXg_8JsmsNCq65onDQkTexuO2AilqSj8b_LexDj9t1x94C3urugDur5WF5qk4trLtqmy17dkF3k0aUcJCIsjqj6xpYCQ7ocMFNnpqFupr_F5NE1FJa2ELNaS6LZkb-gKbiaNIVT1k7IG9YNHF1NigjXPI9-gQ0JWSmjbGN4Hle-uofPF86QI27D52fcthf1-QI=

Sixth, I wanted to know the influence current max current has on hill climbing ability. If I fudge around the numbers for the current running through each of the cells, the torque remains constant. That doesn't make sense. Shouldn't max torque be dependent on max current? At least, that's what some random threads I looked at said. Did I get something wrong? If torque isn't dependent on max current, that means I can reduce the weight and cost of my build by adopting a 6s2p battery configuration. Is there something I'm missing?

This post looks like it's a lot longer than I originally intended, so sorry for the wall of text. In any case,
I would appreciate any help I can get. Thank you and happy holidays!
```

---
## \#2 Posted by: Halbj613 Posted at: 2019-12-26T15:01:11.966Z Reads: 79

```
Hi so couple things I would change but overall decent

Step1: joint he other forum also esk8forum.news

Step2: most people now using 10s or 12s builds 6s is quite low and will not give you massive power

Step3: in regards to bms I don’t know who told you about the discharge rate but your bms should take the max amps you battery can put through, in your case 45amps

Step3: those motors are not exactly the bets they are cheap and probably won’t last very long. Also 1500w is very low for esk8
Top motor brands currently are maytech,flipsky,torqueboards (flipsky is pretty chela and good)

Motor shaft just means how wide the motor shaft is. Your motor pulley (on the drive train) will need to be the same width as the motor shaft

Generally 6355 will be easily powerful enough to take you up steep hills if you get some decent ones and can be further geared by changing pulley sizes

Watts me as the max output of the motor your battery will generally be the limiting factor but often not...
Amps x volts=watts... 45*24= around 1100watts

The trucks are fine but you need a mount and pulleys for them still.

A 3D printer enclosure will be fine but remember those vescs are decent but still cheap and not the most reliable on the market

If there is anything else you would like to know please ask
```

---
## \#3 Posted by: xjujo Posted at: 2019-12-26T15:35:43.392Z Reads: 70

```
Shit I need to go to college eventually
```

---
## \#4 Posted by: FlyingPoptart Posted at: 2019-12-28T11:15:45.066Z Reads: 61

```
Thank you so much! I still need to do some more research on mounts and pulleys and electrical connectors but I'll be sure to ask questions as they come up!
```

---
## \#5 Posted by: Halbj613 Posted at: 2019-12-28T17:25:40.856Z Reads: 54

```
Really though if you want good quality and swears and info’s join the other esk8 forum

Just search up esk8 news forum and it will come up
```

---
## \#6 Posted by: SkateYS Posted at: 2019-12-29T02:58:38.794Z Reads: 44

```
Welcome! I remember when I first started, I wanted something similar! And you know the feeling (want it slow, less torque, etc), but believe me, you will get bored quickly (good thing is, simple battery upgrade can fix that), if you live in a hilly area, consider better ESCs (if you are on a budget, then that's ok, but do a lot of research on VESC configuration, 6s voltage is low, so you motors will pull a lot of current in order to reach the power required to go uphill which means ESC is stressed and heat dissipation a vital). So if you can, use a higher voltage (10s maybe) and a high torque gear ratio (13t motor pulley & 36t wheel pulley). This will reduce the speed and increase your torque leading to less heat.
```

---
## \#7 Posted by: meesie Posted at: 2019-12-29T10:16:44.645Z Reads: 38

```
If you want to climb some hills your motors are okay, BUT, your battery will definetely not like it. I would recommend at least 10s3p for your situation. i read 25% hill grade somewhere? Thats a lot i think. I’m from the netherlands so the only hills i encounter are bridges and tunnels.

As for your vesc, i have two of these in one of my Builds:

€ 46,56  25％ Off | HGLRC FLIPSKY FSESC 50A V4.12 ESC Electronic Speed Control for Electric Skateboard RC Car Boat E-bike E-scooter Robot
https://s.click.aliexpress.com/e/oWQV7hgRp

The flipsky mini’s are rather unstable if i remember correctly and can’t handle loads and heat very well. This is the normal flipsky vesc and for me it works just fine. Even on 12s in FOC.

Oh, and consider sensored motors. With sensors you can get a smooth startup from standstill and in FOC mode (there’s a thread explaining this in detail) your motors run quieter.

For connectors everyone generally uses XT60, or XT90 if you’ve got very high amp draws. For you XT60 will be sufficient.

As one last tip, spend a little more on quality parts when you start out. I’ve completely rehauled my first build about 3 times because i wouldn’t buy the expensive quality stuff. Trust me, it’ll cost you more in the end.
```

---
## \#8 Posted by: FlyingPoptart Posted at: 2019-12-29T17:56:54.645Z Reads: 36

```
Thank you, I'll make sure to select a high torque gear ratio. I'll also use a higher voltage and maybe cap my speed for now. I don't want my controller to be too sensitive but I figure I could futureproof my board for when I might need to consider using it to commute to work.
```

---
## \#9 Posted by: FlyingPoptart Posted at: 2019-12-29T18:32:15.675Z Reads: 35

```
There isn't too many bad hills in my area. I'm currently on break so I can't really calculate the height of the hills so I don't really know if it's actually 25% grade, but it's notorious for being steep that in the summer you would sweat after climbing up it and in the winter people would warn you about not going down one part of the hill because it's too slippery and steep. 

I'll use sensored motors. Thank you for that suggestion.

I'll use a 10S3P battery because of the heat issue. I think that with the heatsink from the later versions and avoiding the minis, I won't have to worry too much about overheating, so that's reassuring. I'll probably use the dual flipsky VESC. 

It looks like XT60s are cheaper so I'll use that, but they come in packs of 5. I probably don't need it for the charging port, but using something else means I have to buy something else. I drew up this wiring diagram so could you take a look at it? I know the XT60 is a little overkill for the 3A or 4.5A of charging, but they come in packs of 5. I'm not sure where to place the 8A fuse for charging either. There's an anti-spark switch built in the VESC, and I think there is enough protection but I wanted to make sure. 

![PNG|690x420](upload://buzW1fbZCNMxgcf1cxmIOxzI93f.jpeg)
```

---
## \#10 Posted by: FlyingPoptart Posted at: 2019-12-29T18:37:07.109Z Reads: 30

```
[quote="meesie, post:7, topic:104938"]
If you want to climb some hills your motors are okay
[/quote]

Oh, and also I had a question about this. If I run 10s3p batteries, I get lower torque than 6s3p batteries in this calculator, and that doesn't make sense to me. Can you explain that to me?

https://calc.3dservisas.eu/?TZDBCsIwEET_JWeRxCZFvcbSkxIo2LvNIYK1gR7Ff3dnEsXb28fubDYvdfNJHdXjvjzVRoqLFM22FV79IGw0MUCTPEjrok-ojCuMnl3xzDSCeaiD-W8uB1hL4hCIUY0jQrbEX9CUfE2aUie018Qrxi149jVp5rMdXVjAllhsaaVGcxxXHgkd-_P3mtiP2IZviNh20Or9AQ==
```

---
## \#11 Posted by: meesie Posted at: 2019-12-29T19:37:03.926Z Reads: 32

```
Hmmmm, i don’t know how that works but that’s not correct. More voltage on same amperage = more watts = more power/torque.

Your diagram misses the antispark switch, and you’ve got 2 vescs. (Unless you drew a dual vesc lol)

Edit: just read your esc has a switch, ignore the latter about the switch
```

---
## \#12 Posted by: Rinze Posted at: 2019-12-29T21:30:28.430Z Reads: 33

```
Hi FlyingPoptart,

[quote="SkateYS, post:6, topic:104938"]
I wanted something similar! And you know the feeling (want it slow, less torque, etc), but believe me, you will get bored quickly
[/quote]

He is right, build something what you can expand later.

[quote="FlyingPoptart, post:9, topic:104938"]
There isn’t too many bad hills in my area. I’m currently on break so I can’t really calculate the height of the hills so I don’t really know if it’s actually 25% grade, but it’s notorious for being steep that in the summer you would sweat after climbing up it and in the winter people would warn you about not going down one part of the hill because it’s too slippery and steep.
[/quote]

I am not a professional in this, but I think it is better to bypass the BMS for braking safety. In other words, if you have to brake because you go down hill and the BMS turns off the power to protect your battery, then you have NO brakes.

I'm also building my own skateboard and maybe this can help you for some ideas.
Again, i'm not a professional, and i'm also still looking for the best steps, but for sure this can help you.
![Connections|290x500](upload://XD4xeS3v9eN7tYemOnhhIDQsES.jpeg)
```

---
## \#13 Posted by: SkateYS Posted at: 2019-12-29T22:28:47.458Z Reads: 31

```
[quote="Rinze, post:12, topic:104938"]
I think it is better to bypass the BMS for braking safety. In other words, if you have to brake because you go downhill and the BMS turns off the power to protect your battery, then you have NO brakes.
[/quote]

I'm glad you mentioned this! Unless he uses a very high amp charging BMS and doesn't charge his board to 100%, which is less likely, cut-offs will happen! No wonder some BMS, never really charge to 4.20v (usually 4.15v, some even 4.10v)
```

---
## \#14 Posted by: spork Posted at: 2020-01-06T06:45:17.861Z Reads: 20

```
[quote="FlyingPoptart, post:9, topic:104938"]
I’m currently on break so I can’t really calculate the height of the hills so I don’t really know if it’s actually 25% grade,
[/quote]

This is where Google Earth comes in handy.  I'm not familiar with UMass, but I popped it up on Google Earth.  I'm kind of guessing you're referring to Clark Hill Road?  If so, that appears to rise about 110' over about 1000' or about 11% grade.  If that's the wrong location, just tell me the street or address and I'll check it out.
```

---
## \#15 Posted by: spork Posted at: 2020-01-06T06:49:47.634Z Reads: 20

```
On a separate note... I built an off-road board with two VESC 4.12's, two 6364 BLDC motors, and two 6S 5AH packs (in parallel).  I've got mine geared for a top speed of 21 mph, and I feel like it climbs hills like a mountain goat without motors or ESC's getting hot.  I'm about to build a 2-wheeled road board, and I'll probably run 10S.

Of course folks are right that more volts means less amps for the same power.  The reason I went with 6S is because I'm running 10" pneumatic tires and I wanted a top design speed in the 20mph range.  So it was tough to put together a steep enough gear ratio for a bigger pack.
```

---
## \#16 Posted by: FlyingPoptart Posted at: 2020-01-06T07:27:34.593Z Reads: 17

```
Lovely! Thank you, I had no clue that google earth had elevation data. I approximated the hill grade of the highest hill I was most concerned about, which is about an average of 16% over 100m, which is a lot less than I expected.
```

---
## \#17 Posted by: spork Posted at: 2020-01-06T07:29:52.916Z Reads: 17

```
Cool.  16% is a healthy grade, but mine does that pretty nicely on 6S.

And I'm not trying to talk you into going with 6S.  Presumably you'll be using much smaller wheels, and it'll be easy to setup the gearing for 10S.
```

---
## \#18 Posted by: spork Posted at: 2020-01-06T07:33:59.820Z Reads: 19

```
Also, as an EE, you might find this interesting.  Shaman is designing a sort of an easier to build, and more robust VESC6.  Sounds like it's going to be fairly bullet proof and cheap.  It will be completely open-source.  Not quite out yet, but I think he's getting close.  Soon as it comes out I'll definitely be building one or two.

https://forum./t/cheap-focer-2-open-source-low-cost-vesc-6-based-esc-prototyped-materials-arrived-for-test-batch/13631/38
```

---
## \#19 Posted by: Halbj613 Posted at: 2020-01-06T21:15:39.913Z Reads: 16

```
Or on the other forum (forum esk8 news )

@jeffwuneo (he is not on here) is designing an awesome vesc6 which has been reverse engineered from the focbox

Great deal for a great vesc there
```

---
## \#20 Posted by: spork Posted at: 2020-01-06T21:29:40.289Z Reads: 19

```
Do you have a link?

Update:  here's the thread in question...

https://forum./t/neobox-open-source-focbox-variant-hw-6-design/12426

Just hours ago, they turned the first post of the thread into a wiki so it can be updated with info and status.  That should prevent everyone from having to read more than 1000 posts to figure out if this is something for them, and how to get one.  I don't see that the wiki has been updated yet, but I presume it will be shortly.   Exciting stuff!
```

---

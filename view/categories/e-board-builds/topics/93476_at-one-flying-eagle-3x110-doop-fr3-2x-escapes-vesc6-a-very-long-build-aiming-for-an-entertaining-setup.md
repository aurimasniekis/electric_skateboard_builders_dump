# AT-One &#124; Flying Eagle 3x110 / Doop FR3 &#124; 2x Escapes VESC6 &#124; A very long build aiming for an entertaining setup

### Replies: 22 Views: 1604

## \#1 Posted by: Vanarian Posted at: 2019-05-11T14:26:02.712Z Reads: 215

```
Well guys allow me to bring my first build topic on this forum. Some pretty awesome creations have popped up this week from @Rollertom and I hope you'll appreciate what I work on, despite not being finished !

So here is project AT-One, these are electric inline skates. What's already under the hood or being crafted to sneak under the hood : 
- 2x Escapes VESC6 (one per skate).
- DD in-wheel motors 85kv 50mm (well it's sorta hub, sorta not hub but it's really in the core of wheel so... DD in-wheel?) with 19awg high temp enamel copper inside + some hybrid experiments, it's pretty scalable so I'll post about it later.
- multi-platform frames... it sits super low while being able to mount on 165, 180, UFS and Trinity skating boots. Basically any boot can do except no cuff marathon ones which are 195mm, doesn't make sense with torquey electric skates (unless you wanna snap an ankle). It was a challenge making these agile with the bulky motors!
- I already have what I need to make a 8S4P battery of 18650 [LG cells](https://eu.nkon.nl/rechargeable/18650-size/lg-hb2-1500mah-30a.html) at home... I'm planning to jump at 12 or 13S instead (probably gonna sell my charger and BMS), eventually sell my new cells to get
[Samsung ones](https://eu.nkon.nl/rechargeable/18650-size/samsung-inr18650-20s-2000mah-30a.html) which are a direct upgrade at no space, discharge, temp or weight trade-off.
- No remote, it's not a longboard or a MTB... I need something intuitive yet with no delay. I don't want a "Zboard" feel either, so I'm exploring weird ideas with analog devices and arduino. 

Here's what it looks like in render (and at the end an IRL pic of what previous version looked like before being crushed in transport ; note that there already was a motor in the ABS frame mockup) : 

3x110 speed slalom/freeride type
https://i.imgur.com/23n57iN.jpg

https://i.imgur.com/bBcDTdA.jpg

4x80 freeride/street type (with a pretty H block)
https://i.imgur.com/bGhO8xe.jpg

Where I'm putting the batteries if you've been wondering (pic is not up to date but you get the idea)
https://i.imgur.com/9nWosSp.jpg

Where all the brain and electronic bits will be contained, I could stack 2x VESC6 inside this one
https://i.imgur.com/652yLsO.jpg

And my (RIP) previous version : 
https://i.imgur.com/uUOeRTI.jpg

Now I have few parts that'll need CNC cutting again ! Since that's expensive, either you guys are interested and I could try to group buy CNC'd parts and also negociate another batch of custom motors from my manufacturer (you can pretty easily make a workable version from skateboarding parts + add a remote combo inside if you don't wanna wait for my "no-remote" system)  or I simply make carbon layers out of parts I'll reprint.

Voilà, thanks for reading and wish to meet&race you all guys ASAP :beers:
```

---
## \#2 Posted by: venom121212 Posted at: 2019-05-11T14:59:43.086Z Reads: 189

```
I can't even imagine how many custom pieces you've had to track down and make work. This is a true diy build man. Well done!
```

---
## \#3 Posted by: Vanarian Posted at: 2019-05-11T15:04:35.725Z Reads: 184

```
Thank you !! ❤️
```

---
## \#4 Posted by: rey8801 Posted at: 2019-05-11T16:26:16.372Z Reads: 174

```
Your idea and realization is really good. Are yo7 planning to basically never actively skate or have a kind of assisted skate? Like for ebike? Becuas win that case the batteries could be smaller and save weight and improve design. Maybe also think at some small vesc version. Now with the mini version of them should save you space again.
Anyhow looks cool. Make it happen!
```

---
## \#5 Posted by: Inline Posted at: 2019-05-11T21:28:20.423Z Reads: 153

```
Very cool, I made an account just to comment on this. I've always been an inline skater, but I've also had an interest in electric transportation. Recently I bought a budget E-Board to satisfy my need for speed, but only because there was no electric inline skate options. Where did you get the motors from? I've been looking for motors like that for a while.
```

---
## \#6 Posted by: Vanarian Posted at: 2019-05-11T23:35:06.734Z Reads: 139

```
@rey8801 Thanks man ! Basically yea I aim for both without needing to switch via a mode, so a leg trigger calibrated enough to respond to the stride or simply the angle of attack? Something similar.

Good point about the weight, I'm trying to keep it low but I need range and pretty big amps too. Escapes should be ready for a beating (+ it got direct airflow and dual heatsinks). Actually the battery rail will accommodate swappable packs so eventually if I can do smaller and bring extras in a backpack this works too. It still needs a strap and hopefully by moving the weight upwards it will feel less like a heavy foot, I might be able to test that soon. Or if I realize I don't draw big amps I can drop 1P per foot ? Road tests will tell.
```

---
## \#7 Posted by: Vanarian Posted at: 2019-05-11T23:38:55.644Z Reads: 121

```
Thanks and welcome ! The motors I got from E-Max with just custom shaft and kv and the rest is homemade. Still needs  extra structure, there's no bolt on yet but it will be once that thing works and is properly tested on road.
```

---
## \#8 Posted by: rey8801 Posted at: 2019-05-12T04:41:30.920Z Reads: 106

```
Based on the size of the motors maybe a 1p is enough. You could think aboit lipo to have the amp in a small size. The actually battery could also be a small one mount at the calf level as you thought or a range extended one that you could fix at the belt. Something flexible and for sure helps with the weight distribution. It can have a fast release system in case of trouble like the weighted belt used for diving.
```

---
## \#9 Posted by: Rollertom Posted at: 2019-05-12T07:48:26.320Z Reads: 98

```
@Vanarian Your mock up looks very nice. I was also considering without remote and virtual skate-controlled. But I am not sure yet if when turning and jumping the Skate is doing what it wants. In my opinion there is no stable and precise measurable thing like for example if you´re measuring torque at a bicycle pedal crank. What I realized at testing most, espacially for faster driving, is the possibility for tilting similar to a monowheel. There motor is controlled by tilting angle if I am right. Also motor force can only be transmitted well if there is tilting because there is no option like in skateboarding to stabilize with both feet. Also if you have one VESC in each skate there is the problem that for straight driving they have to rotate exactly with the same speed and have to communicate together.
```

---
## \#10 Posted by: Vanarian Posted at: 2019-05-12T09:12:35.052Z Reads: 94

```
Yea Lipo graphene for example ? I'd like these for the punch and reliability. I'm looking for something similar to volleyball strech bands or clipsable smooth belts ? I'll pad it with foam so it's soft on the skin :smile:

Despite the small size I expect a lot from these little fellas ! It's derived from a classic 12 poles but I'm packing 36 magnets total inside. + worked on the cooling, air flow and the high temp enamel, so I'll feed it good current (at least what I can withstand I guess). Either it explodes or it'll be a wild mini beast.
```

---
## \#11 Posted by: Vanarian Posted at: 2019-05-12T09:35:59.464Z Reads: 95

```
Thank you! I still need on road tests to see if it's jittery or not but an analog type source like potentiometers or similar thing is straightforward resistors so it should serve as clean input, I can filter the noise with a cap and it'd be good. Eventually if I can use a better ADC than in-built arduino ones, I'll have higher accuracy and quicker polling. In ideal setup I'd hack a gaming gear and get 1000hz ultrapolling, but that's way above my current abilities ! So sticking with simple setup. 

Tilting can be similar, either a big potentiometer (you don't get noise from G forces) or mpu gyro chip (you can make fancy functions with that but need to account with noise from G forces all around).

About the VESC communicating together, I use esp32 modules (it has wifi and BT built in, just a bit painful to use but it's a recent chip and the support and arduino portability has grown a lot since last year) so I thought of reading erpm values from each VESC then adjusting throttle signal based on a thresold for both VESC (example : ERPM difference cannot be higher than +-200). Hopefully in wifi it will be quick enough to keep a responsive throttle. BT could do if signal is fast enough, but there's also consumption to check (which one is less greedy) and I'd like to keep BT in reserve to use with my phone later on (so I can use Vesc-Tool on phone directly).
```

---
## \#12 Posted by: rey8801 Posted at: 2019-05-12T12:33:46.924Z Reads: 84

```
I am sure they an deliver good power. You can always use mpre motors in the future or bigger wheels to host larger motors. Although I like the Lowe profile I also think that will help in stability. I did skate in the past and they look really fun!
Yes I was thinking about a 4-5s graphene lipo or for the belt version multiple 3s that have a good form factor. They will be outside anyway so easy to charge them with a balance charger. For sure you will have plenty of power.
```

---
## \#13 Posted by: Rollertom Posted at: 2019-05-12T16:18:36.899Z Reads: 80

```
OK, but I didn´t get what kind of measurement of the Skates do you wanna measure (force, pressure or something else) in order to controll motors. How much torque does your motor have?
```

---
## \#14 Posted by: ryansinatra Posted at: 2019-05-12T20:24:26.812Z Reads: 73

```
Watching this space :) these are cool
```

---
## \#15 Posted by: Vanarian Posted at: 2019-05-12T21:37:11.052Z Reads: 72

```
Ideally I'd measure the following settings : 
- attack angle of the stride or leg
- direction of each skates and velocity
- erpm for each motor

With this I'm aiming for the most possible natural behavior and under some conditions, drop the throttle in favor of freewheel depending on measured data.

Theoretical max torque supposedly was like 6Nm per motor but in 2wd 1:1 ratio with very limited diameter I suppose that's optimistic. Fortunately (and your videos proved it too) I can kick hard with muscle to compensate if motors lack power.
```

---
## \#16 Posted by: Vanarian Posted at: 2019-05-12T21:40:00.331Z Reads: 68

```
I think I could squeeze up to 68-70 diameter motor in my 110mm wheels before starting to eat the PU away 😆 63mm for example is very doable. But it's heavier too!

Nice to know you've been skating, when was your last time ?
```

---
## \#17 Posted by: rey8801 Posted at: 2019-05-12T23:57:17.259Z Reads: 72

```
Just for fun 2 years ago. When I would have condider myself capable too long ago :laughing:
I was never a pro, but at least I was doing some ramp and trick at the park. Now I will be just ridicolous.
```

---
## \#18 Posted by: rey8801 Posted at: 2019-05-27T13:52:07.014Z Reads: 57

```
Hey, I found this great deal for a small CNC machine and I thought about you, in order to finish your project and start many more. It is in BE but for the price I would really think about it, you can also ship it. The EMCO F1 is a little beast. I just bought a BF20L otherwise I would have jumped straight on it and save 1.5K :sweat_smile:

https://www.2dehands.be/doe-het-zelf-bouw/machines-apparaten/freesmachines/cnc-emco-f1-freesmachine-getransformeerd-533333285.html
He also posted a youtube video showing the machine working. The guy clearly did not used it too much judging by the cutting but the machine itself is great.

What can do this little monster https://www.youtube.com/watch?v=XzOt1r4giiE
```

---
## \#19 Posted by: Balta_6 Posted at: 2019-05-27T15:25:12.132Z Reads: 40

```
Nice to see that you're posting your adventure finally !
Just a question, how does the can of the motor hold the weight ? is it custom made ?
```

---
## \#20 Posted by: Vanarian Posted at: 2019-05-27T17:29:42.601Z Reads: 38

```
Thanks for the link man, this lil machine looks super powerful ! It digs through like it's foam instead of alu.

Yea I need to think about getting one someday, budget won't cut right now but later is another day 😆
```

---
## \#21 Posted by: Vanarian Posted at: 2019-05-27T17:31:45.480Z Reads: 34

```
Thanks man ! Well the can does not support weight in fact, it's trapped in an "exo" shell. The shell does all the hard job✌🏽
```

---
## \#22 Posted by: rey8801 Posted at: 2019-05-27T18:49:39.642Z Reads: 29

```
No problem. I saw it and told that would be perfect and if you can bring it home for 1K is a steal.
```

---

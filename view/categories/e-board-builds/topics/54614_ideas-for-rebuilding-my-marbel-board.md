# Ideas for rebuilding my Marbel board

### Replies: 21 Views: 1619

## \#1 Posted by: jslade Posted at: 2018-05-06T23:24:23.241Z Reads: 207

```
I've got a Marbel board that stopped working over a year ago, so time to do something with it. I really like the board -- great feel on the ride, great weight, great range. I'd be happy to get it working again similar to how it was, or even possibly an upgrade. I haven't ever built a board, but I've been reading for a bit, and I have an engineering background. I fugure I can ramp up pretty quick, but I need some guidance to get started.

I don't know what components stopped working, but I figure I will start with a new ESC - like the FOCBOX. I plan to just go with single drive still, though I guess I'd consider a dual hub motor drive if the weight and other factors are similar -- I ride an Inboard M1 and it performs okay for my needs -- miss the higher speed of the Marbel, though.

Can I stick with the original motor? That would be my preference for simplicity and cost to get going. If I need a different motor, suggestions for one that would work with the FOCBOX and give me similar performance to the original Marbel motor?

Can I reuse the battery pack? How would I know if the cells are still good - any way to test the pack? It's been sitting idle/uncharged for over a year, is that bad? If I were able to test it and verify that the pack is good, what do I need to use it with the FOCBOX? I know BMS's are a thing but not how to choose one, or otherwise what is needed to make a given battery pack work with a given ESC.

Along with the FOCBOX, I assume I'll need a new remote. Suggestions on that? Or can I make the Marbel remote work somehow?

Then there's the question of how to put it all together in the Marbel board. It is designed as a sealed board, with the original charging port coming out through the front bumper. SO I expect I would do the same thing -- seal up the deck with the original cover once I have the components working, then have a lead out the front for charging, and a power switch, I guess. I imagine it will not be very weather-proof, so I'm okay if this has to be a fair-weather board. Or I'm open to the possibility of leaving it unsealed, having a way to just snap the top cover in place or something - like some sort of 3d-printed latch mechanism

Has anyone converted their Marbel in a similar fashion? Interested in experiences and/or ideas how to make this work.
```

---
## \#2 Posted by: Hummie Posted at: 2018-05-06T23:36:47.402Z Reads: 183

```
Wo lot of questions.  Csnt even read it all but get a multimeter and see what the battery shows and u can also test a bunch of other stuff w it.
```

---
## \#3 Posted by: ShutterShock Posted at: 2018-05-06T23:56:47.138Z Reads: 178

```
Any specs or pics or the board in its current state?
```

---
## \#4 Posted by: jslade Posted at: 2018-05-07T00:28:54.617Z Reads: 175

```
I have no idea on the specs. Here's some pics:
https://photos.app.goo.gl/7jmFEqtYAM0DXoIl2
https://photos.app.goo.gl/nmBErLCAojfxn0gS2
https://photos.app.goo.gl/fqv1H7btVHjhKCJU9
https://photos.app.goo.gl/CjkoBmM5zbSM76f99
https://photos.app.goo.gl/DseV5qFVhMcwPT4d8
https://photos.app.goo.gl/8j6JBN1uGcQ3eDJ86

I see mine didn't come out very sharp. Someone else took these from their board: http://www.electric-skateboard.builders/t/inside-marbel-gen-1-skateboard/23117

So I'm guessing their custom-built ESC also integrates a BMS -- the smaller-gauge wires going to the battery pack? 7 red and one black -- does that mean it's 7s?

And the 6 smaller colored wires going out the back to the motor are for the hall sensors?
```

---
## \#5 Posted by: Hummie Posted at: 2018-05-07T00:51:39.882Z Reads: 148

```
Probably n probably for ur last questions.
```

---
## \#6 Posted by: mmaner Posted at: 2018-05-07T01:19:45.908Z Reads: 146

```
There's only a few major components to an electric skateboard...

Speed Controller(s)
Battery Pack (w/ BMS)
Motor(s)
Motor mounts
Wheel Pulley(s) & Motor Pulley(s)

If you are going for a retrofit then the speed controller is out and you need a working speed controller to test the motors. 

You can test the battery by using a volt meater to.measure the current voltage, the charge, and test the current voltage again. If the initial value is above the minimum bfor the pack type and it goes up after charging then you battery is good. This is assuming the BMS is part if the battery pack. 

We can assume your motor mounts and pulley srtup are good if you can turn the wheels.manually and therer are no obstructions or breakage that keeps then from turning freely.

I'd the battery and drive train (belts and pulleys) are good and the battery is good...it's safe to say you can purchase x2 ESC(s) and a remote, connect the speed controller(s)  to the motors, install the remote RX, connect the battery.  Then you can see if the motors work. 

Get that far and I will, as well as 1000 other people, will walk you through the rest.
```

---
## \#7 Posted by: Naysh Posted at: 2018-05-07T02:20:19.402Z Reads: 121

```
Measure your pack, if its zero then a cell or all is defective. If pack is good then its esc. If it's the pack , do you want to rebuild it.
```

---
## \#8 Posted by: jslade Posted at: 2018-05-07T05:25:40.612Z Reads: 114

```
Okay, task for tomorrow is to measure the pack.

If it works, I'll need a new 7S 24V 20A BMS, it looks like, to go along with a new VESC / FOCBOX. Hopefully it's as simple as that I it just works with the existing motor.

One other crazy idea I had: thinking about how I might use the Inboard M1 Powershift battery packs with this board... There should be space in the cavity + FOCBOX. Can the Powershift pack plug into the FOCBOX directly (obviously the physical plug itself is an issue, I mean electrically compatible)?
```

---
## \#9 Posted by: aigenic Posted at: 2018-05-07T06:39:08.862Z Reads: 102

```
If you want to use powershift batteries you ill have to replace motor for sure :)
```

---
## \#10 Posted by: jslade Posted at: 2018-05-07T13:20:19.341Z Reads: 96

```
Why is that? The battery pack obviously incorporates the BMS, but it would still need to plug into the ESC -- so Powershift battery --> ESC --> Motor. Why would I have to replace the motor "for sure"?
```

---
## \#11 Posted by: aigenic Posted at: 2018-05-07T14:05:34.319Z Reads: 86

```
Because marbels battery is 7s (8 wires) but inboard has 12s battery...you would get much higher top speed from the motor and you dont want that :) Also the motor is probably not built for such a high voltage...
```

---
## \#12 Posted by: jslade Posted at: 2018-05-07T17:39:14.197Z Reads: 81

```
Supposing I wanted to go that route -- using the Powershift battery pack in the Marbel deck -- what would I need? Can you recommend:

- motor + mount
- FOCBOX or other ESC
- remote

Not saying it's a good idea, just wondering about feasibility

Some more info on the battery: http://www.electric-skateboard.builders/t/inboard-battery-bunk/13991

I like the idea of the Powershift batteries because I have them, and makes it easy to remove for air travel. But I can accomplish the same with the original 7S3P Marbel battery pack or build a new one if that proves to be unusable (haven't been able to test yet)
```

---
## \#13 Posted by: aigenic Posted at: 2018-05-07T20:54:20.765Z Reads: 68

```
But I must say that I support the idea with powershift batteries, because using FOCBOX on 12s is better than 7s ;) 

IDK what mount does Marbel use and how is the motor mounted to it so I cant really say if you would have to replace it :/ Maybe some pics could help? 

With powershift batteries you would have to necessarily replace: ESC, Motor, remote...maybe mount and pulleys...
```

---
## \#14 Posted by: pat.speed Posted at: 2018-05-07T21:09:17.343Z Reads: 66

```
If you want to use the power shift batteries that’s fine, you will need a new esc (focbox is best or escape) and possibly a new motor if the kV is too high, but I would wait as you can test that when you get the focbox. 

If you do happen to need a new motor/s there are lots to choose from the cheaper ones are Keda and Sk3 motors around 190kv and the more expensive are jlabs, tb, chaka’s and many more
```

---
## \#15 Posted by: banjaxxed Posted at: 2018-05-08T02:54:22.696Z Reads: 64

```
Let's not forget the inexpensive  racerstar motors on Banggood which are sensored which is nice on a single motor setup
```

---
## \#16 Posted by: jslade Posted at: 2018-05-10T01:58:34.762Z Reads: 57

```
I finally got a hold of a multimeter and measured the battery pack - 3.6V across the whole thing, and pretty consistent .4V - .6V across each cell. So I guess I'm good to go on the battery. I'll assume the motor is good as well.

So it looks like I need an ESC, remote, and BMS (might as well since the pack is wired for it)
- ESC: [FOCBOX](http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/) from Enertion - currently $161
- remote: [Nano X](http://www.enertionboards.com/electric-skateboard-parts/nano-x-enertion-2-4ghz-controller/) from Enertion - currently $67
- BMS: [7S 20A](https://www.ebay.com/i/112314398195?chn=ps) on ebay - $7.20

Doesn't sound too bad to get the board usable again. Anything I'm missing?

I still need to figure out how to manage the lid and the front bumper that was previously the charging port and all that. If it works reliably, then I can just seal it up and slap a new grip tape on the whole thing, and have the charging port come out the front like Marbel did it. First to get it working...
```

---
## \#17 Posted by: jslade Posted at: 2018-05-10T04:06:08.386Z Reads: 49

```
Oh and a charger - recommendations? Something that will work for this 7S battery pack, but perhaps also 10S or 12S in the future?
```

---
## \#18 Posted by: Hummie Posted at: 2018-05-10T06:42:37.717Z Reads: 47

```
maybe the bms you chose isn't the best to use.   I don't know details but maybe theres a discharge ability you want it to do or charge rate you'd also want.
```

---
## \#19 Posted by: jslade Posted at: 2018-05-10T16:04:17.025Z Reads: 46

```
I have no idea how to choose the BMS --  other than it being for a 7S pack. So please let me know what I should be looking for.
```

---
## \#20 Posted by: jslade Posted at: 2018-05-12T15:05:22.468Z Reads: 42

```
Maybe a suggestion on a better BMS option? What makes one good?
```

---
## \#21 Posted by: 95devils Posted at: 2018-08-02T16:51:27.454Z Reads: 30

```
any update?
ive got a marbel board but im searching for a pulley to fit the stock 76mm wheels. Im unable to locate a pulley unless i get 1 3d printed.
```

---

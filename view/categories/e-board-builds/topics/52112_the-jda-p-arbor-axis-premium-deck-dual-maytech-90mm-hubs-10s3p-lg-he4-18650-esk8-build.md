# The JDA³P &#124; Arbor Axis Premium Deck &#124; Dual Maytech 90mm Hubs &#124; 10s3p LG HE4 18650 &#124; Esk8 Build

### Replies: 7 Views: 747

## \#1 Posted by: JdogAwesome Posted at: 2018-04-12T23:04:21.998Z Reads: 180

```
The first two paragraphs are going to be about the history of my esk8 addiction/relationship so if you don't care and just want to see my new build, skip over them.

---

My addiction to electric skateboards and everything esk8 related started way back in September of 2015 after I saw Casey Neistat's video about his new Boosted Board (Yes I know everyone has mixed feelings about Casey, thats not what this thread is about.) Anyways after I saw that I knew I had to get one one of these things! Quickly I realized that spending $1k-1.5k on a board was not going to happen and that I needed to find a cheaper alternative. "Of course!" I thought, "I'll just build one myself and save a ton of money!" This was not the case. Im sure all in I spent at least $1000 on my gen 1 and revision 2 board and put so many hours of work into the damn thing because of one, or two, main factors, I tried to be cheap and I didnt know what I was doing. These two main flaws contributed heavily if not solely to the roots problems of my board e.g. the board used a RC Car ESC and had terrible bakes and acceleration which caused two separate crashes resulting in minor injuries. Some of the other problems were, it wasnt waterproof, didnt have a BMS, charged via a JST cable just hanging out of it, used a crappy "relay" switch, had a shitty fiberglass enclosure, used super thick crap copper cable, etc. I could go on all day about the problems this board had and the things I did to try and counteract these but eventually I scrapped everything inside the board, including the batteries (2x Zippy 3S 5Ah LiPo's.) 

I decided to start over again with 4x Zippy Compact 3S 5Ah LiPo's in a 6s2p config and bought two VESC 4.12 to drive my new Maytech 90mmm Hub Motors. The first pic below is of the internals of that which I call "revision 2". This time I had a better understanding of what I was doing as this was about 6 months ago and I put in a bit more money to get it working properly. I fixed the problem of the crappy brakes and acceleration by getting some VESC's and fixed my charging problem by using a BMS and building a charger which charged through a GX16-9 connector on the side of the board. However I immediately realized 6S on these Maytech Hubs was getting me a max speed of 19-20mph which simply wasn't fast enough as I was used to a top speed of 30mph on my Carvon V2 hub. I then rewired the battery into a 12s1p and got a new BMS and BOOM I was reaching a top speed of 35mph, much better! However the hubs where rated for a max of 10S so running them at 12S resulted in me getting a max of about 6 miles of range compared to my 14-16  miles of range I was getting before the battery reconfig. I dealt with this problem though as I wanted to the speed and I wasn't planning on making any long trips so I didn't really need the long range. As you may have noticed I didnt mention anything about the water resistance of the board, which I did increase but it still wasn't waterproof, and was the downfall of this board only about 3 months later. I was riding the board downtown on a bike path when I encountered a street that wasn't plowed properly resulting in their being a lot of slush on the bike path which I rolled right over without much of a thought. About a half mile later I feel like the board is slowing down a lot so I decide to hop off and take a look at the underside. To my horror the entire underside of the board was covered with grey slush and only one of the motors was spinning(Pic of the board below.) I then got an uBer to my final destination and when I opened the trunk to get my board out, it was smoking, oh shit. Thankfully it stopped smoking shortly after and when i opened the board up I found a ton of water damage all over the internals and mainly on the BMS which was completely black and charred. The only component that still worked was my Maytech VESC, my enertion VESC and BMS where dead. And that is where I am today.

![Inside of Board & Slush Covered|444x500](upload://rVJnZQS24LOqWpHHsAF1AVrt05W.jpg)

---

My new build is pretty much from the ground up, new deck, batteries, enclosure, etc. This time I wanted to go about this properly so I decided to model the entire build in F360 with every part in there including the ESC's MOSFET switch, custom control PCB for OLED display and topside battery indicator, mounts for the batteries, etc. Right now im deciding on how to configure my 18650 battery as I have drop through truck mounts on the board so I dont have a ton of clearance underneath. Right now my idea is to have the battery in 3P packs lengthwise up and down the board which makes it long, but very thin. In the config I also thought a great way to secure the battery to the board is using some sheet metal strips that go over the cells and are screwed in place with threaded inserts. I was planning on either bending them by hand, or if im using thicker metal using the press brake they have at [mHUB](https://mhubchicago.com/) in Chicago. FYI mHUB is an amazing space with **LITERALLY** everything a maker or startup would need for fabrication. Anyways take a look at the render below and let me know what you think.

![Battery Layout Hor & Vert V2|444x500](upload://4Z4fPkkuoGvd8bF8Qm7POONUXxE.jpg)

---

Other than that I plan to use a FOCBOX and my leftover Maytech VESC connected over CANBUS to drive the motors. I dont see why using a FOCBOX and a VESC together would have any problems as they are technically the same other than having a different layout and some upgraded components. I also plan to build my own headlights with custom PCB's and some nice Cree LED's, and maybe throw in some WS2812B LED's somewhere along the way as well...

---
Pretty much finished the 10s3p Battery Pack, got them all connected in series and the balance leads soldered on. Still need to run a few more wires to the BMS and main power leads for the battery, but other than that its almost done. Pics below

![IMG_20180415_225230|690x389](upload://oGMP9gAOe9agNAUyO3pbZ9mDCVS.jpg)
![IMG_20180415_224744|690x389](upload://ciUj3axBWfh6UYanx8PzCwFuIFl.jpg)
```

---
## \#2 Posted by: Martinsp Posted at: 2018-04-12T23:18:40.624Z Reads: 161

```
The sheet metal without any sort of additional insulation is not a good idea. The outside of the battery is the negative terminal so if the insulation gets pierced you will short your cells.
I used a similar technique in my first build a couple years ago but I used straps like you find on backpacks but wider. On the ends I secured it to the deck using a screw through an aluminum flat bar to provide more area to hold the strap down. This worked out great, I was not able to make an enclosure for it back then so I redesigned  it by now, but it held the batteries very well! Hope it helps :) 
![Picture1|690x318](upload://qYRtG6Fld32T5UjZXpewJD4nhxq.jpg)
```

---
## \#3 Posted by: JdogAwesome Posted at: 2018-04-13T00:00:08.077Z Reads: 153

```
Yeah I was planning on shrink wrapping all the cells so they wouldn't be right against the supports, thanks for pointing that out! I like your way of using those fabric straps as well.
```

---
## \#4 Posted by: JdogAwesome Posted at: 2018-04-14T04:20:38.055Z Reads: 118

```
Finished spot welding and shrink wrapping all the 3x packs of cells! Just need to wire up all the series connections and get my balance leads figured out. Im using two layers of 6mmx0.15mm thick Pure Nickel strip on all the connections and I plan to use thin braided copper wire for the series and main power connections.
![IMG_20180413_190701|690x388](upload://19zPgOtQKUE5SWZDsZCph5ysKSr.jpg)![IMG_20180413_190558|690x388](upload://6eFJd9muT3WFRaYZNq7SQbeqJxP.jpg)
```

---
## \#5 Posted by: JdogAwesome Posted at: 2018-04-16T04:12:08.727Z Reads: 86

```
Finished the battery pack, I updated the original thread with the pictures.
```

---
## \#6 Posted by: arzi7 Posted at: 2018-04-30T14:28:44.959Z Reads: 72

```
Will you share your vesc tool configuration pics, please?
```

---
## \#7 Posted by: JdogAwesome Posted at: 2018-05-01T00:43:55.602Z Reads: 60

```
Im using the normal BLDC Tool for my 4.12 and FOCBOX, but ill upload pics of the config when its done! I did however post pics of my settings on my Maytech Review which you can find [here](https://www.electric-skateboard.builders/t/maytech-hub-motor-vesc-and-truck-review).
```

---

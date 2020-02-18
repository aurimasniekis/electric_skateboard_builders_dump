# I’m working on a remote, what features do you want?

### Replies: 44 Views: 2065

## \#1 Posted by: JLabs Posted at: 2018-04-04T02:54:31.635Z Reads: 344

```
So I’ve got an electrical engineer helping me design a custom remote that does not use an Arduino anymore. It will be all one PCB and simple to make (I hope). What kind of hardware features do you want to see? My main are:

1. Battery protection and charging
2. Adaptive cruise control
3. Thumb, trigger, or joystick control
4. A screen for real-time data
5. Dual PPM output
5. UART input/output 

So what do you want to see? This is mostly at the hardware stage as of now. I’m hoping to have a thumb wheel, trigger, and wii nunchuck style versions available. I’m also trying to keep the cost reasonable so no lasers or rockets allowed.
```

---
## \#2 Posted by: wafflejock Posted at: 2018-04-04T03:02:10.821Z Reads: 337

```
I've got some cheap lasers available.   Wondering if you've thought about FCC certification or if any of the existing remotes are actually certified or not.  Going to take the HAM test myself this week hopefully and have always worried about trying to produce my own cause of the rules here in the US (know basically no one checks but can get slammed with fines if it interferes with anything important).  Maybe a mode change switch if possible would be nice too.
```

---
## \#3 Posted by: Apolo Posted at: 2018-04-04T03:03:19.984Z Reads: 320

```
I'd say a deadman switch, and have long travel on the thumb wheel
```

---
## \#4 Posted by: mmaner Posted at: 2018-04-04T03:05:48.236Z Reads: 307

```
Spees, MAH used, MAH remaining, average WH should cover most everything and keep the display from being too busy. 

I think trigger and thumb will be the major usage, joysticks take some getting used to. 

Lastly, big ass battery, like charge once a week ride 200 miles battery...if possible. 

Let me know if I can help.
```

---
## \#5 Posted by: dg798 Posted at: 2018-04-04T03:11:18.488Z Reads: 285

```
Long long range thumb that stays put in the pot with now wiggle. Long range connection and maybe a small screen for some data. Also high capacity battery. This would be awesome
```

---
## \#6 Posted by: baxter Posted at: 2018-04-04T06:00:35.262Z Reads: 280

```
My vote is for a nunchuck style remote using PPM. Power comes via an 3000mah 18650. Perhaps a small OLED screen just below the trigger so it can be used right or left handed. The white on black screen would simplified to only show 3 things

1. Speed
2. Main pack voltage (or percentage)
3. Remote control voltage (or percentage)

Cruise control and a dead man’s switch would be cool, plus if you wanted to add more features like selectable menus, you would be able to navigate easily.

Not sure how complex you want to make it, but it I would argue that it should be as simple as possible with AFHSS feature (not sure what it is called exactly) like on the GT2B for signal reliability. 

If you wanted to develop something more distinctive, you could check out my earlier concept thread with “grenade” style throttle inspired by a slot car controller.

http://www.electric-skateboard.builders/t/esk8-remote-control-concept/21898
```

---
## \#7 Posted by: baxter Posted at: 2018-04-04T06:04:06.431Z Reads: 256

```
Though as telemetry would be required, UART would be appropriate
```

---
## \#8 Posted by: High-roller Posted at: 2018-04-04T06:10:50.800Z Reads: 257

```
I'd like to see a remote that's as plug and play as possible, regardless of which firmware I have. I love the ideas showing up in the likes of the phantom remote, the Firefly, and others, but since I'm not much of a programmer I've been a little wary of the potential problems.
I realize that we're still in the early days of this, I'm hoping we'll soon get to a point similar to that of RC vehicles where, for the average user, you don't need to think too much about your components in terms of communication issues. You simply plug everything in, bind and ride.
```

---
## \#9 Posted by: ElskerShadow Posted at: 2018-04-04T22:21:01.466Z Reads: 224

```
Go with a trigger remote for sure ! GT2B style with telemetry
```

---
## \#10 Posted by: Sebike Posted at: 2018-04-04T22:26:30.552Z Reads: 217

```
Super reliable connection. No cut outs.

And THEN comes all the other requested features..
```

---
## \#11 Posted by: b264 Posted at: 2018-04-04T22:30:22.502Z Reads: 213

```
Trigger AND thumbwheel.  That way, for example, I can use the trigger for proper control of esk8 but use the thumbwheel for lights and horn.  If you prefer thumbwheel, this could be reversed.  Also a few extra switches with their own channels.

Quadruple PPM output.  Trigger, thumb, switchA, switchB

If none of that is possible, then just a trigger.  I've seen [other](https://www.electric-skateboard.builders/t/universal-advanced-vesc-remote-control-photon-custom-design/24654) custom remotes that I completely ignore because they don't have a trigger control.
```

---
## \#12 Posted by: JLabs Posted at: 2018-04-04T22:34:57.368Z Reads: 211

```
[quote="Sebike, post:10, topic:51168"]
Super reliable connection. No cut outs.
[/quote]

That will be for sure the #1 priority. 

Thanks everyone for the suggestions! I can’t teply to them all individually but I will definitely implement most of them. 

@b264 thanks for the quadruple suggestion. I’ll do that as it won’t take up that much more space
```

---
## \#13 Posted by: dAeM0N1K3 Posted at: 2018-04-05T00:04:07.504Z Reads: 201

```
A thumbwheel with a rock solid 5Ghz or Bluetooth connection. All 2.4Ghz remotes I've used so far have had disconnects at one point or another, especially in congested urban areas. Small power indicator, bluetooth indicator, low/fast mode. Small form factor that will fit mostly between a clenched fist, but not too small like the Nano-X remote. Lowest possible price tag without sacrificing any of the above.
```

---
## \#14 Posted by: b264 Posted at: 2018-04-05T00:09:33.237Z Reads: 191

```
Lower frequencies will give more solid connections, not higher ones
```

---
## \#15 Posted by: dAeM0N1K3 Posted at: 2018-04-05T00:14:02.335Z Reads: 197

```
Almost every device out there also shares that exact same 2.4Ghz frequency. I'm almost 100% certain this is why I get cut outs in the city streets. Someone's office kitchen microwave wants me to face plant into a taxi in the middle of rush hour. I guess Bluetooth it is then, I've heard nothing but great things about Boosted's remotes, but I don't want a Boosted. We need a custom solution.
```

---
## \#16 Posted by: b264 Posted at: 2018-04-05T00:15:19.085Z Reads: 193

```
Evolve uses Bluetooth and there are countless reports of connection problems.  I'd use a wire before I used Bluetooth...
```

---
## \#17 Posted by: GrecoMan Posted at: 2018-04-05T00:18:07.410Z Reads: 194

```
just make a boosted clone
```

---
## \#18 Posted by: pakue Posted at: 2018-04-05T00:40:14.936Z Reads: 199

```
A few programmable buttons would be nice, like on higher-end cameras. E.g. for turning on/off lights, switching power modes without having to look at the remote or fiddle around with a menu.

Also pro nunchuck style.
```

---
## \#19 Posted by: louwii Posted at: 2018-04-05T01:39:15.808Z Reads: 200

```
+1 for custom buttons to trigger lights, horns, LEDs and whatnot.
```

---
## \#20 Posted by: wafflejock Posted at: 2018-04-05T02:33:12.002Z Reads: 197

```
Used my own homemade nrf based one for a long time now (think 2 years) no drop outs or anything so long as it has proper power supplied it works consistently and doesn't do wifi really just point to point so don't think it goes through exponential back off type strategy for sending packets... In any case it hasn't ever been a problem for me and live at the edge of Chicago so plenty of wifi noise around.

Also did a Bluetooth one before using my phone as the controller... Terrible idea for a few reasons but one is the losing of a paired connection (reapairing a connection on the move is no fun)
```

---
## \#21 Posted by: wafflejock Posted at: 2018-04-05T02:38:54.171Z Reads: 175

```
Replying to me here but the gt2b does have an FCC id despite being made in China.  Fine to design and use your own prototypes in the US but to sell a product anywhere need to get pricey certification which it seems means hiring an rf engineer to a verify everything before paying to attempt the certification process.
```

---
## \#22 Posted by: JLabs Posted at: 2018-04-05T15:57:24.249Z Reads: 165

```
I’m am currently only putting two buttons on the remote, one for cruise/dead man and one for menu selection. It would be easy to put another switch on the remote but for the receiver what would I “put on it” to allow you to program it? Pins? Relay?
```

---
## \#23 Posted by: Dyspro Posted at: 2018-04-05T16:01:34.768Z Reads: 167

```
Really like the boosted / leif design. 

I'd ask for buttons that are not easily pressed while riding and cross board compatibility.
```

---
## \#24 Posted by: bigben Posted at: 2018-04-05T18:32:31.332Z Reads: 160

```
Something that works well with good gloves. (Trigger not too small if you go that way.)
```

---
## \#25 Posted by: Jedi Posted at: 2018-04-05T18:42:26.637Z Reads: 161

```
+1 cruise control please
```

---
## \#26 Posted by: Acido Posted at: 2018-04-05T19:06:01.121Z Reads: 157

```
Make it so a big battery fits, It would be great if an 18650 would fit, get a 35E 3500mah....
Thumb control  and a screen!

And a working failsafe please, also something like a button that blocks the motors instantly if you press it.
```

---
## \#27 Posted by: wafflejock Posted at: 2018-04-05T21:05:54.779Z Reads: 149

```
Deadman switch is the opposite of what you're asking for but usually a good way to go when it comes to cutting power (probably don't want it to apply brakes in case you are at speed, need to just know how to stop by foot braking).  Regarding battery you can almost squeeze an 18650 into my remote shell but it's pretty beefy as is and still doesn't quite a fit one (plus need to cram in electronics around it).  Using a 800mAh battery my controller will last 40+ hrs though so it's not really a major issue.
```

---
## \#28 Posted by: pakue Posted at: 2018-04-05T23:09:31.458Z Reads: 150

```
Just attach some unused IO to solder points. adding a mosfet later is easy.
```

---
## \#29 Posted by: Schulerbible Posted at: 2018-04-05T23:17:10.400Z Reads: 152

```
A nice design, such as the R2 remote or Boosted. Maybe a small display that shows velocity and range.

Basically the Photon remote in an Evolve R2 package ....
```

---
## \#30 Posted by: SirDiff Posted at: 2018-04-06T11:35:52.305Z Reads: 158

```
One thing many didn't mention: price. We know a remote doesn't actually cost much, since the mini trigger style is like 15€ and super reliable, and other people that are developing other remotes told me the production price is extremely low, in comparison to the market price. All the fancy stuff isn't actually needed: we hopefully won't be looking at the remote when riding. As long as it's rechargeable, compact and reliable, that's a good remote.
If you decide to add more features, I think the main one should be the board battery level, in percentage and volts, maybe with a record of the ride stats, so that we can start avoiding volt meters on the board and just use the remote.  
I've been waiting for a good affordable remote for a long time, 100$ is just way too much when a gt2b goes for 20. I'd say 40 is the right spot
```

---
## \#31 Posted by: wafflejock Posted at: 2018-04-06T19:24:07.929Z Reads: 164

```
As far as I can tell this can't be a legit consumer product for such a small community at such a low price point.  I did the pricing on a remote before... can't find mine but can see the one from another very similar one here:
https://docs.google.com/spreadsheets/d/1G6cbB9tymxwAx_ul-3dK_ecZLHnj8iVudTKXk6aNmv8/edit?usp=drive_web&ouid=108173165070170894192

Mine doesn't have the OLED but only $3 of the cost in that, also think of the time to 3d print the shells or if you go the mass manufacturing route need to get a metal mold made/machined for injection molding and need to do that at a very large scale in order to make money back.

As I mentioned in posts above an intentional radiator really needs FCC certification which is also not cheap.  The only way to do this is to go big or stick to DIY and having people do their own assembly programming and leaving the liability on them.

Here's mine for reference and if anyone wants to DIY or make your own or tweak my design it's there for the taking:

https://github.com/shusain/eskatecontroller

https://cad.onshape.com/documents/50e9e32d777391df91fbe5a9/w/19598faab2182f3b574dcfaf/e/52a747c0c2e141ee735a22b8

---

Long story short if you want a cheap remote buy something off the shelf made in the 10s of thousands for RC enthusiasts if you want something unique or more fitting to your needs you're going to need to DIY
```

---
## \#32 Posted by: SirDiff Posted at: 2018-04-06T19:49:45.773Z Reads: 150

```
On what number of units did you calculate those prices? Even with just 50 units, the prices usually drop a lot if you buy in bulk from the manufacturer. Building a couple of remotes obviously isn't worth it, but it might be if you get close to the hundred mark.
@lox897 i know you were doing the same research, maybe you can help, @Sander too :slight_smile:
```

---
## \#33 Posted by: wafflejock Posted at: 2018-04-06T19:51:32.034Z Reads: 150

```
Buying at scale is assuming that you can get them all assembled at scale and sell them all as well otherwise need to have extra money for product not sold and for support/replacements etc.  Looking at the raw hardware cost doesn't tell the whole story.

---

Also I didn't get the numbers in that sheet pretty sure it was from the other popular nrf based one here that's still being developed.  That said the costs are going to be elsewhere with doing this as a 'product'... I also considered doing mine as a 'kit' and potentially even leave out the nrf chips since the intentional radiator stuff is where it really becomes necessary to have certification (which again isn't cheap).

---

As of now I small pile of PCBs used to connect arduino pro mini to a 'standard' nrf board with the built in antenna I've just been giving them away basically at cost to anyone who wants them or is trying to build my controller (or their own).  The PCBs I got made at a qty of 100 and price was $83 (including shipping) so about .83 a piece for a custom board not including any components on it or assembly (used pcbway but prices are pretty comparable from what I've seen between PCB fab houses)
```

---
## \#34 Posted by: LAVAMAN Posted at: 2018-04-06T20:21:39.355Z Reads: 127

```
I am not a member of the NRA, but I prefer triggers
```

---
## \#35 Posted by: Silverline Posted at: 2018-04-06T22:46:51.383Z Reads: 122

```
Damn... looking forward for this remote...

Please make a solid connection, like the Gt2b/ 2,4Ghz link..
Trigger style for me.....
Cool OLED display, with good vision in sunlight, maybe with vibrator, to notify when your reach certain amount of  voltage/wH/mAh
```

---
## \#36 Posted by: Sebike Posted at: 2018-04-06T23:16:00.564Z Reads: 124

```
I want a buzzer on the remote to let you know when your most recent post on the esk8 builders forum has reached a certain amount of likes.
```

---
## \#37 Posted by: Schulerbible Posted at: 2018-04-06T23:30:16.569Z Reads: 129

```
I believe you can easily charge between $100-120 AUD, this is what we pay for the R2 from Evolve and I haven’t met a single person that didn’t buy the new remote!
```

---
## \#38 Posted by: lox897 Posted at: 2018-04-07T03:28:37.356Z Reads: 125

```
I guess so... @JLabs is pretty experienced in the manufacturing field though :slight_smile:
```

---
## \#39 Posted by: myreala Posted at: 2018-04-07T05:18:51.151Z Reads: 118

```
I agree keeping price low should be a priority. Photon is good but $150 for a remote that has 3d printed body is just not gonna happen. I would argue that keeping is below $80 would be best that way you can recover development costs slowly and its not too expensive. Also if you decide to open source the software I and I am sure others would definitely try to add more features into the remote than you can at the beginning. I would say keep the development cycle on software side small and get good hardware, the community can add whatever is missing in the software. Hell, as long as we have enough buttons I am sure we could turn this remote into a full fledged VESC programming tool. Open source would allow people to add whatever is missing for them and that way more people would be inclined to get this remote.
```

---
## \#40 Posted by: jess.t.moody Posted at: 2018-04-07T05:39:35.518Z Reads: 111

```
I need a remote control with plenty of extra buttons for other features (lights, horn, etc). This is a must have (extra buttonz!).
```

---
## \#41 Posted by: SirDiff Posted at: 2018-04-07T12:06:39.070Z Reads: 103

```
Well, evolve itself is overpriced, the remote is just the same. 200$ for a damn remote that costs 20 to manufacture (at most, considering how big they are. Probably less) is just stupid IMHO. We know the best remotes in terms of reliability are the cheapest ones right now, spending 10x just to have reliability issues (evolve coff coff) isn't too smart. I'd stop looking at how much other companies charge for this stuff and start thinking how to improve the community. A good board costs as much as a used car nowadays, we can't keep raising prices just cause this sport is getting more popular and people buy it anyway
```

---
## \#42 Posted by: Schulerbible Posted at: 2018-04-07T12:11:49.424Z Reads: 107

```
I agree, but a decent remote cost some $$$ especially when the enclosure isn't 3D printed. There is always options for people who want to spend less which is good. Personally, I want a remote that works well, maybe has a display which shows some numbers, a few buttons (e.g. light switch) and looks decent. The DIY stuff I've seen so far aren't my cup of tea.
```

---
## \#43 Posted by: SirDiff Posted at: 2018-04-07T12:22:37.160Z Reads: 119

```
Yup, I agree. I love the shape of my benchwheel remote and I was OK with its price and features. It stopped working cause it was poorly made. I'm sure the same could be made for a similar price (35-40€) but with a better reliability, kinda like the mini internals in a benchwheel casing somebody posted on this forum some days ago, for 10/15 bucks more I'm sure they could add an oled screen and a couple of buttons. Obviously, they'd need to go for injection moulding instead of 3d printing
```

---
## \#44 Posted by: baxter Posted at: 2018-04-07T13:07:42.251Z Reads: 123

```
I agree with @SirDiff.  The GT2B is the benchmark example of excellent reliability and cost effectiveness.  Sure, doesn't win many points on the aesthetics, but that's why people modify them into smaller, sexier controllers (e.g. the Badwolf and MasterchoMod).  Until someone comes up with a better controller with the same sort of reliability, they will have a hard time convincing me to move away from it.  

Sure it would be nice having a few bells and whistles on my remote control, and I acknowledge that these bells and whistles cost money. However it would be difficult to justify purchasing that sort of thing at a significant price premium. You have to ask yourself is a remote control that costs $100, five times better than a GT2B (which costs $20)?  Are you getting the best bang for your buck?

On another note:
How about making a remote kit that consists of all the electrical stuff soldered together, except for the case (and maybe the battery), which the buyer could then 3D print with the supplied STL files?  Of course they could have the option of buying it all assembled if they wanted.  This would reduce overall price, tooling and some assembly costs, and allow the user to tweak the electrical components or STL files if they wanted to modify it further.

Thoughts?
```

---

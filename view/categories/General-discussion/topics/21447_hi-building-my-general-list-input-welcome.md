# Hi! Building my general list—input welcome

### Replies: 9 Views: 730

## \#1 Posted by: lastmango Posted at: 2017-04-20T16:07:41.177Z Reads: 88

```
Hi gang—I've been reading through the forum quite a bit, but I'm still well behind the general knowledge curve to be sure. I'm a 48 year old graphic designer from Florida with a casual long boarding hobby. Now I want to go electric.

I was led here after researching many pre-builts and determining the following:
1) I'd like the ability to choose my own deck & some components—I want what's right for "me". 
2) I'd like to really learn more about the specifics & science—always achieved from DIY, not to mention the ability to replace, tweak & improve.
3) I'm a parent, and although I have some discretionary income, spending a lot of money all at once is not in the cards. A piece-by-piece build fits my lifestyle better.

That said, because I'm a designer and not an electrician, I am trying to achieve a "plug-and-play" board of sorts, in the vein of one of RunPlayBack's videos. Aesthetics & simplicity (from an assembly standpoint) are of major interest to me: So… here's what I'm thinking

• MOTORS: dual hub motors (I live in Florida—no hills to speak of, and I want to maintain pushability & clean lines). Thing is, I have no idea what sort of hub motors are best—or even available. I've looked into Enertion & Carvon, but they don't seem available for sale at the moment. Anyone have insight on this? This seems to be my "toughest" find at the moment. I really don't want to do a belt—more interested in hubs.

UPDATE: Pretty sure I'll shoot for a single belt drive for a first build now—don't want to get in over my head, or spend a year collecting the parts.

• BATTERY: I've already purchased this (the only part I have so far)—an Enertion Space Cell Pro 3 (10s3p), but I want to be sure what I connect in the way of a vesc/motors, etc. are matched well to it—not looking for fires & such, lol.

• VESC: Honestly... I'm still reading up on this stuff. Pretty in the dark, but learning more every day—two for a dual motor setup is about as much as I've figured out so far. Gotta read up on BLDC & FOC settings still.

UPDATE: Getting a bit more schooled on this, and thinking I'd like to keep connections as simple as possible—possibly matching connector types if possible to keep soldering to a minimum.

• CONTROLLER/RECEIVER: Still looking, but I'm thinking small & thumbwheel—not trigger.

• DECK: Not sure yet on specifics, but a 38-40" longboard deck seems like my style (non-flex, because of the battery mounted below). I'm looking at Honey decks at the moment, but that's something I don't really need any help with... been skating for a while

• TRUCKS: I'd love to be able to use standard trucks. I already skate on 10" Caliber 2's right now & love them, which is another reason I'm interested in going with hub motors & DIY.

WHAT I WANT TO DO WITH IT: Have fun. Carve. Cruise through backstreets & neighborhoods. Head up small inclines at a decent clip. I don't need eye-rolling torque, or breakneck speed—but I definitely want some power & zip. Topping out in the mid twenty-something mph with ease sounds great. Most important to me though is smooth power transition… I'm a fan of fluid acceleration–I'm not racing. Solid braking ability would be a great thing, too.

Any insight on my initial thoughts on a build would be great. I fully understand that this forum represents a wide range of interests and alliances—casual builders and business owners with their own products—I get that, and I welcome that diversity. I've seen some pretty big political rants in some of these posts, and I'm interested in the tech of things—not the "pick a side" of things. Research is first, but I'd love to get my act together by mid summer, so I can actually get out there too.

Thanks guys! (and gals!)
```

---
## \#2 Posted by: flatsp0t Posted at: 2017-04-20T16:36:15.388Z Reads: 75

```
Well, i will go through this one by one.

**Motors:**
Carvon just launched their V3 Motors via kickstarter. The backers will receive them around end of May. I am not sure, but if i remember correctly, carvon will not sell their motors as standalone. They will however make exceptions for existing customers of his old Motors. I think they are not completely sure, and it will depend on the demand for them in relation to the demand for his completes.

Enertion will not sell their motors as single pieces, but only as part of hir Raptor 2.

There are also some other Hub motors coming up right now by various forum members, but nothing i would recommend to a new builder yet.

**Battery:**
You could use more power for hubs, but it is a good start and we can work with that.

**VESC:**
I dont Recommend Maytech VESCs, as they are missing some important stuff.
There is a complete list of sellers here:
https://www.electric-skateboard.builders/t/worldwide-vesc-directory/16764
You could either go VESCX(not sure if needed here), or a standard VESC 4.12 (I would recommend getting them from AXLE).
We can talk about settings and modes after we figured the rest out.

**Controller:**
Debends on your preferences on Thumb stick or Trigger control.
Thumbstick: I would Recommend the Benchwheel.
Trigger: either the 2.4 GHz mini remote or a modded GT2B (Sparkle or mad munkey mod.)

**Trucks:**
Normally hubs come premounted on trucks because they need some extra mounting to not spin off of the axle. Thea are mostly Standard longboard trucks (Caliber or Paris clones).
```

---
## \#3 Posted by: t0m_r1dd1e Posted at: 2017-04-20T16:42:32.923Z Reads: 62

```
Looks like you're on the right track! If you buy most of your stuff from one place, things will be a lot more plug and play. 

That's a great battery. idk what connector it has on it, but you'll need some sort of splitter to get power to both VESCs and then you'll want some 190KV motors, probably in the 6355 size. Motor mounts can be tricky but you can buy a kit to make everything a lot easier like this: diy-electric-skateboard-kits-parts/torqueboards-dual-motor-mechanical-kit/

The trickiest part for me was picking a deck, finding an enclosure, mounting it to the deck, and finishing everything. I got my enclosure here and would definitely recommend them. He's active on this forum and has exceptional customer service. The first enclosure he sent me was about a half inch more narrow than the specs said and he made and shipped me another one for free, no questions asked. http://psychotiller.com/products/shop/enclosures

Don't worry about the specifics with VESC settings for now. A textbook could be written on it. Basically if you want silent motors, you want FOC mode, and if not, you'll run in BLDC mode. I don't like FOC mode because for me it's easier to control when you can hear what the motors are doing. It also lets people near you know you're there which feels safer for me. You can worry about specifics when you get to that part. It's a little overwhelming at first but it's really not bad. 

Anything specific you'd like feedback on at this point?
```

---
## \#4 Posted by: lastmango Posted at: 2017-04-22T01:14:44.488Z Reads: 46

```
<img src="/uploads/db1493/original/3X/4/5/45c0003532958d330941902f2dd4a3a85d74346c.JPG" width="666" height="500">

Thanks @t0m_r1dd1e —appreciate that. The battery came today, and has a single connector—do you know what that connection type is called? That would be a big help. From what I can gather so far from poking around, I connect the vesc to this connection (though I know I may need to adapt the connection type). To the vesc, I'd connect the bluetooth chip/receiver that should come with the controller, right?. If a dual motor setup, I'd then need to piggyback another vesc to the first vesc (the one connected to the battery). Then, configure my vescs via the software (which I downloaded the other day from Enertion's site). Sound right, or am I way off? Thanks!
```

---
## \#5 Posted by: lastmango Posted at: 2017-04-22T01:37:39.611Z Reads: 40

```
Thanks, man! Helpful info.
```

---
## \#6 Posted by: Blasto Posted at: 2017-04-22T01:53:59.607Z Reads: 40

```
For the sake of keeping things simple, i would go for a single 6374 motor. 1 motor controller, 1 motor, plenty of torque... maybe not as much as a dual, but going dual does complicates a first build.

And that connector you are showing is a xt60 female
```

---
## \#7 Posted by: mmaner Posted at: 2017-04-22T03:59:34.111Z Reads: 35

```
[quote="lastmango, post:4, topic:21447"]
The battery came today, and has a single connector—do you know what that connection type is called?
[/quote]

It's an xt60 or xt90 but I can't really tell the size.
```

---
## \#8 Posted by: lastmango Posted at: 2017-04-23T02:40:53.210Z Reads: 23

```
Thanks, @Blasto ... after some further reading, I think I'll take that advice and switch my plan to a single belt drive motor for this first build.
```

---
## \#9 Posted by: lastmango Posted at: 2017-04-23T02:46:15.759Z Reads: 21

```
Thanks, @flatsp0t! I may hit you up with vesc questions once I get to the settings stage. Decided to simplify my build & try a single belt drive to start.
```

---

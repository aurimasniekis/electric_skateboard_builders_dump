# My first build! - Low $ Toe Dipper / Banggood 5065 200kv / 6s / ESC TBD

### Replies: 23 Views: 1854

## \#1 Posted by: HOPPEMSU Posted at: 2017-09-14T14:07:09.833Z Reads: 256

```
Hi Everyone!  This is my first post and build, and I'm grateful for all the information on the community.

I'm new to skateboarding, and have never ridden an esk8.  This is a very economical (not "cheap") first project.  It is just for playing around to try the hobby, not commuting or long distance riding.  

I'll be the primary user.  My elementary school age kids will want to try it too.  I'm about 200 lbs.  If we like and use it, I'm happy to build new boards later or upgrade parts.  I want top speed limited to 15-17 mph, and would like to be able to limit it further for my kid's use.

I'll use the following parts:

*  An existing longboard from Amazon: https://www.amazon.com/RIMABLE-Rimable-Drop-through-Longboard-41-inch/dp/B01CJU96EY  I'll move the trucks and add spacers so it is not a drop-through, as needed.

* 83mm or 90mm wheels (to be purchased)

* Banggood Racerstar 5065 200kv motor <img src="/uploads/db1493/original/3X/1/6/166bd5c95d083525848152b2ad0017ccb4b40638.png" width="163" height="163">
https://www.banggood.com/Racerstar-5065-BRH5065-200KV-6-12S-Brushless-Motor-With-Gear-For-Balancing-Scooter-p-1117658.html

* Banggood 2.4ghz mini wireless remote https://www.banggood.com/2_4Ghz-Mini-Wireless-Remote-Controller-Receiver-Electric-Skateboard-Longboard-p-1179725.html?rmmds=myorder
 https://www.banggood.com/2_4Ghz-Mini-Wireless-Remote-Controller-Receiver-Electric-Skateboard-Longboard-p-1179725.html

* Banggood pulleys, belt, motor mount <img src="/uploads/db1493/original/3X/9/4/9413aa48045486ed7fe223f73fd0aed3e5a4b4b7.png" width="163" height="163">
  https://www.banggood.com/Electric-Skateboard-Belt-Motor-Mount-Bracket-Pulley-Screws-For-839097MM-Wheel-p-1105929.html  (I'll DIY an aluminum motor mount if that doesn't work)

* Banggood 15T motor pulley (in case 12mm pulley in kit doesn't work well): <img src="/uploads/db1493/original/3X/2/2/223d1e96bf8e647c3f9d6d753ee8bdc8f97cc936.png" width="163" height="163">
 https://www.banggood.com/Racerstar-Motor-Gear-Red-For-BRH5065-BRH5045-Brushless-Balancing-Scooter-Motor-p-1139957.html

* 2x Zippy 5000mah 3s1p 20c, wired in series for 6s  <img src="/uploads/db1493/original/3X/4/c/4cbc3b1a0d0765b6a618bbbc3be6b658b5442836.png" width="200" height="150">
https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html

* Turnigy Accucel-6 charger <img src="/uploads/db1493/original/3X/d/b/db12b3db8ca92863ea4dd439f3cd0b6244aaf03d.png" width="200" height="150">
 https://hobbyking.com/en_us/turnigy-accucel-6-80w-10a-balancer-charger-lihv-capable.html

Can you please help me pick an ESC?  A VESC looks flexible but seems a bit daunting to program.  Also, it would be nice to spend less than $160, which seems to be the going rate for an Ollin Boards or FOCBOX unit.  

Thanks for your guidance!
```

---
## \#2 Posted by: Armin Posted at: 2017-09-14T14:15:39.270Z Reads: 225

```
Hi,

Just want to say that you could be saving money and getting a better product by looking for longboards on ebay/craigslist. There are people out there who buy nice boards but never end up riding it or just don't like the hobby so they end up selling them on sites like eBay for way less than half the price they paid for something that's pretty much new! I'd give that a shot, maybe you can find a great deal.

Also I'd recommend going the extra mile and getting a VESC, it is a bit of a pain to program but there are many guides on this site on how to program them and this community exists to help each other out, so if you do have any issues or questions you can always come back here and I'm sure someone would be more than happy to help :slight_smile:
```

---
## \#3 Posted by: HOPPEMSU Posted at: 2017-09-14T14:22:31.101Z Reads: 211

```
Thanks!  

I looked for used boosted boards, etc.  However, to me, building things is almost always more fun than actually using them.  I just love projects.  The REAL goal is to design and build something cool!

I hear you on the VESC.  From what I read, Chaka and Enertion seem to have the best reviews.  Can you recommend any of the less expensive ones?
```

---
## \#4 Posted by: Armin Posted at: 2017-09-14T15:18:55.303Z Reads: 183

```
Oh I meant longboards as in a deck for your build. DIY is the way to go as you've said, what I meant to say was people on eBay and CL sell high quality decks in good condition for the same price or less as the one you've chosen on amazon.

On the topic of VESC's I'm afraid my knowledge doesn't extend that much for me to give you proper recommendations. I only know things here and there, however I'm sure someone else would comment sooner or later with a more detailed recommendation on this area :slight_smile:
```

---
## \#5 Posted by: HOPPEMSU Posted at: 2017-09-14T16:08:46.274Z Reads: 170

```
Thanks!  

I already have this board.  I bought it for my kids on an Amazon sale for less than $40 a while back.  If any of us get into this, we'll upgrade.
```

---
## \#6 Posted by: jammin Posted at: 2017-09-14T16:13:27.300Z Reads: 163

```
Check out the DIY Electric Skateboard VESC ($100). you could also go with the maytech vesc (but most of them are missing a bootloader). And the vesc is really easy to program! It's literally filling in the right numbers and clicking 'write'.

6s + 20C is a bad call (too much voltage sag). Either increase your C count or cell count. Plus, 200kv at 6s isn't going to be fast at all. I'm not sure how well the vesc does on 6s (I'm concerned about current draw, especially at your 20C). You can control top speed (aka governor) using the vesc settings.
```

---
## \#7 Posted by: HOPPEMSU Posted at: 2017-09-14T17:50:47.025Z Reads: 146

```
Awesome feedback.  Thanks!

I'll look further at batteries.
```

---
## \#8 Posted by: pat.speed Posted at: 2017-09-14T22:01:24.891Z Reads: 133

```
I actually use a 6s battery and it is 20c and I only see around 0.5v sag when accelerating and almost not sag at all once I'm going and about 1v when going up a steep hill. I think those batteries will be fine for you as a first build. As for the esc you can either use a Vesc but they are a bit more expensive and a lot easier to fry than a car esc. I am using the Xcar beast esc from Hobbyking and I love it. I changed the setting so the startup and brakes are smooth. Other people also highly recommend this esc for 6s builds. It is also really cheap just make sure to get the programming card with it too
```

---
## \#9 Posted by: Maxid Posted at: 2017-09-14T22:04:38.751Z Reads: 121

```
Get a VESC - every other ESC will not make you happy and you'll end up buying one later on anyway.
```

---
## \#10 Posted by: darkkevind Posted at: 2017-09-14T23:15:04.051Z Reads: 114

```
[quote="Maxid, post:9, topic:33131"]
you'll end up buying one later on anyway
[/quote]

I second that!
```

---
## \#11 Posted by: scepterr Posted at: 2017-09-14T23:31:58.601Z Reads: 105

```
What's your total cost for all the parts?
```

---
## \#12 Posted by: HOPPEMSU Posted at: 2017-09-14T23:57:06.146Z Reads: 104

```
Right now I am at roughly 260 for everything but the esc, including the charger.  That includes $40 for the longboard I already had.
```

---
## \#13 Posted by: pat.speed Posted at: 2017-09-14T23:59:41.528Z Reads: 99

```
What is your town like? Hilly? Flat?
```

---
## \#14 Posted by: HOPPEMSU Posted at: 2017-09-15T03:23:07.630Z Reads: 86

```
Pretty flat
```

---
## \#15 Posted by: pat.speed Posted at: 2017-09-15T05:39:11.407Z Reads: 81

```
A Vesc might serve well then but if there are any large hills I would be careful about going up then on a Vesc and 6s
```

---
## \#16 Posted by: Maxid Posted at: 2017-09-15T08:45:22.474Z Reads: 85

```
shouldn't be a problem. A VESC can safely handle 50A continous - at 6S that is still 6*3.7V*50A=1110W which is quite a lot.
I had a 150A Car ESC and had it cut out repeatedly during uphill movement - that is scary. So I'd rather get up the hill more slowly but safely.
```

---
## \#17 Posted by: BoostedBuilder Posted at: 2017-09-15T10:59:00.996Z Reads: 74

```
If you can, use a 10s battery!! 200Kv and 10s go together really well but you will have to use a VESC for that!!! It will end up costing a tiny little bit more but you'll not regret it after) E-sk8's are not meant to be really cheap!
```

---
## \#18 Posted by: HOPPEMSU Posted at: 2017-09-15T12:16:28.384Z Reads: 82

```
Thanks for the suggestions.  I haven't actually bought the batteries or the ESC yet.  I think the options now are 10S / VESC or 6S / Car ESC.  I'll look into both.  

I'm trying to be economical, not "cheap" so I really appreciate the suggestions.
```

---
## \#19 Posted by: BoostedBuilder Posted at: 2017-09-15T12:35:57.687Z Reads: 84

```
I'm telling you the complete truth right now!!! Buying a VESC and using it with a 10s battery will be more economical!!!
```

---
## \#20 Posted by: bigben Posted at: 2017-09-15T12:37:59.774Z Reads: 92

```
10s and vesc is the best way to go. 
If you are hell bent on low initial outlay there is this motor which will be faster on 6s and something like an fvt120 esc. 
https://m.banggood.com/Racerstar-5060-BRD5060-280KV-4-12S-Brushless-Motor-For-Balancing-Scooter-p-1117660.html?rmmds=detail-bottom-alsolike
```

---
## \#21 Posted by: Nix Posted at: 2017-09-15T13:14:21.792Z Reads: 85

```
I have about the same setup, but what's the concern of voltage sag and the vesc handling it?
```

---
## \#22 Posted by: Nix Posted at: 2017-09-15T13:31:37.555Z Reads: 82

```
Also, 6s with vesc should be ok. As long as you set the limits right, and 200kv motor w a 6s battery leaves alot of room for upgrades
```

---
## \#23 Posted by: HOPPEMSU Posted at: 2017-10-06T20:13:51.727Z Reads: 60

```
Just a quick update on my project.  I decided to go with:

-  x-car beast 150amp
-  6s (2 x Turnigy 5000mAh 3S 25C Lipo Pack W/XT-90)
-  36 tooth wheel pulley
-  Either 12 tooth or 15 tooth motor pulley (I bought both)
-  Banggood Racerstar 5065 200kv motor

I get this will be a slow board.  I also get that I'm getting older and not very coordinated.  I want to walk before I run...

Parts are starting to arrive.  I mounted the wheel pulley to the 72mm wheels that came on the longboard, just to try it out.  I may order 83mm or 90mm wheels after trying it out.  OR, if I like it, I may give this to my kids and build a new, nicer board for me.

Currently, I'm right at $333 all-in, with a charger, connectors, the board, etc.

Thanks for all your help!  I'll post pictures when the electronic bits arrive.
```

---

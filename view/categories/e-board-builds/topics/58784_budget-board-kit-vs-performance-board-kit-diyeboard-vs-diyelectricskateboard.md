# Budget Board Kit vs. Performance Board Kit (diyeboard vs. diyelectricskateboard)

### Replies: 13 Views: 1977

## \#1 Posted by: Static Posted at: 2018-06-13T20:50:27.321Z Reads: 314

```
Having skated for nearly two decades I was eager to get into the electric skateboarding trend. But without having any previous knowledge of RC components building a board from scratch can be a bit intimidating, especially given the real risk of irreversibly damaging expensive parts. So to start off I decided to use a kit. Ultimately my goal will be to build a board with various parts on my own. 


I started out with the 10s5p Dual Hub (500wx2) kit from <a href="http://www.diyeboard.com/10s5p-360wh-batteryescpower-truck-kit-dual-9052mm-hub-motors-p-598.html">diyeboard</a>, which was a little under $600 usd when complete.

![IMG_20180607_181638|666x500](upload://ukhM64XcxWPizg519n33r5PNa2A.jpg)

Although no instructions were included, assembling this kit took about 30mins, as there really isn't anything to do except mount the trucks and enclosure. Wires were color coded to make things easy. It also comes with a foam pad gasket to keep out moisture. Some people have complained about the electronics being loose in the enclosure so I used rubber grommets and hot glue to secure everything. 

![IMG_20180607_181857|374x499](upload://wq51OYKVX5clEpbXcTsX4WNmnef.jpg)

Riding this thing for the first time was quite an experience (first e-board ride ever). Fast and plenty of torque/acceleration. I'm nearly 200lbs and this board doesn't have a problem pulling up majority of hills. Using a speed app I was able to hit 23mph on this board....which took a while to work up to. 

I've put well over 100 miles on this board and it is still running well. This has been a great kit for the type of <a href="https://www.skateshred.com/wholesale-blank-longboard-decks/kicktail-dark-walnut-deck.html">board</a> it is mounted to. I haven't fully depleted the battery yet, but I suspect it'll do about 15 miles. I haven't felt the range anxiety yet out on long rides. Although, I'd say It makes a better board for quick runs and it feels less imposing in public. It looks like they've upgraded to the new meepo remote but the old remote has been great, really like the reverse option and batt. indicator. 

Cons with this kit:

Expensive shipping to US, was about $50usd. FOC has not worked yet. Managed to get it working with the motors spinning opposite directions, but nothing else. No need really as the motors themselves are already silent. 

10s5p battery, but with what cells? I have a feeling that some unnecessary weight/bulk it being added to this board due to cheaper cells. It's hard to call this a con though at the price.

The main issue for me, however, isn't with the kit. It's the quest for more POWER.

<p>&nbsp;</p>
Enter the <a href="collections/electric-skateboard-conversion-kit/products/pro3-electric-skateboard-conversion-kit">PRO3</a> kit from   

I purchased this kit after much deliberation and $100 discount. The parts all arrived in separate bags and boxes. As with the chinese kit from diyeboard, no instructions were included. Although the sales reps will gladly point you to the youtube page which will somewhat help you piece together information you need to assemble the kit. Most of my help came from this forum. Although I had some issues, most of them were related to being new to the hobby. 

The deck I ended up using also came from <a href="https://www.skateshred.com/wholesale-blank-longboard-decks/40-x-9-5-bottlenose-top-mount-blank-deck.html">skateshred</a>, total cost about $1300usd

![IMG_20180607_181304|666x500](upload://WfkWEKJirXkdN0z4VCDRWSexxr.jpg)
![IMG_20180607_191024|374x499](upload://p0i64K3rd6l56U7N7iVKgyAV1Vn.jpg)

Riding this board with stock settings for the first time was a bit insane. It's not at all in same category as the other kit. The untamed power of this board constantly felt like a wild stallion ready to buck you. Even at 3/4 throttle the acceleration is strong enough to throw you. The motor drag at high speed and sensitive braking were also things that destabilized balance forcing me to constantly stand braced. After many sessions with this board I was able to hit 34mph and finally find my footing (full skin protection a must).

![IMG_20180607_191237|666x500](upload://uRItAsDpA6NVEB2XToXzgRCJrNS.jpg)

Recently I set the VESCs to run in FOC which has tamed the board immensely and made it very quiet. I also remapped the remote and reduced the brake power. All things which have hugely improved the riding experience and were very easy to set up using the wizards in the vesc tool.

Cons with the kit:

If you just want to start riding and don't have any knowledge of where to start on a DIY build chances are you will be a little frustrated in the beginning. Especially since diyelectricskateboard sells you on the "learning" bit and makes you feel like you have more support than reality (talking with them, they have plans to expand the tutorials/guides for their kits so I suspect this will improve). I initially had alignment issues with the drivetrain and trouble getting the key to fit in the keyseats for both motors. I had to file down the sides of the keyseat to get a fit- although this was after damaging a motor pulley. I also think the diyeboard remote is better than the standard nano remote supplied with this kit. There's no speed settings, reverse, or battery indicator. However with a vesc you can change the remote, so not a big problem.

**Edit: Apparently VESC HW4.12 are a risk to run in FOC with a 12s battery. Currently looking for an affordable replacement. I'll give sensored bldc a shot soon and update.

**UPDATE 6/28: I set the TB ESC's back to BLDC mode, although the hall sensor wouldn't detect correctly on one motor so I didn't use sensored. Not a problem though, with the right settings in BLDC mode the board rides almost as nice as FOC. 
<p>&nbsp;</p>
<p>&nbsp;</p>
Overall I am happy with both kits. They serve two different experiences. If you just want to get on the road with a budget and don't plan to make this a focus hobby or want something more portable go with the diyeboard kit. 

If you want to grow with the sport and eventually get better and go faster, I'd consider something easier to scale like the kits from diyelectricskateboard just be prepared to spend time fine tuning. 
![IMG_20180607_181927|375x500](upload://nNxjjcr4BiY5hQWLQh9fCi6BnQi.jpg)

Thanks for reading, if you have questions I can try to answer.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-06-13T22:10:18.959Z Reads: 260

```
I’m pretty sure diyeboard’s esc runs foc straight out of the box, that’s why it’s so damn quiet. I have one of those esc on a belt drive board and it’s so much quieter compared to my dual bldc board
```

---
## \#3 Posted by: loiphin Posted at: 2018-06-14T07:15:24.678Z Reads: 231

```
Thanks for the great post! I am waiting for my PRO3 kit to arrive. I should get it in the next day or so. **What deck did you use for your PRO3 build?**  My deck is a switchblade 38, which has a W concave. I just hope its not too difficult to mount the motors underneath and I still have some clearance for the battery.

I read somewhere that if you are running VESC 4.12's in FOC mode with 12s batteries, you risk blowing the MOSFET driver. Cant remember where I read that though.

Thanks,

loiphin.
```

---
## \#4 Posted by: brenternet Posted at: 2018-06-14T08:19:39.653Z Reads: 202

```
This is a great write up. Did you consider going full DIY on the second board or was it always going to be a kit?
```

---
## \#5 Posted by: Static Posted at: 2018-06-14T13:30:35.353Z Reads: 183

```
@loiphin I used <a href="&lt;a href=&quot;https://www.skateshred.com/wholesale-blank-longboard-decks/40-x-9-5-bottlenose-top-mount-blank-deck.html&quot;&gt;skateshred&lt;/a&gt;">this</a> deck from skateshred. I used the 0.5" risers that came with the kit to get more clearance, although I probably don't need them. 

I've rode several hours with FOC and no issue. I'd be curious to know more about this myself. It'll be hard to go back to BLDC, FOC is just so nice.

@brenternet I built the second board with another kit because the first kit wasn't very involved and I wanted to have some experience with belt drives and vesc. Third board will be ground up DIY.
```

---
## \#6 Posted by: loiphin Posted at: 2018-06-14T13:57:14.002Z Reads: 174

```
http://www.electric-skateboard.builders/t/foc-vs-bldc-for-a-dual-190kv-12s-setup/36258

Thread on burnt out VESC's using them in FOC mode with 12s.
```

---
## \#7 Posted by: brenternet Posted at: 2018-06-14T14:00:59.123Z Reads: 156

```
I feel you on that. Going through my first build now after having off the shelf ones before and there's an awful lot of information out there.

I'm lucky enough to have discovered very experienced builders around me who are willing to share thier knowledge.
```

---
## \#8 Posted by: squishy654 Posted at: 2018-06-14T14:16:31.765Z Reads: 147

```
Nice post dude, tons of good info, thanks for sharing..
```

---
## \#9 Posted by: Static Posted at: 2018-06-14T14:18:00.745Z Reads: 151

```
Will have to try sensored BLDC to see if it compares. Otherwise there has to be a way to set some safeguards to prevent what he did in FOC.

Wish there were more VESCs on the market to choose from.
```

---
## \#10 Posted by: jetsmack Posted at: 2018-08-20T21:08:49.591Z Reads: 102

```
what size and name of the first deck?
```

---
## \#11 Posted by: Static Posted at: 2018-08-20T23:28:17.574Z Reads: 86

```
34" kicktail from skateshred, link is in the post.
```

---
## \#12 Posted by: Psmrman90 Posted at: 2018-11-07T00:45:51.728Z Reads: 62

```
Great post, love the detail and honest thoughts.  Im currently looking to get a pro 1 or pro 2 kit.  May i ask how long the enclosure is?  I want to make a short board for college commuting, just want to make sure I can fit it all on a 30 ish inch board
```

---
## \#13 Posted by: Static Posted at: 2018-11-07T01:25:16.225Z Reads: 56

```
[20in](collections/battery-enclosures/products/12s4p-enclosure-v2), it is not suited for cruiser decks

I'd skip the kit route. You can buy more customized/better parts for the same price. Torqueboards stuff is great but I wouldn't use them for everything. Shop around, look for sales (black friday) copy parts of builds that others have done on the forum.
```

---

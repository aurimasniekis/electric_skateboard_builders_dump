# Mitigating &ldquo;Death Wobble&rdquo;: The implementation of an Adjustable Steering Damper in an Electric Mountainboard

### Replies: 11 Views: 1965

## \#1 Posted by: raz Posted at: 2018-06-16T00:44:32.881Z Reads: 329

```
As some of you know:
One potentially deadly problem that skateboards have is called "death wobble" (or speed wobble / tank slapper / etc.). It is a phenomenon that only occurs when a given riding speed has been reached where riding vibrations resonate with the skateboard's natural frequency.
When resonation occurs these vibrations will produce forces on the skateboard which will make it wobble.

When this occurs your body will try to correct these wobbles instinctively, but it will inevitably overcorrect the wobbles making matters only worse.
The usual thing to do is to not panic and stiffen up your ankles while concentrating on your movement and looking in front of you.

On an electric skateboard you might try to break but you might lose your balance, in that case you just have to let yourself coast while doing the above. You also won't have to concentrate on the brake that way.

There are a few ways to get around death wobble such as tightening your trucks or having them at an angle. What this effectively does is it changes the skateboard system's natural frequency. Death wobble will stop occuring at the speed you were riding at before but it _will_ occur at a different, higher speed.
At a higher speed the vibrations will have a higher frequency (= more vibrations), the wobble will be faster and thus will be harder to correct. 
The skateboard system behaves much like a damped oscillator. When a force is applied it will start oscillating (= wobbling) like a harmonic oscillator and will not stop unless a counteracting force is applied. The counteracting force by default is your body/ankles and the friction caused by tight trucks.

However, you can only tighten up your trucks so much and tightening them will make turning harder. This is where the implementation of an adjustable steering damper becomes interesting.

This is my implementation of a steering damper that can be bought on [AliExpress](https://www.aliexpress.com/item/Damper-Steering-StabilizerLinear-Reversed-Safety-Control-for-Suzuki-GSXR-GSX-R-600-750-1000-1300-Yamaha/32791821784.html). It cost me €29.29 and even though it's cheap it's well made in my opinion. You can find it in all sorts of funky colors. It also has a knob to adjust the damping force. It's all CNC and the knob is clicky, it feels nice in general.

![DSC_0178|690x459](upload://4265xKbo1ianTDVTQ6JXaQwHTm4.JPG) 


Without this upgrade wobble would start occurring in my build around the 25 km/h mark. Unless I tightened the trucks of course. The damper has been mounted in such a way that the adjustment knob is accessible whire riding. When I want to go 40 km/h I just turn the knob and off I go. :upside_down_face:

A possible upgrade would be attaching a servo motor to the knob and controlling the servo motor with a custom app with the VESC. That way the ERPM could be interfaced to the servo motor and in turn the damper could be adjusted without human intervention while riding. But I haven't had the need to do that as I am not THAT lazy. :stuck_out_tongue: 

Extra pictures:
![DSC_0177|333x500](upload://sgrBEkLA5xt6gthWnVRMxwGEtWZ.JPG)![DSC_0171|690x459](upload://16tyUImArnDHOHLdwY0PK4sIK6.JPG)
```

---
## \#2 Posted by: skatardude10 Posted at: 2018-06-16T01:30:50.212Z Reads: 303

```
Does it work for you? I need to try this if it works.
```

---
## \#3 Posted by: Kug3lis Posted at: 2018-06-16T01:41:48.202Z Reads: 300

```
There are electrical ones from bikes, they have electric solenoid which you can regulate with arduino or etc ;) Also there are radial ones :) @Nowind has them in his boards ;)
```

---
## \#4 Posted by: CHAINMAILLEKID Posted at: 2018-06-16T01:49:47.469Z Reads: 291

```
Should experiment moving it around between the front and rear trucks, I'm guessing one of them might work a lot better than the other.
```

---
## \#5 Posted by: Michaelinvegas Posted at: 2018-06-16T01:56:23.677Z Reads: 283

```
Hey...at least they ain’t bungee cords...


http://www.electric-skateboard.builders/t/stabilised-skateboard-truck-anti-speed-wobble-tech-advice-from-a-moron/24902?u=michaelinvegas
```

---
## \#6 Posted by: raz Posted at: 2018-06-16T08:20:59.702Z Reads: 250

```
Hey! I registered last night to get more involved in the forums but I have been lurking around for a few years now. I was browsing the forums to see if someone had figured out a way to minimize speed wobbles and that's when I came by your thread about using an electric damper from a bike. I ordered my steering damper right after reading through half of [that thread](http://www.electric-skateboard.builders/t/trampa-truck-steering-dampening/38970/18). :smile: 

I was not able to find cheap electric ones at that moment and the radial dampers cost 3 times more than the axial dampers. That's why I went for the axial one, with the added benefit that it is easier to mount because no CNC'd parts are needed as it mounts right onto my ATS 12 truck's brake attachment screw hole.
It took 30 minutes to mount the damper. Half of that was for figuring out if my wheel would hit it in tight turns or if a crack would form in my deck after drilling a hole in the deck and mounting it there.

I checked out @Nowind's and [that Korean guy's version](https://www.youtube.com/watch?v=aACAE_WaZEs) of using a damper before coming up with this. 

It is safe to say that this system works perfectly because of the huge improvement in rideability on my board. I was in a hurry just now trying to catch my train and was riding with the damper's setting on minimum and it was a lot wobblier than with the damper's setting on 40% - 50%. It did not feel comfortable at all going that fast without damping. :sweat_smile:

Also, I am not sure if using dampers is a good idea when you end up riding on an uneven terrain. Stiff axles might make a ride harder to control. Having a system that can be turned down easily is handy at those moments.

The damper however does move around it's axis since it uses heim joints. When going over uneven terrain it bounces up and down. I should use a damper to dampen that wobble too. :grin:
```

---
## \#7 Posted by: Okami Posted at: 2018-06-16T11:24:13.912Z Reads: 218

```
Cool implementation. Thanks for bringing this out.

This does seem like a really nice, low cost solution on how to improve stability..

As i understand it is enough with just one dsmper and the rod moves both ways?
```

---
## \#8 Posted by: raz Posted at: 2018-06-16T11:49:10.367Z Reads: 203

```
[quote="Okami, post:7, topic:59066"]
This does seem like a really nice, low cost solution on how to improve stability…
[/quote]

One damper should be enough. When the front truck is corrected the back one will follow. You could add second damper but the added benefit will not be as noticeable as with the first one (just my theory).
If mounted correctly it will be able to move back and forth.
```

---
## \#9 Posted by: skatardude10 Posted at: 2018-06-16T14:10:57.433Z Reads: 195

```
Wouldn't the dampener be better mounted on the rear? Curious...
```

---
## \#10 Posted by: raz Posted at: 2018-06-16T14:49:14.041Z Reads: 200

```
It depends. If you stand on your board and you move you ankles you'll see the trucks rotate. Depending on which truck rotates most that's the truck you want the damper mounted on to.

In my case my rear truck is very stiff, the front one is loose. This minimizes the chance for speed wobbles a bit but still allows me to turn. That is the main reason why I have my damper in the front.
You could have it in the back though.

I turned my rear truck on the lathe so that I may mount the motors easily. I do not have the brake mounting screw holes anymore. This means that I would have to mill a new part to mount the damper. It is easier to just mount it in the front in my case. And I am able to attach the damper very close to my one of my wheels in the front, as there are no sprockets there. That way I am able to get more travel in the damper. More travel means more damping work ( Work = Force * Distance).
```

---
## \#11 Posted by: skatardude10 Posted at: 2018-07-05T21:37:52.101Z Reads: 155

```
Okay, I've spent all week improving my mounts for this steering damper incrementally eliminating flex in the nylon mounts. You can look at the progress in my [build thread starting with this post.](https://www.electric-skateboard.builders/t/the-demonseed-tb-218-tb-6374s-190kv-tb-mounts-chibattery-10s4p-dual-focboxes-superflys/50610/48?u=skatardude10)

Took it out for a test ride mounted to the rear with all the improvements up to this point. 

I can't see why all downhill / fast e-boards don't do this. It's so simple to do, and cheaper than a new set of bushings (as long as you aren't printing 10+ revisions on the mounts, chewing through nylon and rit dye like I have). Even with the hardest chubbies out there, you are still going to have a little bit of wiggle on center, which this completely eliminates.

Here are some quick impressions:

* I get the feeling that my rear truck grips a whole lot better now
* Wobbles are nearly impossible to induce
* With stiff mounts, the damper can really do it's job
* I feel more stable driving my eboard at 35mph than I do driving my car... It's an odd feeling
* I get the sense 5x more that I am riding a superbike that is locked in during straights, turns, hard carves, hard braking... But the ride *really shines* in long drawn out high speed turns and straights
* Perfectly complements 93a wfb chubbies, eliminates the small bit of looseness on center, which I think is why it shines so much on straights and long drawn out high speed turns.
* Rebound from bushings is still there to return you to center along with your own weight in and out of turns, but the adjustable damping is just *heaven* on the rear with no unpredictable snaps back to center unintentionally, locking you to the road. 
* Really, if you are going fast, this is something you have to feel. I don't see how this couldn't be a feeling everyone enjoys, but I'm sure there are people out there that won't like it... I'd attribute that to denial more than anything though, holding that as a personal belief.
* You can still lean and turn as tight as without a damper. 
* You can even essentially turn the thing off if you want. 
* The front truck not dampened means you still have 100% of your agility that you had before
* This isn't a feeling I thought a longboard could have... Feeling like an ultra stable, yet agile superbike, but still able to just turn a knob and feel like it did before.... 

In summary, I see nothing lost by adding this and so *so* **SO** much gained by adding it to my setup. I can't stress this enough... To me this feels like, almost better than sex feeling such confidence at high speeds. Sure I can *become a better skater* and learn to deal with wobbles and instability without a damper... But if I or you have already done that, have already dialed in your ride just right with the perfect angles, bushings, etc... Why not make your board ride just as good but simply remove any potential instability from the equation all together? This just dialed my setup in even better. Got the right duro bushings, don't want to over torque them to go fast, but want adjustability to be as stable as you want at any time? That was the situation I was in and now that problem has been solved for me.
```

---

# First Build &#124; Mountain board &#124; mbs pro 97 deck &#124; Single alien 130kv 6374 &#124; 12S lipo &#124; VESC &#124; alien all terrain trucks + wheels

### Replies: 17 Views: 2102

## \#1 Posted by: Kogtail Posted at: 2017-08-02T23:15:20.227Z Reads: 285

```
Hi guys, this is my first build and my first post here. Please help to check my component selection and see if I am getting anything wrong or missing anything. Thank you :slight_smile:

I am looking to build an electric mountain board mainly for street in bad condition (holes, bumps, rocks etc). Not going dual drive because of the price. 
I calculated that I can reach ~35 km/hr (22 m/hr) top speed with a range of ~50 km (~31 m/hr)
which is more than what I want. 
Currenty cost is around $900 USD including everything on this list and I would like to spend no more than this.

Deck: MBS Pro 97 deck [bought]
[https://www.mbs.com/parts/11404-mbs-pro-97-deck-dylan-warren](https://www.mbs.com/parts/11404-mbs-pro-97-deck-dylan-warren)

Wheels, trucks, motor mounts, drive pulley :
2x 200x50mm (8 Inch) front wheels
2x 200x50mm (8 Inch) with built in drive pulley HTD5 72T 15mm wide2x motor pulley HTD5 15T 15mm wide, 3mm key
2x HTD5 Belt 395mm, 15mm wide
2x Motor mount (50mm and 63mm motors)
1x front truck
1x rear truck for motor mount fitment
[http://alienpowersystem.com/shop/cnc-kit/aps-all-terrain-transmission-kit-200x50-wheels/](http://alienpowersystem.com/shop/cnc-kit/aps-all-terrain-transmission-kit-200x50-wheels/)

Single Motor:
Alien power system 6374 130kv 3200w
[http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-130kv-3200w/](http://alienpowersystem.com/shop/brushless-motors/alien-6374-sensored-outrunner-brushless-motor-130kv-3200w/)

Batteries:
two 6s1p 10c 12000mAh in series to make 12s1p(?)
[https://hobbyking.com/en_us/multistar-high-capacity-6s-12000mah-multi-rotor-lipo-pack.html](https://hobbyking.com/en_us/multistar-high-capacity-6s-12000mah-multi-rotor-lipo-pack.html)

or
two by two 5s1p 25c 5000mAh: 
[https://hobbyking.com/en_us/zippy-compact-5000mah-5s-25c-lipo-pack.html](https://hobbyking.com/en_us/zippy-compact-5000mah-5s-25c-lipo-pack.html)

Remote Controller: [bought]
torqueboards-2-4ghz-mini-remote-controller/
[diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/](diy-electric-skateboard-kits-parts/torqueboards-2-4ghz-mini-remote-controller/)

Speed Controller: [bought]
Vesc

Battery charger, Indicator and : no idea yet

Anti Spark, connectors and wires: don't know yet, will shop in some local electronics shop
```

---
## \#2 Posted by: jammin Posted at: 2017-08-02T23:30:57.377Z Reads: 247

```
I'd recommend getting batteries with a higher discharge rating. Most 12s lipo build are done with 3x4s or 4x3s lipo packs, not 2x6s. Why? The former options will have a lower profile on your deck.

If you wanted a similar mAh, (as an example) you'd buy eight 3s packs: https://hobbyking.com/en_us/zippy-compact-5000mah-3s-25c-lipo-pack.html
The higher discharge rating, the better; I'm running 20C with 2x5s in series with no issues (riding on flats). Then again, if you're gonna run 12s with 12Ah, that's 532.8 Wh. That's quite a lot!!! At that rate you _might_ want to look into li-ion packs.

You can charge anything <=6s with a hobby lipo charger, like the iMax b6. Hope that helps, and good luck!
```

---
## \#3 Posted by: JLabs Posted at: 2017-08-02T23:53:28.776Z Reads: 230

```
Looks pretty good! I have the exact same remote available for half the price :wink:

https://buildkitboards.com/products/mini-remote
```

---
## \#4 Posted by: sl33py Posted at: 2017-08-03T00:06:23.217Z Reads: 218

```
Or better yet get GT2b and put in your own 3d printed smaller enclosure.  Most reliable remote of those I've tried.

Now someone should post up a used matching remote for less than JLabs!  :stuck_out_tongue:
```

---
## \#5 Posted by: Kogtail Posted at: 2017-08-03T00:10:17.229Z Reads: 204

```
Thanks a lot for the recommendation!

Regarding the batteries, how does two by two 5Ah 5S 20C lipo sound? they add up to 10Ah 10S 20C right? 
I am okay with the range of 36.6km with this new battery set up
And is your recommendation about getting li-ion packs instead because of safety reasons?
```

---
## \#6 Posted by: Kogtail Posted at: 2017-08-03T00:10:57.653Z Reads: 193

```
too bad I already bought the remote together with the vesc with a friend from torque haha thanks though
```

---
## \#7 Posted by: jammin Posted at: 2017-08-03T00:13:21.506Z Reads: 194

```
Yup you're exactly right... except it'll be <b>5Ah 10S1P</b>. Li-ion is a better battery technology (imo), more charge cycles and a better form factor for esk8.

I'm running lipo (as do many others) with no issues. but with your past setup, it was gonna be such a pain in a** to charge (with that many cells) that it makes more sense to get a BMS at the very least.
```

---
## \#8 Posted by: Kogtail Posted at: 2017-08-03T00:17:44.218Z Reads: 187

```
5Ah? hmmm shouldn't it be 10Ah since I have 4 batteries in total, 2 sets of "2 batteries in series" in parallel?
```

---
## \#9 Posted by: jammin Posted at: 2017-08-03T01:15:39.572Z Reads: 188

```
sorry my b, I didn't read two by two! Yes you're right :) before buying your batteries make sure you have the space for all of them on your deck
```

---
## \#10 Posted by: ATLesk8 Posted at: 2017-08-03T21:10:31.359Z Reads: 177

```
I got the mini remotes on ebay for $18 shipped... @JLabs

http://www.ebay.com/itm/2-4GHz-Radio-Remote-Controller-Receiver-Binding-Plug-For-Electric-Skateboard-/262779892776?hash=item3d2ee6f428:g:G2kAAOSw9GhYYjLd
```

---
## \#11 Posted by: JLabs Posted at: 2017-08-03T21:25:01.264Z Reads: 168

```
You also posted a topic saying you couldn’t get it to work :wink:

 http://www.electric-skateboard.builders/t/remote-not-pairing-correctly/26764/

Not to mention you have to wait 3-4 weeks for delivery.. @ATLesk8

 My remotes come tested and pre-bound to the receiver. No tricky set up required,. You also get customer support and you support an eSk8 business that actually contributes to this community..
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-08-03T22:20:55.887Z Reads: 156

```
Hahahaha For the win!!
```

---
## \#13 Posted by: ATLesk8 Posted at: 2017-08-04T02:04:47.922Z Reads: 152

```
@JLabs maybe you should actually read the thread to the part where I solve the issue and it is the faulty vesc. I'm currently using 3 of these ebay remotes...ftw...hehe
```

---
## \#14 Posted by: mtgawesome Posted at: 2017-08-06T00:43:05.530Z Reads: 142

```
So do they work well now?
```

---
## \#15 Posted by: ATLesk8 Posted at: 2017-08-06T01:00:53.492Z Reads: 143

```
Yup...they all work fine and bind on first try. I dont like that I have to change batteries or the overall design of the remote but they have seemingly been the most reliable for me so far vs the nano and benchwheel.
```

---
## \#16 Posted by: StormTrooperBert Posted at: 2017-09-11T03:03:19.367Z Reads: 131

```
Hey don't mean to hijack but can anyone tell me if I've got anything to worry about here (aside from the obvious. Clearance under deck, insane top speed etc) I'm running a single 190kv 6374 SK3, Torque VESC, 90mm wheels, 16:32 gears and I just ordered 2 6s 8000 mah lipos I'll be running in series. I'm upgrading from 2 3s 5000mah lipos in series. Anything other than changing battery voltage cutoff start and end? Do I need to re-detect motor? Set any other parameters? Just wanna make sure I don't damage my VESC or any other components. Thanks in advance anyone!!
```

---
## \#17 Posted by: DanSkates Posted at: 2018-04-09T14:37:15.463Z Reads: 72

```
Hey dude!!  Did you ever manage to get this beast put together?
```

---

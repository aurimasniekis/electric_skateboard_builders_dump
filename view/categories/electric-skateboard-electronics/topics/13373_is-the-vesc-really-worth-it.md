# Is the vesc really worth it?

### Replies: 22 Views: 2178

## \#1 Posted by: Charster10 Posted at: 2016-11-20T16:43:17.571Z Reads: 212

```
Right i know this sounds stupid but seriously:

Basically i have a cheap crappy esc from hobbyking now which works ok but the breaks are unreliable and so weakkk. Ive wanted to upgrade to a vesc for a while now and i have a place where i can get them for £90 so do i get one or not? Can someone explain the full difference as is it worth spending that much to upgrade? Please tell me if its worth it or not aha.

Also do you recon i should wait a while after getting the vesc and get a Benchwheel remote for £33 or a GT2B £23 and mod it? 

Please let me know guys! Cheers!
```

---
## \#2 Posted by: chinzw Posted at: 2016-11-20T16:59:39.627Z Reads: 206

```
The VESC is superior in every way compared to a hobby esc. Once you ride a board with a VESC you will never go back to a hobby esc. You should get the Mini Remote or gt2b and mod it.
```

---
## \#3 Posted by: Charster10 Posted at: 2016-11-20T17:10:51.735Z Reads: 202

```
@chinzw are the breaks noisy using the vesc?
```

---
## \#4 Posted by: evoheyax Posted at: 2016-11-20T17:11:57.536Z Reads: 199

```
The VESC can protect your other electrical components by setting limits. It protects itself with heat limits. It protects the battery with a max battery current limit, it protects your motors with a max motor current limit, and if you don't like your brakes, you can make adjustments to make it better (they will take soe researching though as it's not the easiest thing to get right. These limits can all be changed in the settings too. Regen in the VESC means your batteries recharge while braking. Most ESCs working in BLDC mode, and the vesc can do BLDC better than hobby grade ESCs, but also FOC mode, which uses sinusoidal waves instead of trapezoidal waves. The result is near silence and a tiny bit better torque. FOC is mathematically superior to BLDC.

These are the main reasons for going with the VESC. You could argue now also with bluetooth module and app systems like the one I've built, you can also see everything that's going on in your vesc. The beauty of all of this, is you can see what's going on, and make the appropriate setting changes and hardware/gearing changes to make your ride better.

I would recommenced the GT2B and modding it if you feel comfortable doing the mod. I don't know if you can find one near you but I highly highly recommend the mini trigger remote also. By far, the best remote right now IMO besides the GT2B in terms of easy to set up, reliable (no dropouts), batteries for weeks of riding without replacing.
```

---
## \#5 Posted by: Charster10 Posted at: 2016-11-20T17:14:48.130Z Reads: 183

```
@evoheyax thanks for your reply. I see so the vesc is totally worth it. Ive seen some people completely mess up there vescs in foc mode though is that true? If it will be fine then ill order my vesc literally now haha. Also is the vesc noisy when breaking?

Also what would be wrong with the benchwheel remote?
```

---
## \#6 Posted by: evoheyax Posted at: 2016-11-20T17:27:02.692Z Reads: 172

```
Yes, a lot have messed them up in FOC. It is possible to break it, even if you configure it correctly. This is why I recommend chaka vescs. 2 year warranties (even if you fuck it up), never had a single issue with any of the 8 I have from him, But they are a bit more exspensive.

They are really quite breaking wise.

I have no experience with the benchwheel remote, so I can't speak.
```

---
## \#7 Posted by: Charster10 Posted at: 2016-11-20T17:35:17.085Z Reads: 170

```
Ah ok i see. Should i just stick in bldc mode then as its my first one as they probably wont offer a great warranty where im getting it from. Also correct me if im wrong foc mode is just basically a "quite mode" ?  @evoheyax
```

---
## \#8 Posted by: saul Posted at: 2016-11-20T18:08:28.069Z Reads: 160

```
foc is alot more than silent mode, but that is what you'll notice most.
I use it with a carvon hub because it works and feels like a regular board that never stops aka perfect.

but bldc noise is really fun too on a belt drive. it adds to the experience like a motorcycle screaming at you to go faster.....

and no it does not have "Brake Noise" in either mode. a bit of squeek at low speed on bldc but nothing compared to those hobby king things.....

just buy one already. its probably the single biggest improvement you can make for <$100 (<50 if you started with it...)
```

---
## \#9 Posted by: Charster10 Posted at: 2016-11-20T18:44:06.167Z Reads: 145

```
@saul thanks for your reply. Totally understand. Im just worried about whats the chances something will mess up in foc against bldc? Whats the safest option in your opinion?
```

---
## \#10 Posted by: hunter Posted at: 2016-11-20T18:53:20.723Z Reads: 143

```
might be a stupid question, but foc and bldc????? I am right were you are Charster10 =). My Hobbyking ESC is not all crap, but like the thought of 10s more then 6s =)
```

---
## \#11 Posted by: saul Posted at: 2016-11-20T19:06:40.738Z Reads: 142

```
I've only heard of problems with foc on older hardware versions.

for now I use bldc on belt drive, foc on hubs.

@hunter FOC and BLDC are different control modes for the vesc and brushless motors in general.
Bldc is standard what most esc's use.
FOC is a fancy math algorithm also called vector control. 
 https://en.wikipedia.org/wiki/Vector_control_(motor)

again the most noticable difference is on FOC is the silence, since the fets are switched at 30khz which is well above the 20hz -20khz most animals can hear.
```

---
## \#12 Posted by: Charster10 Posted at: 2016-11-20T19:13:20.181Z Reads: 131

```
Im on a belt drive so ill stick to bldc i think. Cheers for your help @saul
```

---
## \#13 Posted by: hunter Posted at: 2016-11-20T20:34:15.978Z Reads: 128

```
thx for the infomation =)
```

---
## \#14 Posted by: Namasaki Posted at: 2016-11-20T22:32:14.783Z Reads: 115

```
@hunter
I started with expensive 12s hobby esc's designed for e-boards and still, when I upgraded to Vesc's the difference was amazing.
Even in BLDC mode the Vesc is quieter.
Throttle is so much smoother and linear.
Brakes are so much more dependable, predictable, smoother and linear.
If you spend the extra to get a Chaka vesc then your safe trying FOC but if you buy a cheap vesc that doesn't have upgraded components then I would keep it simple and stick with BLDC.
Also be carful about staying below the Vesc's erpm limit buy not using too high a KV motor with too high voltage.
example: I run 190 kv motors at 10s voltage. It is below the 60k erpm limit and it is very dependable.
```

---
## \#15 Posted by: racidon Posted at: 2016-11-20T22:54:13.792Z Reads: 105

```
It is, but like many other things, if it's cheap, it's likely crap, I went through 3 VESCs before just spending right amount on a chaka vesc which hasn't failed me at all in the slightest. It actually performed better than the others too
```

---
## \#16 Posted by: hunter Posted at: 2016-11-21T07:49:17.376Z Reads: 87

```
I Got the 190 kv aswell, and was thinking of 10 setup 😀, better go find a good Vesc then 😉
```

---
## \#17 Posted by: Namasaki Posted at: 2016-11-21T12:42:29.596Z Reads: 85

```
Spend a little extra and get the heat sink option. 
It's well worth it.
```

---
## \#18 Posted by: Mrmoonlight Posted at: 2016-11-21T14:00:06.664Z Reads: 75

```
Chaka's VESC's are the real deal. I got the heatsink option and even though I have larger heatsinks on my other VESC's, Chaka's still runs noticeably cooler.
```

---
## \#19 Posted by: treenutter Posted at: 2016-11-21T14:36:14.724Z Reads: 69

```
@Charster10 yes it's absolutely worth it.
```

---
## \#20 Posted by: Bazingazunga Posted at: 2016-11-21T14:43:52.742Z Reads: 64

```
Where are you finding them for £90 man? @Charster10
```

---
## \#21 Posted by: Khaleel Posted at: 2016-11-21T15:04:50.563Z Reads: 60

```
Yeah where are the £90 ones?!? I have only seen them for $150/$170...
```

---
## \#22 Posted by: Charster10 Posted at: 2016-11-21T15:10:35.140Z Reads: 59

```
Aliexpress. The maytech ones
```

---

# VESC Set UP For Dual 6380s

### Replies: 7 Views: 147

## \#1 Posted by: ghols Posted at: 2019-12-22T23:59:15.549Z Reads: 51

```
Hey guys, 

I was wondering if you guys would be so kind as to look at my vesc settings and tell me if I'm going to burn up my vesc. So I finally got my build assembled and went through the vesc tool to set it up. I originally wanted to set it up in BLDC mode, but new tutorials recommend the FOC wizard, so I set it up in FOC. Well, from what I've read, 12s can be a problem for FOC so I'd prefer to be safe in BLDC mode. Anywho, here are the stats and the max amp settings I set up, because tbh it's what I'm worried most about. I've also limited the max erpm to 50000. Or if any of you guys have a similar rig that you've configed, it'd be super helpful to learn what you guys did. 

Motors - two 6380's with max amp capacity of 80 amps each
12s4p battery with 60 amp continuous discharge 
Flipsky Dual VESC 6.6

Any help is appreciated. 
![vesc%20capture|690x399](upload://s1cJ7WX8uUHfYBc3jztLXCCq6f8.png)
```

---
## \#2 Posted by: Soflo Posted at: 2019-12-23T00:41:58.820Z Reads: 48

```
You need to split the battery voltage in half for each esc.  A 12s4p from 30q cells is only capable of 60a discharge total.  So to be safe you'd need to lower each esc down to 30a battery. Also I'd do the same with the brakes. Split that 15 in half for each esc.  
I run the same exact setup hardware wise and I run 70a motor,  -55 current max brake, 29a current battery max,  and -8a battery current max regen. I have zero problems and run my setup hard and fast
```

---
## \#3 Posted by: ghols Posted at: 2019-12-23T00:47:50.136Z Reads: 47

```
Ok gotcha. So, when I limit the battery current to say, 30 each, will the esc put that as a hard stop, or will it still burst up to 60 amps each under times of extreme load?
```

---
## \#4 Posted by: Haze-Gray Posted at: 2019-12-23T15:11:41.458Z Reads: 37

```
Good Question! I have a similar setup and ran foc wizard to configure. Motors - flipsky 190kva two 6374’s with max amp capacity of 60 amps each 12s1p 2 of these in series [Tattu 28000mAh 22.2V 25C 6S1P Lipo Battery Pack with AS150 +XT150 Plug](https://www.genstattu.com/tattu-28000mah-22-2v-25c-6s1p-lipo-battery-pack.html))battery with 120 amp continuous discharge supposedly totally fine by manufacturer and Flipsky Dual VESC 6.6.. i was cruising at full speed saturday and after a few minutes started getting heat throttling. at 30.8 mph, not fun so recommend avoinding if possible. Maybe redo motors with bldc and or limit to 50 amp per? esc and batteries should be able to handle it np but not sure why motors overheating at or near full power for any lenght of time. not that i need to go 30+ but bigger boy so need the power to get moving lol geared 66:14...
```

---
## \#5 Posted by: Soflo Posted at: 2019-12-23T16:31:10.893Z Reads: 31

```
@ghols, it'l basically hold at that power setting. It will not hit the brakes or shut off. When you set a current limit,  it will not go over that limit.  If it did you could destroy your battery.
```

---
## \#6 Posted by: Soflo Posted at: 2019-12-23T16:33:21.922Z Reads: 31

```
Now if you set your limits too high like you had them,  you can overtax your batteries bms and cause it to shut down.  This will stop all current to the escs and probably cause you to fall.
```

---
## \#7 Posted by: ghols Posted at: 2019-12-26T03:44:51.703Z Reads: 19

```
Thanks for your input guys!

Does anyone have a good tutorial on set up in BLDC mode in the new VESC tool interface?
```

---

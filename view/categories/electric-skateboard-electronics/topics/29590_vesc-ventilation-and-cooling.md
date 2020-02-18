# VESC ventilation and cooling?

### Replies: 8 Views: 1610

## \#1 Posted by: filipandre95 Posted at: 2017-08-03T16:43:09.583Z Reads: 250

```
Hi, im building my own compartment for the VESC and battery and wondering if it needs some sort of cooling?
I dont want any holes that let dirt get inside. If I want to mount a small 12v fan with dustfilter, how would I power it the best way? Im using a 12s3p (50,4v) batterypack.
Do you guys use any cooling for the VESC?
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-03T17:01:58.182Z Reads: 250

```
Cooling's not really needed. VESCs have a temp sensor and can shutoff if it gets too hot anyway. Try it out and if you find it's shutting off, you can deal with heat later. Shouldn't really be a problem unless you're running a single uphills in a hot environment.
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-08-03T19:10:36.482Z Reads: 231

```
Yup, @Jinra is spot on
```

---
## \#4 Posted by: evoheyax Posted at: 2017-08-03T19:33:21.174Z Reads: 222

```
I used to think it was super important. But it really just depends on how many amps your going to run the motor at, plain and simple. A 4.12 can do around 32 con, FOCBOX and VESC 6 are 60 con, and Chakas new heat sinked and direct fet 4.12 can do 70 con.

Anything less than that number is fine, anything higher will heat the vesc up. You don't want to average this number really, and many won't. But it depends.

**Things that could cause larger amp draw, and thus, make it more likely to need a heatsink or cooling:**

- Mono drive
- Rider Weight is high (more than 140 lb)
- You ride large wheels (107mm+)
- You run at a lower voltage (standard is 10s or 12s, 6s is more likely)
- Lots of hills (10% grade constant, 20% grade or high at times)
- For belts, In-efficient gearing with the kv
- For hubs, in-efficient kv (> 120 or < 60)

If you are going check check and check, you should think about heatsinks. If not, your probably ok.

Dual drive or even 4wd really helps spread out the heat. Just because your not hitting the heat limit in your daily commute, doesn't mean your not putting more wear and tear on your board because of the higher heats than dual or 4wd.

I am actively working on a set of heatsink designs for the 4.12 so those out there can do higher amps with their 4.12 vescs.
```

---
## \#5 Posted by: filipandre95 Posted at: 2017-08-03T19:48:48.354Z Reads: 214

```
Thanks @evoheyax, this makes me think I need to get dual drive. I have the 4.12 VESC and it cant really push me up hills like my Alien ESC could. I have a extra motor and motor mount so I think im gonna go for it.
```

---
## \#6 Posted by: sl33py Posted at: 2017-08-03T19:56:33.797Z Reads: 201

```
you can add a heatsink to help cool it a bit, or give it a heatsink to load up with heat before it starts to cut power due to temperature.  Easy to do yourself w/ basic tools:
http://www.electric-skateboard.builders/t/how-to-heatsink-your-vesc/26129
Added bonus a flat and more secure way to mount.  Con - it's thicker so might not fit in a slim case.

HTH - GL!
```

---
## \#7 Posted by: evoheyax Posted at: 2017-08-03T22:17:22.395Z Reads: 175

```
You are somewhat limited with the 4.12. Besides the FOCBOX and VESC 6, it's the best ESC, don't get me wrong. But it is better in configs higher than 1 motor. Single drives, I would say get the FOCBOX instead. Unless of course, you've got a nice heatsink.
```

---
## \#8 Posted by: filipandre95 Posted at: 2017-08-03T22:45:16.863Z Reads: 161

```
I just orderd one more VESC. I also have some heatsinks. Im gonna add the other motor in the front. will be a total of 6500Watt! Lets climb some hills! :smile:
```

---

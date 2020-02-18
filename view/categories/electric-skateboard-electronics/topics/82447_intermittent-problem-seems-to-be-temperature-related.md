# Intermittent problem seems to be temperature related

### Replies: 5 Views: 122

## \#1 Posted by: Goonman Posted at: 2019-01-29T03:37:06.899Z Reads: 44

```
2 Almost brand new Maytech MTO6374HAC motors run by focboxs and lipo 12s. I know there is no problem with current supply. One motor getting slightly hotter than the other. After about 5km Rh 53c LH 48c measured from the can. At this point a sought of stumble occurs kind of like a missing phase connection but not so aggressive and kind of like it's coming from only one motor. Unloaded everything works fine. Can't see anything wrong no loose connection or arcing or sparking. Sat looking everything over and motors cooled down to somewhere near ambient ie motors were 35-37c ambient about 32. I don't have ackmaniac app unfortunately.
Could it be just the thermocouple temp and focbox cutting power?
Vesc settings battery 30amp 60amp motor 130amp max. Not even pushing hard or going max speed.
Is 50deg C going trip any thing? I know the stator and winding will be hotter but why so hot anyway.
Change of setting suggestions.
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-01-29T03:46:20.519Z Reads: 36

```
I would guess you have the ESCs set to traction control over CANbus, which means one motor is the "master" and one is the "slave", and thus the master will get hotter than the slave. That combined with the temperature sensor in the motor means it'll start throttling the hotter motor.

I'd guess you have something in your setup that's causing undue drag, possibly belts too tight.
```

---
## \#3 Posted by: Goonman Posted at: 2019-01-29T03:49:49.133Z Reads: 32

```
Yeah that's right traction control over can bus. Possibly slightly different from one side to other in terms of tension. It does 'feel' different. It's chain drive and there is plenty of slack.
Why is it too hot? Surely it's not too hot to put it in danger. I will probably just change the temperature throttle limits then.
Thanks
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-01-29T03:54:22.084Z Reads: 28

```
53C on the can means significantly hotter in the core. For just tooling around on flat ground, it should be a lot cooler than that. The default limit is 80C if I recall correctly. I'd look at your settings and see if there's anything weird in there that could result in such extreme heating - I'd check your ERPM difference for traction control, make sure it's not too small.
```

---
## \#5 Posted by: Goonman Posted at: 2019-01-29T04:13:58.131Z Reads: 23

```
Hmm ok. What should they be? I think I have it 1000. I think VESC normally has it at 3000. I can't remember why I changed it or why it matters.
I will increase it see if it makes a difference.
```

---

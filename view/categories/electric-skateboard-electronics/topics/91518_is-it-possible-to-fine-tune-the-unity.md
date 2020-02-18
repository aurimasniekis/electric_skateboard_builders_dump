# Is it possible to fine tune the unity

### Replies: 14 Views: 503

## \#1 Posted by: Becksy21 Posted at: 2019-04-23T17:59:24.597Z Reads: 135

```
Hi everyone, I finally got my first build out yesterday it’s a haggy set up with a evo deck and 147 pneumatic wheels and I’m using the maytech v2 remote coupled to the unity powered by a Samsung s12 5p battery ![image|375x500](upload://eR8q0R89cp6hP08ncyaNcEBsBvX.jpeg) ![image|666x500](upload://nG6SMdq7F2iLnjCjUHHJflDliC5.jpeg) 
It performed really well the only gripe I have is the acceleration is off the scale for me and if I take my thumb off the remote suddenly it gives one hell of a jolt infact if I’m really careful and ease off the thumb control it’s still sketchy I’m only used to using the mellow which is quite user friendly compared to this, my question is can I fine tune it to be more forgiving or do I need a different remote? I’ve also used it with 97mm abec flys and it was a similar experience any advice would be great 
Thanks bobby
```

---
## \#2 Posted by: venom121212 Posted at: 2019-04-23T18:12:15.631Z Reads: 134

```
Check out the throttle curve feature under the advanced throttle config

![Screenshot_20190423-141233|236x500](upload://psXhYcpXuIjfQeMekCSxIFZR6Iy.jpeg)

You could also turn down your motor current settings
```

---
## \#3 Posted by: rsalmon Posted at: 2019-04-23T18:33:42.094Z Reads: 122

```
[quote="Becksy21, post:1, topic:91518"]
if I take my thumb off the remote suddenly it gives one hell of a jolt
[/quote]

This is a VESC thing unfortunately. Not Unity specific.

You can increase the "Negative Throttle Ramping Time" parameter to 0.3s it should smooth it out a little bit.

Unfortunately, changing this parameter comes at a cost. When you use your brakes, the input will be slightly delayed. You can test different values and see what works best for you. Me personally, I wish this parameter would only affect the ramping time from X Throttle to Zero throttle.. not from X to -X.
```

---
## \#4 Posted by: Becksy21 Posted at: 2019-04-23T18:34:46.049Z Reads: 118

```
Thanks for the info, will I be able to do all the settings over Bluetooth with a android phone? 
I’ve no previous experience with programming a skateboard so any explanation on how one thing affects the other would be great 
Thanks bobby
```

---
## \#5 Posted by: brenternet Posted at: 2019-04-23T18:42:41.162Z Reads: 110

```
You can adjust your curve on your phone, much like ladies do for instagram selfies :grin:

Before you get going though, have a search on the forum for curve threads, they will help you understand how it all works and what you're getting in to.

https://www.electric-skateboard.builders/search?q=throttle%20curve
```

---
## \#6 Posted by: never4getf150forums Posted at: 2019-04-23T18:44:30.924Z Reads: 104

```
what you are feeling when you accelerate and let off the throttle quickly is not something vesc related, however related to your setup.

the tires and belt drive with big ass motors create more drag then you seem to be used to, especially compared with a mellow hub drive that can coast much much easily.

so no way to "fix" it unless you go direct drive, and make the tire completely urethane.. just something you will have to get used to, ease off the throttle don't just let off 100% after hard accelerations.
```

---
## \#7 Posted by: rsalmon Posted at: 2019-04-23T18:52:20.983Z Reads: 99

```
[quote="never4getf150forums, post:6, topic:91518"]
what you are feeling when you accelerate and let off the throttle quickly is not something vesc related, however related to your setup
[/quote]

The setup certainly plays a role, but it actually is vesc related. It happens on urethane belt combos as well.

As an example, the Boosted board ESC smooth out this kind of transition and does not give the jolt.
```

---
## \#8 Posted by: brenternet Posted at: 2019-04-23T18:58:10.426Z Reads: 90

```
[quote="rsalmon, post:7, topic:91518"]
Boosted board ESC smooth out this kind of transition and does not give the jolt
[/quote]

The boosted ESC only needs to deal with one set of hardware bom, factory settings and predicable riding environments. DIY vesc's cater to a millllllion different board styles, terrain styles and belt/gear/DD combo's.

Configuring the vesc to artificially compensate for thane belt drag would destroy a pneumatic MTB build ride as an example. So yes, prebuild manufacturers will be smoother, that's the nature of DIY :slight_smile:
```

---
## \#9 Posted by: rsalmon Posted at: 2019-04-23T19:02:31.271Z Reads: 84

```
[quote="brenternet, post:8, topic:91518"]
The boosted ESC only needs to deal with one set of hardware bom
[/quote]

Yes, absolutely. I wasn't arguing otherwise.
Was just giving an example.
```

---
## \#10 Posted by: never4getf150forums Posted at: 2019-04-23T19:07:13.855Z Reads: 81

```
i'd think the belt/pneumi drag is more impactful to the "jolt" then the firmware is. comparing a boosted drivetrain to pneumi setup are very far apart.. you can kickpush a boosted, but kickpushing a pneumi drive train with those big cans + wide belts on it .. :persevere:

but op should still take your advice and see if it improves his experience

i'd say the best bet for op is to swap out the belts, go for half the size in width but keep in mind it will break in around half the time so buy a few spares
```

---
## \#11 Posted by: Becksy21 Posted at: 2019-04-23T19:29:35.771Z Reads: 71

```
Thanks guys I’ve got plenty to experiment with now I’ll get the settings altered and post my findings, I get there’s no magic fix but if I can just get things a little smoother it’d be great 
Thanks everyone you’re input is much appreciated
```

---
## \#12 Posted by: gmurad Posted at: 2019-04-29T00:33:52.095Z Reads: 52

```
[quote="Becksy21, post:1, topic:91518"]
infact if I’m really careful and ease off the thumb control it’s still sketchy I’m only used to using the mellow which is quite user friendly
[/quote]

I second @never4getf150forums in saying that the "jolt" you are describing when letting off the throttle is a mechanical characteristic of your build, it has to do with the drag created by the high gearing ratio. I don't think this can be fixed via software. For example, making the VESC slowly decelerate when the throttle is let off seems like a bad idea.

First time I experienced this I was very concerned, eventually you get used to overcoming this by shifting your balance.
```

---
## \#13 Posted by: RafaelinMissouri Posted at: 2019-05-17T14:46:09.718Z Reads: 41

```
How to you have your throttle curve set up?
```

---
## \#14 Posted by: venom121212 Posted at: 2019-05-17T16:36:30.462Z Reads: 34

```
![Screenshot_20190513-213024|236x500](upload://4aaCH1PhHSJE3WVuf2vXf2DWzCe.jpeg)

Linearly with a bigger delay in positive throttle ramping time.
```

---

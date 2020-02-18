# Focbox reset on wheel lock up

### Replies: 26 Views: 464

## \#1 Posted by: muchflywow Posted at: 2019-04-08T22:16:34.517Z Reads: 137

```
Hey guys, i have built a mini e dirt bike with a focbox and sensored 6374 motor but I'm having an issue that is probably very specific to me and I'm wondering if anyone has any idea how to fix it.

Issue is, it being a bike the rear wheel sometimes locks up under braking which I'm ok with however this causes the focbox to reset, with no fault codes showing. Is this some sort of safety feature or some sort of fault that's not showing up as a code?

Edit: Under braking i mean, when i apply the disc brakes, not the regen braking.
 ![IMG_20190317_140139|666x500](upload://zvIi69lPgLdAnbK5izKFfoFSJNI.jpeg)
```

---
## \#2 Posted by: b264 Posted at: 2019-04-08T22:23:36.935Z Reads: 128

```
Elaborate on what you mean by "lock up".  Do you mean it's applying brakes?
```

---
## \#3 Posted by: muchflywow Posted at: 2019-04-08T22:36:36.272Z Reads: 123

```
Yes that's why i said under braking
```

---
## \#4 Posted by: b264 Posted at: 2019-04-08T23:00:30.630Z Reads: 118

```
Are you running sensored or unsensored?
```

---
## \#5 Posted by: muchflywow Posted at: 2019-04-08T23:49:05.835Z Reads: 112

```
Do you guys read the post lol?
```

---
## \#6 Posted by: b264 Posted at: 2019-04-08T23:58:58.489Z Reads: 110

```
You said the motor is sensored.  So are you running in sensored mode?  You can run a sensored motor in unsensored, sensored, or hybrid mode.

Also, free advice...
```

---
## \#7 Posted by: muchflywow Posted at: 2019-04-09T00:16:07.670Z Reads: 102

```
I'm running in hybrid bldc mode
```

---
## \#8 Posted by: muchflywow Posted at: 2019-04-09T20:20:24.781Z Reads: 91

```
no one knows? anything? this has literally never happened to anyone?
```

---
## \#9 Posted by: mynamesmatt Posted at: 2019-04-10T00:57:54.484Z Reads: 87

```
[quote="muchflywow, post:5, topic:89855, full:true"]
Do you guys read the post lol
[/quote]

[quote="muchflywow, post:8, topic:89855"]
no one knows? anything?
[/quote]

you're not really helping your case here champ
```

---
## \#10 Posted by: muchflywow Posted at: 2019-04-10T04:16:02.968Z Reads: 83

```
Well he's asking questions that I've already stated answers to in my post
```

---
## \#11 Posted by: mynamesmatt Posted at: 2019-04-10T06:13:23.715Z Reads: 77

```
[quote="muchflywow, post:10, topic:89855, full:true"]
Well he’s asking questions that I’ve already stated answers to in my post
[/quote]
quit the attitude bucko. for the record you **_did not_** answer the questions in your original post that he asked. He's just trying to help, and I'm certain that he knows more than you. if i was @b264 i wouldnt be replying anyway as you don't deserve it
```

---
## \#12 Posted by: robthebuilder Posted at: 2019-04-10T06:52:08.423Z Reads: 73

```
Am I really reading this? :joy: What an attitude for someone who needs help, damn....
```

---
## \#13 Posted by: mynamesmatt Posted at: 2019-04-10T07:06:27.918Z Reads: 73

```
@robthebuilder glad im not the only one seeing it
```

---
## \#14 Posted by: lrdesigns Posted at: 2019-04-10T07:20:22.074Z Reads: 70

```
[quote="muchflywow, post:1, topic:89855"]
Edit: Under braking i mean, when i apply the disc brakes, not the regen braking.
[/quote]

So it resets when you apply the mechanical disk brake? Its not really a use case on skateboards but there must be others using VESCs on bikes. 

We need to see **screen captures of all your vesc settings**, there may be something with them that can fix the issue. 

And how many cells are you using?

I'm guessing  some sort of voltage or amp spike that makes the vesc go ohh shit and it shuts down to protect its self. Data logging would make it easier to figure out.

Also make it repeat the issue, then plug it onto the PC without turning it off and check for errors by typing "fault" in terminal. This should reveal the error.
```

---
## \#15 Posted by: sayekim Posted at: 2019-04-10T10:39:08.936Z Reads: 66

```
It should not reset. 

If I accelerate and then let it free roll it doesn’t reset nor does it do that if I were to foot brake. Maybe it does, I never tried but I don’t see how a mechanical brake would have any effect on the esc at all. 
Maybe since it is a dirt bike you are applying the mechanical brake whilst accelerating in which case it would effect the esc since it might overheat this way.
```

---
## \#16 Posted by: muchflywow Posted at: 2019-04-10T12:52:46.809Z Reads: 63

```
I'm running 12s LiPo so 50.2V fully charged. I'll get some logs but i don't think it's giving me any faults last time i checked.
```

---
## \#17 Posted by: robthebuilder Posted at: 2019-04-10T16:59:05.202Z Reads: 61

```
A voltage spike might be the issue. I'm no expert what so ever but it feels like it might cause a problem if the motor just suddenly stops without a "brake input" to the VESC (focbox). 

Maybe there is even some kind of safety function in the VESC in case the motor seizes or if something is blocking the motor from spinning.

If you apply the two brakes at the same time, will the VESC still reset then? I mean the disc-brake and the regen-brake. If there is no problem then, it might be some kind of safety function that can be disabled.
```

---
## \#18 Posted by: muchflywow Posted at: 2019-04-10T21:43:00.447Z Reads: 54

```
Regen is automatic when i release throttle so it already is braking with both. I think there is some sort of motor stop safety for board riders so the board doesn't just keep trying to spin the wheels in case you hit something. Wish there was an option somewhere but i don't see it to disable anything like that.
```

---
## \#19 Posted by: robthebuilder Posted at: 2019-04-11T09:28:18.028Z Reads: 49

```
So the motor brakes when you let go of the "gas"? Mine doesn't, that's why I ask. It will regen I know, but it won't brake. What if you try to actually use both Brakes at the same time?
```

---
## \#20 Posted by: muchflywow Posted at: 2019-04-11T22:57:20.076Z Reads: 42

```
I thought regen is braking, it's at -20A for regen, i don't have anything hooked up to cause the motor to actually brake so it's disc brake only braking.
```

---
## \#21 Posted by: brenternet Posted at: 2019-04-11T23:04:14.047Z Reads: 40

```
@Deodand Jeff, I know this is a little off topic but can you possibly offer this gent any insight?
```

---
## \#22 Posted by: Blasto Posted at: 2019-04-11T23:12:13.534Z Reads: 39

```
Possibly hitting the over voltage limit, that is determined by the "maximum input" setting. That would cause the focbox to throw a fault and cut the power to the motors in self preservation
```

---
## \#23 Posted by: district9prawn Posted at: 2019-04-12T00:51:04.439Z Reads: 29

```
If the cpu really is crashing and resetting, there should be a watchdog fault code at reboot.
```

---
## \#24 Posted by: robthebuilder Posted at: 2019-04-12T05:42:45.563Z Reads: 27

```
At least on my VESC the motor will regen just by rolling, but the maximum regen set, is used when you brake as hard as possible (regen brake).

The maximum "brake-strength" is set by the "motor min (regen)"- value (-20A in your case). A lower value (like -40A instead of -20A) will give you a harder brake and therefore more regen.

And please guys, correct me if I'm wrong :)
```

---
## \#25 Posted by: muchflywow Posted at: 2019-04-12T19:22:20.356Z Reads: 25

```
Yea i never regen brake if that's a separate function from just letting go of throttle. I think it's programmed to fully regen at 0 throttle, i don't remember it's been a while. Sorry i haven't gotten any logs it's been gross weather in Chicago and i haven't ridden it all week. It's nice outside today and tomorrow so hopefully I'll get some logs and maybe faults.

Thanks for the discussion, we'll figure something out.
```

---
## \#26 Posted by: muchflywow Posted at: 2019-04-17T17:36:52.193Z Reads: 21

```
Ok so this is weird, it's not doing it anymore. I'm getting abs overloads at the weirdest times though. Like after i do a wheelie and as I'm slowly turning around I'll get an abs overload. I think i might have loose wiring somewhere that's causing all these issues. I need to go over all the connections and solder points, even inside the focbox.
```

---

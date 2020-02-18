# Did I do it again?!?&hellip;&hellip; reverse polarisation

### Replies: 47 Views: 388

## \#1 Posted by: epster Posted at: 2019-01-16T14:35:58.360Z Reads: 154

```
Hey guys could you look trough my wiring and check if anything is wired the wrong way. I am getting a negative amperage when i pull the throttle and i have no idea why.

![1547648617837635080341674205554|375x500](upload://wwchisTuV6Ev6Rpk9RwugPPBbkf.jpeg) 
Startibg from vesc rightside of most upper xt90 is plus wired middle xt90  bottom part of plug is plus bottom xt90 rught side is plus wired

![15476487859176792868226646822611|375x500](upload://qIYNJQcDZIKgp4c2qnSmk9n8b3S.jpeg) 
Upper xt90 is plus on upper side of the plug
Middle xt90 has posituve on side where there is a label
Lower xt90 has positive on right side

Oh yeah pls dont look  at the wire colours i know they are wrong haha

Hopefully i didnt fry my esc :sweat_smile:
```

---
## \#2 Posted by: venom121212 Posted at: 2019-01-16T14:39:07.444Z Reads: 142

```
Give some more details on how many batteries you have, use Microsoft paint if you have to. Can't really tell from the pictures to well.

It looks like your middle connector and top connector are both sending positive to that bottom connector
```

---
## \#3 Posted by: epster Posted at: 2019-01-16T14:48:09.596Z Reads: 133

```
I will get on it and go make it in paint!
```

---
## \#4 Posted by: venom121212 Posted at: 2019-01-16T14:51:25.225Z Reads: 126

```
Great, I'll do my best and call in master @b264 if need be
```

---
## \#5 Posted by: epster Posted at: 2019-01-16T15:18:52.869Z Reads: 112

```
Ok i got it this is how it looks. @venom121212 

![new%20circuit%20batteries%20and%20vesc|689x388](upload://nSsFN0hmV1H5fwTCgamGxNrlkMz.png)
I can see why you would want me to show it to you like this haha :smile:
```

---
## \#6 Posted by: JonathanLau1983 Posted at: 2019-01-16T15:29:50.887Z Reads: 99

```
That picture and diagram seems to indicate you have two packs in parallel and then series for the other one.
```

---
## \#7 Posted by: epster Posted at: 2019-01-16T15:31:19.885Z Reads: 99

```
Oh i didnt mean to do that. I made an xt90 series plug looked it up and checked it. and that one workes so if the part on the right is vague. because of the drawing. its just an xt90 series plug for the 2 horizontal batteries to make them in series. :slight_smile:
```

---
## \#8 Posted by: JonathanLau1983 Posted at: 2019-01-16T15:32:07.456Z Reads: 98

```
Is my red line connecting two packs? Negative should lead to positive on the other pack.
![image|394x499](upload://4Grba4sMKvl3kn1G8GlwjwBb5OO.jpeg)
```

---
## \#9 Posted by: epster Posted at: 2019-01-16T15:34:47.143Z Reads: 92

```
Ehm no. The red line you drew is the plug (upper left) coming from the anti-spark in the middle of the board. So that plug has no batteries connected. However the line is going towards the end of a plug where a battery is connected.
```

---
## \#10 Posted by: Benjamin899 Posted at: 2019-01-16T15:36:01.864Z Reads: 90

```
can you make a better drawing?
```

---
## \#11 Posted by: epster Posted at: 2019-01-16T15:39:14.605Z Reads: 88

```
![image|623x500](upload://udvrEAQCRJFLwXmI4iBhTHy7UEa.jpeg) 
Does this help?
```

---
## \#12 Posted by: epster Posted at: 2019-01-16T15:39:34.873Z Reads: 89

```
Better in what way? I am not really experienced with how i should make such a drawing.
```

---
## \#13 Posted by: Benjamin899 Posted at: 2019-01-16T15:41:28.590Z Reads: 88

```
Make it logical, it doesnt have to model reality, just the connections.
```

---
## \#14 Posted by: JonathanLau1983 Posted at: 2019-01-16T15:43:50.060Z Reads: 85

```
If you're sure the series connector you have is correct, and you have the polarity coming out of it right then the rest looks okay.
```

---
## \#15 Posted by: Jumpman Posted at: 2019-01-16T15:45:50.567Z Reads: 84

```
Can you explain what you mean by negative amperage?  Do you mean your motors are spinning in the wrong direction?
```

---
## \#16 Posted by: epster Posted at: 2019-01-16T15:45:55.524Z Reads: 80

```
![image|689x387](upload://8ThDqUEOvt3CR3L7Kkuu0MILCDr.png) 
Better? @Benjamin899
```

---
## \#17 Posted by: epster Posted at: 2019-01-16T15:46:46.242Z Reads: 79

```
No I mean. When i pull the trigger. The metr app says it gets a negative amperage. The amperage goes from 0 to a max of -3.5A trigger fully pulled. So my remote connects, my metr app still works, and I dont have reverse enabled.
```

---
## \#18 Posted by: Benjamin899 Posted at: 2019-01-16T15:52:06.336Z Reads: 75

```
i mean, it looks right, but man this is a weird way to wire them up.
```

---
## \#19 Posted by: epster Posted at: 2019-01-16T15:52:16.897Z Reads: 75

```
I am sorry if i dont answer your guys questions. I try to but some things i just dont understand about electronics.
```

---
## \#20 Posted by: epster Posted at: 2019-01-16T15:53:22.842Z Reads: 72

```
Oh is it? How would you have wired it up then? I was struggling with the 3x 4S so I thought this was the best way to do it. But its good to hear that I have it wired up correctly.
```

---
## \#21 Posted by: Benjamin899 Posted at: 2019-01-16T15:56:42.049Z Reads: 66

```
don't take my word for it being correct. I said it looks correct, i would have made only array where i would plug all lipos into to make it 12s, not make on 8s and wire it around and hang one additional 4s.
Edit: i shouldn't have said it is correct, my bad. So i retract that, i should only state that i am 100% sure off.
```

---
## \#22 Posted by: epster Posted at: 2019-01-16T15:59:20.568Z Reads: 65

```
Ah yeah that would be smarter. Thanks! I will wait for confirmation from others :slight_smile: .
```

---
## \#23 Posted by: venom121212 Posted at: 2019-01-16T15:59:34.829Z Reads: 64

```
Check that parallel connector. Are you sure it's wired properly?
```

---
## \#24 Posted by: epster Posted at: 2019-01-16T15:59:56.031Z Reads: 61

```
Which one do you mean, the anti-spark?
```

---
## \#25 Posted by: venom121212 Posted at: 2019-01-16T16:00:23.113Z Reads: 64

```
The battery parallel connector you covered on the bottom of the pic
```

---
## \#26 Posted by: J_Dizzle Posted at: 2019-01-16T16:01:18.888Z Reads: 64

```
I don’t think that’s a parralel connector, it’s a series
```

---
## \#27 Posted by: epster Posted at: 2019-01-16T16:01:31.008Z Reads: 63

```
Yeah thats all good. Before i bought another battery I used that plug and that was already checked and well. By other guys from the forum :slight_smile:
```

---
## \#28 Posted by: epster Posted at: 2019-01-16T16:02:10.331Z Reads: 60

```
Yeah its a series connector.
```

---
## \#29 Posted by: venom121212 Posted at: 2019-01-16T16:02:29.641Z Reads: 56

```
My apologies series is correct. How about the Xt90s loop you made? Is the resistor end board side?
```

---
## \#30 Posted by: J_Dizzle Posted at: 2019-01-16T16:02:54.937Z Reads: 54

```
If that is a series connector then your wiring is fine, when you draw it with the long wires it does look a little sketchy but I understand, you have to make do with what space you have available
```

---
## \#31 Posted by: Benjamin899 Posted at: 2019-01-16T16:03:38.205Z Reads: 54

```
true, the resistor is only on one side @epster
```

---
## \#32 Posted by: epster Posted at: 2019-01-16T16:04:14.165Z Reads: 55

```
Ehm I am guessing you are talking about the Xt90 spark plug loop right? Sorry dont know all the terms. What do you exactly mean with resistor end board side? Ah @Benjamin899 got it haha.
```

---
## \#33 Posted by: venom121212 Posted at: 2019-01-16T16:04:57.400Z Reads: 56

```
It should only be on one side of that Xt90s but it's usually on the key part, not the board part. Also I usually see them on the positive wires, not negative. Regardless, your drawing shows the loopkey wired backwards. Officially calling in @b264 to confirm.
```

---
## \#34 Posted by: epster Posted at: 2019-01-16T16:12:02.522Z Reads: 55

```
I was thinking about getting a multimeter for future build improvements etc. Is this a good one to buy? Or is there another one you guys would recommend. https://hobbyking.com/nl_nl/handheld-digital-multimeter-set-an8009-orange.html
```

---
## \#35 Posted by: venom121212 Posted at: 2019-01-16T16:12:56.483Z Reads: 54

```
Fluke or tenma are good brands. Even a cheap one will get you by in many situations.
```

---
## \#36 Posted by: Benjamin899 Posted at: 2019-01-16T16:14:23.379Z Reads: 53

```
yeah a cheap one for starters is all you need. Basicly what you need is measuring Volt,Amps and Resistance.
```

---
## \#37 Posted by: Jumpman Posted at: 2019-01-16T16:19:39.445Z Reads: 52

```
Thanks.  I get what you mean now.  It seems like your vesc is trying to brake when you pull the trigger.  I guess you’ve already done the motor detection and remote setup successfully, but it might be worth double checking the remote settings to see if everything looks correct.
```

---
## \#38 Posted by: epster Posted at: 2019-01-16T16:20:44.728Z Reads: 52

```
Ok thanks. I will get on that now.
```

---
## \#39 Posted by: epster Posted at: 2019-01-16T17:17:18.707Z Reads: 47

```
Ok so the issue I am having right now is that when i pull the trigger the amperage goes from arround -0.1A to between -0.05A to -0.15A rapidly varing between those values. When i pull the break there is a positive Amperage. I cant figure out how I am supposed to flip those values.
```

---
## \#40 Posted by: bartroosen12 Posted at: 2019-01-16T17:20:56.753Z Reads: 46

```
But you board works?
In my bms app I also get negative amps when pulling amps and positive when braking?
```

---
## \#41 Posted by: epster Posted at: 2019-01-16T17:21:59.028Z Reads: 44

```
Nope it doesnt.
Forget about that other part. :slight_smile:
```

---
## \#42 Posted by: bartroosen12 Posted at: 2019-01-16T17:24:07.199Z Reads: 44

```
Have you measured the output voltage? Just very simple to check if it's the right voltage.
But damn what a complex wiring schema.
```

---
## \#43 Posted by: epster Posted at: 2019-01-16T17:24:43.236Z Reads: 46

```
I cant I can only check the individual voltage of the batteries with my charger.
```

---
## \#44 Posted by: epster Posted at: 2019-01-16T17:47:16.252Z Reads: 45

```
UPDATE:

The VESC is dead. :frowning:. After doing the motor detection I can conclude that it is done. My motor, remote, metr module and batteries are fine. I think that it just couldn't the handle the damage done to it earlier (couple if months ago) hence the title did I do it again.
When I was doing the detection I smelt a bit of smoke then I knew there was something wrong. Disconnected the anti spark, metr module, remote and then there was a tiny spark. I kinda saw this coming thats also a reason why i created this post.

But lesson learned. Always be careful and pay attention otherwise a lot worse things could have happened.
```

---
## \#45 Posted by: Battosaii Posted at: 2019-01-16T18:29:52.537Z Reads: 43

```
Well I wired my antispark loopkey and killed my Focboxes not repairable. Yours may have just blown the drv chip and that is repairable.
```

---
## \#46 Posted by: venom121212 Posted at: 2019-01-16T18:33:35.857Z Reads: 41

```
Call the DRV wizard! @JohnnyMeduse
```

---
## \#47 Posted by: epster Posted at: 2019-01-17T13:58:22.248Z Reads: 30

```
Can I see if I blew the DRV with the blind eye? Because i have no idea how i am supposed to see that.
```

---

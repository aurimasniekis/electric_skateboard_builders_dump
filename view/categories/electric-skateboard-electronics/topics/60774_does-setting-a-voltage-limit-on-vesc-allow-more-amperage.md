# Does setting a voltage limit on vesc allow more amperage?

### Replies: 12 Views: 322

## \#1 Posted by: slade Posted at: 2018-07-03T05:29:58.497Z Reads: 129

```
I have 2 192kv motors that recommend to only use a 10-12s setup to power them, but there is a bms I saw on GreatScott's ebike battery video I'd like to get that is 13s, and then I'd make a 13s4p configuration.

I know that I can use the VESC tool to set the max voltage to be within the motors' acceptable voltage range, but how is the power coming from the battery reduced? Is it being step down with a buck converter to get lower voltage/higher amperage, or is the extra energy just converted to heat through some LDO regulator? Does anyone have any knowledge of the actual mechanism that limits the motors' voltage?
```

---
## \#2 Posted by: b264 Posted at: 2018-07-03T05:52:17.476Z Reads: 121

```
[quote="slade, post:1, topic:60774"]
I know that I can use the VESC tool to set the max voltage to be within the motors’ acceptable voltage range, but how is the power coming from the battery reduced? Is it being step down with a buck converter to get lower voltage/higher amperage, or is the extra energy just converted to heat through some LDO regulator? Does anyone have any knowledge of the actual mechanism that limits the motors’ voltage?
[/quote]

It's not reduced.  There is no mechanism.


Just use the 13S BMS with a 10S or 11S battery.  The VESC components aren't rated high enough to safely use with anything over 11S anyway.
```

---
## \#3 Posted by: slade Posted at: 2018-07-03T07:24:30.198Z Reads: 100

```
[quote="b264, post:2, topic:60774"]
It’s not reduced. There is no mechanism.
[/quote]

I guess that I'm trying to refer to is the physical mechanism that is enforcing the software set voltage limit
```

---
## \#4 Posted by: b264 Posted at: 2018-07-03T08:02:01.299Z Reads: 89

```
Whatever limit you're referring to probably just shuts down the entire ESC.  There is no voltage clamping.  That would be the job of a BMS if it were to exist, and not of the ESC.
```

---
## \#5 Posted by: Maxid Posted at: 2018-07-03T10:38:09.629Z Reads: 78

```
Your motors do not really have a voltage limit at 12S. You can go way higher.
```

---
## \#6 Posted by: abenny Posted at: 2018-07-03T13:00:39.177Z Reads: 65

```
motors cn go higher, he stated vesc components are not rated for greater than 11s...if u wanna do it be my guest
```

---
## \#7 Posted by: Maxid Posted at: 2018-07-03T13:12:32.267Z Reads: 62

```
I think @Deckoz has been running 13S and had no problems.
But the intial post is full of misconceptions as i understand it.
```

---
## \#8 Posted by: abenny Posted at: 2018-07-03T13:14:30.034Z Reads: 61

```
i think sub 11s is just a safe rule of thumb to follow, to make sure you don't blow your chips. you are right, there are definitely people who surpass it
```

---
## \#9 Posted by: Luuke Posted at: 2018-07-03T13:42:58.664Z Reads: 58

```
You could limit the voltage by lowering the max dutycycle of your PWM.
I think default is 95%. So converting 12S @ 95% => 13S @ 87,7%
```

---
## \#10 Posted by: wafflejock Posted at: 2018-07-03T13:47:14.966Z Reads: 57

```
This is really just adjusting the average voltage though yes?  I mean it's still at whatever voltage it's at just for shorter periods giving a lower average but if the components have low capacitance then it is still spiking the voltage up to whatever is coming in.
```

---
## \#11 Posted by: wafflejock Posted at: 2018-07-03T13:50:08.648Z Reads: 56

```
@slade you can limit the amperage which will effectively keep your components safe.  Amperage is what results in heat loss and wears on components ultimately so limiting it allows you to keep the battery and motor in safe limits.  I believe the vesc simply limits the duty cycle in order to keep the amperage within limits you set.  That said believe the MOSFETs or drv chip are rated for 60V maximum buy would need to pull up the datasheet.
```

---
## \#12 Posted by: Deckoz Posted at: 2018-07-03T21:10:03.257Z Reads: 38

```
[quote="Luuke, post:9, topic:60774"]
I think default is 95%. So converting 12S @ 95% =&gt; 13S @ 87,7%
[/quote]

Why the hell would you do that. Lol. We all want 100% duty and are stuck at 95%. No way in any shape or form would I lower max duty, that's just bonkers
```

---

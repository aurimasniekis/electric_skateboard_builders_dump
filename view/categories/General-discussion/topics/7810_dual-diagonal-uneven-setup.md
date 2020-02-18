# Dual Diagonal Uneven Setup

### Replies: 22 Views: 1627

## \#1 Posted by: ra.rend Posted at: 2016-08-17T17:34:41.745Z Reads: 183

```
I have enertion's 6355 190kv on the rear and have torqueboard's 200kv just lying around. I plan on mounting the 200kv motor to the front. Is that a bad idea? I was also thinking on unplugging the front motor when not needed. Will the master vesc still work if the slave vesc isn't connected to a motor?
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-17T17:36:34.921Z Reads: 184

```
You can do it, but it's not efficient. It can provide additional torque and acceleration though, which is worth a try. You do not need to have slave vesc connected to a motor for it to work, but I'd recommend powering it down vs leaving the phase wires unconnected.
```

---
## \#3 Posted by: ra.rend Posted at: 2016-08-17T17:42:34.488Z Reads: 175

```
I would need a dedicated power switch for the slave vesc then?
```

---
## \#4 Posted by: lowGuido Posted at: 2016-08-17T17:47:05.632Z Reads: 168

```
nah, just do it.
set them up as 2 separate ESCs don't use canbus just Y cable the PWM headers
```

---
## \#5 Posted by: Jinra Posted at: 2016-08-17T17:49:21.177Z Reads: 162

```
No, you can just unplug the power connector when you want, but as @lowguido said, you can split the servo cable and unplug that as well.
```

---
## \#6 Posted by: ra.rend Posted at: 2016-08-17T18:18:08.454Z Reads: 151

```
I have the space cell enclosure and I don't wanna have to open it when I need to switch to dual or mono. Would keeping the 2nd vesc and motor plugged in (while not being used) bad?
```

---
## \#7 Posted by: ra.rend Posted at: 2016-08-17T18:19:34.939Z Reads: 148

```
Will it send power back to the battery?
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-17T18:20:09.692Z Reads: 144

```
Why would you want to switch it to mono? I'd just be worried about the loose phase cables dangling around. You're also setting the VESC up for a dual drive. If you unplug it won't be optimized for single drive.
```

---
## \#9 Posted by: ra.rend Posted at: 2016-08-17T18:27:12.620Z Reads: 136

```
I wanted to save battery for longer trips. But your right.  I didn't think about the different VESC settings for dual vs mono. I feel so dumb right now 😁.  Dream ruined :frowning: Any other options for long range of a mono drive but power of dual drive?
```

---
## \#10 Posted by: Jinra Posted at: 2016-08-17T18:28:23.018Z Reads: 132

```
The range you get from a mono shouldn't be too big vs a dual. Just go dual. Otherwise, get a bigger motor for power and single drive.
```

---
## \#11 Posted by: ra.rend Posted at: 2016-08-17T18:32:08.079Z Reads: 128

```
Thanks for your help! Is it hard to turn (i.e. the trucks feel more stiff)on a dual Diagonal setup when accelerating?
```

---
## \#12 Posted by: Jinra Posted at: 2016-08-17T18:33:24.502Z Reads: 128

```
Are you asking if the weight of the motor affects turning? If so, then no not really. Though you can have some slippage when turning at low speed with narrower trucks.
```

---
## \#13 Posted by: ra.rend Posted at: 2016-08-17T18:43:29.835Z Reads: 123

```
No, not the weight. I mean when you're turning, the inner wheel can't be spinning as fast as the other wheel and since theyre at the same erpm - it should be more stiff? Does the traction control setting solve this?
```

---
## \#14 Posted by: Jinra Posted at: 2016-08-17T18:45:36.628Z Reads: 121

```
Traction control is set to 3000 erpm by default, which should be enough leeway to prevent any issues. You can always adjust it to be higher or lower as well.

I turned off traction control as it gave me problems when hard accelerating.
```

---
## \#15 Posted by: Hummie Posted at: 2016-08-17T18:48:23.707Z Reads: 119

```
They run independently with the different escs.  I think traction control comes into effect when a wheel looses contact w the ground or ends up freely spinning somehow 

Anyone ever experiece an effects from a single strong motor on handling (turning, accelerating, braking)?
```

---
## \#16 Posted by: Jinra Posted at: 2016-08-17T18:50:21.245Z Reads: 116

```
This happens to me sort of often. I try to hard turn and end up lifting 2 wheels on one side off the ground and it spins full RPM. Really hoping someone starts selling 200mm+ calibers so I stop lifting.
```

---
## \#17 Posted by: Hummie Posted at: 2016-08-17T18:59:24.980Z Reads: 117

```
That's weird cause my motor will stop spinning when I lift it off the ground while the other is still spinning. I thought it was he traction control being implemented
```

---
## \#18 Posted by: longhairedboy Posted at: 2016-08-17T18:59:33.771Z Reads: 119

```
In my experience traction control doesn't make any difference really in overall handling, but it does seem to keep the wheels from just spinning wildly when you happen across super slippery pavement such as mossy or slimey areas or carve really hard and lift one of the drive wheels off the ground. It helps quite a bit in those situations. 

When using a single motor i have on several occasions carved hard enough to lose drive traction and yes, it does mess with you a little. 

I also haven't really noticed a lot (read: did notice some, just not a lot) of difference in battery life on one motor VS two when i stopped deliberately trying to get the most range out of the one motor and just rode it like i would a dual, which is to say recklessly fast. When riding a dual in a way as to get the most range, it comes out roughly the same as a single.
```

---
## \#19 Posted by: Jinra Posted at: 2016-08-17T19:00:49.680Z Reads: 109

```
It probably is your traction control kicking in. I just have mine off because it causes other problems.
```

---
## \#20 Posted by: ra.rend Posted at: 2016-08-17T21:54:28.858Z Reads: 105

```
@longhairedboy how many miles are you getting with the space cell on dual?
```

---
## \#21 Posted by: longhairedboy Posted at: 2016-08-18T13:54:13.229Z Reads: 81

```
if we're talking about the original 10S3P design, the most i ever got was 15 miles.
```

---
## \#22 Posted by: ra.rend Posted at: 2016-08-18T14:07:21.628Z Reads: 75

```
That's actually more than enough for me. Guess I'm going dual! Thanks!
```

---

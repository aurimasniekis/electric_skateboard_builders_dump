# Problem with braking, Need some help

### Replies: 18 Views: 771

## \#1 Posted by: onepunchboard Posted at: 2017-08-28T21:03:45.581Z Reads: 103

```
for FOCBOX I'm using -80a for braking cuz I have single motor. regardless, when I brake, it works for up to 80% of throttle but when I go all the way it doesn't brake as hard. I increased the batt charge rate to  50amp but didn't do anything.

It feels as if, the vesc is cutting out the power to half to protect something.
```

---
## \#2 Posted by: cwazy1 Posted at: 2017-08-28T23:27:52.567Z Reads: 99

```
If your battery min is set at -50a, and your battery was actually being charged at 50a, you'd be in trouble. The lowest number you should be setting on your battery min is dictated by your battery setup.

Battery max has nothing to do with braking.

Can you screen shot your bldc settings
```

---
## \#3 Posted by: onepunchboard Posted at: 2017-08-28T23:31:42.246Z Reads: 92

```
Update: I use controller trim to make it brake more, it works little better (i use ebay mini rc remote). but it still does when i pass 35kmh. I use median filter maybe I should turn off?
```

---
## \#4 Posted by: onepunchboard Posted at: 2017-08-28T23:38:00.026Z Reads: 89

```
I can't connect bldc at the moment. I use lipo 2*5a 10s (I meant two 5s in series) rated for 5c charging. so 5x5x2=50amp so within safe limit. and won't go that much actually, but I'm ganna change back later. cuz it didn't do anything

I'm pretty much 80a -80a batt 80a -50a absolute 130 slow absolute checked
erpm max 65k default rest
```

---
## \#5 Posted by: onepunchboard Posted at: 2017-08-28T23:41:24.711Z Reads: 84

```
I'm thinking since I use 260kv motor, the vesc is loaded too much and giving up?
but there wasn't any reboot in vesc. 
my gear ratio was 12:36 and wasn't much of a concern since it stoped well regardless the issue, now using 15:36 makes the problem apparent. 
Maybe I should step down to 200kv motor?
```

---
## \#6 Posted by: Namasaki Posted at: 2017-08-29T01:11:34.956Z Reads: 74

```
[quote="onepunchboard, post:4, topic:31671"]
I use lipo 2*5a 10s rated for 5c charging. so 5x5x2=50amp
[/quote]

Are you saying you have 2 10s 5ah batteries connected in parallel?
```

---
## \#8 Posted by: onepunchboard Posted at: 2017-08-29T01:24:23.020Z Reads: 70

```
No in series. I meant 5s*2
 I used this setting to test the brake with half ful battery. it didn't hurt anything.
```

---
## \#9 Posted by: onepunchboard Posted at: 2017-08-29T01:27:52.884Z Reads: 68

```
Maybe I should increase absolute to135 to see if this change anything
```

---
## \#10 Posted by: Deckoz Posted at: 2017-08-29T01:37:15.973Z Reads: 68

```
Do you have any of the nano remote variants? If so is the rear switch in the down position? Down is -100 to +100 ppm throw, while   up is -80~ to +80~
```

---
## \#12 Posted by: onepunchboard Posted at: 2017-08-29T01:39:30.043Z Reads: 66

```
No I have mini remote, one that looks like a rc remote, but I am ganna re do the ppm too
```

---
## \#13 Posted by: Deckoz Posted at: 2017-08-29T01:42:13.251Z Reads: 64

```
Gotcha - just figured I'd ask
```

---
## \#14 Posted by: Namasaki Posted at: 2017-08-29T01:51:26.659Z Reads: 64

```
[quote="onepunchboard, post:8, topic:31671"]
No in series. I meant 5s*2
[/quote]

If you have two 5s 5ah batteries connected in series, its 10s 5ah
So 5C charge is 25a, 
Not 50a. 
It's 5c x 5ah          
Not 5C x 5ah x 2
```

---
## \#16 Posted by: onepunchboard Posted at: 2017-08-29T04:09:07.631Z Reads: 53

```
oh okay. I did mistake there. thanks
```

---
## \#17 Posted by: onepunchboard Posted at: 2017-08-29T04:11:30.169Z Reads: 55

```
So here is my set up, (I know my batt cut off is low, but leave me alone with that.)
I changed couple things like brake limit as of now, Will test it tmr.  goodnight
<img src="/uploads/db1493/original/3X/b/2/b2e13f82d681745dc0943f5eb47b54248254fcd7.png" width="690" height="430"><img src="/uploads/db1493/original/3X/2/4/24d5c21c2a5b8044eb0f611e2aa0a337cc09087b.png" width="690" height="436"><img src="/uploads/db1493/original/3X/7/8/7831b0ca241fb29a5fd8b7b69924fcedaf9a5e78.png" width="690" height="441">
```

---
## \#18 Posted by: Clonkex Posted at: 2017-08-29T05:28:47.516Z Reads: 48

```
You know you can edit your posts, right? You seem to be deleting them pretty frequently.
```

---
## \#19 Posted by: onepunchboard Posted at: 2017-08-29T13:13:14.189Z Reads: 43

```
Yeap srry. Just lazy XD
```

---
## \#20 Posted by: onepunchboard Posted at: 2017-08-30T05:23:12.348Z Reads: 33

```
update: changed setting didn't do much help, other than increase absolute max. I chaged to FOC mode to see if it differs from BLDC
```

---
## \#21 Posted by: onepunchboard Posted at: 2017-08-30T20:34:29.277Z Reads: 27

```
Update: FOC has wayyy better braking power. not dead stopping but smooth and quick. no loosing power like BLDC. I think the motor was giving up as I brake very hard than vesc protection kicks in. which did not have in previous vesc I had.
now FOC feels buttery smooth that kinda lacks kicks of torque. but I like it
```

---

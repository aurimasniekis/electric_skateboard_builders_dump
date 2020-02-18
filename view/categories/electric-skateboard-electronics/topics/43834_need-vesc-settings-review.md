# Need VESC Settings review

### Replies: 7 Views: 439

## \#1 Posted by: wheinrichs Posted at: 2018-01-16T03:14:39.780Z Reads: 75

```
So I think I have all my setting correct on my VESC but I figured I'd check with someone here to make sure I don't fry the thing before I have a chance to use it. I'm running 4 of these [batteries](https://hobbyking.com/en_us/turnigy-battery-5000mah-5s-20c-lipo-pack-xt-90.html?___store=en_us) as a 10s2p set up one a single drive sk3 6364 190kv and controlling it with the HK-GT2B. Let me know if anything looks weird or should be changed, thanks! 
![44 PM|690x431](upload://nskcWIThN2HaD6UNNRPcsHQoiJK.png)
![54 PM|690x431](upload://eb47MF8JVBPNvlCIj5JaBO1Gg7H.png)
![08 PM|690x431](upload://xEF3bScCl3CCAafyJPPNTBbCrS6.png)
![19 PM|690x431](upload://7vVFaZE7fty9HhAiFNP03yOe7uH.png)
![20 PM|690x431](upload://8slZcTSvsnS6ynyaFf3vb988QNn.png)


One last thing, it looks like when I try and brake the motor stops instantly. Right now it's just set up on my table so theres no load, but I wanted to make sure this is normal.
```

---
## \#2 Posted by: Colson003 Posted at: 2018-01-16T03:22:22.939Z Reads: 53

```
Change max input voltage back up to 57volts. 
Even thought you'll never exceed 60,000erpm, may as well set it to 60,000 and -60,000. Then make sure limit erpm with negative torque is turned off. 

Yes, for it to stop immediately is normal for no load, you could even change your battery min to -20a for stronger brakes at high speeds.
```

---
## \#3 Posted by: westonbe Posted at: 2018-01-16T03:23:33.223Z Reads: 52

```
I would change your battery max to 50A or lower. The vesc's limit is 50A. I blew up a vesc because of this. Although, mine was set at 65A, it probably wouldn't have blown if I didn't max throttle it up a 35 degree football field length hill.
```

---
## \#4 Posted by: wheinrichs Posted at: 2018-01-16T03:38:22.625Z Reads: 48

```
Okay will do, thanks for the advice!
```

---
## \#5 Posted by: wheinrichs Posted at: 2018-01-16T03:43:10.746Z Reads: 49

```
@Colson003  I thought that the max input voltage should be around what you expect? at 10s with 4.2 wouldn't that be 42 volts? I added the extra 3 to account for the battery spike.

Just so I understand what does the "Limit ERPM with negative torque" affect?

And I figured to be safe I'd charge the batteries at 1c which is where I was getting the 1 amp.
```

---
## \#6 Posted by: Colson003 Posted at: 2018-01-16T05:06:38.976Z Reads: 46

```
@wheinrichs  at 45 you should be fine, I was saying 57 because that is what basically everyone keeps it at. I have mine at 57 and I'm just on 6s. 

"Limit erpm with negative torque" means that if you hit the erpm limit (which is basically impossible on 10s at 190kv) the brakes will be applied. 

Even at -20amps or 2c, there would only be 20amps being sent back to the battery when you're close to top speed. It would only be for a second or two at most. Thats not the best explanation, but if you understand duty cycle then that would make more sense.
```

---
## \#7 Posted by: wheinrichs Posted at: 2018-01-16T05:08:04.902Z Reads: 44

```
@Colson003 no that makes perfect sense, thanks for your help I really appreciate it!
```

---

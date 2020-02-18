# VESC Settings Verification

### Replies: 7 Views: 1556

## \#1 Posted by: Emerson Posted at: 2016-12-12T17:09:06.379Z Reads: 173

```
Hello everyone, I've been exhaustively reading every bit of VESC help on the forum and think I've configured things properly but a few extra set of eyes would be helpful as this is my first time (and first post).  Suggestions? Reaaaallly shooting for not blowing the VESC up here :slight_smile: 

Motor: Enertion R-Spec 190kv 6372
Batteries: 2 x 3S 40C 4000mah Zippy LiPo in Series (6S1P)
Remote: FS-GT2B
[TorqueBoards VESC](diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/): Model 4.12 with 2.18 Firmware

<img src="/uploads/db1493/original/3X/1/1/1176a762553dca7b42995c33a39e89b3daae3c9f.JPG" width="690" height="406">

<img src="/uploads/db1493/original/3X/b/4/b437a0665cf0c4d3e96087368bae593774523b9c.JPG" width="690" height="408">

<img src="/uploads/db1493/original/3X/1/e/1e648c1e21132415f094c83c904921568883f786.JPG" width="690" height="407">
```

---
## \#2 Posted by: NickTheDude Posted at: 2016-12-12T17:15:05.477Z Reads: 137

```
Looks good to me. I think your Batt max setting is a little conservative. Raising it a little would give you some more power. But overall looks like you're set!
```

---
## \#3 Posted by: Emerson Posted at: 2016-12-13T14:56:36.791Z Reads: 112

```
What settings would you suggest?  Out of all my forum searches I can't seem to find a good explanation as to what the basis should be for selecting a number.  I do know the higher the number the more brake force but what are the actual calculations that need to be done?
```

---
## \#4 Posted by: Ackmaniac Posted at: 2016-12-13T15:41:07.487Z Reads: 109

```
1. I recommend to set the battery cutoff start to 21,6V (3,6V) and end to 20,4V (3,4V). Lipos have less voltage drop but they are also empty at a higher voltage then li-ion which could go down till 3,0V or even 2,5V.

2. Set your motor max to 70 or 80A, you can lower it if it is too strong.

3. Set the battery max also to 70. Or at least to 50A. Otherwise you won't have much power on a 6S system.

4. Set Max ERPM to 60000 and Min ERPM to -60000. You will never reach these values but just to be safe.

5. Set absolute Max amps to 130A. (don't ask, just do it)

6. Adjust your min and max pulsewith by enabling the display checkbox and read the values when the trigger is on full power and full brake. Set it to these values. Afterwards you can reduce the deadband if you like.

7. Ohhhhhh, And set the Batt min (regen) to -12A. Because -4A is too low and would result in very bad brakes at high speed. With your battery you can even go up to -20A i guess, but try it at -12 first.

I think that's it.

No thank you needed. This button does that as well :joy:
[Donations](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4R86CGGZDVE9W)
```

---
## \#5 Posted by: Emerson Posted at: 2016-12-13T17:42:22.492Z Reads: 89

```
Thanks for the assistance!  I do have a few questions though.
1. Understandable.
2. I've read that the motor max for the R-Specs is 80A (continuous?) but was afraid of potential issues for some reason, thanks for the confirmation here.
3. Would this be determined by my C-Rating multiplied by my Ah?  Theoretical max for me would be 40*4=160?
4. I'm assuming this is based off of [Chaka's post](http://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125).  I wonder why the defaults wouldn't be set to this in the first place.
5. I know this is the standard number and several people mention it on the forums...Wouldn't this be a calculation based off of the theoretical max amp draw assuming low voltage?  In my case due to Battery cutoff start at 21.6V, Rated wattage of the motor is 3000W which brings my max Amps to about 139.  I'm really just piecing this all together as my electrical knowledge is poor at best.
```

---
## \#6 Posted by: Ackmaniac Posted at: 2016-12-13T18:43:01.198Z Reads: 85

```
2 I've read that the motor max for the R-Specs is 80A (continuous?) but was afraid of potential issues for some reason, thanks for the confirmation here. 
**Correct**

3 Would this be determined by my C-Rating multiplied by my Ah? Theoretical max for me would be 40*4=160?
**That would be the maximum for the battery. But it doesn't make sense to go higher than the motor max. And you want power that is controllable. If you want more power and speed then you should uprade your system to a 9S, 10S or 12S.**

4 I'm assuming this is based off of Chaka's post. I wonder why the defaults wouldn't be set to this in the first place.
**Because originally it was for a vesc which could only handle 50V. But the newer versions can handle up to 60V, but you want some safety buffer. So keep it at 57V. No issues on my 12S System with that.**

5 I know this is the standard number and several people mention it on the forums...Wouldn't this be a calculation based off of the theoretical max amp draw assuming low voltage? In my case due to Battery cutoff start at 21.6V, Rated wattage of the motor is 3000W which brings my max Amps to about 139. I'm really just piecing this all together as my electrical knowledge is poor at best.
**I also don't understand this value completely. Need to check the source code to know how it is handled. But no time atm.**
```

---
## \#7 Posted by: Emerson Posted at: 2016-12-13T20:45:44.014Z Reads: 75

```
I really do appreciate all the effort here, this is a huge help!  

I'm guessing the ERPM limit doesn't matter as I've capped off the Volts and Amps below theoretical max for the entire system.  I'll give this a go for a while and then hopefully move to your Extended BLDC-TOOL with WATT Control mode.  I want to be able to appreciate that upgrade and all your hard work :slight_smile:   Perhaps at some point I'll even feel comfortable with FOC.
```

---

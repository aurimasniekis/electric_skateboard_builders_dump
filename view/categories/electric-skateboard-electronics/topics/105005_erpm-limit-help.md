# ERPM Limit Help!

### Replies: 7 Views: 98

## \#1 Posted by: MadPatch Posted at: 2020-01-01T16:58:51.488Z Reads: 30

```
So I have tried to read about ERPM limits and understand it, but don't really fully understand it. This is what I know, my vesc (torqueboards vesc 4.12 hardware 3.63 firmware) supports upto 60k erpm. My max rpm of my motor (torqueboards 6374 190KV) with my setup is 4,628rpm and I saw that erpm = (rpm*motor poles) **can someone tell me does motor poles mean the physical number of coils, or something else??** Then my real question comes from the vesc tool setup, I want to protect my vesc and not destroy it and have learned erpm comes into a major play when mainting your vesc. **The default ERPM Max value = 100k on vesc tool, so I changed it to 60k, will that stop my board from contining to speed up when it reaches that limit??** And is there anything other settings I should change to help not ruin my vesc, thanks! 

Oh and if its helpful I am running a custom built 8s3p 18650 battery pack.

And on a side note I have seem some mixed reviews on people using torque boards vescs on foc, so does anyone have experience with using those vescs on foc and if I should?
```

---
## \#2 Posted by: mynamesmatt Posted at: 2020-01-01T17:39:48.221Z Reads: 26

```
Erpm is (voltage x KV x pole pairs) .
eg i have a 192kv 6374 motor with a 10s battery. Normally motors have 14 poles (magnets inside the can) which is 7 pole pairs.
so (nominal) 36v x 192 x 7 = 48,384

for you it'll be

(8x3.6v = 28.8) x 190 x 7 = 38,304

that's your erpm.

physics wise, your board cannot exceed this erpm as it can only push out the maximum voltage to the motor which it receives from the battery. Having your erpm limit at 60k erpm is just fine. 

tb vescs can run foc just fine. just not so much on 12s. Any lower that 10s it should be fine with. pretty much, just don't do anything stupid you're not sure about and you'll be fine. always triple check before pressing that apply button

edit: another thing, do not, in any circumstance apply more than 50a battery amps to your vesc. Usually 35-40a battery amps should be completely fine. Motor amps however, don't exceed 100a and you'll be right 🤙🏼
```

---
## \#3 Posted by: Pura-Vida Posted at: 2020-01-01T18:03:45.814Z Reads: 25

```
On Lacroix board, conceptor recommands to limit on focbox to 90A when discharging and -40A during recharging phases ( when you are braking). Battery are 12s6p of Sanyo™ NCR20700B.
```

---
## \#5 Posted by: mynamesmatt Posted at: 2020-01-01T18:33:34.459Z Reads: 22

```
[quote="Pura-Vida, post:3, topic:105005"]
90A when discharging and -40A during recharging phases ( when you are braking). Battery are 12s6p
[/quote]

the 6p provides Max output of 120a. So its combined for the unity. Unless it's across 2 esc's where each cell would need to ve able to provide 30a per cell
```

---
## \#6 Posted by: MadPatch Posted at: 2020-01-01T21:23:14.495Z Reads: 17

```
Okay awesome thanks! And what should I limit the max regen be?
```

---
## \#7 Posted by: MadPatch Posted at: 2020-01-01T21:25:32.136Z Reads: 15

```
Also, fully charged the cells are 4.2 so shouldn't use use 4.2v instead of 3.6 when calculating erpm? Thanks.
```

---
## \#8 Posted by: mynamesmatt Posted at: 2020-01-01T23:15:55.468Z Reads: 13

```
[quote="MadPatch, post:6, topic:105005"]
And what should I limit the max regen be
[/quote]

your max regen should be 3 times the maximum charging current of the cells you have. 3x as you have a 3p pack

[quote="MadPatch, post:7, topic:105005, full:true"]
Also, fully charged the cells are 4.2 so shouldn’t use use 4.2v instead of 3.6 when calculating erpm? Thanks
[/quote]
yes you can. but you only have the full charged voltage for a few minutes at the start of the discharge but whatever
```

---

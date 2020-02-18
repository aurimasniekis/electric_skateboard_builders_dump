# Brakes cutting out in FOC

### Replies: 10 Views: 538

## \#1 Posted by: goldrabe Posted at: 2018-02-08T15:07:21.033Z Reads: 92

```
Hi Builders,

i made a build with two generic 90mm Hubs which are available from many Chinese sources.
I did set them up with two Vesc´s in FOC mode. Everything is working fine except the brakes.
I will get brakes for a split second and after that the board just coasts. If i pull the trigger just slightly i get brakes for a longer time but they will cut out either.
I run them on a 10s5p Samsung 30q pack which is not fully charged.
My Vesc Settings are.

Motor max 60A
Motor min -60A
Absolute Max 130
Battery Current Max 25A
Battery Current Max Regen -20A

Any input would be really appreciated!!
```

---
## \#2 Posted by: rich Posted at: 2018-02-08T15:11:02.423Z Reads: 90

```
If you have maytech/greenmotion or similar cheap HW this behaviour is normal, unfortunately they don't like FOC. Don't FOC it up!
```

---
## \#3 Posted by: goldrabe Posted at: 2018-02-08T15:15:52.830Z Reads: 87

```
Thanks for your reply!
I installed the latest firmware on them, @psychotiller confirmed that even the Maytechs can do FOC now. I am still hoping that it is more a setting kind of thing.
```

---
## \#4 Posted by: psychotiller Posted at: 2018-02-08T15:35:29.814Z Reads: 80

```
I did in fact confirm that 3.3 likes foc. What version vesc do you have? Changing the firmware on older HW isn't going to make unicorn sounds come out of your older maytech vescs...
```

---
## \#5 Posted by: goldrabe Posted at: 2018-02-08T15:43:27.493Z Reads: 72

```
Thanks for chiming in!

I bought them in December `17, 4.12 HW. They still have the old stickers on the transistors not the blue ones for the Super Vesc, are they too old for FOC?
```

---
## \#6 Posted by: psychotiller Posted at: 2018-02-08T15:46:28.643Z Reads: 73

```
Yeah...The newest 3.3 versions are FOC solid. No guarantees on previous offerings. (Though, I have had a couple of older versions that didn't burn up using FOC.)

Try lowering your regen settings, and "Uncheck Limit erpm with negative torque"
```

---
## \#7 Posted by: goldrabe Posted at: 2018-02-08T15:48:28.840Z Reads: 70

```
I see,
thanks man! Rolling back to BLDC.
Lesson learned!
```

---
## \#8 Posted by: psychotiller Posted at: 2018-02-08T15:49:22.612Z Reads: 69

```
See my edit
```

---
## \#9 Posted by: goldrabe Posted at: 2018-02-08T15:51:55.105Z Reads: 67

```
Okay!
i will try that!
Your help is really appreciated!
```

---
## \#10 Posted by: bevilacqua Posted at: 2018-02-08T16:01:24.813Z Reads: 62

```
Try doing the C18 Mod (Explained on the Vedder Forum). That fixed my DRV errors while braking.
```

---

# When does the Space Cell battery cutoff begin to kick in?

### Replies: 11 Views: 1260

## \#1 Posted by: michaelcpg Posted at: 2016-06-15T07:55:38.375Z Reads: 162

```
Hey guys,

I've been using a Space Cell for a month or two on a board I've built that is essentially the same setup as a Raptor Mono without the CF deck. 
Something I started wondering today is that, if I'm using the recommended Raptor battery cutoff settings in the VESC (33V Start, 28V End) at what percentage level on the battery meter should I expect the cutoff to start kicking in?

I've never let the battery go below a ~30% or so reading on the meter as a matter of trying to prolong the life of the battery but I'm curious to know at what point I should actually worry that the board would start cutting the power back?
```

---
## \#2 Posted by: NIK Posted at: 2016-06-15T08:06:52.196Z Reads: 161

```
0 percent if im not mistaken.
```

---
## \#3 Posted by: Skitzor Posted at: 2016-06-15T08:14:28.421Z Reads: 156

```
Personal experience on a dual raptor:
At around 20% left on the battery, depending on how much throttle you put in, you'll see the display go down to 0%. When the backlight is going out as well at 0% you're almost at the cutoff. This gives me a fair warning to change batteries.
```

---
## \#4 Posted by: michaelcpg Posted at: 2016-06-15T08:29:02.836Z Reads: 148

```
Thanks for the input guys. Just to confirm, 0% is about equivalent to cutoff start or end?
```

---
## \#5 Posted by: Skitzor Posted at: 2016-06-15T08:44:48.454Z Reads: 137

```
Like in my example. 20% on the battery. Not throttling.
If you throttle, it will start going down to 0%. If you leave the throttle it will go up to 20% again.
```

---
## \#6 Posted by: Tarzan Posted at: 2016-06-15T12:55:08.935Z Reads: 126

```
Just try it! You can't destroy the battery with you VESC settings.
```

---
## \#7 Posted by: Namasaki Posted at: 2016-06-16T00:57:20.842Z Reads: 107

```
My understanding is that you should never run any type of lithium battery bellow 20%.
And that goes for your cell phone and tablet as well.
And Doesn't the Space cell maintain 36v regardless of how much charge it has?
If unlike Lipo batteries, it does maintain constant voltage, then what good would a low voltage cutoff be?
```

---
## \#8 Posted by: Jinra Posted at: 2016-06-16T01:00:28.539Z Reads: 105

```
Here you go:

http://www.electric-skateboard.builders/uploads/db1493/original/2X/f/fb95302d91aa992329d1d0ccb21f626ae71fc139.png

Space Cell or any other Li-ion/Lipo batteries do not maintain constant voltage, it works the same way as most all other batteries. Not saying this chart is how the battery meter on the space cell reads, but gives you a rough idea. Keep in mind running it to 0% won't necessary harm the batter much since  the BMS prevents the voltage from going to low. Samsung tests their 25R's life cycle by going all the way down to 2.5v which is way below what this chart reads at 0%.
```

---
## \#9 Posted by: Namasaki Posted at: 2016-06-16T01:02:31.795Z Reads: 103

```
So, when the space cell is fully charged, its at 42v not 36v?
Btw, Nice chart
```

---
## \#10 Posted by: Jinra Posted at: 2016-06-16T01:18:36.224Z Reads: 100

```
yes it's 10s so 42v full charge
```

---
## \#11 Posted by: Skitzor Posted at: 2016-06-16T06:44:35.925Z Reads: 88

```
AFAIK, the BMS should take care of those low voltages.
As Others have suggested (and reading from the table) there should still be 2,5V in the cells at 0% but what I was trying to explain is that the soft battery cutoff of the raptor is around 20% charge. 

When you're at 20%, go full throttle and are able to cut it off. Using the regenerative braking will charge it sufficiently enough and it will be back around 20%. There's no way, that with the standard settings Enertion puts in, you could drain it to 0%. And if I'm not mistaking 20% should mean there's still 2,8V in each of the cells.

Also it's a LiNiCoMnP composition.
```

---

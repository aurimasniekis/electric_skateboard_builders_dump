# Receiver won&rsquo;t turn on

### Replies: 22 Views: 1641

## \#1 Posted by: englertvolum Posted at: 2016-09-02T15:09:51.554Z Reads: 82

```
hi!
im working on first build, and it first assemble everything worked just fine - i triggered the remote and motor was working.
i unplugged the cables and started to enclouse everything, then i connected the cables again, and the RC recevier won't turn on anymore (suppose to be a red led light).
i checked the voltage and its 5v as it suppose to be for what i know.

do i miss something ?
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2016-09-02T15:13:42.698Z Reads: 79

```
Do you have any Picture ? What remote are you using ? What type ESC (or VESC) ?
```

---
## \#3 Posted by: englertvolum Posted at: 2016-09-02T15:28:37.621Z Reads: 75

```
its a vesc.
the remote is quanum 2.4GHZ
<img src="/uploads/db1493/original/2X/c/ce88e48e3ad70c71cc9ad003a60519792025ec92.jpg" width="690" height="388">

as you can see, the cable is connected to the vesc. and it gets 5v, i just checked again.
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2016-09-02T15:48:39.451Z Reads: 71

```
Did you have made your own servo cable? Did you try reversing the servo cable ( the Ground should be at the exterior)
```

---
## \#5 Posted by: englertvolum Posted at: 2016-09-02T16:03:29.573Z Reads: 68

```
yeah i made the serv cable - and it works. i measured the voltage and its 5v stable.
and yes i tried to switch it in every possible direction.
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2016-09-02T16:15:32.527Z Reads: 66

```
Did you have done the configuration using the bldc toilette ? Also, is the led on the receiver stop flashing when the remote is on?
```

---
## \#7 Posted by: englertvolum Posted at: 2016-09-02T16:18:44.741Z Reads: 65

```
sorry for the ignorance, but what BLDC is ??
and no, i didnt do any configuration, at first assemble, it work just fine.
then i unpluged everything and plug it again - doesnt work anymore.
```

---
## \#8 Posted by: Skitzor Posted at: 2016-09-02T16:21:26.455Z Reads: 61

```
You will need to configure the PPM settings in the BLDC tool of the vesc.
You possibly also need to bind it again. 
You should measure 5V and 3,3V on the receiver end
Hope this helps a bit
```

---
## \#9 Posted by: englertvolum Posted at: 2016-09-02T16:22:50.366Z Reads: 57

```
what do you mean 5v AND 3.3v? 
and if i have to configure the PPM setting' why did it wok first time i plugged it ?
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-09-02T16:26:21.071Z Reads: 54

```
Before using any VESC you need to configure them using the BLDC Tool... Vesc are NOT plug and play, you need to be careful with them
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2016-09-02T16:28:01.008Z Reads: 55

```
No.... 3,3v you mesure is from the pwm pin and is an average made by the meter you use.
```

---
## \#12 Posted by: JohnnyMeduse Posted at: 2016-09-02T16:28:44.253Z Reads: 57

```
http://www.electric-skateboard.builders/t/connecting-vesc-to-motor/8761/6?u=johnnymeduse
```

---
## \#13 Posted by: Skitzor Posted at: 2016-09-02T17:49:01.318Z Reads: 56

```
So? If its configured right he should measure it...
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2016-09-02T18:04:04.021Z Reads: 53

```
The voltage should changent depending on the trottle position, what is show by tour meter is the rms voltage, witch may not always be the real voltage, but a approximation base with the frequency
```

---
## \#15 Posted by: englertvolum Posted at: 2016-09-02T19:08:46.057Z Reads: 49

```
okay, i just configured the vesc using the bldc tool. and it didnt change anything - there is still no light or other response from the receiver...
other suggestion?
```

---
## \#16 Posted by: englertvolum Posted at: 2016-09-03T06:40:18.944Z Reads: 38

```
Is it possible that when I reconnected all the cables, I connected the servo cable backwards and it fried the receiver?
In that case if I'll buy new receiver will it work with my quantum remote or should I buy a new remote as well?
```

---
## \#17 Posted by: elkick Posted at: 2016-09-03T07:47:03.503Z Reads: 38

```
Those quanum remotes seem to be the most unreliable. I have not yet heard from anybody that it works well.
```

---
## \#18 Posted by: sl33py Posted at: 2016-09-03T07:49:58.725Z Reads: 38

```
I got rid of mine - loved the size, but it ate batteries really quickly and honestly looks too much like a gun.  Just not the kind of attention i wanted, so switched to modified GT2b in badwolf v2.  

Where are you located englertvolum?  Maybe a nearby esk8 member can loan you another tx/rx to test.
```

---
## \#19 Posted by: englertvolum Posted at: 2016-09-03T07:55:56.056Z Reads: 39

```
I'm from Israel, I don't think there's a lot of sk8's around.
```

---
## \#20 Posted by: sl33py Posted at: 2016-09-03T08:00:08.241Z Reads: 41

```
a bit far from me... (Seattle) but you might be surprised.  There are quite a few folks here!

A spare receiver isn't a bad idea to have just in case.  I can't recommend the GT2b more, especially with a smaller case like flatline, master cho, baby buffalo, or badwolf.  Even riding w/ full size remote for a while isn't too much trouble IMO.  Eventually you'll want it smaller and pocketable - but easily done w/ some 3d printed enclosures and a few hours spare time!
```

---
## \#21 Posted by: racidon Posted at: 2016-09-03T08:02:48.700Z Reads: 43

```
you can always test your receiver out by plugging it into a USB header. They supply 5 V. Just be sure to be using the correct pins. It will say what's what on your motherboard :)

Edit:
You could also get a USB cable. Cut it and use the Red for + and Black for GRND, wire this to a servo plug and plug your receiver into a computer USB port or even a USB charger to check power
```

---
## \#22 Posted by: englertvolum Posted at: 2016-09-03T11:48:00.460Z Reads: 33

```
Thanks everyone, I'll try and I'll update you guys.
```

---

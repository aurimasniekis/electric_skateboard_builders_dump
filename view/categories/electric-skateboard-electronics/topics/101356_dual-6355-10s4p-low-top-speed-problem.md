# Dual 6355, 10s4p low top speed problem

### Replies: 7 Views: 100

## \#1 Posted by: Blubbking Posted at: 2019-09-04T18:53:35.997Z Reads: 51

```
Hey guys. I completed my build but I Need a bit of help i think.

I built a 10s4p Samsung 30Q Battery and Dual 6355 190kv, Focbox Unity board. I use 85mm Caguamas.

My Problem is that i can not go over 36km/h. ANd i do not understand why. I would have liked to hit 40-45km/h. Gearing is 16/36. Maybe my settings are wrong?. 
This are my Focbox Unity Settings:
Max Battery Discharge: 60A
Max Braking Regen: -30A
Max Motor Current: 50A
Max BRake Current: -50A
Motor Temp Limits: 100C°
Motor Beta: 4100 (what does this setting even mean)

The Torque is crazy and i reach the Top Speed almost instantly. So i think there is potential for more Speed.

Would be greatly appreciated if someone knowledgeable can help me out !
```

---
## \#2 Posted by: Superflim Posted at: 2019-09-04T19:05:54.864Z Reads: 46

```
You should put your numbers into this calculator.
https://calc./#/0
If you need to higher top speed make your motor pulley higher teeth. For example 18
```

---
## \#3 Posted by: Blubbking Posted at: 2019-09-04T19:10:49.831Z Reads: 43

```
The calculator says i should reach 40km/h loaded. That`s what makes me think there is something wrong with the Unity settings.
```

---
## \#4 Posted by: Superflim Posted at: 2019-09-04T19:30:55.719Z Reads: 38

```
I doubt the unity settings are limiting your speed.
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-09-04T19:42:03.548Z Reads: 35

```
How are you measuring your speed? If you're using the inbuilt calculation of the unity app, it's critical to get all the drivetrain numbers correct for an accurate speed. If you haven't already, try checking that against a GPS speed reading.

You can also check your ERPM limit, it might have somehow gotten set lower than it should.
```

---
## \#6 Posted by: Blubbking Posted at: 2019-09-04T19:49:40.973Z Reads: 33

```
I did use a GPS Speed measurement App so the reading should be accurate. Where do i acess erpm Settings in the Unity App. ?
```

---
## \#7 Posted by: MysticalDork Posted at: 2019-09-04T19:52:05.425Z Reads: 31

```
That I don't know. I've only used the official BLDC-tool and vesc-tool from Vedder, never the unity version which is basically a more simplified and locked-down version.
```

---

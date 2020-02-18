# Is this Vesc compatable with this battery

### Replies: 15 Views: 877

## \#1 Posted by: notepad Posted at: 2017-03-06T21:45:46.697Z Reads: 57

```
<p>Hello,

The <a href="diy-electric-skateboard-kits-parts/vesc-the-best-electric-skateboard-esc/">VESC </a> in question and the <a href="https://hobbyking.com/en_us/multistar-high-capacity-6s-16000mah-multi-rotor-lipo-pack.html"> Battery </a> in question.

Im thinking of getting two of the batteries and making it 12S1p.

Whats your thoughts?</p>
```

---
## \#2 Posted by: IsTalo Posted at: 2017-03-06T21:54:13.063Z Reads: 57

```
But we need to know your motor man.

Vesc is compatable with batteries that goes from 3s to 12s, that is a 6s one, so It will work fine

But Vesc have a ERPM limit, so depending on your motor, it could not work
```

---
## \#3 Posted by: notepad Posted at: 2017-03-06T21:56:06.451Z Reads: 55

```
whoops sorry, 

 the motor im looking at getting is <a href="https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-168kv-brushless-outrunner-motor.html"> this one </a>,  a Turnigy 168kv sk3
```

---
## \#4 Posted by: IsTalo Posted at: 2017-03-06T22:07:53.448Z Reads: 47

```
You could even put 10s on this motor man, you are losing power using 6s, but ok, you could use
```

---
## \#5 Posted by: jmasta Posted at: 2017-03-06T22:08:42.559Z Reads: 46

```
How fast do you want to be able to go?  168kV would be perfect for 12S, and would work well at 10S.  But 6S and 168kv just doesn't produce enough RPMs in my opinion.  Your max weighted speed will likely be in the 13-18 mph range, depending on gearing ratio and wheel size
```

---
## \#6 Posted by: notepad Posted at: 2017-03-06T22:12:35.727Z Reads: 46

```
I was gonna put two of these batteries in 12s1p config to get the needed voltage.

My aim is to get around 28-30mph, so I wasn't gonna skimp out on the VESC.
```

---
## \#7 Posted by: Jebe Posted at: 2017-03-06T22:15:35.818Z Reads: 39

```
[Use this calculator here to calc speed with particular motors and gearing](http://toddy616.blogspot.com.au/2013/07/electric-skateboard-calculator.html)
```

---
## \#8 Posted by: notepad Posted at: 2017-03-06T22:18:32.983Z Reads: 36

```
What motor efficiency do you thing I should put in?
```

---
## \#9 Posted by: Jebe Posted at: 2017-03-06T22:52:51.684Z Reads: 31

```
go 70 - anything else is a bonus
```

---
## \#10 Posted by: notepad Posted at: 2017-03-06T23:06:05.992Z Reads: 27

```
Cool,

70% efficent on 12S,  with a 16-36 gear ratio and 80mm is 35kph (21mph).

Do you know if you can buy maybe a 30 teeth gear or maybe 90mm wheels,  and I was aiming to get to around 50kph (30mph),  or should I just conciser getting a higher kV rated motor, maybe a <a href="https://hobbyking.com/en_us/turnigy-aerodrive-sk3-5065-236kv-brushless-outrunner-motor.html">236kv </a> one?
```

---
## \#11 Posted by: jmasta Posted at: 2017-03-06T23:08:35.870Z Reads: 24

```
Long story short, don't use over 170kV at 12S with the VESC because of the ERPM limit

And a 30T wheel pulley won't work because of the smaller diameter.... 32T is possible but can be tricky

Also, consider different batteries.  Those Multistar batteries have a terrible reputation and have been known to have lots of voltage sag
```

---
## \#12 Posted by: notepad Posted at: 2017-03-06T23:15:26.607Z Reads: 23

```
Interesting, I didn't know that, so i am glad I do now as I am planning my first build!

Basically 30mph is my goal with about 20 miles of range.  Is there anything you could recommend to get those speeds?
```

---
## \#13 Posted by: notepad Posted at: 2017-03-06T23:19:18.532Z Reads: 22

```
How about dropping down to a 10S battery with 80mm wheels?

Gears would be 16-32 with a motor of 236kV.

how does that sound?
```

---
## \#14 Posted by: jmasta Posted at: 2017-03-06T23:28:03.392Z Reads: 21

```
Use that calculator to find a good mix of gear ratios:

* The motor pulley should be between 14T and 20T (Anything bigger and the pulley starts to interfere with the motor mount bolts. Anything smaller and the belt slips).  

* Wheel pulleys are usually 32T to 40T (Smaller gives more speed and less torque. Smaller also means more road clearance.  But anything under 32T is too small to physically mount it to the wheel)

I made my own pulleys, so I was free to choose any gear ratio.  But if you don't have that capability, you will need to use whats on the market and your gear ratios will be more constricted
```

---
## \#15 Posted by: notepad Posted at: 2017-03-06T23:31:14.333Z Reads: 20

```
Thats a good bit of information!!

Thank you so much for the help, At this rate I should make a collection for new people because this is great.

You've helped so much,  than you!
```

---

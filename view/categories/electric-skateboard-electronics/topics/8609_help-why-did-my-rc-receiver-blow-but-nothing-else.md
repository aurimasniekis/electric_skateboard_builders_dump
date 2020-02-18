# HELP &#124; Why did my rc receiver blow but nothing else?

### Replies: 12 Views: 662

## \#1 Posted by: Pathaim Posted at: 2016-08-29T23:10:38.908Z Reads: 67

```
Hey guys, yesterday when building my board an incident occurred, was working fine til i moved stuff around and i connected the batteries together wrongly (in the series connector), i wasn't focusing and believe i accidentally plugged in the 2 negatives of the battery instead of negative to positive. when i plugged in the rc receiver it blew, why did it blow but nothing else? (pretty sure the esc is fine cause still spark when i plug it into the battery) Thanks.
```

---
## \#2 Posted by: michaeld33 Posted at: 2016-08-29T23:28:04.409Z Reads: 62

```
The ESC could still be broken, just because it sparked does not mean it works.
```

---
## \#3 Posted by: Pathaim Posted at: 2016-08-29T23:30:49.580Z Reads: 60

```
any way to test it?
```

---
## \#4 Posted by: michaeld33 Posted at: 2016-08-29T23:31:03.499Z Reads: 56

```
is it a vesc? Also what batteries are you using?
```

---
## \#5 Posted by: Pathaim Posted at: 2016-08-29T23:33:35.905Z Reads: 51

```
no, hobbyking esc. 
http://www.hobbyking.com/hobbyking/store/uh_viewItem.asp?idProduct=49242
```

---
## \#6 Posted by: Pathaim Posted at: 2016-08-29T23:34:27.909Z Reads: 48

```
using 2x 3s 5200mah multistar batteries in series. i had it working before before unplugging stuff and being an idiot and not looking lmao
```

---
## \#7 Posted by: michaeld33 Posted at: 2016-08-29T23:38:01.067Z Reads: 45

```
The first thing that worries me about this is that it is water cooled, and you are running it at 6s, so unless you have a water cooled skateboard (which would be sweet), you are going to run into an issue eventually most likely. The other thing is there shouldn't be an issue here, you are running a 6s setup, but you accidently hooked it up in parallel, so you were only giving it 3s (that's how I understood it at least), therefore, something must've been backwards or incorrect because it should work fine. Was the servo cable plugged in right?
```

---
## \#8 Posted by: Pathaim Posted at: 2016-08-29T23:52:49.226Z Reads: 42

```
servo cable? i don't think i plugged it in parralel because battery 1 negative went into battery 2 negative, and battery 1 positive and battery 2 positive went into the xt60 connector. I did not change ANYTHING from when it was working except i might of accidently plugged in the batteries wrong
```

---
## \#9 Posted by: michaeld33 Posted at: 2016-08-29T23:55:14.693Z Reads: 41

```
when you connect negative to negative and positive to positive, that's referred to as parallel. Positive to negative//negative to positive is known as series. I am asking if you plugged in the ESC cable that connects to the receiver backwards.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2016-08-29T23:57:58.948Z Reads: 40

```
Did you try with another receiver ???
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2016-08-30T00:00:47.811Z Reads: 42

```
Also, maybe there some protection on your ecs for these kind of manipulation, but the receiver might not have these... Or you just blowup the 5v regulator of your esc... Did you have been able to run a motor since the incident, or you assume it work because of the spark ?
```

---
## \#12 Posted by: Pathaim Posted at: 2016-08-30T00:23:30.177Z Reads: 34

```
might of plugged it in backwards too but shouldnt create a spark, also haven't tested it yet getting another reciver soon. and yes i assume it works. also should i take the cover off and put a hetsink on the esc
```

---

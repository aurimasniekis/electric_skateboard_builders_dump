# Dual Motors Mountainboard 8s 5000mah

### Replies: 8 Views: 607

## \#1 Posted by: zblad Posted at: 2017-06-07T02:15:13.640Z Reads: 105

```
Hello,

I finally finished my mountainboard and this thing is insane.  My only issue is I cant start from a dead stop without my motors cogging and going crazy.  I am using...
Dual Vesc
Dual 213kv sk3 motors
Two 4s 5000mah zippy batteries in series

if I did my math right my battery should be able to handle 150amps and the motors I believe are able to handle 65amps.

My motors are setup as BLDC its also strange when I'm driving it feels like one of the motors will cut out and then kick in and then cut out.  Not sure if that's the traction control or not.  Let me know if you need to see my settings and I will post them up.
```

---
## \#2 Posted by: Nowind Posted at: 2017-06-07T12:57:06.123Z Reads: 79

```
Check your startup boost parameter... set it to 0.05 or at max 0.1.... make things better.... 

Also what you set as motor current?

Whats your gear ratio ?

8S on Vesc on EMTB is not ideal too IMO
```

---
## \#3 Posted by: zblad Posted at: 2017-06-07T18:46:45.543Z Reads: 55

```
I have my battery max at 65amps and my motor max at 65amps.  What should I have had used instead of 8s?  I read online and people said 8s was a safe voltage and that anything greater tends to burn the VESCs up...
```

---
## \#4 Posted by: DavidC Posted at: 2017-06-07T18:50:50.678Z Reads: 51

```
VESC don't give much amps, contrary to ESC, so you must go with at least 10S ou better 12S! It will be quite safe unless you choose FOC that will probably FUCK the VESC.
```

---
## \#5 Posted by: zblad Posted at: 2017-06-07T19:01:44.670Z Reads: 46

```
GRRR I just got my batteries yesterday if I would have known I would have went 12s right off the bat.
```

---
## \#6 Posted by: DavidC Posted at: 2017-06-07T20:10:38.626Z Reads: 41

```
One more 4S Lipo and you have a 12S system using them in series
```

---
## \#7 Posted by: zblad Posted at: 2017-06-07T20:12:14.947Z Reads: 40

```
haha yeah thought of that right after damn shipping was so spendy tho lol.  So do you think I wont get smooth start unless I go to 12s?
```

---
## \#8 Posted by: Challlsss Posted at: 2017-06-07T20:23:47.912Z Reads: 40

```
probably not
I have 6S (regular longboard) 
and unless it's really really smooth I have to kick start
```

---

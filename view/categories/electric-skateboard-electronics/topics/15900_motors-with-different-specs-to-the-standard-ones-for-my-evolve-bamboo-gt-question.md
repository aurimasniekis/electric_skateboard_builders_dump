# Motors With Different Specs to the Standard Ones for My Evolve Bamboo GT - Question

### Replies: 11 Views: 2888

## \#1 Posted by: Milly1990 Posted at: 2017-01-11T11:07:27.522Z Reads: 265

```
Hello Everyone, Hopefully there are a few motor / electronic gurus out there for this question!

Basically i have an Evolve Bamboo GT, the stock motors that come with the board are 150kv & 1500Watts each. (2of) So my question is, I have found 2 different motors that are dimensionally identical and also come with the same wiring and plugs! one is rated at 140kv and the other at 200kv. I have no idea how i calculate the wattage from these values. I understand that KV is RPM per volt but that's about it. The main reason i have this query is because i would like to know what would happen if instead of the 150kv motor i used 140kv or the 200kv and are they compatible with the motor controller in the board? What kind of effect would it have on the battery and speed? would it cause any kind of electrical damage?

See attached motor data sheet for the 2 motors i have found <img src="/uploads/db1493/original/3X/2/0/205c353d194b4cfe22f1f2b57a7b0cefe93e53a0.PNG" width="690" height="174">

from what i understand the BGT is 36V. i get motor RPM of around 5400 so...
RPM divided by Volts = kv =
5400 Divided by 36 = 150
150kv
this motor is rated to 1500 watts from what i gather by "3000 watts of duel motor power"

The new motor is rated at 1200 watts and is140kv or.. motor 2 is 1650 watts and 200kv

Any info on this would be much appreciated. I am basically trying to find out if these motors are suitable for my Evolve Bamboo GT and if so, what the differences of the motors would make to the board and battery performance!

Thanks :grinning:
```

---
## \#2 Posted by: JLabs Posted at: 2017-01-11T11:45:35.129Z Reads: 238

```
The higher the kv the more the speed, but you looks some torque. You can use http://calc.esk8.it to calculate top speed. Changing the motor will not cause any electrical damage.

Edit: I wouldn't buy the 140kv if you have 150kv already, there really wouldn't be a difference. The only reason I would change is if the motor was bad.
```

---
## \#3 Posted by: Milly1990 Posted at: 2017-01-11T12:03:18.395Z Reads: 231

```
Yep agree 100% the main reason was for spare motors and spare parts, possibly a custom build using some evolve parts further down the line.

Would the remote control read out, display the correct the top speed with the 140KV motor or would the board 'think' the speed is calculated as it is programmed for 150kv?
```

---
## \#4 Posted by: JLabs Posted at: 2017-01-11T12:38:12.627Z Reads: 215

```
Not sure how they calculate it. It may but Evolve's speed controller is not my cup of tea
```

---
## \#5 Posted by: Milly1990 Posted at: 2017-01-11T12:51:59.373Z Reads: 208

```
What effect does a lower kv and lower wattage motor have on the battery ?
```

---
## \#6 Posted by: lrdesigns Posted at: 2017-01-12T06:26:32.269Z Reads: 176

```
If in practice it draws less current then it will be more gentle on the battery. But 10kv is a pretty small difference.
```

---
## \#7 Posted by: Milly1990 Posted at: 2017-01-12T12:59:49.222Z Reads: 164

```
Ok cool, thanks for that. yea it draws less amps so i guessed it would prolong the battery life and possibly get a little more range!
```

---
## \#8 Posted by: Maxid Posted at: 2017-01-12T14:12:38.080Z Reads: 155

```
My guess is that you will not see or feel a difference with the 140kv one compared to the 150kv motor.
With the 200kv nobody knows how the Evolve speed controller deals with this.
The VESC needs motor detection to run smoothly so I would expect that you'd need to do the same when you attach a different motor.

My recommendation: stick to the 140kv one. The Evolve ones will most probably be just a rebranded version of this anyway.
```

---
## \#9 Posted by: Milly1990 Posted at: 2017-01-12T14:17:08.348Z Reads: 140

```
Ok cool, thanks for the help and the explanation.

I can see on the remote the RPM of each motor when they are in use. with these 140kv motors would the wheel speed and RPM be correct? is it a case of getting the RPM somehow from the motor sensors or is it electronics in the board that are programmed for 150kv? does the board calculate the speeds by knowing how many Volts and amps its giving the motor or does the signal come directly from the motor?

Any ideas?
```

---
## \#10 Posted by: Maxid Posted at: 2017-01-12T14:20:43.622Z Reads: 136

```
It should since the speed controller knows about the revolutions (otherwise how could it make the motor turn).
Don't worry too much about the kv - I doubt that Evolve had them specially made and/or that the 140kv number is set in stone. The motors do probably have kv values somewhere in between.

This is all just guessing however.
```

---
## \#11 Posted by: Milly1990 Posted at: 2017-01-12T14:27:10.368Z Reads: 130

```
Ahhh ok, i understand. Thanks for that mate, really appreciate the info :)
```

---

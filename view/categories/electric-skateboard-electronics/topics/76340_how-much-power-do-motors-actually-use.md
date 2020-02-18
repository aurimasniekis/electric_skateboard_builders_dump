# How much power do motors actually use?

### Replies: 11 Views: 408

## \#1 Posted by: Slydunan Posted at: 2018-11-28T05:47:20.724Z Reads: 180

```
From hub motors with <500w listed max to 6374 with >3000w, how much do these motors actually use to push you around? Do different setups use significantly different amounts of power to accomplish the same amount of work? Lets say a belt drive and a hub motor going 35mph with a 150lb person...is there a way to to estimate the power needed to accomplish this?

Also is there even a point in larger motors if you cant supply the power to make use of it?  For two 6374 motors at 42v and they will need >100amps to even come close to that max. A 12s5p battery with 15a discharge cells wont even get you there.
```

---
## \#2 Posted by: pat.speed Posted at: 2018-11-28T05:55:24.900Z Reads: 172

```
The general consensus is street boards take about 250-300w at speed of 25km'h
```

---
## \#3 Posted by: Okami Posted at: 2018-11-28T06:19:10.809Z Reads: 163

```
I think this can be compared to cars.. bigger motors just have more 'resource' to push you faster / harder, has more torque..

Small size hub motor will probably be like small engine car.. a lot slower, takes a while to accelerate and struggles to do hills.

Havent rode low power / high power hub motors but this is how I feel about power delivery in general
```

---
## \#4 Posted by: linsus Posted at: 2018-11-28T10:35:56.555Z Reads: 124

```
Traditionally the power stated is called "rated power". As in what this motor MAX is able to perform. What conditions you need to get that power. Is a whole other question.

This is elementary physics. Combined with the basics of how an electric motor works. Internet is a hellova drug. Use it. Or pick up a book. Just my two cents.
```

---
## \#5 Posted by: iTzDiego Posted at: 2018-11-28T10:39:20.753Z Reads: 108

```
[quote="linsus, post:4, topic:76340"]
Combined with the basics of how an electric motor works. Internet is a hellova drug. Use it. Or pick up a book. Just my two cents.
[/quote]
got any reccomendations or links?
```

---
## \#6 Posted by: linsus Posted at: 2018-11-28T12:11:23.518Z Reads: 96

```
Any educational basic level book on electric power, electric drive systems. I'd recommend the books I have but they're in swedish..Guess interwebz is your best bet unless you visit a library...fast search gave me the book "electric motors and drives" seems decent

Edit: even found a PDF of 3d edition :D http://www.emic-bg.org/files/Electric_Motors___Drives.pdf
```

---
## \#7 Posted by: Slydunan Posted at: 2018-11-28T12:56:25.043Z Reads: 84

```
Did you even read what my question was?
```

---
## \#8 Posted by: linsus Posted at: 2018-11-28T13:09:28.134Z Reads: 78

```
....yes?. You're wondering how do to force calculations and translate them to power.. again. elementary physics. 

question number two is regarding larger motors. Again. Basic induction motor knowledge. Do some searching instead of trying to be spoonfed answers.
```

---
## \#9 Posted by: Okami Posted at: 2018-11-28T13:47:18.976Z Reads: 68

```
I think some info is in hummie hubs thread, otherwise check metr vesc logs people have posted.

Profesor shart.. had some graphs but as far as I know he got banned but u might be able to find his posts, unless they got deleted also
```

---
## \#10 Posted by: Jalapeno Posted at: 2018-11-28T13:54:38.689Z Reads: 63

```
Search this forum for https://metr.at/r/
It will get you for example posts like these https://www.electric-skateboard.builders/t/vesc-hw-4-12-temperature-comparison/23230
Then you can search for the type of motors you have/want and desired speed.
But do take voltages and especially currents read with a pinch of salt (find multiple logs) because there is no guarantee that the ESC is calibrated and spitting out correct measurements.
```

---
## \#11 Posted by: Slydunan Posted at: 2018-11-28T14:05:32.269Z Reads: 55

```
Thanks, thats very helpful!
```

---

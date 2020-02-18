# Motor detection fails - *measure flux linkage* - Conclusion phase wire shorrted

### Replies: 40 Views: 856

## \#1 Posted by: Superflim Posted at: 2018-12-26T10:41:36.084Z Reads: 122

```
So I have this problem with my motor. At the beginning it was making a weird noise when I powered the motor, I solved this by re-doing the motor detection. Now something had happened during a test ride and 1 of the 3 motor cables got loose. 

When I try to do motor detection to let it flow fluently again, I can't because  'Measure flux linkage' doesn't work. The motor tries to spin and fails miserably, or does spin but with that terrible noise, and still gives off a 'failure'. 
I'm using VESC-tool

What have I tried:
- re-uploaded firmware
- re-booted the system
- changing the variables (amps and the other I forgot), which was said could help in the 'help' tab of the program. Before all of this happened I didn't even have to change those it already worked solid.
- replugged wires

I've checked out multiple topics but I can't come to an conclusion. I never extended my motor cables so a bad solder couldn't be it and basically (I think) nothing happened in the past days what could have caused this problem.
```

---
## \#2 Posted by: dareno Posted at: 2018-12-26T11:25:29.668Z Reads: 104

```
[quote="Superflim, post:1, topic:79003"]
‘Measure flux linkage’
[/quote]

The flux capacitor has gone bad.  You need to source a new unit and re-install.

https://www.oreillyauto.com/

Use this link and tap 121G into the search engine
```

---
## \#3 Posted by: Superflim Posted at: 2018-12-26T11:30:31.535Z Reads: 99

```
Could you point me in the right direction? What is that where can I find it.

I’m by no means advanced with technical stuff, idk maybe it’s above my skill level
```

---
## \#4 Posted by: Superflim Posted at: 2018-12-26T11:37:29.555Z Reads: 96

```
It’s not even 1 April yet :joy:
```

---
## \#5 Posted by: dareno Posted at: 2018-12-26T11:40:30.121Z Reads: 94

```
I'm sorry but it just seemed too good an opportunity to miss.  :sunglasses:
```

---
## \#6 Posted by: dareno Posted at: 2018-12-26T11:45:22.639Z Reads: 92

```
First thing to try is physical.  Take the belt off and spin it by hand.  Does it have a lot of resistance?
If it does then do not under any circumstances do another detect.  If it spins freely and as it used to then you could try to up the duty cycle and re detect.
```

---
## \#7 Posted by: Superflim Posted at: 2018-12-26T11:47:00.980Z Reads: 87

```
I don’t think it has more resistance than usual
```

---
## \#8 Posted by: Andy87 Posted at: 2018-12-26T11:47:08.823Z Reads: 88

```
first spin it by hand and than take the bell off.
if you take the bell off you can´t spinn it by hand :stuck_out_tongue_winking_eye:
```

---
## \#9 Posted by: Superflim Posted at: 2018-12-26T11:48:24.773Z Reads: 81

```
What do you mean by the duty cycle? Where can I find it
```

---
## \#10 Posted by: dareno Posted at: 2018-12-26T11:50:49.733Z Reads: 85

```
Stop it andy we've had enough fun with this fella.  The belt.  The belt off.  Not the bloody bell.  :joy:

You got a screen shot of the duty cycle window for him?
Its just below the detect button.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-26T11:54:19.307Z Reads: 84

```
first the dual cable from @Wraith and than the "belt"...
I really was reading bell... sorry for that... :joy:

But @Superflim which motor is it?
can you hear that strange sound also when turning with hand?
you sure no any of the phase wires touch each other with blanc parts?
you doing motor detection without belt on, right?
because that can be a reason too.
did you try motor detection in bldc too or only foc?
```

---
## \#12 Posted by: Superflim Posted at: 2018-12-26T12:00:31.676Z Reads: 84

```
Alien power systems 6374 200kv

No strange sounds when turning with hand

No nothing touching but there is a bit of wire exposed where the heat shrink got off. I’ll put some new on.

Yes I do without belt.

Have tried bldc and foc both
```

---
## \#13 Posted by: dareno Posted at: 2018-12-26T12:06:14.756Z Reads: 83

```
Get the detect page up and look just below the little detect arrow.  There is a window with duty cycle there.  Up it it small increments until the vesc detects the motor.  When a motor fails detection it will cog and make a brrrrrrrr noise.
```

---
## \#14 Posted by: Superflim Posted at: 2018-12-26T12:09:03.371Z Reads: 83

```
You mean this? ![555fcf77c706894681fc829237a77f08|690x426](upload://5EGUtZXUN6vLSUws5pBT9PEWNpx.png)
```

---
## \#15 Posted by: dareno Posted at: 2018-12-26T12:13:19.149Z Reads: 79

```
Go to the motor detect page and screen shot it
```

---
## \#16 Posted by: Superflim Posted at: 2018-12-26T12:18:17.498Z Reads: 79

```
![eb32f7b0c12286e2ded64bd6c46bfc6a|690x412](upload://hXdYSpZwzLlsG0MvMorrxJIUuO6.png)
```

---
## \#17 Posted by: dareno Posted at: 2018-12-26T12:24:03.950Z Reads: 77

```
@Andy87 Mate can you help this guy?  
@Superflim I use bldc tbh.  Apologies for the wasted time but I'm sure andy will sort you out.  foc is like a different language to me.
```

---
## \#18 Posted by: Andy87 Posted at: 2018-12-26T12:31:06.291Z Reads: 77

```
I never needed to change any parameters to get my motor detection successfull done.
@Superflim if you have a multimeter you could measure the resistance between tha phase wires. A to b, a to c and b to c.
They all should have the same resistance
```

---
## \#19 Posted by: Wraith Posted at: 2018-12-26T12:33:45.643Z Reads: 77

```
Yeah I’m gonna put those cables on the side for now lol
```

---
## \#20 Posted by: FredrikHems Posted at: 2018-12-26T12:43:43.192Z Reads: 79

```
Check for faults. I had this exact problem, and supposedly there was a drv fault.
```

---
## \#21 Posted by: Superflim Posted at: 2018-12-26T12:49:51.175Z Reads: 76

```
Luckily no fault codes
```

---
## \#22 Posted by: Superflim Posted at: 2018-12-26T12:50:10.853Z Reads: 76

```
How am I supposed to measure the resistance? I have to cut the wires?
```

---
## \#23 Posted by: Andy87 Posted at: 2018-12-26T12:51:00.227Z Reads: 78

```
No. Just set your multimeter to ohm.
Tha measure from bullet connector to bullet connector
```

---
## \#24 Posted by: Andy87 Posted at: 2018-12-26T12:51:17.763Z Reads: 78

```
That for all three combinations of cables
```

---
## \#25 Posted by: Superflim Posted at: 2018-12-26T13:09:20.396Z Reads: 78

```
found it @andy87

damn what now 
![15458296888949025679972401770035|375x500](upload://eUZn3o1XwunloShzETMPcX3QXCc.jpeg)
```

---
## \#26 Posted by: Andy87 Posted at: 2018-12-26T13:15:44.535Z Reads: 72

```
how old is the motor?
if you ordered the motor directly form APS you can just sent bruno a mail. very likely they will just replace it if it´s not too old motor.

don´t do any detection again as long as there is a short.
you could fry your vesx with it.
```

---
## \#27 Posted by: Superflim Posted at: 2018-12-26T13:16:23.409Z Reads: 75

```
Got it second hand.
No idea how old it is tbh...

Any chance I could repair this myself?
```

---
## \#28 Posted by: Andy87 Posted at: 2018-12-26T13:18:02.915Z Reads: 72

```
https://www.electric-skateboard.builders/t/not-sure-if-you-have-shorted-phase-wires-here-is-how-to-test-them-without-frying-your-esc/78693?u=andy87
```

---
## \#29 Posted by: Andy87 Posted at: 2018-12-26T13:20:31.104Z Reads: 70

```
you can try to get some heat shrink over the phase wire.
if that works it would be the most easy way.
if not, you can cover the broken part with epoxy.
or take off the top part and solder a new phase wire on.

how ever, do the test i linked before you connect the motor to the vesc after you fixed the damaged part.
```

---
## \#30 Posted by: Superflim Posted at: 2018-12-26T13:23:36.192Z Reads: 64

```
But the result of the first 2 solutions named in your post above leave the battery with 2 phase wires left?
```

---
## \#31 Posted by: Andy87 Posted at: 2018-12-26T13:29:30.683Z Reads: 62

```
I don´t understand what you mean.

just cover the damaged isolation with heat shrink..
if that´s not possible you can cover tha part with is damaged with epoxy to isolate the phase wire again.
if you do so, than take care that no epoxy comes into the motor and the bearings. best way is to take off the bell and cover the suroundings with tape and than fill up the area where the cables come out with epoxy.
to make sure the short is gone after, you should check the phase wire with the multimeter before you connect the motor to the esc.
```

---
## \#32 Posted by: Superflim Posted at: 2018-12-26T13:31:44.602Z Reads: 62

```
I'll first check if it is really shorted
```

---
## \#33 Posted by: Superflim Posted at: 2018-12-26T13:42:51.545Z Reads: 58

```
[Uploading...]()

I don't know if you can see it very clearly but almost all the wires are torn apart, not just the insulation
```

---
## \#34 Posted by: Andy87 Posted at: 2018-12-26T13:51:34.701Z Reads: 58

```
Pictures still uploading.
You uploading a movie? 😅
```

---
## \#35 Posted by: Superflim Posted at: 2018-12-26T13:53:18.324Z Reads: 61

```
![IMG_20181226_145239|375x500](upload://tN8Iy5cYucVPbdg4jWzjvHel3IC.jpeg)

not the best pic but from what I can see here only is one the insulation is still intact
```

---
## \#36 Posted by: Andy87 Posted at: 2018-12-26T13:59:26.770Z Reads: 58

```
That’s the part where the phase wire is soldered to your silicon wire.
The only good way to fix this is to solder on new wires.
As min thats the only option i know in this case.
```

---
## \#37 Posted by: Superflim Posted at: 2018-12-26T14:14:00.219Z Reads: 53

```
if I would solder the wires back to each other do you think it will work? do I really need new wires?
```

---
## \#38 Posted by: Andy87 Posted at: 2018-12-26T14:17:52.345Z Reads: 56

```
Nu i can’t see everything so good as you, but mir me it looks like as min on the middle phase wire already more than half of the wire off.
So sooner or later it will rip off totally and at the moment you would push all amps over a smaller diameter than the other phases.

To solder a new wire on the phase and isolate everything again should fix it, but it’s definitely not an easy thing.
Not sure if I would do it with mine or just buy a new motor.
```

---
## \#39 Posted by: Superflim Posted at: 2018-12-26T14:22:00.730Z Reads: 55

```
I guess I'll just give it a try and if it doesn't work out I've learned something new!

thank you for the advice @andy87 @dareno 

awesome community! I <3

edit: all of the wire is off I think, or maybe 1/10 is left ;)
```

---
## \#40 Posted by: Andy87 Posted at: 2018-12-26T14:24:01.356Z Reads: 55

```
Check YouTube, maybe you can find some tutorials how to do it best.
Don’t forget to make a documentation about it and post it here.
If you done it successfully it could help other people in future too 😉
```

---

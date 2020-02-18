# I have a problem with my engine for my skateboard

### Replies: 6 Views: 431

## \#1 Posted by: Hansg Posted at: 2017-06-20T18:16:16.228Z Reads: 86

```
Hi my name is Hans Gomez i am new in this topic, i want you i help with building my skateboard electric. I bought this Enertion engine but this is not fast. I want to know that I need to reach a high speed, 
I currently have the following components:

- Enertion Engine
- Batery 5000 mAh
- Speed control

In the official page says that this engine reaches 45 km / h

https://youtu.be/pRkmhat_Pd4
```

---
## \#2 Posted by: leonsc Posted at: 2017-06-20T18:20:42.196Z Reads: 79

```
What cell count is the battery ur using also its a motor not engine ☺
```

---
## \#3 Posted by: gran4babidi Posted at: 2017-06-20T18:52:40.444Z Reads: 70

```
I am no expert but I am pretty sure that with just one 3s 5200mah battery you will never get much speed... but I could be wrong lol :smiley:

you can always use the calculator to get an estimate of the speed youre looking for.
http://calc.esk8.it/#{"batt-type-lipo":1,"batt-cells":3,"motor-kv":190,"system-efficiency":80,"motor-pulley-teeth":15,"wheel-pulley-teeth":36,"wheel-size":83}|
```

---
## \#4 Posted by: pennyboard Posted at: 2017-06-20T18:58:10.640Z Reads: 64

```
Okay, first you should put heat shrink or at least electrical tape around the bullet connectors on the phase wires, cause if they short together while your running the motor it could kill your esc (I know this will kill a vesc and am guessing that it will probably kill the esc you are using too). 

The reason you are not going fast is that you are using a 3 cell battery. The rpm of the motor is determined by the voltage put through it. This rotor is 190kv I believe so it will spin at 190 rpm for every volt put through it. So if you put 11.1 volts through it, which is the voltage that your battery puts out, then it will spin at 2,109 rpm. 

In order to increase the speed of the motor, you need to increase your battery voltage. This is done by buying more batteries like you have and wiring them in series to increase the voltage. Adding one more 3 cell battery will double your voltage and hence double you speed. (because two 3 cell batteries in series looks like a 6 cell battery, which has 22.2 volts).
```

---
## \#5 Posted by: Mikenopolis Posted at: 2017-06-20T19:16:40.896Z Reads: 53

```
you'll need 10s or 12s in order to hit that speed.
```

---
## \#6 Posted by: sl33py Posted at: 2017-06-20T19:26:20.486Z Reads: 52

```
As other have already told you - one 3s battery will give you poor performance and low speed.  Getting a second battery (match the exact same battery you have now), will double your speed.

If you want to figure out speeds - use an online speed calculator:

http://calc.esk8.it (pretty nice - kudos to whomever made this)
<img src="/uploads/db1493/original/3X/c/f/cf27d2747342d9e58400fd3c453391d3189d5efc.jpg" width="369" height="499">

Now you can look at gearing changes to hit the speeds you want.  First i'd go with more voltage - assuming your ESC can handle more than 6s.  Make sure of this before you go higher voltage than 6s (22.2v nominal).

When you want to go faster you will typically adjust voltage first, then gearing.  Last a higher kv motor (but that's pretty $$$, so i'd avoid if possible).

If you really want to go fast, i'd also suggest a different skateboard deck/type.  The short double kick skateboard in your video will be tough to control at higher speed (your skill obviously unknown).  A longer longboard deck, or downhill deck would be easier to control at higher speeds.

Good luck!
```

---

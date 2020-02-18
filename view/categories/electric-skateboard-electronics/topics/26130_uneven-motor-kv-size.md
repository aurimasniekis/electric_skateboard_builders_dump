# Uneven motor kv/size

### Replies: 5 Views: 618

## \#1 Posted by: niktwo17 Posted at: 2017-06-25T10:08:25.353Z Reads: 71

```
Hey guys
Ive been riding my eboard since 4 months and i really enjoy it. Im using a VESC, 10s 5000 20c turnigy battery and an alien 6374 170kV motor.
However, i want more power and acceleration now.
Now the question:
Is there any problem combining another motor brand/size/kV with my existing motor?
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-25T10:15:30.323Z Reads: 71

```
I only have experience with 1 motor FYI so just talking based on theory here.  The second motor will have a second VESC and the VESCs will communicate over CANbus so one will get the signal from the remote and pass along the info over the CANbus but I believe both will independently determine the actual signals/power being sent to the motor so in theory that sounds like it should work.  That said if you have different motors you're going to have different torque curves and other characteristics so there is going to be some imbalance between the force applied to one wheel vs the other.  I'm really pretty surprised to hear you think it's lacking on acceleration seeing as how I have a very similar setup (slightly lower kv 149) and have never had any issues with torque (I use my board as primary transportation along with public transit, so ride up hills as often as they come up in the Chicagoland area and have let much bigger people try my board and had it almost run out from under them cause of the push).

**Edit** Would be curious to know what problems you're having in particular does the motor just keep snapping back instead of being able to rotate or what's the result of not having enough torque? just the feeling of acceleration or something else?
```

---
## \#3 Posted by: niktwo17 Posted at: 2017-06-25T10:30:43.227Z Reads: 62

```
Ok thanks for your answer
So its not that the board is too slow, it manages to throw almost everyone of. I gets me to topspeed (40 kmh) in round 4 seconds. 
Actually the transmission is problematic. My carbon moror mount cant hold full power really and bends. On my 80a kegels i can do burnouts.
Ive tried a dual setup and acc/braking is just smoother and less stressfull for the components i think
I also became a bit speed obsessed and want more now :joy:
But an alien 6355 170kV should work without problems right?
```

---
## \#4 Posted by: wafflejock Posted at: 2017-06-25T11:15:15.912Z Reads: 59

```
Heh yeah I would imagine if it's the same kv and just slightly different torque you probably won't have any issue really I mean even two motors of the same model from the same manufacturer are going to have some variations in the first place and so long as each is being given the same throttle signal and attempting to get to the same speed I don't think it'd be more of an issue than if they were from the same manufacturer.  Hopefully someone with experience with this will chime in.

Keep in mind too though you're just adding more torque/acceleration not to the top speed so if you're just going for higher top end you'd either need to bump the voltage up or bump up the wheel size or bump up the kv on the motor.
```

---
## \#5 Posted by: laurnts Posted at: 2017-06-25T13:06:17.470Z Reads: 43

```
@lowGuido Did this before.  http://www.electric-skateboard.builders/t/uneven-dual-rear-drive/113
```

---

# 6s battery on a 10s motor?

### Replies: 13 Views: 5390

## \#1 Posted by: forangejuice Posted at: 2016-01-04T16:21:53.385Z Reads: 186

```
As the title says im wondering if i could use a 10s motor with a 6s battery? This would work out really cheap for my budget for my build but if necessary would buying 2 6s batteries and putting them in series to give an equivalent 12s voltage work with the 10s motor?
```

---
## \#2 Posted by: NerijusM Posted at: 2016-01-04T16:27:08.947Z Reads: 186

```
Will work perfectly fine.
Just keep mind on KV (RPMs of motor).
```

---
## \#3 Posted by: forangejuice Posted at: 2016-01-04T16:37:34.023Z Reads: 184

```
oh wow im surprised that 6s would work on 10s motors, so its a 236kv motor does this change anything?
```

---
## \#4 Posted by: NerijusM Posted at: 2016-01-04T16:42:40.510Z Reads: 181

```
You will not get full power for motor, but you will get all power from 6s setup.
KV is good for eboard. You can use that motor.
```

---
## \#5 Posted by: forangejuice Posted at: 2016-01-04T16:44:28.013Z Reads: 179

```
Thanks man!! Really apprecited
```

---
## \#6 Posted by: longhairedboy Posted at: 2016-01-04T17:19:11.511Z Reads: 170

```
10S is the maximum for those motors, so yes 6S will work out just fine. I used to use 245kv motors on my 6S build, and currently i have 270kv motors on it. 

higher kv basically means the motor spins faster with less torque, and lower kv means it spins slower with more torque. You can finely tune the performance of the motors a little more by adjusting the pulley ratios also.
```

---
## \#7 Posted by: Hummie Posted at: 2016-01-04T17:26:11.772Z Reads: 164

```
Doing 12s with a 10s motor, likely will be ok.  The enamel on the windings will breakdown with too much voltage and manufacturers typically use the same enamel on motors that they will rate for different max voltage.  The bearings max rpm are often the limit.  Or they will assume too many amps will be pushed through with a high voltage but it isn't really the voltage that's the problem
```

---
## \#8 Posted by: onloop Posted at: 2016-01-05T00:13:23.266Z Reads: 155

```
[quote="Hummie, post:7, topic:907"]
The enamel on the windings will breakdown with too much voltage
[/quote]

I am not sure about the accuracy of this statement, I think it's better to say this: The insulative coating on motor windings is rated based on the temperature it can handle if the there is too much HEAT (approx 300deg c) the insulation may melt. 

Generally speaking higher battery voltage = lower motor current under load. So higher voltage should generally mean less heat in the motor. Heat increases as current increases.

Now we have ESC's that can handle higher voltage, Such as the VESC which can handle 12S, there is really no reason not to use high voltage. Simply need to choose your desired speed and design the drive train around that. 

The other consideration If you are using LIPO it means charging is more complicated as most LIPO chargers are only able to charge 6S batteries, so you need to charge in parallel.

I wrote an article that goes into detail about designing a drivetrain: 
http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
```

---
## \#9 Posted by: Hummie Posted at: 2016-01-05T03:12:28.260Z Reads: 130

```
The enamel will burn up with heat as you say.  There are enamels rated for different heat.  But the purpose of the enamel is to stop shorts between the windings.  It's insulation just as with wire that is insulated with silicone but it's thinner.  It's so thin that it can be broken down by high voltage. So I read

Also higher voltage does not a cooler motor make. Amps and amps alone make inductance in a motor.  I'm not sure of the details and have been trying to find out how voltage effects things.  You can push more amps with a higher voltage.  Having a higher voltage necessitates more amps if the resistance stays the same according to ohms law V = I X R

The goal of higher voltage will get more power possibly as the voltage is the force pushing the amps but with an electric vehicle you could run a very low voltage and use a high kv motor and other than the losses in the wires there aren't any drawbacks.  There is that ability to jam amps in the motor with higher voltage though
```

---
## \#10 Posted by: trbt555 Posted at: 2016-02-29T16:37:50.228Z Reads: 104

```
Power P=VxI (Watt)
I is inversely proportional to V.
For a given load (requiring power P), current will drop as voltage increases.
You can't just apply Ohm's law to a brushless motor, because the motor has an impedance, and we're not using DC but trapezoidal AC to run the motor.
Heat losses are quadratically proportional so if you halve the current by doubling the voltage, you'll quarter the heat losses.
So yes, higher voltage equals cooler electronics, including motor.
```

---
## \#11 Posted by: Hummie Posted at: 2016-02-29T18:14:10.587Z Reads: 103

```
Thank you for explaining this. I'm still confused about inductance in the motor though. I though inductance was only a product of amps x turns.  How does voltage make a motor turn? Is an amp always just an amp? 


 I understand somewhat how you're saying since its ac and not dc the heat is determined by the impedance instead of resistance and therefore halving the current will quarter the heat. Ok impedance is like ac resistance but it still leaves me wondering what voltage does in a motor.

As an example:
you could lower your kv by x10..by increasing the motor's turns by x10...and you've now increased the torque the motor can produce 10x per amp. you're still utilizing the amps and volts don't come into the equation.    What's an equation that includes voltage other than w= I x v in a motor?
How does current drop when voltage increases?
```

---
## \#12 Posted by: trbt555 Posted at: 2016-02-29T19:03:20.985Z Reads: 91

```
You should read [this][1] article by B. Vedder, which gives an excellent insight into exactly the questions you're asking. Not an easy read though.


  [1]: http://vedder.se/2014/10/chosing-the-right-bldc-motor-and-battery-setup-for-an-electric-skateboard/
```

---
## \#13 Posted by: Hummie Posted at: 2016-02-29T19:20:22.543Z Reads: 87

```
I've read it before. Don't remember it answering the question but maybe it's in there
```

---

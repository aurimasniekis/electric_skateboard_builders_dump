# Motor draws more current than the battery supplies (free energy?)

### Replies: 12 Views: 847

## \#1 Posted by: solidgeek Posted at: 2017-08-07T23:31:51.105Z Reads: 196

```
I was out for a long ride today, with my VESC 6 and some heavy 97mm wheels. Very nice ride, the VESC 6 surely is amazing. I am using the Metr.at Bluetooth module to log every ride, and today I noticed something weird. According to the data, my motor is always drawing more current than coming from the battery.

https://metr.at/r/Fxoi6

Because of this high motor current I experience one "stop of acceleration" as I reached the max current setting of 50A. I was accelerating uphill, with a single Turnigy Aerodrive SK3 - 6374-192kv. The max current was triggered at 17:33:40.

Is it normal that the motor current is that much higher than the current coming from the battery? As an upcoming electrical engineer this makes no sense to me :smile: 

Any advice would be appreciated :)
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-07T23:38:57.952Z Reads: 184

```
This is normal. From my understanding, while battery amps provide a certain amount of current at a given voltage, the motor is not always running at that voltage. Since the motor voltage relies on duty cycle, more amps are needed to drive the motor.

For example, a 36v battery with 40a battery max can supply 1440w of power. If your running 50% duty cycle (18v), you'll need 1440/18 = 80 amps of current in the motor to match the available power input.

Anyone please feel free to correct me if I'm wrong.
```

---
## \#3 Posted by: solidgeek Posted at: 2017-08-07T23:43:27.329Z Reads: 173

```
Well, that makes perfect sense, thank you! :-) Any idea of how I can avoid max current being reached, without making max current higher, f.x. 60 amps?
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-07T23:45:09.653Z Reads: 168

```
I wasn't clear on what problem you were having in the original post. Was the VESC throwing an error code or something? Perhaps posting your BLDC tool screenshots would be more helpful.
```

---
## \#5 Posted by: solidgeek Posted at: 2017-08-07T23:50:56.919Z Reads: 154

```
I don't think the VESC gave an error code, however, I don't know for sure because I didn't connect it when I came home. I just had a complete decrease in acceleration for a second or so, and after that, I just continued at a slightly lower throttle.

I am using a VESC 6, so the interface is quite different from what many of you are used to :P - and I can't connect it tonight, as I am not home at the moment...
```

---
## \#6 Posted by: jmasta Posted at: 2017-08-07T23:53:00.343Z Reads: 137

```
I believe the difference between Battery Amps and Motor Amps is because of the stored energy in the VESC's capacitors.  Battery Amps are essentially refilling the capacitors, which are like a high discharge reserve that feeds current to the motor
```

---
## \#7 Posted by: Jinra Posted at: 2017-08-07T23:54:46.272Z Reads: 134

```
perhaps voltage sag is triggering battery cutoff. screenshots would help :)
```

---
## \#8 Posted by: solidgeek Posted at: 2017-08-07T23:59:50.425Z Reads: 132

```
Maybe, however according to the data the battery voltage doesn't seems to get that low. Of course it could have missed some data points. I will try giving it a ride tomorrow, same hill and see if I can replicate the error :slight_smile: 

Thanks for the assistance!
```

---
## \#9 Posted by: HTownBomber Posted at: 2017-08-08T00:04:57.274Z Reads: 127

```
No, the caps are only there to smooth out voltage spikes from the rapidly-switching fets, creating inductance in the battery cables.
```

---
## \#10 Posted by: solidgeek Posted at: 2017-08-09T14:31:35.886Z Reads: 112

```
I change my settings, and it works like a charm! Very nice ride today, a total of 18km, no over current failures :)

Motor max: 60A
Motor min: -60A
Battery max: 40A
Battery min: 10A

@Jinra thanks for the explanation, helped me understand my vesc a lot better :)
```

---
## \#11 Posted by: Darkie02 Posted at: 2018-11-15T10:36:26.951Z Reads: 64

```
So how does this work under braking when you brake hard at 60a but batt min is 12a were dose it go. (Has to go some were right)?

Store it in the cap on the Vesc or some thing until there full? If so how much can thay holed until thay brake or just relice the brakes sending you flying?
```

---
## \#12 Posted by: professor_shartsis Posted at: 2018-11-15T13:56:39.559Z Reads: 46

```
depending on the rpm of the motor, that 60a motor current will be different voltages. 60a motor current at 50% of no load rpm will be 60a @ half the battery voltage. if that’s more power than 12a battery current @ battery voltage, then the motor current during breaking will be reduced so that 12a bat current isn’t exceeded. that’s my understanding.
```

---

# Different motor KV&rsquo;s

### Replies: 8 Views: 7893

## \#1 Posted by: Frankenstein Posted at: 2016-05-07T03:45:43.365Z Reads: 392

```
So I've been looking around the forums and I've noticed something.

Maybe I just haven't searched hard enough, but I haven't seen a good thread on why someone HAS to use a motor with less than 300kv with any explanation. It's just "You shouldn't use a motor more than 300kv" with no reason for it. Does anyone have an experience with using a higher rated KV motor with a lower voltage battery and a high gear ratio?

Say, a 600kv motor with a 4s 5000mAh 20C and a 1:3 ratio? 

My theory is the power required to push a rider and the torque needed to get started. The lower the KV the higher the torque, if I'm not mistaken, but how much torque do you really need if you're not dealing with hills?

Hope this creates a good discussion!
```

---
## \#2 Posted by: onloop Posted at: 2016-05-07T04:03:53.598Z Reads: 388

```
it has to do with minimising heat, lower voltage tends to mean higher current draw which means hotter motors, hotter everything....

high current should be avoided, that's why a lot of people are trying to build with higher voltages now....

Of course, when you increase the voltage the motor wants to spin at a higher RPM & there is only so much mechanical reduction that can be achieved.

So you then need to counter this with lower KV motors.

The idea is to build an electric skateboard that is usable for a human passenger....

It needs to climb hills & also it needs to have a top speed that you can actually utilise...

So you tend to find due to design constraints & the voltage we use Motor KV tends to fall between 200-300kv.

Higher voltage tends to mean lower KV....
```

---
## \#3 Posted by: onloop Posted at: 2016-05-07T04:04:24.592Z Reads: 352

```
I wrote an article about this topic.

http://www.electric-skateboard.builders/t/beginners-guide-to-building-your-own-electric-skateboard-drivetrain/53
```

---
## \#4 Posted by: onloop Posted at: 2016-05-07T04:06:50.113Z Reads: 323

```


This info only applies to a satellite configuration, hub motors are a different story.
```

---
## \#5 Posted by: laurnts Posted at: 2016-05-07T11:28:07.141Z Reads: 298

```
Honestly Ive never tried with higher KV but I doubt it will satisfy you. The price is great, the speed is marvelous as it rotates faster, but the torque or the wattage in overal seems to be lower.

Why we stick with this low kv is that the biggest shit eboard has to take is not top speed but torque. It needs to handle just that, very good. Low KV motor tends to have longer cans and that means more torque. You could or would probably seen soon in the future higher kv with longer can to provide more torque but its not here yet and it would not fit dual drive config. At least its going to be very wide out when mounted.

And yes higher voltage means less current draw, less heat, less stress on batteries as well as electronics. Amps is the enemies for electronics, the things that cause problems, such as sparking, blowing up drv, burning wires, etc.

If you also look mechanically, the gear within eboard is already at an ideal diameter. I couldnt imagine if the pulleys needs to be larger to accomodate the gearing for the motor. Its likely that it has larger diameter than the wheels.
```

---
## \#6 Posted by: Hummie Posted at: 2016-05-07T16:42:55.731Z Reads: 267

```
I've heard it both ways, someone on here said something about the motor being an ac curcuits and therefore if the motor runs on higher voltage it produces less heat (there's some formula but forget it that he posted), but I've also heard from people who Defianately know what they're talking about that you get the same heat to torque with a higher kv motor because yes it needs more amps to produce the same torque as a lower kv motor but the windings are fatter and have less resistance and ultimately it balances out.  My money is on this last explanation but would like to know for sure.  
I think also with a higher voltage using ohms equation you end up with more amps for a given resistance allowing you to push more power through the motor
```

---
## \#7 Posted by: Lloydd Posted at: 2016-05-09T18:38:43.303Z Reads: 226

```
interesting theory @hummie. One thing worth noting i think is that sure a higher KV motor that has thicker windings and a lower internal motor resistance which would possibly balance the temp difference at the motor, but on the flip side,  all that amperage is being pushed from your batteries through your conductors and the ESC. 

The esc has amperage ratings and fixed levels of resistance as well (unless there are ESC's that are rated for constant high current) so perhaps any balanced heat levels at the motor (from having less resistance although higher amperage as you mentioned) you would still have the extra heat generated at ESC from higher current flow. Also the conductors between your battery, esc and motor have resistance values that if you apply higher amperage to it will generate more heat. One could then say use a larger gauge wire but then you start adding additional weight and bulk to the board. 

The concept of higher voltage = lower amperage is something that is widely used across the electrical utility industry but when applied to eboard's, as Onloop said theres a limit to the mechanical reduction needed to properly gear the motors and it seems they found a nice balance for the sizing of gears relative to motor rpm/torque ratios.

Sorry if any of that was confusing to read, I'm not always the best at conveying my message lol
```

---
## \#8 Posted by: Hummie Posted at: 2016-05-09T19:06:50.227Z Reads: 209

```
This is an awesome tool

 http://www.bavaria-direct.co.za/constants/#Efficiency

Varying the inputs u can run a low kv and high voltage vs high kv and low voltage scenario.  And add heat!

True the rest of the system will be subjected to higher amps with the high kv but the difference in weight between 10aug or 14 is minor and I think almost all the losses would be in the motor
```

---

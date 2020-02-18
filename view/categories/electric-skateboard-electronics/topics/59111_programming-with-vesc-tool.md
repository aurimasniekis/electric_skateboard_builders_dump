# Programming with VESC-tool

### Replies: 3 Views: 409

## \#1 Posted by: Flor Posted at: 2018-06-16T18:01:51.043Z Reads: 90

```
Hello, everyone I am here (in fact a salesman advised me to come back to my problem).

I'm trying to make an off-road e-scooter (I'll post pictures when the mechanical part is more advanced).

For the electrical part of my vehicle here is what I have in my possession:

- 2 Multistar 20Ah 6S 10C batteries (connected in series therefore 12S)
     (shop link: https://hobbyking.com/en_us/multistar-high-capacity-20000mah-6s-10c-multi-rotor-lipo-pack-w-xt90.html)

- 1 motor Aerodrive SK3 6374 192kv
     (shop link: https://hobbyking.com/en/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html)

- 1 VESC controller enertion FOCBOX
     (shop link: http://www.enertionboards.com/electric-skateboard-parts/FOCBOX-programmable-brushless-motor-controller/)

I tried to realize the program based on the documentation of VESC-Tool but I messed up.

Here are the different values ​​that I had written:
   - Motor Max: 40A
   - Motor Brake Max: -15A
   - Battery Max: 40A
   - Battery Max Regen: -15A

I had chosen the FOC mode, and the test of resistance and inductance (LR test), the motor made a small noise but it looks normal, however the VESC did not appreciate it.

So I stopped everything and I went to find a solution on the "chat" of the vendor of the VESC.

This one was called "faults", there was nothing, so no particular damage on the VESC according to him.

Here are the things he told me:
   - it's a problem of values ​​and setting.
   - Motor Max is too big, 30A is better because the VESC can 60A
   - for a 192kv engine, 12S is not ideal (and it can be dangerous in FOC mode)
   - and finally he advised me to help me correct the values.

That's why I'm here today, I hope to find a solution to my problem.

How to go from 12S to 10S? I heard about BMS for batteries, is it necessary? What are the most sensitive values ​​to start my electrical tests?

Finally, I thank you in advance of the ESK8 and this seller who reassured me a little.

Thanks thanks thanks,
Flor

(Sorry for the communication, I'm french)
```

---
## \#2 Posted by: Pimousse Posted at: 2018-06-17T10:03:13.374Z Reads: 57

```
The seller gave you bad info : 
Motor max is not linked to the battery. So you can put 65A on each, that does make no difference.
Motor min shouid be the opposite of your motor max (e.g -40A if motor max = 40)

Check e-sk8.fr/forum, we have tutorial for VESC configuration in french.
```

---
## \#3 Posted by: Flor Posted at: 2018-06-19T04:15:56.647Z Reads: 45

```
Ok, I'll go for a walk on the French forum, it may be clearer

Thank you
```

---

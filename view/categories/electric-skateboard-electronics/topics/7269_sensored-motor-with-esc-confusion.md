# Sensored Motor with ESC confusion

### Replies: 9 Views: 1303

## \#1 Posted by: MattCarl Posted at: 2016-08-07T18:46:30.336Z Reads: 88

```
So I bought[ this motor](diy-electric-skateboard-kits-parts/electric-skateboard-motor-6355/) from diy electric skateboard and [this esc](https://www.amazon.com/FVT-120A-Brushless-Sensored-Sensorless/dp/B00LWH3YIA) from amazon, both sensorless/sensored compatible. I hooked it up in the sensorless configuration and it worked fine, but I'm confused on how to hook it up in the sensored configuration. 

The instructions for the motor says to make sure the ABC motor wires are hooked up correctly to that on the ESC, but the colors are different and they don't say what is what (yellow, blue, and black on the motor... blue, yellow and orange on the ESC). 

The motor has a ribbon cable that corresponds to a port on the ESC but there is only one way to plug it in. So does the order of the motor phase wires matter in the sensored configuration or can I simply plug in the ribbon cable from the motor to the ESC and it'll function as sensored fine? Thanks in advance!
```

---
## \#2 Posted by: Jinra Posted at: 2016-08-07T18:48:47.219Z Reads: 84

```
Pictures would be very helpful
```

---
## \#3 Posted by: MattCarl Posted at: 2016-08-07T18:51:35.907Z Reads: 84

```
<img src="/uploads/db1493/original/2X/b/b95a5b266bfba3819d65d61701fb642fa569c901.jpeg" width="666" height="500">
<img src="/uploads/db1493/original/2X/c/c64177a56f33cfe5735cc07b09cc25d06fbed957.jpeg" width="666" height="500">
```

---
## \#4 Posted by: Jinra Posted at: 2016-08-07T18:54:06.799Z Reads: 78

```
yep so plug in the sensor wires and for the phase wires you're going to have to try it out in various orders to find which one works best and spins the direction you want. You'll know when its optimal when you dont cog when accelerating. You may have to switch some of the sensor wires.

Check out this flow chart.

https://endless-sphere.com/w/index.php/Determining_the_Wiring_for_a_Brushless_Motor
```

---
## \#5 Posted by: MattCarl Posted at: 2016-08-07T19:02:11.636Z Reads: 74

```
ahh ok so I can switch around the phase wires in the sensored configuration and still be ok? the instructions on the diyelectricskateboard website said:

"If you do not have A, B and C motor wires plugged in properly to the motor when trying to use sensored mode.
The motor will burn and smoke. If you do not connect it properly. We will not be held liable for any damages."

Thus why I was nervous to connect the phase wires in the sensored configuration. the flowchart suggests switching around the sensor wires in the ribbon cable and keeping the phase wires constant. That would mean cutting the ribbon cable and switching around the connections? Should I try switching the phase wires first?
```

---
## \#6 Posted by: Jinra Posted at: 2016-08-07T19:03:34.781Z Reads: 66

```
don't throttle too much. If you're applying a lot of power to the motor and it doesn't want to move this will cause heat and probably burn out your motor and/or ESC. Just throttle momentarily to check if it's spinning right.
```

---
## \#7 Posted by: MattCarl Posted at: 2016-08-07T19:09:49.471Z Reads: 61

```
I tested it in unsensored mode with the phase wires and figured out the right combination of the phase wires to get the correct rotation, so plan of action would be:

Connect phase wires in same combination as unsensored correct rotation
Connect the ribbon cable
turn everything on 
give brief, low throttle, if spinning smoothly and correctly then i'm good, test full throttle.
if not, switch phase wires and retest.
If I switched all the phase wires and still not running smooth then consult flow chart you posted to switch around sensor wires.
```

---
## \#8 Posted by: Jinra Posted at: 2016-08-07T19:11:23.380Z Reads: 59

```
sensored will be pickier on the combination of the phase wires. I don't think unsensored really matters which combo as long as it's spinning in the direction you want.
```

---
## \#9 Posted by: MattCarl Posted at: 2016-08-08T14:51:15.634Z Reads: 44

```
Alright, thank you for the help!
```

---

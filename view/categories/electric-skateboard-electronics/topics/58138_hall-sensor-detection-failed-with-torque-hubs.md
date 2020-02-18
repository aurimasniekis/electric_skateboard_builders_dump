# Hall sensor detection failed with torque HUBS

### Replies: 12 Views: 352

## \#1 Posted by: nordlicht Posted at: 2018-06-07T14:42:26.376Z Reads: 94

```
Hi,
so I've got the torque hub 130KV and a VESC using the BLDC tool.
Before I built the housing I connected the motor to the VESC ran the BLDC tool and could just hit "start detection" and I would have my sensors detected.
Now I built the housing and it doesnt work anymore, it always responses

Hall sensor detection failed:
-1, 2, 4, 4, 1, 1, 5, -1

I measured all 3 cables and have the rectangular signal like I know it. I also checked the connection on the board, all cables have connection.
I'm really confused and dont understand that at all. Do I have to make some settings in VESC before I start the detection? It isnt the battery voltage, max input is set to 53V (12S setup), cutoff start to 45,6 and minimum at 8V.

Anyone has a clue?
```

---
## \#2 Posted by: mmaner Posted at: 2018-06-07T14:45:15.188Z Reads: 90

```
Did you select FOC on the Motor tab and Sensored or Hybrid on the FOC tab?
```

---
## \#3 Posted by: nordlicht Posted at: 2018-06-07T15:33:26.374Z Reads: 79

```
I selected BLDC on as Motor Type and did nothing on the FOC tab.
I selected sensored on BLDC tab.
```

---
## \#4 Posted by: mmaner Posted at: 2018-06-07T15:35:22.328Z Reads: 74

```
Try setting it to FOC on th emotor tab and Sensored or Hybrid on the FOC tab and reattempt the detection.
```

---
## \#5 Posted by: nordlicht Posted at: 2018-06-07T15:39:16.228Z Reads: 69

```
Motor Type was set to FOC. in BLDC tab was the Sensor Mode set to Hybrid and  in FOC tab the Sensor Mode to Hall, still just a failed detection
```

---
## \#6 Posted by: nordlicht Posted at: 2018-06-07T15:42:58.935Z Reads: 66

```
Oh I just realized now you wanted me to measure the Hall Sensors in the FOC tab.
There it just popped a green message "Hall Result Received" and there are now 8 parameters. I dont know tho whether that was succesful or not?![foc_detection|625x500](upload://qn9Mo92lyOXiPSNiAnnREXmPOSV.jpg)
This is how it looks like
```

---
## \#7 Posted by: deucesdown Posted at: 2018-06-07T15:52:34.191Z Reads: 60

```
IIRC bvedder said the hall sensor detection code in BLDC mode is very basic. He put a lot more into hall detection in FOC.
```

---
## \#8 Posted by: efichip Posted at: 2019-09-13T17:18:25.670Z Reads: 24

```
Hello,
I connect the new BLDC motor and sk8 and try to detect the parameters in vesc tool, but detection is failed. Reason: Sensor detection failed. Can anybody help me?![Sensor%20Failed|690x407](upload://6aMGn2Ff2lqqfzjehMPf4JSyOlI.png)
```

---
## \#9 Posted by: mmaner Posted at: 2019-09-13T18:54:34.021Z Reads: 19

```
I've had that problem many times with the newest VESC tool. One reason could be your battery charger level. Sometimes s low battery will cause a failed detection. Also, are you running 83mm wheels?

If it's but the battery it wheels, try another firmware to isolate the issue to the VESC tool or motors. 

https:///how-to-ackmaniac-esc-tool/
```

---
## \#10 Posted by: efichip Posted at: 2019-10-01T16:59:53.488Z Reads: 19

```
Hello mmaner,
I was tried measure the motor resistance and inductance in FOC Settings with your tool, but detection mesure is bad (Could not measure the motor resistance and inductance). I have the Turnigy D5035-125KV Sensored Brushless Motor from hobbyking and 4 Li-ion Panasonic NCR18650B for testing.
(https://hobbyking.com/en_us/dt6376-14p-sensored-motor-125kv.html)
Can you advise please?
```

---
## \#11 Posted by: mmaner Posted at: 2019-10-01T17:39:17.205Z Reads: 16

```
1st, it's not my tool.  It's built and maintained by @Ackmaniac, I just wrote a how-to (tutorial) about it. 

2nd, I've never used those motors so Im not sure how I can help. Are you getting a successful BLDC detection?  Post some screen shots of the ESC-Tool, that will help a lot.
```

---
## \#12 Posted by: Sn4pz Posted at: 2019-10-01T18:02:42.112Z Reads: 15

```
For what it's worth, you should probably just return those motors and get the 70kv version. I also had issues with these hubs, same sensor issue you had, as well as efficiency so poor you could actually only scrape 10 miles out of a 10s4p 25r pack. Additionally, when at a standstill, pulling with more than ~30% throttle would make the hubs chatter endlessly

On the other hand.... They are A LOT of fun. The unwieldiness makes it interesting lol. I hit my top speed of 40mph with those, but I cant recommend it :stuck_out_tongue_closed_eyes:
```

---

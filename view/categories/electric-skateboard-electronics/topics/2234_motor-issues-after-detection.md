# Motor issues after detection

### Replies: 6 Views: 1683

## \#1 Posted by: arpitdave Posted at: 2016-04-08T22:24:58.252Z Reads: 83

```
So i did the motor detection and followed the directions according to Marcin Sleziak's video instruction. However, after selecting current no reverse with brake and writing configuration the motor is not rotating. I have a FS-GT2 and when i press the throttle i do see a green light on the VESC. I have already uploaded the firmware for my VESC 4.10 already. help?
```

---
## \#2 Posted by: treenutter Posted at: 2016-04-09T03:12:55.101Z Reads: 76

```
@arpitdave After you write the config you need to reboot VESC. You also need to pair you gt2b with the receiver. Have you tried both of these steps?

Oh wait - you're seeing a green light so you are paired and presumably rebooted. In that case, I'd guess that you haven't selected a motor control option. Select BLDC from the motor tab, write config, reboot.
```

---
## \#3 Posted by: arpitdave Posted at: 2016-04-09T04:27:14.892Z Reads: 76

```
hmm i did that but still no motor response. When i do the start detection on that same page I get a bad detection result received error. Any other ideas?
```

---
## \#4 Posted by: treenutter Posted at: 2016-04-10T01:13:40.980Z Reads: 63

```
@arpitdave "The bad detection result received" error might be a very important clue. Does your motor spin up during detection? Can you control it through BLDC Tool using the keyboard? Perhaps there's a wiring issue between your motor and VESC.Double-check the wiring to make sure everything is right, posting a pic here would help all of us to review your setup and give you advice :) Screenshots of your BLDC Tool Configurations would be helpful a well.
```

---
## \#5 Posted by: arpitdave Posted at: 2016-04-10T15:33:37.271Z Reads: 55

```
The motor does not spin up during detection. Is it supposed to? I am going to re-solder the motor connections to the VESC and attach a picture soon.
```

---
## \#6 Posted by: treenutter Posted at: 2016-04-10T18:45:08.052Z Reads: 50

```
@arpitdave Yes, it is supposed to spin up during motor detection. If it doesn't, something is wrong. There are several tutorials to check out. @onloop [made this one about motor detection](http://www.electric-skateboard.builders/t/vesc-faq-motor-detection-step-by-step-guide/500) I'm suspecting that your wiring needs some correction. GL!
```

---

# Switching between acceleration and reverse

### Replies: 3 Views: 589

## \#1 Posted by: ayospringroll Posted at: 2016-12-06T22:42:05.703Z Reads: 63

```
I was wondering if there is a way to switch between accelerating and reversing within the bldc tool? Im currently using a GT-2b mod and there are some switched not being used so I was wondering if I could use a switch on the controller to switch between accel and reverse.

I know there is reverse option in the bldc but I want to be able to hold the break at a stop and in the rare case that I need to reverse I could flip the switch and have a reverse option.
```

---
## \#2 Posted by: Ackmaniac Posted at: 2016-12-06T23:17:45.421Z Reads: 49

```
Would be doable. But some safety regulations need to be implemented so that it doesn't switch by accident while you are driving. Easiest way would be via Nunchuk. But it also would be doable for dual boards and maybe even for singles where the UART channel would be used for that.The rest needs to be done in the firmware.
Many different ways, but this feature doesn't really sound to be attractive enough that it would be worth all the time.
```

---
## \#3 Posted by: ayospringroll Posted at: 2016-12-06T23:22:46.163Z Reads: 43

```
I see where youre coming from with this not being safe and useful :sweat_smile: I just noticed that the Evolve GT has a reverse option on the controller so I thought it would be cool to try and implement it onto my build. 

Thank you for your feedback!
```

---

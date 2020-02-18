# DYI Electric scooter build need help!

### Replies: 5 Views: 175

## \#1 Posted by: bperez3 Posted at: 2019-09-27T17:04:43.682Z Reads: 59

```
Let me start with giving you guys some back ground on my build, It's a old school Goped ESR750, I removed the old brushed motor, controller and SLA batterys and I installed a single 6380 170 kv motor from Torque boards, focbox vesc and a 10s10p liion battery. I made it belt driven  and its running a 16 tooth on the motor and a 80 tooth on the wheel. The wheels are 10 inch and I'm using a ebike throttle to control the vesc. So my build as a few issues, let me start by saying I keep failing motor detection when I try it in bldc mode. So I run my build on foc mode, idk if the reason I can't use the bldc mode is because I'm trying to use a foc box with the new Vesc tool  instead of the bldc tool? any ideas? The second issue I realized I'm losing power after riding for like 10 mins, I think the vesc might be reaching the temp limit. Idk if this is happening because of the gear ratio, my weight (250 pounds) or because the vesc is in a enclosure. I'm only running 25 battery amps and 60 motor amps.I'm only reaching like 22 mph for a few mins before it slows down to 15 mph. My thoughts were to find a way to run bldc mode and lower my battery amps. What do you guys think?
```

---
## \#2 Posted by: Gamer43 Posted at: 2019-09-27T18:53:31.577Z Reads: 51

```
A few things

BLDC detection fails because of certain detection settings, you need to set the duty cycle higher. A decent ESC shouldn't need to do bldc detection but I digress. 

It's overheating because FOCBOXes use that garbage known as directFET which get super hot on FOC. 

You'll want to keep using FOC, I'd recommend getting a different ESC such as a sinusoidal Kelly controller.
```

---
## \#3 Posted by: bperez3 Posted at: 2019-09-27T20:26:31.506Z Reads: 48

```
Thank you , so I do want to use bldc mode instead of foc mode. What settings would you recommend ?
```

---
## \#4 Posted by: Gamer43 Posted at: 2019-09-27T20:41:41.627Z Reads: 46

```
Try these settings when running detection
![image|232x137](upload://qqxGVLHXwwSHHZUX0o4RJYubq9a.png)

Also, BLDC will run a lot cooler for the ESC than FOC, but the motor may get hotter.
```

---
## \#5 Posted by: bperez3 Posted at: 2020-01-30T14:29:38.844Z Reads: 11

```
Thank you by the way it worked
```

---

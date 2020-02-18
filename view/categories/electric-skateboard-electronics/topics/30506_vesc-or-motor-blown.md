# Vesc or motor blown?

### Replies: 5 Views: 565

## \#1 Posted by: jourm Posted at: 2017-08-13T18:14:12.386Z Reads: 86

```
Hello, new user here. I finished my first build(12 s lipo, 4.12 Vesc running on foc, single turnigy sk 6374 168 kv motor, alien power systems motormount and drive system, Nyko kama) and it worked really well for about a week. But then, suddenly it just stopped working, and now i dont know wether the problem is with my vesc or motor. The vesc get power and leds light up, blue always and yellow when i hit the accelerator, but the motor does not respond at all. When i plugged it into bldc tool there are no fault codes and nothing seems to be wrong. I would be really happy for any thoughts or ideas about what might be wrong or what i can do to fix it.
```

---
## \#2 Posted by: Jinra Posted at: 2017-08-13T18:15:22.994Z Reads: 82

```
Keep in mind fault codes disappear when you turn the VESC off and back on. Make sure you check BLDC tool for faults as you're getting the lights.
```

---
## \#3 Posted by: jourm Posted at: 2017-08-13T18:45:10.086Z Reads: 72

```
Thanks, connected it again and gave it some power with the arrow keys in bldc tool, looking at the graphs current is really low, but erpm goes up, but still no fault codes <img src="/uploads/db1493/original/3X/2/4/24c5d9bc33f92724c6c8e10649a173b50adc6b00.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/2/f/2fd178fcc6c678afabf2cfbf00f8ddc896f7d28c.jpg" width="690" height="388">
```

---
## \#4 Posted by: Jinra Posted at: 2017-08-13T18:46:54.449Z Reads: 68

```
If you have PPM mode enabled the arrow keys won't respond, you gotta use your controller. Also you can check fault history (in the same session) by going to terminal and typing "faults" in case there's no fault codes at that immediate time.
```

---
## \#5 Posted by: jourm Posted at: 2017-08-15T15:06:17.362Z Reads: 32

```
Thank you for your help. I'm still not seeing anything wrong with my vesc, so I'm beginning to suspect that the motor might be shorted out or something
```

---

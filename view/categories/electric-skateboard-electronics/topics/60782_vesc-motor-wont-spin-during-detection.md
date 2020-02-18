# VESC Motor Won&rsquo;t Spin During Detection

### Replies: 15 Views: 609

## \#1 Posted by: gigoy Posted at: 2018-07-03T08:46:57.932Z Reads: 100

```
I have a HK Sk8. I was running it in FOC and it was working fine. Changed deck, trucks and mounts, setup again on ackmaniac tool but this time I wanted to use BLDC because I felt it had better braking "umph" than when in FOC. 

Started detection - at first it's acting crazy it's making some whiny sounds and tries to spin. Bad detection results. Checked wires and physical connection, same results. Unplugged power, rebooted VESC then *poof*, smoke. Disconnected everything.

Plugged it back in, and everything seems to be working, except it doesn't detect motor. Bad detection results. 

Here's a GIF (EDIT: there's a long pause after hitting the Play/Detection button):

[[img]https://i.imgur.com/x4n22u7.gif[/img]]([img]https://i.imgur.com/x4n22u7.gif[/img])

It doesn't show any results and checking RT data, those are the things that show up. It doesn't show any type of fault. On the VESC itself though, I've noticed I've not seen the red light show up even once when it used to before when it was still working.

I thought it could be the motor (Sk8 6374 192kv), used a different ESC all with the same settings and everything works in FOC and BLDC and no problem in detection.

Any ideas on how to get this fixed? Or is it even still repairable?
```

---
## \#2 Posted by: Ishayc Posted at: 2018-07-03T09:52:11.865Z Reads: 87

```
Re-upload the GIF. It's dead.
```

---
## \#3 Posted by: gigoy Posted at: 2018-07-03T10:05:15.816Z Reads: 87

```
Re-upped. Thanks for the heads up
```

---
## \#4 Posted by: gigoy Posted at: 2018-07-03T17:42:45.487Z Reads: 77

```
Still stuck
```

---
## \#5 Posted by: Holyman92 Posted at: 2018-07-03T17:56:35.626Z Reads: 77

```
Isn't detection only for foc and hybrid mode tho... 

I thought the problem with bldc was that it didnt have detection which is why u have to kick for initial take off
```

---
## \#6 Posted by: Jc06505n Posted at: 2018-07-03T18:20:27.174Z Reads: 76

```
No, your confusing Sensors / Sensor-less and BLDC / FOC
```

---
## \#7 Posted by: GrecoMan Posted at: 2018-07-03T18:25:57.179Z Reads: 77

```
wait wait wait whhhaaaatttt??
```

---
## \#8 Posted by: Benjamin899 Posted at: 2018-07-03T18:37:24.346Z Reads: 76

```
sensors just tell the position of the motor, hence being able to start with sensors from standstill and a higher efficiency since the vesc can better time the intervall to accllerate and waste less energy. Also it gets quiter.
```

---
## \#9 Posted by: gigoy Posted at: 2018-07-03T20:06:11.298Z Reads: 68

```
Thanks for the clarification. Any idea though what's happening with the ESC?
```

---
## \#10 Posted by: Benjamin899 Posted at: 2018-07-03T23:56:56.904Z Reads: 65

```
where did the smoke come from? vesc?
```

---
## \#11 Posted by: gigoy Posted at: 2018-07-04T01:28:26.834Z Reads: 65

```
Yeah from the VESC
```

---
## \#12 Posted by: barajabali Posted at: 2018-07-04T02:18:05.293Z Reads: 62

```
@guyguy seems like your situation. Blown fet likely culprit
```

---
## \#13 Posted by: gigoy Posted at: 2018-07-04T05:29:32.362Z Reads: 49

```
Finally took shrink wrap off.

![20180704_172542|690x388](upload://5GMZVN5k2OVkrVdXSRkHdWRx9fx.jpg)

![20180704_172226|281x500](upload://4ryfMcIhoOinTi7acKDg5l6vyrY.jpg)

EDIT: added more pictures

![20180704_174026|690x388](upload://kNdQIOSFg6EQ92Z1hfjhO95oq6P.jpg)

![20180704_174133|281x500](upload://vNT385qc0xBW9qLXlgZjYIidJBL.jpg)

![20180704_174221|281x500](upload://nZpciERQW6jPoCrLuXlRhMGi4vc.jpg)

I'm no expert but it looks like that drv8302 got BBQed. Is it something I can fix. Any links of videos or instructions on how to do it?
```

---
## \#14 Posted by: Benjamin899 Posted at: 2018-07-04T10:55:14.242Z Reads: 41

```
you can replace it, but it is not an easy task. just search here and on youtube
```

---
## \#15 Posted by: gigoy Posted at: 2018-07-04T12:09:40.342Z Reads: 40

```
Can't seem to find them in stock
```

---

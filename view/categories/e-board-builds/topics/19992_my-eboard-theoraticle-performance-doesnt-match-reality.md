# My eboard theoraticle performance doesn&rsquo;t match reality!

### Replies: 14 Views: 922

## \#1 Posted by: Tal Posted at: 2017-03-30T09:11:16.793Z Reads: 176

```
Motor: sk3 213kv 6364
Esc: vesc
Battery: 10s4p
I can't reach 25 km/h , can't climb hills...
On paper those specs should have taken me 25 km/h uphill... 
IDK what the problem is... Any suggestions?
```

---
## \#2 Posted by: monkey32 Posted at: 2017-03-30T09:13:41.799Z Reads: 176

```
More info please;
Settings
Pulley ratio
Load on board
Hill grade 
Favorite burger toppings.......:wink:
```

---
## \#3 Posted by: Tal Posted at: 2017-03-30T09:20:02.254Z Reads: 173

```
I weight 90 kg, board weights 7 kg and the vesc restricts amp output to 47.. I have ridden a different board with the same specs up 25% hill grade at 20 km/h and didn't push the throttle to its limit
```

---
## \#4 Posted by: Tal Posted at: 2017-03-30T09:23:37.810Z Reads: 170

```
I don't remember the gear ratio and right now the board isn't near me but I'm sure its not the issue because the other board has the same ratio... I think it might be the vesc but don't know what exactly
```

---
## \#5 Posted by: Ackmaniac Posted at: 2017-03-30T09:25:02.310Z Reads: 164

```
Just post Screenshots of your VESC settings.
```

---
## \#6 Posted by: laurnts Posted at: 2017-03-30T10:38:17.159Z Reads: 157

```
[quote="Tal, post:1, topic:19992"]
Motor: sk3 213kv 6364Esc: vescBattery: 10s4p
[/quote]

This is impossible, it must be wrong configuration / incompatible VESC hw fw.
I had those incompatibility once, there is almost no power out put at all, especially on FOC mode.
```

---
## \#7 Posted by: Northlake Posted at: 2017-03-30T17:31:23.903Z Reads: 129

```
Definitely the VESC settings go into the BLDC and change them using a tutorial video.
```

---
## \#8 Posted by: Tal Posted at: 2017-04-11T13:45:48.102Z Reads: 93

```
<img src="/uploads/db1493/original/3X/7/3/73ff0e5fc955d7a0110f53d0f2d79bd53e58d0ed.jpg" width="666" height="500">
@monkey32 @laurnts @Northlake
```

---
## \#9 Posted by: laurnts Posted at: 2017-04-11T14:24:45.613Z Reads: 89

```
Also provide photo of your VESC, battery, board, bms, etc. Because the VESC settings seems to be ok.
```

---
## \#10 Posted by: Ackmaniac Posted at: 2017-04-11T15:03:34.337Z Reads: 80

```
Just make some changes:
Absolute max to 130A
Minimum Input Volatge to 8V
Maximum input voltage to 57V
Battery cutoff start to 30V
Battery cutoff end to 28V

And then please also post the other settings.
What is your gearing (Motor pulley teeth/ wheel pulley teeth)
Is the Battery charged. Does the battery voltage fit with the VESCs shown voltage in the realtime tab.
```

---
## \#11 Posted by: laurnts Posted at: 2017-04-11T15:34:19.423Z Reads: 72

```
My biggest fear is that if its using lipo, the lipo have been drained before (totally empty) to under 3.6v. So it practically can't be used anymore.
```

---
## \#12 Posted by: Tal Posted at: 2017-04-11T15:51:10.937Z Reads: 71

```
Battery : 36V 10AH samsung 25R
Battery is charged .

@Ackmaniac  which settings to post?
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-04-11T16:08:27.534Z Reads: 70

```
Bldc, advanced and PPM tab.
```

---
## \#14 Posted by: Tal Posted at: 2017-04-13T11:47:49.625Z Reads: 41

```
I solved the problem. thanks ! Turns out to be a settings problem like you said
```

---

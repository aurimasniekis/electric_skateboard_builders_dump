# Why does my motor cut out for a split sec

### Replies: 20 Views: 2244

## \#1 Posted by: tylerswan11 Posted at: 2016-06-01T04:54:18.201Z Reads: 176

```
I dont know if this is the right spot to post but i was wondering if anyone could help me out. I made my own electric longboard using 

2 6s 1550mAH 60-130c batterys wired in series 
12s esc from diy electric longboards 
turnigy 192kv motor with a max amps of 80

I currently have the max forward force limited to %40 and when i go max throttle (so %40) the motor cuts out for a split sec. Is this because im sending more than 80amps to the motor so it cuts out? and if so what can i do to stop this (it can be really scary when going 17mph.

Thanks
```

---
## \#2 Posted by: tylerswan11 Posted at: 2016-06-01T04:55:54.435Z Reads: 175

```
i was going to get a watt meter to test it out but dont want to get it if thats not the issue.
```

---
## \#3 Posted by: Namasaki Posted at: 2016-06-01T05:30:31.598Z Reads: 164

```
I don't think your problem is because of overloading the motor. It sounds more like you have a loose wire somewhere or your remote is loosing connection with the receiver. check all your connection. motor to esc, esc to battery, esc to receiver.
I had the same problem one time with a brand new motor. When I pulled on the connections, one of them came right off the wire. Bingo! bad solder joint.
If all your connections are good then it could be your remote. some are not dependable. 2.4 ghz rc remotes seem to be the best.
Bluetooth and wii remotes are prone to spotty connection or so I've heard.
I use an RC 2.4 ghz remote it has dropped signal on occasion but it connects instantly so just flipping its switch off and back on reconnects it back now. it never disconnected while I was under power though. only when I was coasting for a long time like going down long hills.
```

---
## \#4 Posted by: Iceni Posted at: 2016-06-01T05:33:08.793Z Reads: 150

```
It could be voltage sag from the batteries tripping the low voltage cutoff in the ESC
With 1500 mah you don't have much headroom for spikes of current draw.

Something to note with the C values is they are, in practice, generally around half of what they print on the label, if even that much.
```

---
## \#5 Posted by: tylerswan11 Posted at: 2016-06-01T16:50:17.374Z Reads: 117

```
I was thinking it was a connection issue to but it happens consistantly at 35%-40% power
```

---
## \#6 Posted by: tylerswan11 Posted at: 2016-06-01T16:55:50.582Z Reads: 114

```
and if i understand everything correctly i have, at full charge 50volts (aka over the max voltage for the motor) but the motor is built for 10s to 12s. So this should be fine correct? but relating to what Iceni said, with 12s worth of batterys i should have a maximum of atleast 38 volts at all times. and this happens when im at 38 or 50 volts so voltage sag couldnt be the problem either, right?
```

---
## \#7 Posted by: tylerswan11 Posted at: 2016-06-01T17:18:07.741Z Reads: 108

```
also it still cuts out at same power % even when im not riding it.( just propping it up and letting wheel spin) and maybe its just coincidence but %40 of my max amps (130c*1550mAH) is 80 and thats the max amps the motor can handle
```

---
## \#8 Posted by: evoheyax Posted at: 2016-06-01T17:20:02.902Z Reads: 107

```
Then its your batteries. 1500 mah is very little. Voltage sag I've found can be quite high. On my space cell for example, I sometimes experience a sag of 25%. since its 7500 mah, thats around 1800 mah of sag, more than your batteries.

I'm working on a massive 16000 mah 12s battery board right now. Even with this, I'm only expecting around 20 miles of range.

I would get bigger batteries if I were you. Those guys are just way to small. Your likely hitting the low voltage cutoff of the esc under load. This happens very quickly due to your extremely small battery size. 8000 mah+ should be the min on any board IMO. You don't really have all of those mah to spare, due to voltage sage. It's hard to use the last bit of juice in your battery, and its dangerous, as it only takes one cell out of balance when your battery is running low to ruin the battery pack. That happened to my 12s 8000 mah battery pack (2x 8000 mah 6s).
```

---
## \#9 Posted by: tylerswan11 Posted at: 2016-06-01T17:24:13.253Z Reads: 97

```
Thanks you!!
```

---
## \#10 Posted by: g4tv4life Posted at: 2016-06-01T17:26:34.103Z Reads: 97

```
you could try rewiring the 2 batteries in parrell instead of series for a quick test. The board will just lose some top speed, but it will let you quickly and cheaply test if voltage sag is the problem.
```

---
## \#11 Posted by: Namasaki Posted at: 2016-06-01T17:42:00.805Z Reads: 93

```
If your batteries are 60c then they are capable of 93 amps continuous. 
If you put your batteries in parallel instead of series, you will defeat the purpose because you will draw twice the current from your battery at 6s than you will at 12s.
You said that your motor cuts out only for a split second. 
So if it just hesitates momentarily, you could be snapping to full throttle too suddenly. 
What other Esc settings are you using?
If you using the low voltage cutoff on that Esc, try setting it to off and see if it still cuts out. 
Note that the low voltage protection on that Esc is known to be inaccurate. So you can't trust it to protect your batteries. And it could be tripping pre-maturely.
Better to leave it off and use a low voltage alarm on each battery.
```

---
## \#12 Posted by: tylerswan11 Posted at: 2016-06-02T00:19:07.859Z Reads: 82

```
ok ill try that. Thanks!!
```

---
## \#13 Posted by: tylerswan11 Posted at: 2016-06-02T00:28:47.580Z Reads: 79

```
ill tell u my settings when i try changing the cutoff
```

---
## \#14 Posted by: Namasaki Posted at: 2016-06-02T01:15:42.951Z Reads: 78

```
Also, try turning your fwd pwr to 100%.
I just did some bench testing with mine at 40% fwd pwr with a clamp voltage/current meter on the 3phase side of the motor. and at full throttle I read the same voltage and current as when it was at 100%.
Seems there was just less torque when I squeezed the wheel it just felt weaker at 40%
```

---
## \#15 Posted by: tylerswan11 Posted at: 2016-06-04T03:30:00.924Z Reads: 69

```
nutral range 3%
 motor timing very high 
acelweation low
running mode for/break 
break force %70 
drag break %0 
cut off (was 3.4) now nothing
max forward force %100 
max reverse force 20% 
motor rotation normal
and at %100 aceleration it hasnt cut out yet and i feel like ive passed the %40 mark. So i think we are good now. Thanks
```

---
## \#16 Posted by: Namasaki Posted at: 2016-06-04T03:51:43.827Z Reads: 65

```
I'll bet it was the low voltage cut off.
```

---
## \#17 Posted by: tylerswan11 Posted at: 2016-06-04T03:53:57.100Z Reads: 65

```
i actually just turned that off. firstly i change the max power. but i also could have just had a stretch of time i got lucky and it didnt happen
```

---
## \#18 Posted by: Namasaki Posted at: 2016-06-04T13:07:40.581Z Reads: 62

```
I read somewhere that the low voltage control is not accurate unless you start with a fully charged battery because it calculates the number of cells by total voltage.  The voltage range with Lipos is too wide. 
I just don't trust that feature.
```

---
## \#19 Posted by: DeathCookies Posted at: 2016-06-06T08:53:05.586Z Reads: 53

```
[quote="Namasaki, post:18, topic:4092"]
because it calculates the number of cells by total voltage
[/quote]

That was my problem. One time i had one cell at about 3V and everything else at 3.7V... That was not that nice...
```

---
## \#20 Posted by: Namasaki Posted at: 2016-06-06T11:52:36.604Z Reads: 48

```
That's  a good example of why we can't trust it. 
Better to have a low voltage alarm plugged into the balance wires monitoring every cell individually.
```

---

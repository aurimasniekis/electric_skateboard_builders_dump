# FocBox and sensored motors trouble

### Replies: 5 Views: 916

## \#1 Posted by: Fetteperson Posted at: 2017-09-12T19:19:25.067Z Reads: 167

```
Hello everyone,

Since I wasn't all to happy about the VESC, I got myself Focboxes. I connected it all the same way as I did with the Vesc. unfortunatelly, when I am doing motor detection, the hallsensor test always fails. Then I read, that I don't need to connect the temperature plug. Does it mean, I have to remove it? The order of all the other cable is the same as on the VESC? I also asked enertion... they told me to lower the minimum voltage to 32.5, 29.5 V. Since I am not at home, I couldn't test that yet, but for me it seams a little weird. (I'm using 12S)
And this happens to all the Focboxes and motors.

Anyone had the same problem?
```

---
## \#2 Posted by: Blasto Posted at: 2017-09-12T19:27:28.663Z Reads: 171

```
[quote="Fetteperson, post:1, topic:32990"]
minimum voltage to 32.5, 29.5 (I'm using 12S)
[/quote]

they may have misunderstood, those voltages are for 10S

It is the same pinout as other vesc, however there was an error in the label

http://www.electric-skateboard.builders/t/mislabeled-focbox/30840
```

---
## \#3 Posted by: E1Allen Posted at: 2018-02-08T20:33:08.173Z Reads: 105

```
So I thought I would continue to use a current post about FocBox and hall sensor issues.  Yesterday I took my board out to a hill to do some testing.  I went up the hill just fine with no issues which was around .7 miles and fairly steep but temps on focbox never went over 70.  Once I got to the top I got off the board turned around and started to go down the hill and I started to brake maybe 10 feet after coasting and the left wheel just locked up while applying brake.  it continued to do this at low speed. but when I coasted a little faster and braked it didn't do anything and only the right motor was applying braking force.  Also the working motor was appearing to work fine however it felt slow as in slow acceleration and braking.  Fast forward to at home on the bench, the motor that quit working was on hybrid setting however the Hall sensor detection failed when I tried to run it.  So it operates fine in sensorless mode.  So I'm not sure if a wire came loose or I had a component failure either in the motor or Focbox.  The other motor, the one that felt weak when I looked in BLDC tool had somehow went to default settings on the motor config, so it was just limited to 25 motor amps on a single motor so it was slow.  Why did it reset?   I'll post metr of the ride up and the ride down where I ended up with overcurrent faults.  Which probably had to do with the hall failure somewhere and the motor just coming to a halt.  

uphill

https://metr.at/r/NhZDK

downhill

https://metr.at/r/5no6E

Any advice or help appreciated.
```

---
## \#5 Posted by: ShutterShock Posted at: 2018-02-09T00:31:20.972Z Reads: 82

```
So I'm kinda in this same situation. I can never get the bldc motor detection to go through on my focboxes, idk why. I haven't looked it up yet because I switched to foc, and all detections worked perfectly fine.

Been running in foc for like two weeks without really any issue, so I'm not sure if I would try to switch back to bldc but it would be good to have that as a backup or another option.

Keep in mind I'm referring to hybrid bldc and sensored foc
```

---
## \#6 Posted by: E1Allen Posted at: 2018-02-09T01:28:36.615Z Reads: 74

```
So you're running unsensored FOC? I'm just frustrated one quit and the other reverted to stock settings. As in why did that happen.
```

---

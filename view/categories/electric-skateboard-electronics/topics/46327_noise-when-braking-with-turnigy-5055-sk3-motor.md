# Noise when braking with turnigy 5055 SK3 motor

### Replies: 11 Views: 538

## \#1 Posted by: HCWH97 Posted at: 2018-02-13T22:35:25.761Z Reads: 79

```
Hi 
When I brake with my SK3 motor with a 150A Trackstar gen2 ESC my motor makes a high pitch noise... Do any of you know how to fix it, and what is causing it?
```

---
## \#2 Posted by: GrecoMan Posted at: 2018-02-13T22:50:15.126Z Reads: 76

```
design and manufacture a new motor
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-02-13T22:55:17.712Z Reads: 70

```
ESCs designed for applications other than esk8 are not optimized for the task they're being used for in esk8. This can lead to issues like noisy or unreliable braking.
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-02-13T22:56:13.621Z Reads: 66

```
Are you sure the sound is coming from the motor and not the ESC? Its normal for car and other RC ESC’s to make a got damm annoying sound when braking..
```

---
## \#5 Posted by: Rinzler Posted at: 2018-02-13T22:57:21.754Z Reads: 60

```
That is normal sound considering you use a car esc. It kinda sounds like a train horn, the only fix that fixes the issue would be getting a vesc or a different kind of esc which commutates the motor at a higher frequency which we dont hear, around 30000kHz
```

---
## \#6 Posted by: HCWH97 Posted at: 2018-02-13T22:58:20.001Z Reads: 55

```
It sound like it is coming from the motor, but i am not sure
```

---
## \#7 Posted by: HCWH97 Posted at: 2018-02-13T22:59:17.992Z Reads: 53

```
Thanks, that was helpfull - what u guys recommend for a cheap VESC?
```

---
## \#8 Posted by: HCWH97 Posted at: 2018-02-13T23:00:07.133Z Reads: 51

```
Thanks for the answer :) - what would you then recommend for a cheap VESC?
```

---
## \#9 Posted by: Rinzler Posted at: 2018-02-13T23:16:16.462Z Reads: 46

```
@HCWH97 You should do a bit of reading on the forum about the VESC. So there are three variants of the VESC: 4.12, FOCBOX(VESCX) and the VESC 6.4. The shittiest is the VESC 4.12- there are plenty of vendors around and these are mainly china produced, have limited watt output on 6s, and tend to be the least reliable and some cant even run FOC, also they tend to let the magic smoke out close to 60,000eprm. The FOCBOX is great, it solves the issues of the 4.12 with bigger watt output(heatsink) and new mosfets that raise the 60,000erpm limit, they also run foc reliably. The 6.4 is the VESC 6, the best and last iteration of the VESC which eliminates the erpm worry, and is also more reliable in FOC, best watt output but they are quite pricey.
```

---
## \#10 Posted by: Ishayc Posted at: 2018-02-14T06:06:19.548Z Reads: 34

```
Had the Trackstar gen II before. The noise from the motor, lack of brakes and acceleration curve drove me crazy. 
Switched to vesc and no regrets.
```

---
## \#11 Posted by: Namasaki Posted at: 2018-02-15T00:19:16.325Z Reads: 22

```
[quote="HCWH97, post:6, topic:46327, full:true"]
It sound like it is coming from the motor, but i am not sure
[/quote]

The noise might be coming from the motor but the ESC is causing it.

Switch to a Vesc and your only question will be, "why didn't I do this in the first place?"

Also, It would be well worth it to save and get a good Vesc like the Focbox and not the cheapest you can find.
```

---

# About the live data from the VESC via UART

### Replies: 7 Views: 1326

## \#1 Posted by: nordlicht Posted at: 2018-04-10T10:59:32.611Z Reads: 148

```
Hi,

I'm readin the live data of the VESC with an Arduino Mega via the UART channel. Got it working just fine.
Yet I have trouble understanding some of the Information I get :smile: I hope you can help to clarify.

Those are the values:

* avgMotorCurrent
Ok this one is pretty clear. The average current of all 3 motor phass

 * avgInputCurrent
This would be the current drawn from the battery
* dutyCycleNow
I control the VESC with PPM, so this would be the uptime of my signal in ms I guess?
* rpm
rounds per minute. SHOULD be clear, yet it shows a value of 45000 when running idle (without load, just in air). That would be 750 rounds PER SECOND. I just cant believe that. Do you have information on that data?
* inpVoltage
The battery voltage. No question here.
* ampHours
So those are the ampHours CURRENTLY DRAWN? or the remaining?
* ampHoursCharged
Are those the AmpHourse charged due to recuperation?
* tachometer
So whats that? The speed? Speed could be easily calculated from rolldiameter (using HUBS here) and a gear ratio of 1:1, but I cant find an option to tell in BLDC tool which rolldiameter I'm using
* tachometerAbs
And those would be the whole distance travelled than?

Cheers, thanks for your time,
Nordlicht
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-04-10T11:49:35.905Z Reads: 132

```
[quote="nordlicht, post:1, topic:51798"]
avgInputCurrent

This would be the current drawn from the battery
[/quote]
it's not that easy, at least the value doesn't seem to represent the actual amp draw for my board. I don't know about this though, didn't research it further yet.

[quote="nordlicht, post:1, topic:51798"]
dutyCycleNow

I control the VESC with PPM, so this would be the uptime of my signal in ms I guess?
[/quote]

I can't confirm but i think it's the duty cycle of the motor output and not the RC Input.

[quote="nordlicht, post:1, topic:51798"]
rounds per minute. SHOULD be clear, yet it shows a value of 45000 when running idle (without load, just in air). That would be 750 rounds PER SECOND. I just cant believe that. Do you have information on that data?
[/quote]
It's rpm times pole count, so you have to divide this value by 7 (i think) for most motors since they have 14 poles.

[quote="nordlicht, post:1, topic:51798"]
So those are the ampHours CURRENTLY DRAWN? or the remaining?
[/quote]
The drawn amp hours since booting, the VESC doesn't know how much amp hours are left in your battery.

[quote="nordlicht, post:1, topic:51798"]
Are those the AmpHourse charged due to recuperation?
[/quote]
exactly.

[quote="nordlicht, post:1, topic:51798"]
So whats that? The speed? Speed could be easily calculated from rolldiameter (using HUBS here) and a gear ratio of 1:1, but I cant find an option to tell in BLDC tool which rolldiameter I’m using
[/quote]
That's not the speed. Each rotation your motor completes this value should go up by one, but since you're having multiple poles in you motor you have to take your pole counts and multiply them by 3. with 14 poles this would be 42, that means 42 pulses of the tachometer equal one motor rotation.
This value goes up and down depending on which direction the motor is turning.

[quote="nordlicht, post:1, topic:51798"]
tachometerAbs

And those would be the whole distance travelled than?
[/quote]
it's the same as the regular tachometer, but it just gets bigger regardless of motor direction.
```

---
## \#3 Posted by: nordlicht Posted at: 2018-04-11T08:40:19.298Z Reads: 92

```
Well, that is one hell of a reply! Thank you. Once the board is on the streets, I'll check those values back and give feedback.
```

---
## \#4 Posted by: spork Posted at: 2018-04-24T07:34:08.078Z Reads: 82

```
This is a super useful thread.  Thanks!

But one (dumb) question...

"It’s rpm times pole count, so you have to divide this value by 7 (i think) for most motors since they have 14 poles."

If it's rpm times pole count, and you have 14 poles, would you want to divide by 14?
```

---
## \#5 Posted by: nordlicht Posted at: 2018-04-24T13:08:38.848Z Reads: 72

```
Yes. You want to devide by 14. My HUB maxes out without load at around 54km/h which seems really plausible for 24V.
```

---
## \#6 Posted by: spork Posted at: 2018-04-26T06:10:11.034Z Reads: 63

```
Now I'm wondering if maybe 7 is right after all.  From wikipedia...

"The number of magnet poles divided by 2 gives the ratio of magnetic field frequency to motor rotation frequency."

So do we really want to divide by 7 for a 14 pole motor?

https://en.wikipedia.org/wiki/Outrunner
```

---
## \#7 Posted by: PI3RR3 Posted at: 2019-01-04T09:35:03.483Z Reads: 38

```
Can you provide a tutorial on how to get live data from the vesc with an arduino?
I would really appreciate =)
```

---

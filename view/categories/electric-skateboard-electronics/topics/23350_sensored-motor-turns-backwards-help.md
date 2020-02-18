# Sensored Motor Turns Backwards. Help

### Replies: 18 Views: 498

## \#1 Posted by: flywithgriff Posted at: 2017-05-18T02:34:49.893Z Reads: 96

```
I have just set up my new 10s build with a sensored motor and it turns the wrong direction. I have tried changing the wiring order and it makes the motor stutter one way and nothing at all the other. Ideas?
```

---
## \#2 Posted by: JLabs Posted at: 2017-05-18T02:39:33.664Z Reads: 97

```
If you change any of the phase leads you have to re run motor detection. It could also be misplaced sensors that only run properly in one direction.
```

---
## \#3 Posted by: flywithgriff Posted at: 2017-05-18T02:41:24.637Z Reads: 97

```
I changed the phase wires but didn't know about the motor detection part! 

The motor turns the correct direction during motor detection but it just stutters when using the remote. The only combination of wiring i can find that it spins with the remote makes it run backwards
```

---
## \#4 Posted by: longhairedboy Posted at: 2017-05-18T02:59:28.078Z Reads: 90

```
yup this happens to me all the time. Flip two phase leads, re-run motor detection, and you'll be golden.
```

---
## \#5 Posted by: flywithgriff Posted at: 2017-05-18T03:01:43.667Z Reads: 87

```
Nope, it just jerks in opposing directions. Literally no matter how they are ordered.
```

---
## \#6 Posted by: KTMinni Posted at: 2017-05-18T03:01:57.808Z Reads: 87

```
Don't forget to write config after the detection!!!!
```

---
## \#7 Posted by: flywithgriff Posted at: 2017-05-18T03:03:12.041Z Reads: 84

```
.......damnit.......

I clicked apply motor detection settings every single time.... not write config.... im an idiot...
```

---
## \#8 Posted by: longhairedboy Posted at: 2017-05-18T03:03:48.316Z Reads: 83

```
[quote="KTMinni, post:6, topic:23350, full:true"]
Don't forget to write config after the detection!!!!
[/quote]

 This. The point of detection is to get the right values. With sensors, you have to make sure they take by applying the settings. Some of them won't apply on thier own though on occasion, so make sure they're all set right based on the feedback you got.
```

---
## \#9 Posted by: mmaner Posted at: 2017-05-18T03:04:01.800Z Reads: 81

```
Lol, I've done that a thousand times 😀.
```

---
## \#10 Posted by: longhairedboy Posted at: 2017-05-18T03:04:18.395Z Reads: 79

```
... and also you have to save your settings. lol
```

---
## \#11 Posted by: flywithgriff Posted at: 2017-05-18T03:04:42.506Z Reads: 74

```
I can't believe i did that...
```

---
## \#12 Posted by: flywithgriff Posted at: 2017-05-18T03:05:26.966Z Reads: 71

```
Thoughts on Hybrid versus just running Sensored?
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-05-18T03:08:18.463Z Reads: 70

```
hybrid will give you more top end and still give you the benefit of sensors at startup as well as lower end acceleration in general in my experience.
```

---
## \#14 Posted by: KTMinni Posted at: 2017-05-18T03:09:14.156Z Reads: 67

```
Hybrid good if you're running bldc but FOC doesn't have the option.  Hybrid allows smooth control at low speeds and and then limitless speed on the top end(you know only limited by your motor/battery/eRPM)
```

---
## \#15 Posted by: flywithgriff Posted at: 2017-05-18T03:10:08.237Z Reads: 65

```
Ok awesome guys. Im setting up my 10s build for the first time. Just making sure im setting it up right. This is quite a jump coming from a 6s setup.
```

---
## \#16 Posted by: KTMinni Posted at: 2017-05-18T03:10:56.094Z Reads: 66

```
Man I loved riding my 10s!  I disassembled my battery and probably sending them to get spot welded so I'm out for a few days.
```

---
## \#17 Posted by: flywithgriff Posted at: 2017-05-18T03:12:21.071Z Reads: 64

```
Ill be riding this one for the first time tomorrow after work! If I can ever get this remote to ever get more than half a throttle response. It doesn't engage throttle until 58%. Its a remote i picked up from MEB but just cant get it trmmed out.
```

---
## \#18 Posted by: KTMinni Posted at: 2017-05-18T10:56:00.839Z Reads: 48

```
You have to adjust the minimum pw(pulse width) in the VESC.  Mine I think the minimum was like 1.7 or something.  Anyways just try to get the green bar in the config for ppm to 50%
```

---

# Can not stop the VESC

### Replies: 3 Views: 131

## \#1 Posted by: AutoCar Posted at: 2019-09-15T01:44:21.144Z Reads: 69

```
Hi, I am using the Focbox to build a robocar. I have some questions I hope you guys can help me. I know most of you are building skate board, but you guys use the Focbox a lot so your expertise may help me. For my car, I send some computer messages to the Focbox to navigate the car. Once I stop sending the message, the car will stop immediately. Recently I found, however, it was no longer the case. Even when I stop sending message, the car continue move, at a slower speed. This is a big problem for me. Do you know why?
```

---
## \#2 Posted by: Wajdi Posted at: 2019-09-15T06:32:17.216Z Reads: 49

```
How are you sending your commands?
```

---
## \#3 Posted by: Fosterqc Posted at: 2019-09-15T08:46:16.617Z Reads: 31

```
Computer messages, obviously.

jk. 

@AutoCar 

Pretty sure that means USB?

So you are in the VESC tool or other means of interfacing from PC to VESC?

Not hooked up to a Arduino or other microcontroller?
 
A good simple play would be to use normal RC multi channel Receivers PWM output to VESCs
```

---

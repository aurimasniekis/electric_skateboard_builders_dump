# Double checking one-wheel VESC settings

### Replies: 2 Views: 122

## \#1 Posted by: Sc0urge Posted at: 2019-09-15T11:18:46.369Z Reads: 20

```
I've finished the build on my homebrew onewheel, and i'm going through the setup in VESC tool.

I've read a bit on the forum, and set up my motor with what i think is right, but i'm a noob, and would prefer not to catch fire, or kill my electrics.
Motor: [Phub 36V/600w](https://www.aliexpress.com/item/32823573279.html) 
Battery 10S2P 30Q (unknown BMS)
VESC Flipsky 4.12

I've set the motor up via wizard as FOC, and limited the current, and miniumal regenerative braking
![image|661x356](upload://2KTDAOOXsj72OuK1kOIdS5R27w7.png) 

Also set the battery voltage cuttoff as between 34V and 31V

it'll be arduino driven via PWM, so using PID speed control, no reverse

the goal is for standard onewheel forward control, no need for reverse, i don't think i'll need braking via motor as it'll just see me go A over T.
```

---
## \#2 Posted by: Fosterqc Posted at: 2019-09-15T11:29:44.928Z Reads: 19

```
Huh so by no reverse you mean it will just have limited amps in braking and less amps to accelerate backwards for balancing? And the Arduino outputs full reverse and the vesc limits the current. 

Are you using some open source code or did you write it? I'm actually a Arduino noob you can import a PID loop from the sketches tab though so not much may be involved. 

It would be cool to see a spin-up test.
```

---

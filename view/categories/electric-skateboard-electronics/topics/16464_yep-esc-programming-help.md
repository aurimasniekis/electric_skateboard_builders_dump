# YEP ESC programming help

### Replies: 3 Views: 1288

## \#1 Posted by: krloz Posted at: 2017-01-22T01:08:27.735Z Reads: 68

```
Hi  fellow sk8rs
I am currently building a board with a couple o YEP 60A esc and I am having trouble programming them as i dont understand how some of the parameters influence on how the board drives. has anyone used this esc on their board and can tell me wich options you used and why. i am using the programming card.
thank you very much for the help
```

---
## \#2 Posted by: chuttney1 Posted at: 2017-01-22T04:58:08.921Z Reads: 59

```
This video can  help you in programming. https://www.youtube.com/watch?v=zAwYZJdbT68

I think no one here uses aeroplane ESC in eboard builds as it does not fit for this application. It may not really last long. You will have to experiment with the settings when you ride.  Some of us the VESC because it surpasses ESCs used in RC aeroplanes and RC cars I can explain some of the things. What motor are you using?

Timing: advance timing gives more power on the higher end. Retarding/lowering timing gives more power on the lower end. Torque varies with timing.  
Brake: ?. How hard brakes are applied.
Governor mode: Sets upper limit on motor speed. You will have to search how the P and I gain affect this. 

There is some RC site like rcgroups.com where people have the same ESC brand. Much of the other options such as PWM frequency, startup power and startup speed don't really apply to what we use. 

From rcgroups.com for PWM frequency. https://www.rcgroups.com/forums/showthread.php?2669447-PWM-settings The main thing is what it does as quoted by RCMan.

 "Have you looked at what Castle says about PWM?
“This setting changes the frequency with which the controller sends power pulses to the motor. With some motor types, the higher the frequency the more efficient the motor will run, but always at the expense of increased heat within the controller. If you decide to experiment with changes to PWM, use a wattmeter, a tachometer and a temperature gun to find out how changes affect your entire power system. An increase in PWM frequency will always increase the controller temperature. It may or may not decrease the temperature of the motor.”
```

---
## \#3 Posted by: krloz Posted at: 2017-01-22T10:00:03.159Z Reads: 40

```
Hello chuttney1
thank you very much for all this info
I had already watched tht video. and pretty much every video on youtube about this esc. my problem is more on how each option influences on the driving rather than on how to program the esc with the card.
actually, the explaining you did on does parameters helped me more than all de youtuvideo watching i did.
I am driving a Turnigy Aerodrive SK3 - 5065-236kv with a 5:1 relation on 8" MB wheels
```

---

# FAULT_Code DRV8302 -trouble shooting- help needed

### Replies: 15 Views: 440

## \#1 Posted by: Andy87 Posted at: 2018-07-15T12:07:09.661Z Reads: 72

```
Looks like today I fired my first VESC...Just don't understand how and why...
Last week I had sometime an ABS_Over_Current Fault, but it was just randomly and didn't effect my riding.
Yesterday I was out for a 20km ride and all was good.
For the first 4min of my ride today everything was fine. Than I needed to stop because of traffic.
In the moment I wanted to continue driving my master VESC just stoped working.
I looked the log file I recorded and there was nothing special about motor or battery current.
I didn't hit max speed or something like this, but the PCB and Mosfet temp already have been around 68 degrees.
So first question is, how it can happen that the temp rise up so fast so high without big current flowing?
Second question, is there an opportunity to see that the DRV chip is really broken?
I opened the cover and couldn't find anything unusual.

I have a VESC form @esk8 based on HW4.12. 

![IMG_4876|375x500](upload://jW3yvrkjdRfEHUfxTjZczZWVokW.jpg)
I run dual with motor max 80A, bat max 40A on a 11S4P HG2 battery and 190kV Motor.
Gearing is 15/59 on 6.5 inch pneumatics
```

---
## \#2 Posted by: esk8 Posted at: 2018-07-15T15:31:06.563Z Reads: 56

```
The problem is with the settings
The esk8 controller can only 60A
Since the motor max value is set to 80A
The controller does that for a while
but at some point that's too much.
The max motor may only be 60A.
But that has already been mentioned in many topics.
V4.12 with Mosfet's max 50A and Directfet's max 60A.
11S with a 190KV engine can be reached via the 60K ERPM.
Were the limits set to 60K?
The 60C ° are normal at 60A, that the temperature has gone up
were closer to the settings of 80A.
It does not always have to be a hole in the DRV when it's broken.
Ever read the default in the terminal?
Is there DRV error?
When turning on the controller what LEDs are visible?
Blue, and blinks red 3x?

Greeting Attila
```

---
## \#3 Posted by: Andy87 Posted at: 2018-07-15T16:12:54.085Z Reads: 51

```
Ok that’s new for me.
Thought the max current related to the max battery current and that hw4.12 can handle max 50a input.
Never the less I set the motor max to 80a I never reached more than 40a according to all the log files I have. So that shouldn’t be the issue.
The max erpm was set to 60000 and -60000 and I also never reached it.
If I power on the vesc I get three times red light. No blue light anymore. 
If to look the live data in the bldc tool than I see the DRV fault. That’s the only fault i see. Is there something like fault history log in the bldc tool? Would be nice if I could look if there more faults than only the drv.
```

---
## \#4 Posted by: esk8 Posted at: 2018-07-15T17:06:06.164Z Reads: 50

```
The DRV error is the problem in itself.
Motor max means how much A should go through the fets,
direction motor and that is 60A max. at Directfets
And the maximum battery current means with how much A the battery should be discharged.
Since the controller is not limited.
You have the LG HG2 with 20A discharge and 4P
What 80A equals that shared by 2 controllers
makes 40A maximum per controller, so you did not come across 40A.
but the batteries can go over these values for a short time
Unfortunately, I can not say exactly what made the mistake.
But it is strange that the red LED is still flashing and the blue is not working anymore
Usually it's the other way around after a DRV error
```

---
## \#5 Posted by: esk8 Posted at: 2018-07-15T17:08:38.327Z Reads: 48

```
How much did you enroll in Batt min?
```

---
## \#6 Posted by: Andy87 Posted at: 2018-07-15T17:29:08.198Z Reads: 48

```
I mean i never came over motor 40a.
Battery never over 36a.
The battery min was set to -7a.
The motor min to -45a
Strange was that I had last week already a abs over current fault. Only in time of switching on.
I made some trouble shooting and found out that if I disconnect the motor sensor wires the fault disappear. 
After two days I tried again with sensor wires and all was good. Couldn’t explain this, but maybe it was already a sign?

Just in case I would take a try and change the DRV chip. What else I need to do after? Flashing firmware?

And a general question to the motor amps.
I read here often that it’s not so important to which value it’s set. I even read that you can set it to 200a and from there start to go down till you found your perfect settings?
How can people write like this?
I thought also other controllers like focbox etc use directfets??? I‘m a bit confused now.
```

---
## \#7 Posted by: DeathCookies Posted at: 2018-07-15T17:33:59.970Z Reads: 48

```
The battery Max setting should be only 60a but the Motor max can be higher.
Only if you Pull more than 60a continous from the battery you can smoke the Esc after a while
```

---
## \#8 Posted by: Andy87 Posted at: 2018-07-15T18:09:39.599Z Reads: 44

```
That’s what I always thought and that’s how I set up my vesc. For sure the battery amps depends from your battery and from the ability of your vesc to get rid of the heat. But with a good heatsink a vesc 4.12 should be able to handle min 50a. Which is not so easy to draw in dual for constant current 😅
The motor amps shouldn’t matter as you can’t really overload your motor.
But that’s don’t match with what @esk8 said
```

---
## \#9 Posted by: esk8 Posted at: 2018-07-15T18:09:49.738Z Reads: 40

```
Motor max is the setting how much ampere the
Controller can give the engine.
Limited by the fet's
I speak for our controller now!
I drive VTC6 with 3120mAh 10S / 6P
which corresponds to 180A.
Each controller can get up to 90A from the battery
If I set 90A at motor max, the controller will try this
To give 90A, but how long?
But I think I have found the mistake.
Your batt min was too low, -7A is too little.
The controller only gives your battery back 7A
Your engines produce much more
So the controller is not going anywhere with the remaining energy
and distributed them on the pcb which caused the error due to an overvoltage on the pcb
If you had taken the original settings,
Motor max 60A
Mottor min -60A
Bat Max 60A
Batt min -20A
nothing would have happened.
I've measured that the 63 motors can produce up to 54 volts
which also have to go back to the battery, otherwise it destroys the PCB.
I think the controller already has too much power at the first fault
brought the PCB.
It can happen that the superfluous current causes motor detection to be lost.
You do not notice that and next time you drive without engine detection
That can kill the DRV.
```

---
## \#10 Posted by: Andy87 Posted at: 2018-07-15T18:16:32.339Z Reads: 37

```
Sounds logic but still don’t understand some things.
As i run dual and set twice 7a my total bat min was 14a which is already not so far from 20a.
I don’t understand why the energy while breaking go through the pcb. The motor can produce heat and give away the energy plus the -14a back to the battery. And that’s always just for a peak time.🙈
```

---
## \#11 Posted by: Andy87 Posted at: 2018-07-15T18:18:53.051Z Reads: 35

```
And how about the repair question?
If I replace the drv.
Can you say me if it’s necessary to upload something? Do i need special Tools for it?
```

---
## \#12 Posted by: esk8 Posted at: 2018-07-15T18:20:04.111Z Reads: 34

```
But that is only a guess!
Because something like that has already happened to me.
```

---
## \#13 Posted by: DeathCookies Posted at: 2018-07-15T18:25:18.439Z Reads: 35

```
[quote="esk8, post:9, topic:61908"]
Motor max is the setting how much ampere the
Controller can give the engine.
Limited by the fet’s
[/quote]
You mean that we should only use 60a Motor max?
You have three Phase wires and at least three mosfets. Each could run at 60a. So you would not have a Problem by running more than 60a Motor max?!
```

---
## \#14 Posted by: esk8 Posted at: 2018-07-15T19:08:53.780Z Reads: 33

```
You need a the Bootloader for flash the DRV Chip with an StLink USB Stick
```

---
## \#15 Posted by: Andy87 Posted at: 2018-07-16T09:58:26.033Z Reads: 31

```
I read a bit more about Bat min settings here...
If to take the words from @Ackmaniac and Trampa right, it 100% can´t be the reason why the DRV broke.
1. the energy converts to heat in the motors + the recharge of 14A to the batteries 
2. if the VESC heat up by any reason, the temp. limit should shut down the VESC before it broke. Means I could just don´t break anymore, but it wouldn´t kill my DRV.
3. I looked through all log files and while breaking I never hit the 6A per VESC, so it means even my low 7A per VESC setting wasn´t reached.

I guess it´s was somehow connected with the ABS_Over_current messages I had last week.
Usually the ABS Fault indicates a lose component, shitty solder joint, or something like this. Visually I couldn´t find anything lose.
Buuuut the VESC cover was broken when I got them delivered. 
You said everything should be fine non the less, but who knows maybe some component was hit or affected...who knows...now it´s too late.

If you interested you can find the explanation here (and comment 69 what Trampa said):
https://www.electric-skateboard.builders/t/focing-around-weak-brakes-and-cutout/33203/66?u=andy87
```

---

# BLDC Settings? Whats wrong?

### Replies: 15 Views: 805

## \#1 Posted by: Cuprani Posted at: 2017-02-10T22:54:37.971Z Reads: 91

```
I recently build my board. The same setup as a friend of mine, but I'm missing a lot of power.

Specs:
DIY VESC
Single 190 kv 3150 watt motor
12S1P Lipo (20c) 5000mAh

Here is a log of a recent run
https://metr.at/r/W8Ak0

I have 2 problems.
At 50 - 75% brake, the regenerative current gets to high and as a result it stops braking.
This gives really dangerous situations.
The max braking current is set at -12A, but as you can see above at 7:31:39 PM at about -3A it stops braking as a result of over current.

Also I miss a lot of power. 
My setup should run 40A easy, but the max current (full throttle uphill) is not more then 16A.
Also the duty cycle never is more than 50%, regarding full throttle.
Could anyone look at my settings or suggest what could be wrong?

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_Motor.jpg[/img]

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_BLCD.jpg[/img]
(detection of motor was OK)

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_Advanced.jpg[/img]
(did not change anything here)

[img]https://sites.google.com/site/nilsvdg2/home/BLCD_PPM.jpg[/img]
(Receiver gets to 99,9% at ful throttle and 0% at full brake)
```

---
## \#2 Posted by: Tonto2k Posted at: 2017-02-11T11:43:02.328Z Reads: 62

```
You got 60kph !!! Wow 😳
```

---
## \#3 Posted by: Cuprani Posted at: 2017-02-11T12:54:02.807Z Reads: 62

```
No, that was wheelspin. Max speed was 34 km/h.
But my friend with exact the same setup does do a 60 km/h on a straight road.  I do not even come close. 

[img]https://sites.google.com/site/nilsvdg2/home/IMG_20170211_135114_417.jpg[/img]
```

---
## \#4 Posted by: Martinsp Posted at: 2017-02-11T13:20:56.642Z Reads: 60

```
Hey there, I dont know what your problem is unfortunately but that log is interesting. What is it made with?
```

---
## \#5 Posted by: Cuprani Posted at: 2017-02-11T13:44:07.715Z Reads: 62

```
The log is made with my phone with an bluetooth module for the vesc.

https://metr.at/shop
Also works with android and apple watch. Really nice!
```

---
## \#6 Posted by: Bender Posted at: 2017-02-11T14:31:32.743Z Reads: 64

```
I'm very curious bout this too
I'm having a similar problem. On an older set up I could draw 50 amps at times and now it peaks at 15-16 amps. The only things that are different in set up are the anti-spark switch and the metr Bluetooth module, but I don't that could be it.

What does your setup look like?
Have you compared it too your friends, and also looked at his BLDC settings?
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-02-11T15:29:13.218Z Reads: 59

```
The BLDC settings look ok to me. A bit powerfull but should be working. I also think something physically is wrong. And that you got a overcurrent error doesn't really make sense in this situation. 
Do you have a BMS in between or a anti spark switch that doesn't work properly. Or bad soldering.
Maybe the VESC has some trouble as well but my first guess is that something isn't correct with your battery cables.
```

---
## \#8 Posted by: PXSS Posted at: 2017-02-11T15:33:39.729Z Reads: 60

```
Is the firmware different from vedders?
If so try going back to original firmware maybe its a bug in the custom firmware
```

---
## \#9 Posted by: Cuprani Posted at: 2017-02-11T19:59:39.174Z Reads: 53

```
I have no BMS jet. It's underway from China, and I will only use it to charge, and not to discharge.
I have an HV powerswitch. 

Battery condition looks just fine. Al is balanced at the same voltage. Resistance is about the same in all cells. I can't see how you can wire it wrong as it just runs about 50V in parallel. 

Firmware on the VESC is stock. It's a 4.12 VESC with 2.18 software.
```

---
## \#10 Posted by: Bender Posted at: 2017-02-11T20:47:11.831Z Reads: 51

```
well i just figured out the amp issue. METR shows the battery amps by default and you customize the layout to get the motor amps. that shows me more what id expect peaking at 40-50 amps

next thing to check is your gearing ratio. tell us more about your set up
```

---
## \#11 Posted by: Cuprani Posted at: 2017-02-11T23:26:37.950Z Reads: 46

```
16T on engine, 36T on a 90mm wheel.
See [here](http://www.electric-skateboard.builders/t/cupranis-dutch-custom-build-6374-190kv-3150w-12s) for full specs.

I will check if I can find other amps, but still my duty cycle only hits 49% max, so somehow it is not even trying to fully power the motor. That's why I think it is in the settings somehow.
```

---
## \#12 Posted by: Eboosted Posted at: 2017-02-12T06:01:02.682Z Reads: 42

```
Go to terminal and write faults, what do you get?, post the results here

Edit:
I see the fault is overcurrent, but when you write faults in terminal, it gives you additional  information such as values the VESC was runing at the moment of the fault, not just the text.

I'm having the same problem on my 10S first build, VESC shows a 57.8V when the fault occurs, I though the problem could have been the BMS shutting down, but now I wonder why do you get the same fault if you are not ruing a BMS and you are not exceeding the maxuimun input voltage of the presetted 57V on BLDC tool....
```

---
## \#13 Posted by: Cuprani Posted at: 2017-02-12T13:59:55.517Z Reads: 41

```
@Eboosted 
How do I write faults? I see no option to do so..

[img]https://sites.google.com/site/nilsvdg2/home/BLDC_Terminal.jpg[/img]
```

---
## \#14 Posted by: Cuprani Posted at: 2017-02-12T14:08:21.571Z Reads: 36

```
O haha, you just meant TYPE: "fault" I figured out just yet :nerd:
When I do so there is no fault because I haven't driven it.

As there is snow outside today and I do not have spikes or winter tyres I will test it later on..
```

---
## \#15 Posted by: Eboosted Posted at: 2017-02-12T14:53:40.269Z Reads: 35

```
You need to ride it and, before turning off the power switch, plug the USB cable and type faults. If you turn off the board faults will be erased. 

Charge your board 100% and ride it as fast as you can and brake, do this in an empty or underground parking lot to avoid the snow.
```

---

# EMAX - 820kv XA2212 brushless outrunner with MayTech VESC 4.2v

### Replies: 22 Views: 895

## \#1 Posted by: arsh Posted at: 2018-03-08T14:18:38.873Z Reads: 137

```
Hello, 

This probably sounds stupid but I ordered Maytech's VESC or in general a VESC without first checking that VESCs has a speed limit (ERPM) of about 100,000 (or 60,000, can't recall the exact number). That means I can not properly run a 820kv motor (very small and very light) using VESC. 

My project is not related to skateboards or drones, it is a class project and I wanted to use VESC for two reasons:
1- It has Serial pins so I can measure current , temperature and rpms and log them 
2- It seems to have a nice bi-directional positional control thus I was hoping to use it in a robotic application. 

I also do not need a very high speed (rather I need a high torque) but I can not use gears (project requirements) as well as low kV (means more weight) outrunners (weight requirements). 

So I was hoping if anyone here can help me set this up as I am pretty confused about the motor and battery parameters. (I know this is easy stuff but when I use low amps in bldc-tool, the motor is not detected). 

Also I am using FW 2.18 and not using VESC-tool because for some reasons, I am unable to update the firmware from BLDC as well as from VESC tool. Everytime I update the FW, it says it is updated but when I reconnect my VESC, the same old FW is detected in it. 

I also emailed MayTech's support who actually first gave me VESC-tool application (which I had already tried) and when I complained about firmware not being changed after update, the sent me a link to STLink which I still have to buy. 

So I have two queries really:

I need to run 820kV outrunner (very slow speed) with VESC, please tell me if that is possible on 4.2 hardware with 2.18 FW 

I am unable to use the TX RX pins as I have tried 3 Arduino VESC libraries and non of them seems to get any data from the TX pin, is there anything else I should do? 

Thank you 
Arsh
```

---
## \#2 Posted by: Der6FingerJo Posted at: 2018-03-08T14:37:29.811Z Reads: 119

```
What Voltage do you plan on using? 
eRPM depens on kv, pole count of the motor and the used voltage.
```

---
## \#3 Posted by: arsh Posted at: 2018-03-08T15:15:43.697Z Reads: 112

```
I have different supplies, I can either use a 12 to 24 volts 5 A Toyotech Supply ( http://dhinst.com/shop/goods/goods_view.php?&goodsno=186785783&category= ) 

or I have Lipo batteries the one I currently have is Tiger Atomic Platinum 3500 mAh 5C 6S (the site link is currently down). 

To be honest, I will use any volts which will give best torque and slow speed (under 3000 RPM). I have already tested my project with Inrunners (but with sensored and with Maxons controllers) and simple Maxon DC motors and now I want to try Outrunners
```

---
## \#4 Posted by: TarzanHBK Posted at: 2018-03-08T15:30:40.407Z Reads: 93

```
It´s really hard with that motor.
Test it with a 4s battery - with a 7 pole pair motor on 820kv this will bring you up to 85.000 erpm max.
You could then limit max erpm to 60.000 and you´ll be fine.
```

---
## \#5 Posted by: TarzanHBK Posted at: 2018-03-08T15:32:15.862Z Reads: 87

```
just saw your power supply - use 12V on it and limit erpm
```

---
## \#6 Posted by: arsh Posted at: 2018-03-08T15:44:54.227Z Reads: 81

```
Thank you, 

I will check it but what should be the battery cutoff start and battery cutoff end in the case when I am using supply? I suppose it does not matter in that case ? Is it reasonable if I further decrease the max eRPM to 20,000?
```

---
## \#7 Posted by: Der6FingerJo Posted at: 2018-03-08T15:57:47.177Z Reads: 75

```
Cutoff makes no sense in this application, so set it to something below 12V. 
If 20000 eRPMs are enough for you it's ok
```

---
## \#8 Posted by: arsh Posted at: 2018-03-09T09:35:22.777Z Reads: 62

```
I tried the motor and VESC with power supply on 12V with 5A battery limit, 20,000 ERPM max and  the motor does not even move in this configuration (that means before when I was using the battery, the motor was moving a in a jerky fashion though the detection says bad parameters recieved), now it is not moving at all. 

Is there anything else I can try with this VESC? I don't think that I have burned it as it never actually worked properly in the first place for me to burn it later :smile:
```

---
## \#9 Posted by: TarzanHBK Posted at: 2018-03-09T09:45:13.177Z Reads: 54

```
Did motor detection work or not? Does the Vesc show any faults?
```

---
## \#10 Posted by: arsh Posted at: 2018-03-09T09:49:50.967Z Reads: 57

```
The following are my settings. No the motor was not detected neither it moved when I set the 12 V as max battery voltage. However on Read Default Config and then writing them makes the motor turn a bit (around 360, using arrow keys and then stop suddenly after each key press) 




![Capture|690x408](upload://3fjevUofT9gvLhaox3pYkEWGTYX.JPG)![Capture1|690x410](upload://jiiTXxK2OcJHGvCsC7j2BPSZ5Rt.JPG)
```

---
## \#11 Posted by: RedEagle Posted at: 2018-03-09T09:53:22.622Z Reads: 46

```
If you want to update the firmware
1. Go to http://www.vesc-project.com/
2. Create account and download vesc tool
3. Connect vesc to pc
4. Go to firmware tab and upload the bootloader to the vesc
5. Wait. Vesc should restart itself after 30 sec
6. Update the firmware
7. Wait. Vesc should restart after 30 sec
8. If it doesn't work try again. It can take a few times for it to succeed
```

---
## \#12 Posted by: arsh Posted at: 2018-03-09T10:03:20.037Z Reads: 48

```
Hello RedEagle, 

I have already followed these steps before. Though I did follow them again. 

I have the VESC-tool executable. 
I run them and connect to the VESC (in limited mode) 
I went into Firmware tab, under Bootloader I tried to upload the bootloader (I suppose I had to use the second image, in first image below) 
Then I waited like a minute and then restarted the VESC. 
I then tried the firmware update under Include Files. It says that the firmware is updated, upon re-connecting the VESC, there is always the same FW 2.18 instead of 3.X.X


![Capture2|690x439](upload://griVnvCtyZREUyd1yjJdhztibs9.JPG)![Capture3|690x441](upload://orb8TF65vcfl4eYaQmZBD1sFq1G.JPG)
```

---
## \#13 Posted by: RedEagle Posted at: 2018-03-09T11:00:27.701Z Reads: 37

```
Bootloader should have been uploaded. Did you see the lights flash? Try updating the firmware after a day or so. It'll work eventually.
```

---
## \#14 Posted by: TarzanHBK Posted at: 2018-03-09T15:35:08.195Z Reads: 34

```
you have FOC enabled in the first picture. Change to BLDC and try again.
```

---
## \#15 Posted by: E1Allen Posted at: 2018-03-09T15:55:26.299Z Reads: 30

```
Yeah. Make sure the motor isn't attached when u put it to BLDC then run motor detection.  Also in the PPM tab are you getting a signal from the TX?
```

---
## \#16 Posted by: arsh Posted at: 2018-03-10T03:01:43.526Z Reads: 25

```
Okay. 

I think I might give up on this VESC. I don't think that this is going to work as I tried PPM signal (which worked using Arduino, Servo and in BLDC-tool I used Displayed Only option). but when I tried UART, it did not work after too many attempts, nor did motor detection worked. Lesson Learnt: NO MORE CHINESE PRODUCTS :frowning: 

I used Maxon Inrunner Motors and their drivers to drive them. Now I understand that I can use the same driver if I had a sensored outrunner motor. But I checked and found that there are no sensored outrunner motors under 100g weight (basically all low kV outrunners in range of 50-300 kv are too heavy for my application).  

So can anyone suggest a small under 100g (or around 150g is fine) outrunner motor that is sensored? I might be able to use it with Maxon Drivers 

Other than that, can anyone also confirm that if I buy VESC 6.0 (which looks really cool btw), will it work for very small outrunner motor or is it specially designed for only skateboards and co? 

I am inclined towards using VESC instead of a simple ESC for two reasons, I need position control and data logging. Thus with ESC I will have to use current sensors.
```

---
## \#17 Posted by: Cobber Posted at: 2018-03-10T03:34:22.356Z Reads: 27

```
add your own encoder to any motor...
```

---
## \#18 Posted by: arsh Posted at: 2018-03-10T04:07:59.478Z Reads: 28

```
By sensored, I meant the hall sensor. For position control, I will of course add in the encoder. However Maxon Controllers requires that inrunners have hall sensors for better performance so I suppose if  Iam going to use outrunner with Maxon drivers I better buy outrunners with hall sensors (and then add encoder myself)
```

---
## \#19 Posted by: Cobber Posted at: 2018-03-10T04:15:23.663Z Reads: 27

```
yes add your own

here is a rig another member has made, but there are lots of ways of going about it, a pcb, magnets glued...

<img src="http://www.electric-skateboard.builders/uploads/db1493/optimized/3X/3/5/35b3b2e537ec76f31bad387d32aa9d888fb840c7_1_690x388.jpg" alt="20180309_134300"/>

look in to it, it's not that hard
```

---
## \#20 Posted by: arsh Posted at: 2018-03-10T04:25:50.409Z Reads: 27

```
and can you confirm if VESC 6.0 works for outrunner motors with 900kv - 1400kv ? Knowing that I would like to avoid making any changes to VESC 6.0 hardware like for example changing the shunt resistor for small motors etc. ? 

P.S: I just want to be really really really sure before I order any more hardware. I would also like to know if VESC 6.0 has bootloader capabilities because I guess Maytech does not have boot loader and their support sent me a link to buy STLink hardware which is another headache :confused: (for me at least now)
```

---
## \#21 Posted by: Der6FingerJo Posted at: 2018-03-10T08:18:40.231Z Reads: 24

```
https://youtu.be/ugD6T4MPXUw

Benjamin uses a 800kv motor in this video, that might help you. 
Bootloader shouldn't be an issue with VESC6, at least it never was with mine.
```

---
## \#22 Posted by: arsh Posted at: 2018-03-11T04:19:17.928Z Reads: 17

```
Thank you for this video. 

In the start, Benjamin said something about the shunt and how it was difficult to use it with 0.1 mili-Ohm shunt and how he used a propeller to simulate the load. I won't be using a propeller in my application. and did he change the shunt (which I believe is a small resistor) on VESC? 

Apologies if I asked something stupid
```

---

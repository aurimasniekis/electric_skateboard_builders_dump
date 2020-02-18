# My VESC is not responsive

### Replies: 22 Views: 436

## \#1 Posted by: Gorfo99 Posted at: 2018-05-24T13:38:41.039Z Reads: 85

```
I recently bought a VESC from  and initially it went through the motor detection stage successfully. However, after connecting the receiver to the VESC, it would pair with the remote but wouldn't control the motor what so ever. So after 6 hours of me and my Mechatronics teacher going through the settings, we still couldnt get it to work. Now if I try to connect my VESC to the computer it doesnt even detect the motor anymore. I have no idea what could be wrong and am also in a tight schedule. SOS.
```

---
## \#2 Posted by: goldrabe Posted at: 2018-05-24T14:09:31.266Z Reads: 80

```
Did you choose the correct com port for the vesc in the Vesc or BLDC tool?
Did you read the configuration of the vesc after connecting it again?
Did you choose the correct channel on your reciever after binding it?
```

---
## \#3 Posted by: Gorfo99 Posted at: 2018-05-24T14:15:53.413Z Reads: 75

```
Yeah the port is COM3, Channel is 1 on the receiver and what configurations exactly do you mean? I can send screen shots of my curent VESC settings
```

---
## \#4 Posted by: goldrabe Posted at: 2018-05-24T14:26:10.501Z Reads: 67

```
Is it the same channel where you did the binding on?
Try the other channels, on my remote it was channel 2 if i recall it correctly. I did set it and forgot it, but it's on a different channel then you make the binding on.
Did you set the failsafe for your remote? 
Each time you reconnect your VESC you have to read the configuration you did on the VESC first before proceeding.
```

---
## \#5 Posted by: Gorfo99 Posted at: 2018-05-24T14:27:13.710Z Reads: 60

```
alright ill try to switch to channel 2, could you walk me through on how to set the failsafe on the remote?
```

---
## \#6 Posted by: Gorfo99 Posted at: 2018-05-24T14:33:58.225Z Reads: 54

```
okay so i have an update, i went into input the setup wizard and i can now see that the remote actually inputs something ( i can see the bar moving when i activate the throttle, i have no idea what its called ) but the VESC flashes a red LED 3 times and the motor does not spin.
```

---
## \#7 Posted by: goldrabe Posted at: 2018-05-24T14:35:14.251Z Reads: 58

```
Do you bought the remote from diyelectricskateboards?
They have a tutorial on YouTube on how to set it up.
I am away from my computer at the moment and do not recall it 100% but if you use the search tab here you will get plenty of information. I think there was a thread about it just today.
If you don't set it your board will accelerate full power when your remote looses connection with the reciever or you turn off the remote.
Sorry that I can not do more for you, i hope you get everything sorted in time!
```

---
## \#8 Posted by: Gorfo99 Posted at: 2018-05-24T14:36:18.515Z Reads: 56

```
yeah i've watched so many videos on it but the videos only say to plug it in and its supposed to work, which mine doenst
```

---
## \#9 Posted by: goldrabe Posted at: 2018-05-24T14:38:23.007Z Reads: 53

```
Are you using the VESCTOOL or the BLDC tool?
```

---
## \#10 Posted by: Gorfo99 Posted at: 2018-05-24T14:39:39.988Z Reads: 50

```
ESC Tool by Ackmaniac
```

---
## \#11 Posted by: goldrabe Posted at: 2018-05-24T14:45:41.284Z Reads: 47

```
Can you see the signal from the remote in the app settings?
```

---
## \#12 Posted by: Gorfo99 Posted at: 2018-05-24T14:46:25.859Z Reads: 50

```
yeah i could when setting it up, but now the VESC is flashing red
```

---
## \#13 Posted by: goldrabe Posted at: 2018-05-24T15:12:36.824Z Reads: 44

```
Did you reflashed the firmware?
```

---
## \#14 Posted by: Gorfo99 Posted at: 2018-05-24T16:02:55.560Z Reads: 37

```
yeah i did yesterday but i can try and do it again today if that's what you reccomend
```

---
## \#15 Posted by: goldrabe Posted at: 2018-05-24T16:07:07.126Z Reads: 37

```
Can you read the configuration of your motor settings?
```

---
## \#16 Posted by: goldrabe Posted at: 2018-05-24T16:15:37.540Z Reads: 36

```
Could you do motor detection after you reflashed the firmware?
```

---
## \#17 Posted by: Gorfo99 Posted at: 2018-05-24T16:21:50.256Z Reads: 34

```
I dont think the motor detection worked after the firmware flash but i am not certain. Here are my motor settings ![image|690x440](upload://c2edZz6hWCZxDQKt7mZBWkgFFj4.png)![image|690x439](upload://boydx3BklE4PjBpMjnm65HCIXMl.png)![image|690x442](upload://h9G73ICXznFfwMRnVuozviN6tLa.png)![image|690x440](upload://3KCR8AfzBPfJcv56q5zXEv0893D.png)![image|690x446](upload://qAxB7sLGQrj8XeyDobnDE61J9Wk.png)![image|690x439](upload://iEsfNmjtIrZG5e2xuXeO7VmDzPW.png)
```

---
## \#18 Posted by: ThermalM16 Posted at: 2018-05-24T16:22:05.434Z Reads: 33

```
Hi, if you already reflashed the FW, and you're still getting 3 red flashes, you blew the DRV
```

---
## \#19 Posted by: ThermalM16 Posted at: 2018-05-24T16:23:00.232Z Reads: 33

```
Also make sure you're reflashing with 4.12 FW and nothing else
```

---
## \#20 Posted by: Gorfo99 Posted at: 2018-05-24T17:46:18.455Z Reads: 30

```
Yeah the only fw ive used is the 4.12, im not home right now so i cant test it at the moment but hopefully blowing the drv isnt the case :x if it is, is the only solution getting a new vesc?
```

---
## \#21 Posted by: TowerCrisis Posted at: 2018-05-24T18:07:47.431Z Reads: 27

```
Have you checked for faults yet? When hooked up go to the command line and enter "faults" with no quotes. It'll spit out any errors that it's had since the last boot up.
```

---
## \#22 Posted by: ThermalM16 Posted at: 2018-05-25T03:54:51.810Z Reads: 16

```
Or getting it repaired. I offer a repair service if it comes to that.
```

---

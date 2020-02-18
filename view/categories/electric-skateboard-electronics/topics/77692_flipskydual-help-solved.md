# FLipskydual help (solved)

### Replies: 20 Views: 548

## \#1 Posted by: Bobby Posted at: 2018-12-11T10:03:46.111Z Reads: 151

```
I got my dual 4.12 flipsky running and when i do motor detection, both motors work fine. Im having issues with my remote only running one of the motors at the end....... So i do motor detection on one hub, run input wizard and set it as the master. Everything working great so far.

I then do the other motor, run motor detection and its good. I set it up as the slave and  at the very end only one of the two motors spins when i accelerate on the remote... Any help would be appreciated. Im using a nano x with koowheel hubs and using @mmaner settings for the flipsky dual....
```

---
## \#2 Posted by: Andy87 Posted at: 2018-12-11T10:09:05.643Z Reads: 150

```
can you change settings on the slave when connected to the master via the CAN button in the VESC Tool?
if no, than something wrong with your CAN bus or the settings for the CAN communication.
```

---
## \#3 Posted by: Bobby Posted at: 2018-12-11T10:10:44.734Z Reads: 143

```
should i be connecting with a canbus cable even if its a dual? how can i access can communication in the vesc tool
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-11T10:15:58.923Z Reads: 133

```
i don´t have a dual 4.20, but there should be a switch to toggle between dual and single mode.
it´s located in the middle up, close to the capacitors.
make sure the switch is in the left position.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-12-11T10:16:38.330Z Reads: 125

```
https://cdn.shopify.com/s/files/1/0011/4039/1996/files/Dual_FSESC4.20_100A_MANUAL_20181106.pdf.pdf?14152829648107869006
```

---
## \#6 Posted by: Bobby Posted at: 2018-12-11T10:18:49.820Z Reads: 119

```
yea i have it on.... i followed the exact steps as the guy on the video in the flipsky youtube.... cant for the life of me figure out what im doing wrong
```

---
## \#7 Posted by: Andy87 Posted at: 2018-12-11T10:21:54.496Z Reads: 119

```
double check that in your vescs the can communication is enabled and that the master is 0 and the slave is 1.
the wizzard should set this up for you usually, but .... who knows....
if that´s not working, try to connect them via CAN bus cable if you have one to hand.
if it´s working after, than there is a problem with the internal CAN bus on the PCB probably
```

---
## \#8 Posted by: amazingdave Posted at: 2018-12-11T10:32:31.098Z Reads: 113

```
Somebody else mentioned an issue like this resolved by changing the traction control settings...

I’m on a dual 6.6 and have traction control on ackmaniac firmware with no issues. 

Sorry can’t be of any more use than that!
```

---
## \#9 Posted by: sayekim Posted at: 2018-12-11T11:14:12.215Z Reads: 102

```
Yeah check the id’s. 

Also try connecting the receiver to the other one.
```

---
## \#10 Posted by: briman05 Posted at: 2018-12-11T13:41:55.206Z Reads: 94

```
There is no can cable port but there is a can switch on it you can turn can on or off by that switch it may be defaulted to off when they send it from the factory.
```

---
## \#11 Posted by: Andy87 Posted at: 2018-12-11T13:51:02.449Z Reads: 88

```
What is this?
![image|523x500](upload://dvuwwc8HOBTENDOuyFAIZdgVvG5.jpeg)
```

---
## \#12 Posted by: briman05 Posted at: 2018-12-11T13:53:51.850Z Reads: 81

```
Well it shouldnt its has the switch that is dumb.

cause they have this on it.

![image|690x345](upload://ltfuhhZ33fcobljWqGMnriMD2V4.jpeg)
```

---
## \#13 Posted by: Andy87 Posted at: 2018-12-11T14:06:25.892Z Reads: 80

```
I know about the switch but there also the connections for the can.
So in theory you can connect a can cable too.
```

---
## \#14 Posted by: briman05 Posted at: 2018-12-11T14:08:22.247Z Reads: 79

```
I guess if the switch fails you can still connect it with the cable that seems smart but dumb at the same time.
```

---
## \#15 Posted by: Andy87 Posted at: 2018-12-11T14:15:42.013Z Reads: 79

```
That’s why I recommended that he should try if he get connection via external can cable. 
If that’s the case the switch or the connection on the pcb faulty
```

---
## \#16 Posted by: sayekim Posted at: 2018-12-11T19:57:48.626Z Reads: 72

```
Not if you want 4wd right?
```

---
## \#17 Posted by: briman05 Posted at: 2018-12-11T20:04:56.581Z Reads: 72

```
Well yes but I would say more people are going to do dual then 4wd
```

---
## \#18 Posted by: mtuan293 Posted at: 2018-12-11T22:42:59.878Z Reads: 63

```
Make sure the one set up as a master should have the ppm cable connect to the Nano X receiver. The other one doesn’t come with a cable, so if you set it up as a master, chances are thing won’t work. 

Also, make sure the Can bus ID of the slave and master is different. Usually the master is 0, and slave is 1.
```

---
## \#19 Posted by: Bobby Posted at: 2018-12-12T05:09:16.544Z Reads: 57

```
Problem solved. Used a canbus and it worked first time... also honestly it could have been my fault as well. I did update one side  of the vesc and never updated the other until tonight so it could have been running two different version. Doh!  Either way it works now. Thanks for all the help guys
```

---
## \#20 Posted by: ARetardedPillow Posted at: 2018-12-12T05:24:50.717Z Reads: 57

```
Same thing on my 6.6 actually,  the switch on the pcb didn't really work, but I didn't have time atm so I just swapped it out for some singles
```

---

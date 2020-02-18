# Faulty Receiver Please Help

### Replies: 6 Views: 127

## \#1 Posted by: harrygellis Posted at: 2019-07-25T22:11:53.702Z Reads: 31

```
So I've just finished my electric skateboard and its working fine and I decide to use vesc tool to improve it so with the receiver plugged into my flipsky vesc and the vesc I use the vesc tool. I had to update the firmware on the vesc and I changed some of the power settings on the vesc. I then go to run the board normally and the receiver is no longer working. I've isolated the problem to either the receiver or the remote. Now when I plug the reciever into the vesc it just maxises out the motor untill unplugged whilst the light on the receiver flashes like there no transmitter. Please Help.
This is the receiver and transmitter I use.
https://www.ebay.co.uk/itm/Electric-Skateboard-2-4GHz-Remote-Controller-Transmitter-Receiver-Binding-Plug/192790265927?hash=item2ce3320047:g:zo0AAOSwJD1cd425
Again thanks for any help.
```

---
## \#2 Posted by: esk8_hui Posted at: 2019-07-25T22:27:44.536Z Reads: 29

```
I had the exactly same symptom yesterday. I think I just reconfigured the PPM and it was gone.

I haven't figured out the reason maybe someone else can explain it.
```

---
## \#3 Posted by: harrygellis Posted at: 2019-07-26T10:28:09.528Z Reads: 19

```
Thanks for your responce. What settings did you change because I've tried every different control type and it either has the same problem or theres no responce at all.
```

---
## \#4 Posted by: esk8_hui Posted at: 2019-07-26T14:46:18.060Z Reads: 17

```
So yesterday the problem happened again but this time I noticed it is because when I was doing input setup the pulses was not detected correctly. So at normal position on the remote it applies full throttle until I did full brake. After that I did a input wizard again and corrected the mapping curve. I think you just need to make sure you are following the exact instructions in the input wizard. Here is my corrected values: ![Screenshot_20190726-073858|243x500](upload://y9x0037zcJIZMDyUhAtHMqMzRSl.png)
```

---
## \#5 Posted by: b264 Posted at: 2019-07-26T15:40:37.433Z Reads: 13

```
Did you set the failsafe?

https://forum./t/how-to-bind-the-mini-remote/95

Then, after that, set your center/min/max pulsewidths in the VESC tool
```

---
## \#6 Posted by: harrygellis Posted at: 2019-07-27T11:35:46.825Z Reads: 6

```
So I fixed the problem, my receiver cable on the vesc was plugged in the wrong way aswell as the control type being different to the default. Thanks for everyone's help.
```

---

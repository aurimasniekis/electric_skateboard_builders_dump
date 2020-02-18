# Vesc not responding to remote

### Replies: 19 Views: 2661

## \#1 Posted by: Ryanliu Posted at: 2017-02-11T04:53:04.731Z Reads: 217

```
just upgraded to vesc from a rc car esc
i connected my vesc to my motor and 6s battery and my controller that i binded to the reciever that is connected to the vesc.
The setup it unresponsive and the pulsewidth in BLDC tool isnt moving when i move my throttle. I used this same throttle and bound it to my rc esc setup and it works so what could be wrong?
Links to my parts:
VESC: http://www.ebay.com/itm/112204958459?_trksid=p2057872.m2749.l2649&ssPageName=STRK%3AMEBIDX%3AIT
Motor: https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-149kv-brushless-outrunner-motor.html
Battery (2 of these in series to get 6s): http://www.ebay.com/itm/Traxxas-11-1V-5000mAh-25C-3S-LiPo-Battery-with-TRA-ID-TRA2872X-/162097468113
```

---
## \#2 Posted by: JohnnyMeduse Posted at: 2017-02-11T05:04:40.856Z Reads: 208

```
Reboot your vesc ,??
```

---
## \#3 Posted by: Ryanliu Posted at: 2017-02-11T05:08:11.331Z Reads: 198

```
tried that.
```

---
## \#4 Posted by: Ryanliu Posted at: 2017-02-11T05:09:44.908Z Reads: 191

```
<img src="/uploads/db1493/original/3X/6/2/62aaf2facb2330d60ccabbdb22fd6be82263e914.png" width="690" height="388"><img src="/uploads/db1493/original/3X/7/4/742f1de81a62ff12fc8f43da188443e3607078ad.png" width="690" height="388">
here are my BLDC tool settings
```

---
## \#5 Posted by: JohnnyMeduse Posted at: 2017-02-11T05:28:30.586Z Reads: 175

```
Do you have any picture of your setup?
```

---
## \#6 Posted by: Ryanliu Posted at: 2017-02-11T06:00:36.234Z Reads: 174

```
<img src="/uploads/db1493/original/3X/8/a/8aca404a732cab2e2c9511b8f081e821ad6bbfb6.jpeg" width="375" height="500">
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-02-11T07:47:29.027Z Reads: 163

```
Have you try changing the channel ?
```

---
## \#8 Posted by: Ryanliu Posted at: 2017-02-11T08:12:56.868Z Reads: 165

```
Yes i tried using the remote while charging it and also using it after it is charged
```

---
## \#9 Posted by: JohnnyMeduse Posted at: 2017-02-11T18:01:31.998Z Reads: 159

```
Are your servo cable plug in the ch1 or ch2 ?
```

---
## \#10 Posted by: Ryanliu Posted at: 2017-02-11T21:59:33.144Z Reads: 156

```
Channel 1 and the red led is on when i turn my controller on so they r connected
```

---
## \#11 Posted by: JohnnyMeduse Posted at: 2017-02-11T22:38:22.676Z Reads: 154

```
Hummm... but in your picture your plug in the channel 3 or the binding channel... You should be plug in the ch1 see the image below. 

<img src="/uploads/db1493/original/3X/a/1/a1219a4443eb5b8b03489bac68a6644e5e8b7bdd.jpg" width="512" height="442">
```

---
## \#12 Posted by: Ryanliu Posted at: 2017-02-12T20:23:20.858Z Reads: 145

```
Just tried changing it to channel 1 and the same problem persists
```

---
## \#13 Posted by: Ryanliu Posted at: 2017-02-12T21:38:12.365Z Reads: 146

```
The red led shows it is connected but the vesc doesnt respond to it
```

---
## \#14 Posted by: JohnnyMeduse Posted at: 2017-02-13T22:06:10.053Z Reads: 142

```
Sorry for the late answer... I'm not really sure of what went wrong with tour remote, but maybe retry the process following this video

http://www.electric-skateboard.builders/t/vesc-faq-setting-up-receiver-and-brakes/244?u=johnnymeduse
```

---
## \#15 Posted by: linkedtim Posted at: 2017-11-04T17:25:35.705Z Reads: 97

```
@Ryanliu did you ever come to a resolution on this? I think I'm having a similar/the same issue and can't seem to get it working. I know the post is super old, but I didn't see a resolution anywhere. I've tried both ppm and  UART connections to no avail.

https://www.electric-skateboard.builders/t/help-did-i-fry-my-vesc/37065
```

---
## \#16 Posted by: Gorfo99 Posted at: 2018-05-18T12:44:09.964Z Reads: 61

```
I'm currently having the same issue, did you ever find a solution?
```

---
## \#17 Posted by: Cieszyn Posted at: 2019-02-19T06:54:41.477Z Reads: 30

```
Up. I have the same issue. It was working before, but lately i can't map the remote, vesc doesn't respond and doesn't read the movement of two of my rc remotes (shows - 100% ppm)
```

---
## \#18 Posted by: Conor Posted at: 2019-08-01T16:48:55.358Z Reads: 13

```
Anyone find a solution yet???
```

---
## \#19 Posted by: itsrow Posted at: 2019-10-18T15:59:27.412Z Reads: 6

```
Did you find the solution to this?  I have 3 VESCs that don't respond to any input from UART or PPM.
```

---

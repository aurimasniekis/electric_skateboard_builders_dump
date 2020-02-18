# Vesc red led, does not react to remote control

### Replies: 27 Views: 2252

## \#1 Posted by: Stefan Posted at: 2016-09-30T12:46:45.554Z Reads: 116

```
Hey everyone,

i recently installed a vesc and had to flash the firmware on it. Now after configuring it within bldc, i recognized that the vesc shows a red led instead of the green one. What does this mean? The motor will spin when doing a motordetection in bldc but the board does not react to the remote control.
```

---
## \#2 Posted by: Blasto Posted at: 2016-09-30T12:51:44.173Z Reads: 116

```
You need to configure the remote in the bldc tool.

You need to configure the motor parameters first (motor detection)
```

---
## \#3 Posted by: Stefan Posted at: 2016-09-30T13:00:13.046Z Reads: 114

```
I did both.
```

---
## \#5 Posted by: Stefan Posted at: 2016-09-30T13:15:45.300Z Reads: 99

```
The problem is not solved?
```

---
## \#6 Posted by: evoheyax Posted at: 2016-09-30T15:16:08.608Z Reads: 91

```
What is your fault code?

Connect your vesc to the BLDC Tool, go to Realtime Data, then click activate sampling. The last line on the left will tell you your fault code. if it's DRV**** where * is a wildcard, then your screwed. Other wise, it will point you towards what setting need to be changed. Flashing the wrong firmware will fry the DRV, so I hope you used the right firmware and selected the default.bin file when you flashed it.
```

---
## \#7 Posted by: Stefan Posted at: 2016-09-30T15:51:09.705Z Reads: 87

```
It says fault code none
```

---
## \#8 Posted by: Blasto Posted at: 2016-09-30T15:53:13.729Z Reads: 82

```
Make sure your receiver is in the right channel. In the ppm tab, tick the ppm display. You should see the ppm signal
```

---
## \#9 Posted by: Stefan Posted at: 2016-09-30T15:58:58.697Z Reads: 81

```
<img src="/uploads/db1493/original/3X/6/a/6a5d87994238bda07101a5b9213049146e80c0c5.JPG" width="665" height="500">

But does this even matter? The vesc show the red led with or without the receiver connected.

Edit:
I forgot to say that the pulsewidth is nearly constant at 55%
```

---
## \#10 Posted by: Blasto Posted at: 2016-09-30T16:05:01.139Z Reads: 76

```
Can you show a pic with the led on? I want to see the led position, the colors could have been swaped (doesnt affect performance)
```

---
## \#11 Posted by: Stefan Posted at: 2016-09-30T16:13:11.698Z Reads: 76

```
I made a picture when the vesc turned off. With the blue led on you would not see anything beside it on the image.

<img src="/uploads/db1493/original/3X/0/b/0b701f4bbce60adfe372ad5c6220ae9af8fd6574.JPG" width="666" height="500">

Led 1 is always red, led 3 is always blue and led 2 blinks 3 times red on start up.
```

---
## \#12 Posted by: Blasto Posted at: 2016-09-30T16:19:21.678Z Reads: 75

```
Ok, led 1 should be a green led, but it's red, no big deal, just color.
```

---
## \#13 Posted by: Stefan Posted at: 2016-09-30T16:20:02.509Z Reads: 74

```
So 2 middle led would be red if there was a problem with the vesc?
```

---
## \#14 Posted by: Blasto Posted at: 2016-09-30T16:22:44.688Z Reads: 72

```
Yes, led 2 will constantly blink 3 times if there was a fault code.
```

---
## \#15 Posted by: Stefan Posted at: 2016-09-30T16:25:42.598Z Reads: 70

```
Okay. Then the problem should be somewhere with the bluetoothconnection...
```

---
## \#16 Posted by: Blasto Posted at: 2016-09-30T16:27:48.659Z Reads: 70

```
make sure your receiver is in the right channel.

I don't know what remote you have, but you seem to have another channel on the header

<img src="/uploads/db1493/original/3X/c/3/c33676ee8b2666ea46e7020e8b6da6ce532e80fe.jpg" width="690" height="463">
```

---
## \#17 Posted by: Stefan Posted at: 2016-09-30T16:37:02.771Z Reads: 68

```
That's true. I'm using the channel the remote was connected to when i opened the board for the first time. Changing the channel does not change anything. The pulsewith displayed in bldc still stays nearly constant at 55%. But shortly after i changed the channel the board somehow accelerated for a short time and then stopped again without touching the remote. I am not quite sure if the bluetooth receiver maybe broken.
```

---
## \#18 Posted by: Blasto Posted at: 2016-09-30T16:39:43.617Z Reads: 66

```
what remote do you have? maybe your remote is not binded to your receiver
```

---
## \#19 Posted by: Stefan Posted at: 2016-09-30T16:42:35.989Z Reads: 66

```
I got the standard remote that came with the magneto board. It is one of those chinese cloneboards. It should be binded because a led indicates the battery status. That's why i suppose that the transmitter should be okay.
```

---
## \#20 Posted by: Blasto Posted at: 2016-09-30T16:47:14.881Z Reads: 66

```
I think it's a steez remote... you can try this

http://www.electric-skateboard.builders/t/enertion-raptor-change-the-radio-channel-on-hand-controller-steeze/1314?u=blasto
```

---
## \#21 Posted by: Stefan Posted at: 2016-09-30T17:03:56.139Z Reads: 62

```
This does affect the remote. When i change the channel the remotes led does not indicate the battery status of the board. So the remote must have been on the right channel.
```

---
## \#22 Posted by: Blasto Posted at: 2016-09-30T17:06:55.920Z Reads: 61

```
ok, i am not familiar with the remote you are using... would you have a link to it online?
```

---
## \#23 Posted by: Stefan Posted at: 2016-09-30T17:08:53.937Z Reads: 62

```
It is this one:
https://magnetoelectricskateboard.com/products/magneto-bluetooth-controller?variant=6827418629
```

---
## \#24 Posted by: Blasto Posted at: 2016-09-30T17:15:01.026Z Reads: 59

```
that looks exactly like the steez remote... do you have a configuration manual or something? 
<img src="/uploads/db1493/original/3X/3/d/3d3d843a77a00864261df4f4d0defafbee0c476e.jpg" width="607" height="396">
```

---
## \#25 Posted by: Stefan Posted at: 2016-09-30T17:19:45.333Z Reads: 53

```
Yes, but it does not help. Only a few words on how to accelerate and what the leds mean...
```

---
## \#26 Posted by: Blasto Posted at: 2016-09-30T17:31:37.875Z Reads: 53

```
sorry man, i'm not familiar with steez type remotes neither, but there's info on the forum, like the link at the top
```

---
## \#27 Posted by: Stefan Posted at: 2016-09-30T17:41:39.099Z Reads: 53

```
Okay. But thanks a lot for your help.
```

---
## \#28 Posted by: PDXroses Posted at: 2017-05-13T19:50:29.634Z Reads: 34

```
Gents, I'm at my wits end with my remote.  I'm fairly new to this so it's probably me, not the remote.

1- Can I take a remote controller and receiver that's working fine on Board A and then plug it into the Board B and expect it to work?

I have an Alien Power Systems remote control (RF).  It's set on CH2 and was working great on my first skatebaord.

Really appreciate any help you can provide.
```

---

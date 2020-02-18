# Upgrading Chinese clone with Vesc

### Replies: 20 Views: 2517

## \#1 Posted by: aotr Posted at: 2016-09-15T14:24:17.316Z Reads: 190

```
Hi! 

I bought i Chinese clone board, and yes. It SUCKS! The acceleration is horrible and the breaking is even more horrible. Therefore i decided to buy i VESC to replace the current ESC which i expect is the main problem. A guy on youtube, Dr. Circuit did this apparently  with good results 

https://www.youtube.com/watch?v=So3g9zoAS7M

After receiving the VESC and opening the board i have a few things I am unclear of. I hope you guys can help me out! :slight_smile:

So here is my VESC and the ports i think i need to use. Also of cause the USB port for configure it. 

  <img src="/uploads/db1493/original/3X/5/a/5a9f8e1a971c27d1518111a55184807ed4b4d054.png" width="690" height="355">

And this is the internal of the board 
<img src="/uploads/db1493/original/3X/5/8/58dca66233e36a38125d8905b3169898e12baa75.png" width="425" height="500">

I would like to reuse the bms and the controller. Is it possible, just to replace the ESC with the VESC?

also. the VESC has three pins to connect to the receiver but the receiver has that white connector with many ports coming from the ESC. Also. There is two wires coming from the ESC, soldered to the receiver board. What about those?

<img src="/uploads/db1493/original/3X/4/6/468a59e073b333c8ca8ec4e83cf8520bef958868.png" width="690" height="448">

I hope someone has some thoughts on this :slight_smile:

Thanks!
```

---
## \#2 Posted by: DeathCookies Posted at: 2016-09-15T14:34:21.199Z Reads: 177

```
[quote="aotr, post:1, topic:9640"]
There is two wires coming from the ESC, soldered to the receiver board. What about those?
[/quote]

Are you sure that these two cables go to the receiver or do they go to the BMS and **then** to the receiver?
```

---
## \#3 Posted by: aotr Posted at: 2016-09-15T14:39:11.055Z Reads: 177

```
I i not sure. does this picture clear things up?
<img src="/uploads/db1493/original/3X/b/3/b3a4cadc1df4b262f4bcd4d3be7fce3b26d5b8ac.png" width="647" height="500">
```

---
## \#4 Posted by: chinzw Posted at: 2016-09-15T17:05:52.689Z Reads: 149

```
The two wires (red/black) im pretty sure its for the fan.

The other wires going to the ESC im guessing are the PPM and Hall Sensor.

It would be great if you can post more pictures of the wires, where the connect, etc.
```

---
## \#5 Posted by: aotr Posted at: 2016-09-15T20:07:50.275Z Reads: 137

```
Those wires being for the fan would make a lot of sense! If i would replace the ESC should i just cut those?

Here is some more pictures. Please let me know if other photos are needed:) 

<img src="/uploads/db1493/original/3X/0/2/027fab0b55403f39f291ed36de2af3acf8e0ea36.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/6/56db5dcd8265ae91dda5c094075f81bea026c00f.JPG" width="375" height="500">

<img src="/uploads/db1493/original/3X/5/8/5882b3dd7e2c3d0ce42fdfd0d636878409570c18.JPG" width="375" height="500">
```

---
## \#6 Posted by: chinzw Posted at: 2016-09-15T20:35:52.899Z Reads: 110

```
Ok, so from those pictures, i can asume the black and red are fan, the other 8 (cant really count them properly from the pictures) should be PPM(3 wires)+SENSOR(5 wires)
```

---
## \#7 Posted by: aotr Posted at: 2016-09-15T20:55:18.243Z Reads: 112

```
okay thank you! I have tried to take a better picture.

<img src="/uploads/db1493/original/3X/7/9/79273df74534fee557a33a08c9d74de33e08144d.JPG" width="375" height="500">

Would it be at all possible to use the VESC with that controller, and how would i go about connection it to the receiver board?
```

---
## \#8 Posted by: chinzw Posted at: 2016-09-15T20:58:26.263Z Reads: 107

```
Hmm, after seen the wiring again, i think you might be better off replacing the receiver too.
```

---
## \#9 Posted by: aotr Posted at: 2016-09-15T21:00:54.134Z Reads: 104

```
oh okay. as you may be able to see. The receiver is soldered to the BMS too. can you tell me why this is. And would i need to do something simular
```

---
## \#10 Posted by: chinzw Posted at: 2016-09-15T21:04:41.788Z Reads: 103

```
Hmm, probably some connection for the receiver to relay the battery status to the remote/esc
```

---
## \#11 Posted by: aotr Posted at: 2016-09-15T21:13:10.779Z Reads: 104

```
Okay. that makes sense too :) So, do you think i could just replace the receiver and add for example the  2.4GHz Nano Remote cutting the wires to the receiver board

thanks a lot for your help :)
```

---
## \#12 Posted by: aotr Posted at: 2016-09-15T21:19:05.189Z Reads: 103

```
And also. the white plug just in front of my index finger. is that just for powering the receiver board do you think? and can i just remove that? :) 

<img src="/uploads/db1493/original/3X/d/9/d9adef5f54460e698c26777f2876dcae587f339d.jpeg" width="355" height="500">
```

---
## \#13 Posted by: chinzw Posted at: 2016-09-15T21:20:18.803Z Reads: 96

```
Its hard to tell. I think you'll need to get a tester and start probing wires.
```

---
## \#14 Posted by: aotr Posted at: 2016-09-15T21:22:14.105Z Reads: 93

```
When you say a tester.do you mean a voltmeter?
```

---
## \#15 Posted by: chinzw Posted at: 2016-09-15T21:23:07.442Z Reads: 91

```
multimeter, one that at least has volt, resistance and continuity
```

---
## \#16 Posted by: aotr Posted at: 2016-09-15T21:24:38.575Z Reads: 90

```
okay. where would you measure to get inforation about that white connector? :slight_smile:
```

---
## \#17 Posted by: 2-alex-2 Posted at: 2016-09-15T21:27:56.756Z Reads: 93

```
Red and black wire could be the switch for the esc and its just been wired into the main switch so it all comes on at same time.
```

---
## \#18 Posted by: aotr Posted at: 2016-09-16T21:29:29.664Z Reads: 81

```
Thank you for Your replys! Anyone with other information? :)
```

---
## \#19 Posted by: aotr Posted at: 2016-09-17T08:32:32.874Z Reads: 72

```
Now I have ordered a remote and some xt60 connectors from alienpowersystems. Will try to update the topic when I recieve it :)
```

---
## \#20 Posted by: kameezy Posted at: 2017-05-23T15:49:54.030Z Reads: 32

```
How did the VESC upgrade go?  What clone board did you have?

I was thinking of doing the same thing to my Lectric Longboard (similar to Magneto/Luuov/LecDec/MelonBoard/Backfire)
```

---

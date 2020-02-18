# New TORQUE Hub motor street deck build

### Replies: 7 Views: 1112

## \#1 Posted by: Vort3x Posted at: 2017-05-24T16:52:36.302Z Reads: 199

```
Just got this hub motor kit from . Inspired by a build I saw and rode last year from @RunPlayBack I'm building it on a regular street deck.<img src="/uploads/db1493/original/3X/f/4/f4d7ac80f42e3b4b95b6bf99d587db4a2f1dfc53.jpg" width="690" height="388">
 
I was surprised to not see anyone else on here with this new kit in all black on 90mm wheels. I'm guessing that's because it's new and there are no pics on their site yet, Actually, this item stills says back order. I utilized the chat window to ask when they would be back in stock and was told they had them so I clicked that order button. Shipping was super fast from TX to MI. Ordered Fri, delivered Mon.<img src="/uploads/db1493/original/3X/1/d/1df8d5f3ff4a7834521ddf48489eb6efa08e6b8e.jpg" width="690" height="388">
<img src="/uploads/db1493/original/3X/1/6/167171e3352bd775315ccb3d33a4f37ceffc9ccc.jpg" width="690" height="388">
For batteries, I built two 5s3p 18650 packs and made a series connector for the vesc to combine them for 10s. I didn't want to use a BMS because I'm deep into RC and I have really good chargers that I can use for this. I can only go up to 6s on the charger though, so that's why I split them up. Still need to buy or build a proper enclosure and figure out the best way to access the connectors easily for charging. For now I just have the packs attached to the deck with some 3M dual lock and duct tape. <img src="/uploads/db1493/original/3X/4/a/4a0c4f7be86ffe229957e25f54f7dbd97398d1ec.jpg" width="690" height="388">

This was my first VESC / bldc setup so it was a bit of a struggle. I was having a hard time getting the VESC to connect. Turns out I needed to download a driver for windows 10. Next I was having difficulty getting the remote to respond. This ended up being a dumb mistake on my part. I had the servo plug connected to the wrong port on the receiver. It always ends up being something simple you take for granted that you overlooked. Once I got that sorted, I did a motor detection, rounded the values, wrote config, and rebooted.<img src="/uploads/db1493/original/3X/0/1/0172ae131d3d3a9275d49a1c6b1997d4b778d2de.jpg" width="690" height="388">

My inital current limits were 50, -50 for motor min and max. Took it out for a test and the motor was getting hot after about 5 minutes. I dropped the current limits down to 40-40, tested again and it was running much cooler. Just warm to the touch. So, then I was ready for the first real ride. Took it to a jogging track and put about a half mile on it, then stopped to check voltage and temperature. This is where the story goes downhill. Voltage was good. Temps were the same as before, just warm, but when I went to take off again the motor just stuttered and wouldn't go. I tried cycling the power. Same thing. Tried spinning the motor via bldc with the arrows - same thing. Tried a motor detection and it failed. Now the motor is just completely unresponsive.

I thought maybe the VESC was the issue, so I hooked up another motor to it, ran a detection, and it spooled right up. Just to be sure, I threw another motor on there, same thing, worked great. So, now I have to send it back for RMA which I hate doing. Hopefully they have  more hub motors in stock so I can buy another one while this one is being inspected and a determination is made.Best case scenario, they'll have another motor so I can get back to riding and they'll replace my original one and I'll upgrade this thing to duals.

Can anyone think of anything I may have done wrong? The setup is pretty simple and I don't think a 50 amp limit and riding conservatively for the first ride should burn up a motor. Especially since it ran for another half mile after dropping down to 40a. Really strange that it went from riding great to just not working anymore. It was a blast to ride by the way. I also have a e-mtb which overall I prefer, but that connected to the ground feeling of urethane wheels is very addicting.

Well, if you made it this far, thanks for reading. If you have any suggestions or tips let me know..

Thanks guys.<img src="/uploads/db1493/original/3X/5/8/5895f93db05c9a49b8cf994012914cd8072c1f37.jpg" width="690" height="388"><img src="/uploads/db1493/original/3X/b/0/b015b6ed2d2437a17d0e19e017f029708956fb09.jpg" width="690" height="388">
```

---
## \#2 Posted by: Davey Posted at: 2017-05-24T18:17:42.831Z Reads: 162

```
Looks nice! Are these the same motors they use on their rocket boards?
```

---
## \#3 Posted by: Vort3x Posted at: 2017-05-24T18:25:14.966Z Reads: 159

```
I don't own a rocket board, but from the pictures it looks exactly the same. Maybe @torqueboards can confirm.
```

---
## \#4 Posted by: Blix Posted at: 2017-05-24T21:58:45.395Z Reads: 128

```


2 quick questions :slight_smile: 
Is it the 130KV version?
Why do they even offer 75KV, any advantages?
```

---
## \#5 Posted by: JLabs Posted at: 2017-05-24T22:03:52.320Z Reads: 122

```
Higher kv = more speed, lower kv = more torque.

So if you want to climb hills (not saying the hubs can or can't do that) you want the lower kv. If you ride mostly flats and want speed you get the higher kv version.
```

---
## \#6 Posted by: Vort3x Posted at: 2017-05-24T22:26:34.393Z Reads: 110

```
This is 75kv
```

---
## \#8 Posted by: Vort3x Posted at: 2017-05-24T23:17:10.741Z Reads: 100

```
@Smorto Read towards the end of the post. I had to send the hub motor back because it stopped working.
```

---

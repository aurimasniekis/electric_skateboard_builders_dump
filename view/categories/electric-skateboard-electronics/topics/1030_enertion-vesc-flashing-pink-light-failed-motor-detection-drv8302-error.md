# Enertion vesc flashing pink light - failed motor detection DRV8302 error

### Replies: 31 Views: 5708

## \#1 Posted by: disastorm Posted at: 2016-01-17T20:13:28.144Z Reads: 252

```
Hello,

My first vesc ended up working fine, but with my second one when I powered it on I heard some kind of noise and it has a constantly flashing pink light. The BLDC tool can load and write data, but when trying to detect the motor it fails. Anyone know what the issue is?
```

---
## \#2 Posted by: chaka Posted at: 2016-01-17T20:16:28.760Z Reads: 257

```
Go to the terminal tab in your bldc tool and type "faults" without parenthesis after a failed detection and see what comes up.
```

---
## \#3 Posted by: disastorm Posted at: 2016-01-17T20:21:58.821Z Reads: 253

```
It said no faults registered since startup. Do you know what the pink blinking light means ?
```

---
## \#4 Posted by: disastorm Posted at: 2016-01-17T20:27:18.630Z Reads: 247

```
It felt a little hot so I checked the temperature realtime data tab and it looks like its running alot hotter than my other vesc.

My working one says the Mosfet Temperature is 24 degrees C shortly after turning it on.
My broken one has it at 44 degrees C shortly after turning it on.

Oh just noticed theres a fault code in the real time data charts.
It says: DRV8302

I just searched the forum for the error code and it sounds like I'll need to replace the chip? It looks like in one thread @onloop  mentioned the vesc is under warranty ( http://www.electric-skateboard.builders/t/vesc-blew-up-any-ideas-edit-solved/201/3 ) so can I send it back for a replacement? It happened as soon as I plugged it in the first time using the space cell.
```

---
## \#5 Posted by: cmatson Posted at: 2016-01-17T21:49:03.727Z Reads: 230

```
That was how my first VESC died.. (It was my thread that you linked) 

It turns out it died because I had done a crappy soldering job with a 10$ soldering iron..

Could we get some pics of your VESC?
```

---
## \#6 Posted by: disastorm Posted at: 2016-01-17T21:49:52.449Z Reads: 223

```
The only thing I soldered was the connector plugs for the motor, it was from the most recent vesc shipment so it came with the capacitors already on it as well. I'll get some pics
```

---
## \#7 Posted by: cmatson Posted at: 2016-01-17T21:50:43.537Z Reads: 220

```
ya, I figured it was from the new batch.

Still, I know someone else on here had a problem with a crappy soldering job that was from a pre-soldered batch.
```

---
## \#8 Posted by: disastorm Posted at: 2016-01-17T21:58:29.856Z Reads: 226

```
The plastic wrap and the residue from removing the Enertion Sticker makes the photo a bit hard to see, but here are some photos. If its really important I can try to clean the residue or just remove the wrapping itself for better pics.

<img src="/uploads/db1493/original/2X/4/42a08524ba6e7114dfb4c3d94b135a856cf17ce4.jpg" width="375" height="500"><img src="/uploads/db1493/original/2X/2/243c36854df16803213acf3ad0317985ac6922c9.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/6/6528c10d0edae22157655e5250c7205c7b518fa7.jpg" width="375" height="500">
<img src="/uploads/db1493/original/2X/2/2b6a5c008adbfe736c143217391147a69dcd58e6.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/e/e20424d59133f3c633f410e2eab79c94f2fcca25.jpg" width="666" height="500"><img src="/uploads/db1493/original/2X/b/bc3ab2aca30a8163a44725d94c699ad08076bfe9.jpg" width="666" height="500">
```

---
## \#9 Posted by: trbt555 Posted at: 2016-01-18T06:05:56.105Z Reads: 204

```
Dead on arrival. Warranty.
```

---
## \#10 Posted by: disastorm Posted at: 2016-01-18T10:23:20.232Z Reads: 202

```
@onloop @EnertionSupport Should I go ahead and Submit a return via the enertionboards.com Account Dashboard ?
```

---
## \#11 Posted by: EnertionSupport Posted at: 2016-01-18T15:43:56.307Z Reads: 201

```
Yes, please do. 

Link this thread in your RA request so we know which one is yours. It will also show that we've already troubleshooted your VESC on this thread.
```

---
## \#12 Posted by: disastorm Posted at: 2016-01-18T19:43:38.906Z Reads: 200

```
Ok, submitted. Thanks.
```

---
## \#13 Posted by: disastorm Posted at: 2016-01-25T09:13:00.126Z Reads: 190

```
@EnertionSupport Is there anything I have to do afterwards ? It looks like the return is "pending". Do I need to wait for some kind of validation, and then send you guys the VESC back ?
```

---
## \#14 Posted by: disastorm Posted at: 2016-01-25T18:20:18.094Z Reads: 189

```
@EnertionSupport Nevermind, just got the authorization email. Should I remove the soldered female connectors from the wires before sending back or can I just keep those on ?
```

---
## \#15 Posted by: EnertionSupport Posted at: 2016-01-26T01:33:41.596Z Reads: 183

```
You can keep your bullet connectors, and just send us the VESC.
```

---
## \#16 Posted by: Flo Posted at: 2016-01-30T13:21:00.621Z Reads: 183

```
I have the exactly same problem. I have a 4.7 VESC from Enertion Boards. I just came home from my studies abroad and was really excited to start with my new vesc. At first my vesc is stuck to FW 1.10. Seems I have to flash the bootloader. Already ordered a stlinkv2 to do that. Then I read data from the vesc and putted the sk3 168kv data on it. After reboot I wanted to start it. After one turn it stopped working, flashes red, gives back a DRV8302 failure and the Mosfet temp is around 40 Degrees. Hope that is covered by warranty and I can send it back? You'd like to see photos of the VESC for that? As mentioned on the VESC Blog i checked for R16. But R16 is not installed so that can't be the problem.
```

---
## \#17 Posted by: EnertionSupport Posted at: 2016-01-30T23:09:55.277Z Reads: 181

```
Hi Flo, All owners of Enertion VESC that want to submit an RA must create their own NEW thread with detailed information about the specific problems they are facing before an RA will be considered/approved. We ask for this because there have been several VESC returns that have been clearly damaged due to user error or have no faults at all. Also, there is a 60-day warranty on Enertion Electronics so please check the date of purchase.

Please read this 
http://www.electric-skateboard.builders/t/vesc-faq-my-vesc-doesnt-work-help-qiqo/672
```

---
## \#18 Posted by: Flo Posted at: 2016-01-31T01:22:37.822Z Reads: 175

```
I just started a new Thread:
http://www.electric-skateboard.builders/t/vesc-red-blinking-no-firmware-update-possible-no-motor-turn/1177
please let me know which additional information would be helpful :)
```

---
## \#19 Posted by: disastorm Posted at: 2016-02-01T05:58:25.355Z Reads: 162

```
Sorry I've been a little delayed. I'll be shipping my package back this week. Thanks.
```

---
## \#20 Posted by: disastorm Posted at: 2016-02-02T00:20:20.849Z Reads: 155

```
@EnertionSupport  Just shipped it today, but it is via Registered Airmail so it will take around 3-4 weeks to arrive back to you. It will also require a signature on delivery. I included my authorized return # in there as well. I hope that is suitable. Thanks.
```

---
## \#21 Posted by: disastorm Posted at: 2016-02-19T08:53:46.242Z Reads: 136

```
@EnertionSupport Looks like it still hasn't reached you guys yet, although its apparently in Australia now. Just wondering what will happen after it reaches you? I will get some kind of store credit or something, and then I need to re-order the vesc? Does this mean it will be the April batch one ( or whatever the current batch is at the time of ordering ) ?
```

---
## \#22 Posted by: EnertionSupport Posted at: 2016-02-19T12:22:12.846Z Reads: 133

```
Yes, we will look into what might have caused your VESC to fail, and then credit you pack if that looks to be the best solution.
```

---
## \#23 Posted by: disastorm Posted at: 2016-03-02T22:21:46.195Z Reads: 128

```
@EnertionSupport I don't know why its taking so long as their hasn't been an update on the tracking in weeks ( when I checked last night ). Do you know if you guys got it and the tracking just didn't update. Or is it possible its stuck in customs or something like that?
I don't have the tracking number with me atm but I"ll post it in here later. My return number is #25.
Thanks.
```

---
## \#24 Posted by: EnertionSupport Posted at: 2016-03-03T01:40:57.362Z Reads: 123

```
We will take a look at it- sometimes shipping it all the way down here can just take a while.. 

If you want to DM us the tracking number that'd help too.
```

---
## \#25 Posted by: disastorm Posted at: 2016-03-03T03:49:56.607Z Reads: 120

```
@EnertionSupport Here is the tracking.. it got to Australia almost a month ago and no updates since.
https://tools.usps.com/go/TrackConfirmAction?tLabels=RE575146555US
```

---
## \#26 Posted by: disastorm Posted at: 2016-03-07T05:02:19.560Z Reads: 116

```
@EnertionSupport Have you been able to check and see if you got it and maybe the tracking just never got updated? If not maybe I can email the postal service about it.
```

---
## \#27 Posted by: onloop Posted at: 2016-03-07T05:48:13.765Z Reads: 116

```
I have not got it, what was the original order number?
```

---
## \#28 Posted by: disastorm Posted at: 2016-03-07T06:32:07.804Z Reads: 116

```
@onloop The original order was order #1182 and the Return order is return #25  
I really have no idea whats up with the mail transit. Could it be stuck in customs or something ? I suppose it could just be really slow but I heard it usually doesn't take longer than 3 weeks or so.
```

---
## \#29 Posted by: disastorm Posted at: 2016-03-22T06:42:47.363Z Reads: 106

```
@onloop I submitted a request to usps customer service to see if they can give me any info on the package. Not sure if they will though since its in Australia with no updates.
```

---
## \#30 Posted by: onloop Posted at: 2016-03-22T12:29:33.757Z Reads: 110

```
Hey bro, not sure what's going on, probably got lost... Man i'll give you the benefit of the doubt and have issued a store credit! happy easter.
```

---
## \#31 Posted by: disastorm Posted at: 2016-03-22T19:06:43.713Z Reads: 105

```
@onloop Wow thanks man, I appreciate it. Hopefully it turns up in the future. Happy Easter to you too!
While I was waiting for this whole process, I had ended up ordering a Vesc from another place. I can probably order another from Enertion as a backup, but I noticed you have a wireless controller so I might get that.
Thanks again!
```

---

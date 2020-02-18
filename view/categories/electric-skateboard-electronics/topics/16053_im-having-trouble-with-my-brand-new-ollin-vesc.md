# I&rsquo;m having trouble with my BRAND NEW OLLIN VESC!

### Replies: 35 Views: 2391

## \#1 Posted by: Smorto Posted at: 2017-01-13T20:57:31.399Z Reads: 187

```
HELP! I just received my @chaka VESC about a week ago and it is not functioning properly. I hooked it up to a 4s 5000mah 20c Zippy LiPo and my motor, and set it up according to the Esk8 Support VESC tutorials. As soon I was done programming however and did a bench test, the VESC no longer connected to my laptop or the BLDC Tool. I tried all different USB ports, as well as deleted and re-installed the tool to no avail. I thought to myself that this was fine because it still functioned just without that capability. I jury rigged everything to my board for a first ride in the basement which was awesome. I duct taped everything on and it worked wonderfully. Today though, when I was going to do the same thing again, the VESC refused to even function as it had just two days ago when it was attached to my 8s battery of two 4s batteries in series. Instead, it gives me the blue light but instead of three flashing red lights then a solid blue, it just blinks red. I believe this indicates an error which sucks as I had't done anything to induce it! The weird thing is though, when I connect it to just one of the 4s batteries it functions perfectly... It still does not connect to the BLDC tool though so I can't search for faults in the terminal :cry:. I made a video of my problem [Here](https://youtu.be/8IsZD1xozzI). Any help would greatly be appreciated because I am pretty upset that this is happening as I haven't done anything to make this happen as far as I know.
```

---
## \#2 Posted by: Blasto Posted at: 2017-01-13T21:13:26.892Z Reads: 181

```
Set your max voltage to 57V

Sorry i didnt read (tldr) just watched the video
```

---
## \#3 Posted by: Smorto Posted at: 2017-01-13T21:14:17.845Z Reads: 178

```
I believe it is set to 57...
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2017-01-13T21:14:50.179Z Reads: 173

```
please post screen shoot of your setting...
```

---
## \#5 Posted by: Smorto Posted at: 2017-01-13T21:15:31.170Z Reads: 170

```
I can't because my VESC can't connect to the bldc tool. Did you read the post? :confused:
```

---
## \#6 Posted by: Blasto Posted at: 2017-01-13T21:27:29.130Z Reads: 165

```
Really strange that you connected once to the bldc tool and it doesn't work anymore. Are you able to inspect the usb port for any broken pads or physical damage?
```

---
## \#7 Posted by: JohnnyMeduse Posted at: 2017-01-13T21:28:11.013Z Reads: 165

```
did you try to connect it with only the 4s...
```

---
## \#8 Posted by: Smorto Posted at: 2017-01-13T21:32:32.269Z Reads: 164

```
Yes, that did't work either. 
This is without the VESC connected but it is the exact same screen as when it is connected. It never switched to "USB modem 301" or whatever it is supposed to say, it just stays as bluetooth etc.
<img src="/uploads/db1493/original/3X/f/4/f438b1c89dee4583d5cea435c7277f053a1017a4.png" width="690" height="376">
```

---
## \#9 Posted by: Smorto Posted at: 2017-01-13T21:34:25.083Z Reads: 160

```
That's the weird thing... the entire VESC looks in perfect condition. I would really like to hear @chaka's opinion on this issue as it is his product.
```

---
## \#10 Posted by: JohnnyMeduse Posted at: 2017-01-13T21:38:46.898Z Reads: 153

```
there is no value on this one.... better contact Ollin Co. ( best way is probably their web site)
```

---
## \#11 Posted by: Smorto Posted at: 2017-01-13T21:44:44.260Z Reads: 145

```
I just sent a message on their contact page.
```

---
## \#12 Posted by: chaka Posted at: 2017-01-13T23:05:05.256Z Reads: 140

```
It sounds like you set your voltages to improper values. If you leave the vesc connected to a power source that is in conflict with the set values you can corrupt the firmware. Send it in and we can reflash it and get you rolling. Might also be best to use this downtime to build an enclosure too. :grin:
```

---
## \#13 Posted by: Ackmaniac Posted at: 2017-01-13T23:09:14.510Z Reads: 135

```
I think as long as the motor runs with 4S it should be possible to get a connection with the PC.
```

---
## \#14 Posted by: Smorto Posted at: 2017-01-13T23:17:35.057Z Reads: 135

```
Hah!  I agree about the enclosure. I have been speaking to one of your customer service people about this same issue and they were saying pretty much the same thing. However, I still am failing to see why the USB port is no longer functioning??
```

---
## \#15 Posted by: Smorto Posted at: 2017-01-13T23:19:31.961Z Reads: 130

```
I would agree but for some reason it doesn't want to connect, even when I try using the 4s battery to connect to the PC.
```

---
## \#16 Posted by: chaka Posted at: 2017-01-13T23:29:23.014Z Reads: 130

```
If the firmware has been corrupted it will not connect to the bldc tool. That slow spool-up in the video is also telling me something is wrong with your settings. It should spin up to max rpm much faster than that.
```

---
## \#17 Posted by: Smorto Posted at: 2017-01-13T23:39:57.205Z Reads: 129

```
Ok, the customer service person I am talking to from your company says that I just need to send it in and you guys will re-flash the firmware free of charge which is awesome. Is there anyway you could set it up for me to avoid any other future problems? I know I am asking a lot but I don't want to mess it up again. I would give you my motor and battery specs of course if you decided you could do that for me.
```

---
## \#18 Posted by: chaka Posted at: 2017-01-13T23:55:41.476Z Reads: 124

```
We can run through the setup process once you get it back. Send us an email with your contact info when you are ready and I will help you out. It is best if you can tune the VESC yourself.
```

---
## \#19 Posted by: Smorto Posted at: 2017-01-14T00:03:49.633Z Reads: 124

```
Sweet, I will try to get it out to you Monday since I don't have school! So I would just send a message on your contact page saying my e-mail and name and what else would you need?
```

---
## \#20 Posted by: chaka Posted at: 2017-01-14T00:07:30.293Z Reads: 125

```
We can run through motor detection over the phone. Shouldn't take more than a few minutes.
```

---
## \#21 Posted by: Smorto Posted at: 2017-01-14T00:21:46.477Z Reads: 116

```
Ok, that sounds good
```

---
## \#22 Posted by: Smorto Posted at: 2017-01-14T01:49:13.074Z Reads: 110

```
Ok, something weird is defiantly happening with my VESC. I just soldered on an anti-spark switch and a voltage meter to my circuit and now when I plug that in the VESC flashes red three times and then stops, as it is supposed to. Then I can accelerate to full throttle as it should. However, now there are no brakes, pushing up on my trigger now does nothing. This makes it even more confusing and I hope it is still just a firmware issue. When I go to brake, the red LED flashes once again.
```

---
## \#23 Posted by: chaka Posted at: 2017-01-14T01:59:13.879Z Reads: 106

```
We will take care of it either way.  No way of knowing what the initial cause was now since it looks like you may have fried the drv by running it without getting the settings sorted. Take your time with your build, it seems like you are rushing through it. I don't mean any offense but you will have a much better experience if you hold off riding your board until you get everything tucked away and secured.
```

---
## \#24 Posted by: Smorto Posted at: 2017-01-14T02:05:45.074Z Reads: 106

```
Ok, this test ride was just a proof of concept/test ride but I understand what you are saying. I do have trust that you will work your magic and fix my VESC. :slight_smile:
```

---
## \#25 Posted by: chaka Posted at: 2017-01-14T02:12:39.254Z Reads: 104

```
Can you give me a list of what you remember changing in the bldc-tool? Low voltage cutoff values, bldc or foc mode, ppm settings. Anything you can remember. It will help us find out what happened so we can make sure it doesn't happen again.
```

---
## \#26 Posted by: Smorto Posted at: 2017-01-14T02:40:15.115Z Reads: 109

```
Ok, I might not be exactly right but here are what I believe I set each setting to
Motor Max-30.00 A
Motor Min (regen)-(-20.00  A)
Batt Max-20.00 A
Batt Min (regen)- (-5.0 A)
Absolute Max-130.00 A
The temperature limits I left the same
I am running an 8s setup so that is what I set my voltage limits to
**Maximum input voltage-33.6 V**-Maybe this is where I went wrong, this is supposed to be set to 57?
Battery cutoff start- 26.4 V
Battery cutoff end-24 V
Min ERPM-(-100000.00)
**Max ERPM-60000**-This could be wrong as well
As for the motor detection, all I did was run it, click apply, then clicked write configuration.
For my startup boost, I believe I put 0.045 or 0.040 I can't remember which
For the remote settings, I chose PPM and Current no reverse with brake
I believe that is all I set. It is my guess that the Maximum input voltage is where I went wrong though I don't know very much about this.
```

---
## \#27 Posted by: chaka Posted at: 2017-01-14T16:09:03.924Z Reads: 98

```
Who told you to adjust the max voltage value? That is where your trouble started. You then dropped down to 4s which triggered the low voltage limp mode which likely corrupted the firmware. 

Probably just needs to be flashed again but I will stress test on our equipment to be sure there is no issue with your drv.
```

---
## \#28 Posted by: Smorto Posted at: 2017-01-14T16:27:04.615Z Reads: 98

```
Sweet thanks! I just dropped it off at the post office, estimated delivery is Tuesday but I doubt that because Monday is a holiday. You should know it is my package because it is from Sam Morton with my address, and I also taped a little note saying that it is the VESC that needs to be flashed to the packing around the VESC. When you receive it if you can just post something on here to let me know that it made it there safely that would be great.
```

---
## \#29 Posted by: Smorto Posted at: 2017-01-15T21:41:47.832Z Reads: 95

```
While I wait for my VESC, I'm taking your advice @chaka and making an enclosure :slight_smile:.<img src="/uploads/db1493/original/3X/d/b/db0b917d8834d80f60690c1518e98d5742e67de3.jpg" width="690" height="459">
```

---
## \#30 Posted by: Smorto Posted at: 2017-01-18T12:21:57.990Z Reads: 87

```
Ok, so according to tracking it is believed to your PO box. Just checking in to see if you have received it.
```

---
## \#31 Posted by: chaka Posted at: 2017-01-19T18:47:39.506Z Reads: 82

```
Hi Sam,

We have Melissa working full time again answering emails. Be sure to inquire vie email in the future for more prompt service.

I checked our incoming mail and did see your package, we will run it through testing and give you a prognosis later today.
```

---
## \#32 Posted by: Smorto Posted at: 2017-01-19T19:43:34.165Z Reads: 80

```
Awesome thanks. When you say e-mail do you mean the contact page on your site or the e-mail address itself?
```

---
## \#33 Posted by: chaka Posted at: 2017-01-19T19:45:40.926Z Reads: 81

```
jclark@ollinboardcompany.com  

Website contact form also works if you don't have an ongoing email with us.
```

---
## \#34 Posted by: Smorto Posted at: 2017-01-19T19:47:08.809Z Reads: 81

```
I do have an e-mail chain from your contact page but it was neuctitlan@gmail.com. Would you recommend I use that or the one you mentioned?
```

---
## \#35 Posted by: chaka Posted at: 2017-01-20T15:10:50.834Z Reads: 74

```
Whatever is easiest for you, the main point is it gets checked much more than we check this forum. ;)
```

---

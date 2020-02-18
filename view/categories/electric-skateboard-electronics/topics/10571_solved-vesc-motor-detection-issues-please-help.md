# (SOLVED) VESC Motor Detection Issues - Please help!

### Replies: 11 Views: 4625

## \#1 Posted by: backinblack626 Posted at: 2016-10-03T16:15:44.347Z Reads: 442

```
So a quick background. This is VESC number 2 Brand New from . First one burned up the DRV after a handful of rides, so I just got another one while waiting for the first to have the DRV repaired.

I built my board with the following components:
 -6364 SK3 Turnigy 245kv Motor
 -6s 8000mah nano tech lipo battery pack
 -ec5 connectors
 -high amp on off switch
 -brand new VESC firmware 4.18 from 

So earlier today I tried reading the configuration on the VESC. It read it and I changed my voltage settings for the battery I was using. I tried to do motor detection, but it just wont detect and I cannot figure out why. I talked to Dexter from  earlier and we went through the settings which seemed just fine for voltage and amperage. Nothing else really changed except he told me to go into Motor Config > Advanced > Max Current Ramp Step to .04 instead of .4. Every time I wrote this config and read it, it would immediately change this value back to .4 no matter how many times I wrote it. So Dexter recommended I reload the latest firmware. I did that successfully, and got the Max Curent Ramp Step to stay at .04, but I still cannot get it to detect my motor. I know it reacts this way when some of the settings are out of range but everything looks healthy? This is my second VESC and the first fried my DRV chip after less than 1 full discharge on my battery so id really like this one to work properly. I am in the hole around $1000 since the beginning of this project and have not been able to ride my board for more than an hour or two total. I have been through countless tutorials and FAQs but cant find a lot of information on bad motor detection or where to start looking for issues.

So when I go to detect motor, it spins, but not smoothly and makes a lot of noise. Then one more short burst of unsmooth movement before it shows me in the bottom right in red the message "Bad Detection Results Received". It can measure R and L under the FOC tab, but when you go to measure the flux linkage it says the same message. No fault codes what so ever. Connects and reads firmware fine every time. My arrows can control my motor but, again, its choppy back and forth movement obviously not working properly.

What am I missing? I will literally PAY someone who is very familiar with the BLDC tool to sit and speak with me on the phone and just answer some general questions since this is the only area of this build that I seem to lack knowledge in. I have spent countless hours trying to get help, watching tutorials and guides, reading forums etc. and I cant seem to figure this one out. I have taken a video that shows exactly what its doing, as well.

[Motor Detection Problem Video](https://www.youtube.com/watch?v=Ng3kdIk48u8)
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-03T17:17:29.126Z Reads: 393

```
That looks exactly like batt min cutoff, maybe you forgot to write and reboot after changing those?
```

---
## \#3 Posted by: backinblack626 Posted at: 2016-10-03T18:02:19.800Z Reads: 390

```
That's exactly what I said! So I disconnected, reconnected, then read config and it still has all values set, so it's definitely written because it reads it and changes it. Weird rigth?!
```

---
## \#4 Posted by: sl33py Posted at: 2016-10-03T19:44:50.283Z Reads: 377

```
@backinblack626 - hey man.  Watched your video and definitely looks a bit odd.

A couple things from old VESC troubleshooting...  Have you tried swapping the USB cable to shorter (in video it looks somewhat long)?  I would also try to avoid crossing any/all power cables in case EMF/noise is causing an issue.

I'd also try changing the current from 6a to maybe 8a and re-try?  I'd first try the USB and clearing any/all power cables between the VESC and your computer.  A quick test and see if it helps.

Hope it's a simple fix, GL!
```

---
## \#5 Posted by: backinblack626 Posted at: 2016-10-04T13:08:26.450Z Reads: 343

```
I will try everything you recommended as soon as I get this pile of fluids and strength in materials homework done! Will update later today. 

If all else fails, I'll send my vesc and motor back to  to see if Dexter can figure out. 

Thanks for the help guys! Much appreciated!
```

---
## \#6 Posted by: Namasaki Posted at: 2016-10-04T23:09:31.633Z Reads: 314

```
Maybe when you loaded default configuration some setting on another page is off.
I never had a problem using a usb extension cable with mine.
You might try re-flashing the firmware and starting over.
```

---
## \#7 Posted by: backinblack626 Posted at: 2016-10-04T23:23:48.496Z Reads: 302

```
Haven't had time to mess with it today, but I have also tried reloading firmware and starting over =(
```

---
## \#8 Posted by: torqueboards Posted at: 2016-10-05T02:22:36.950Z Reads: 291

```
- USB 2.0.
- Make sure it's the correct COM port.

Only settings, you typically need to change.
- Battery cut off voltages
- Verify max voltage is at 57V
- Motor Detection
- Double check your Amp limits are correct for your setup.

Every VESC is tested multiple times. We make sure not to send any VESCs that haven't been tested. It's a ton of work on our end too but it has to be tested.

Are you trying to use FOC or just setting up for BLDC?

Let us know.
```

---
## \#9 Posted by: backinblack626 Posted at: 2016-10-06T19:24:48.501Z Reads: 279

```
Please watch the attached video. I just received the VESC and when I tried to program, I did exactly what you said. I set voltages and amperages where they need to be and went to detect my motor and it just says "Bad Motor Detection Results". The original post has a detailed description of the problem, as well. I received an email back from you guys on Tuesday saying that I could get an RMA # to send my VESCs back with my motor to see if you guys can figure it out. I purchased the warranty for one of them too.

Like I said, its not the DRV because it responds to the arrow keys, just not linear and not smooth and won't detect. Im not saying its a problem on your guys end by any means. I just have no where else to turn for support except the forums or the original vendor and at this point I am at a loss... and I just want to ride before it gets cold out :cry:
```

---
## \#10 Posted by: backinblack626 Posted at: 2016-10-07T16:16:31.990Z Reads: 259

```
FIGURED IT OUT!!! PROBLEM SOLVED! So when I extended the leads to my motor, there must have been a solder/flux bridge causing a really high resistance in 1 out of the 3 phase wires. It was weird because when tested the first time, after motor was originally modified, it had continuity, so I think it was my fault for a poor solder connection on my motor. Now BOTH VESCs detect my motor beautifully and everything works as it should! :heart_eyes:

I want to start by saying thanks to TorqueBoards and Dexter who held my hand through this headache even though it was not their product that had any issue, it was my hardware. I think I bothered him just about every day and he never tried to get rid of me, just helped. Just glad the issue is solved!

If anyone ever has a motor detection issue with message "Bad Motor Detection Results Received" with no fault codes and unsmooth jittery motor operation that is able to be controlled with your keyboard keys, then you most likely have a problem inside the motor or in the phase wires coming off the motor, like I did. Use a digital multi meter to test resistance between each combo of the 3 leads to see continuity between them. The numbers should be very low (about .1ohm). If you see numbers in kOhm or MOhm you know immediately there is a huge resistance and probably the cause of your motor detection problems.
```

---
## \#11 Posted by: epss4 Posted at: 2017-08-11T20:12:48.479Z Reads: 169

```
hi , i have exacly the same problem , i have a 6s 5000 mah 20c lipo battery  with 260 kv 6355 motor and vesc from  , i dont have any extender for my motor ..... i tried everithing , do you suggest me something , you are my last hope @backinblack626
```

---

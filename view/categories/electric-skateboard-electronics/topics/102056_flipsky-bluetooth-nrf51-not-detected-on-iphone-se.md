# Flipsky Bluetooth (nrf51) not detected on Iphone SE

### Replies: 29 Views: 239

## \#1 Posted by: PaleRider Posted at: 2019-09-21T16:28:24.106Z Reads: 47

```
Hi,
I've tried to connect my Iphone on the BT module, but my phone doesn't detect it.
I've activate the PPM+UART mode and set it to 9600 bauds in vesc-tool.

Is there something else I should do?
Thank you.
```

---
## \#2 Posted by: Stan8 Posted at: 2019-09-21T16:53:51.218Z Reads: 45

```
Are you using an app to connect to it? I use xmatic with my iphone and it works with no problem.
```

---
## \#3 Posted by: PaleRider Posted at: 2019-09-21T18:26:15.676Z Reads: 40

```
Before buying an app, first I wanted to try to connect directly on the phone, as some says the Flipsky module works with Iphone and some says it's not.

Can you detect the module in your Iphone BT setting too, or just with the app?
```

---
## \#4 Posted by: pundahh Posted at: 2019-09-21T18:30:11.825Z Reads: 33

```
It only shows up on the bluetooth screen after I connect it through an app. 

Your baud-rate should also be at 115200.
```

---
## \#5 Posted by: PaleRider Posted at: 2019-09-21T18:31:06.062Z Reads: 34

```
OK.
I read it was supposed to be st at 9600...
```

---
## \#6 Posted by: pundahh Posted at: 2019-09-21T18:32:05.775Z Reads: 34

```
9600 is for hm-10 modules
```

---
## \#7 Posted by: PaleRider Posted at: 2019-09-21T18:34:00.361Z Reads: 34

```
All right. Thanks.
Is there another app ( free) I could try to be sure my module is working with my Iphone?
```

---
## \#8 Posted by: pundahh Posted at: 2019-09-21T18:38:26.353Z Reads: 34

```
Not that I know of. If you have an android you could check. 

I'd just buy the app. Its only a few bucks and you have a bluetooth module already, and you need the app to read telemetry anyways :stuck_out_tongue:
```

---
## \#9 Posted by: PaleRider Posted at: 2019-09-21T18:39:57.699Z Reads: 32

```
I have planned to buy this app, but I don't think my firmware is compatible yet (3.61).
```

---
## \#10 Posted by: pundahh Posted at: 2019-09-21T19:01:42.545Z Reads: 31

```
downgrade to an older firmware :)
```

---
## \#11 Posted by: Stan8 Posted at: 2019-09-21T19:19:05.109Z Reads: 30

```
There are a lot of Bluetooth module which are undetectable by your phone directly but can through an app.
```

---
## \#12 Posted by: PaleRider Posted at: 2019-09-21T19:21:49.203Z Reads: 28

```
No way!
It tooks me 2 years to finaly decide to install my vescs on my board, don't ask me to touch it again :grinning:
(and furtheremore, I see I need to upgrade my IOS too to install it)
```

---
## \#13 Posted by: Ben.Nexus Posted at: 2019-09-21T19:46:11.226Z Reads: 29

```
Just also gonna throw this out here 
![image|635x500](upload://6GYmgHiIyDkI8vslhgAUIo0b67t.jpeg)
```

---
## \#14 Posted by: PaleRider Posted at: 2019-09-21T19:48:38.573Z Reads: 29

```
Yes, but some people managed to make it work anyway.
Someone left a message on their website on the BT page.
That's why I bought it despite they says it won't work on Iphone.
```

---
## \#15 Posted by: PaleRider Posted at: 2019-09-21T20:04:44.566Z Reads: 29

```
Well,
I just bought this:
https://www.electric-skateboard.builders/t/new-version-2-1-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340

It's working!
```

---
## \#16 Posted by: pundahh Posted at: 2019-09-21T20:09:20.394Z Reads: 25

```
The module does work for iphones. I believe "can only support android mobile device" on flipsky's website refers to the vesc-tool app.
```

---
## \#17 Posted by: pundahh Posted at: 2019-09-21T20:09:55.260Z Reads: 25

```
yay! unfortunately the data map website is no longer active so that feature is out :frowning:
```

---
## \#18 Posted by: PaleRider Posted at: 2019-09-21T22:18:25.098Z Reads: 24

```
... and I just tried to change values of the VESC within the app and it fucked-up my setting.

At least I know my bluetooth module is working :wink:
```

---
## \#19 Posted by: pundahh Posted at: 2019-09-21T22:32:59.982Z Reads: 24

```
[quote="PaleRider, post:18, topic:102056"]
it fucked-up my setting.
[/quote]

what do you mean by this?
```

---
## \#20 Posted by: PaleRider Posted at: 2019-09-21T23:04:29.054Z Reads: 23

```
I mean: one of the vesc didn't work anymore after the upload, so I had to reconfigurate it in vesc-tool and still I'm having a minor issue.

What happened is, when I opened the app, it shows me a wrong value in motor max:
![IMG_9288|282x500](upload://9Mb03mR09Cl8NS64LQwrYP0I9DW.jpeg) 

I entered a correct value "35" (and corrected the wrong battery number too ) and "upload" and then the front motor wouldn't work anymore.
I reconfigured it in vesc-tool, and the app still shows me the curious number.

But now the front engine is having an issue when full throttle unloaded (not launching but hesitate to go).
I don't know if it is linked but I didn't have this issue before playing with this app.
I hope the vesc is OK... Still launching perfectly when I'm on it, so.
```

---
## \#21 Posted by: emmaanuel Posted at: 2019-10-14T22:59:25.423Z Reads: 14

```
Hi @PaleRider, I've just fix this bug in the app.
You need to remove the app from your iPhone and install it again. let me know if you have problem.
```

---
## \#22 Posted by: PaleRider Posted at: 2019-10-14T23:20:29.710Z Reads: 13

```
Thanks 
Im gonna check this tomorrow.

By the way, I'm having another issue with your app.
I don't have any GPS speed (only speed from VESC with gear ratio and wheel size)
```

---
## \#23 Posted by: emmaanuel Posted at: 2019-10-15T18:01:03.417Z Reads: 11

```
Did you allow the app to get your position "always" ? It's necessary to calculate your speed when your phone is in your pocket.
```

---
## \#24 Posted by: PaleRider Posted at: 2019-10-15T18:16:39.447Z Reads: 12

```
Yes.
It asked me that and I allowed it, but GPS doesn't work within the app.
And today, I deleted the app and downloaded the new version.
It's stuck on " getting configuration".
so it doesn't work anymore :neutral_face:
```

---
## \#25 Posted by: emmaanuel Posted at: 2019-10-15T19:02:52.128Z Reads: 11

```
Can you send me the debug log ?
```

---
## \#26 Posted by: PaleRider Posted at: 2019-10-15T21:15:57.147Z Reads: 10

```
I was ready to do it, but while I was looking on the debug text I noticed the problem:
"Can forward" was ON in the app.
I turned it off, and it's working now.

Values of the VESC are now correct too.
Good job :sunglasses:
```

---
## \#27 Posted by: emmaanuel Posted at: 2019-10-15T21:20:05.331Z Reads: 10

```
Ok. great news !
I missed a change in the VESC protocol. 
Happy to see everything is ok now.
```

---
## \#28 Posted by: PaleRider Posted at: 2019-10-16T00:10:55.133Z Reads: 9

```
[quote="emmaanuel, post:27, topic:102056"]
Happy to see everything is ok now.
[/quote]

Sorry, I meant the app is working again (communicate with vesc), you fixed the bug about the wrong values, but I don't think the GPS is working.
I'll test it the next dry day and let you know.
```

---
## \#29 Posted by: emmaanuel Posted at: 2019-10-16T16:44:47.775Z Reads: 9

```
Ok, let me know.
If you still have gps problem, send me the debug logs.
```

---

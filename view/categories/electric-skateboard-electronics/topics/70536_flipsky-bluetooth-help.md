# Flipsky Bluetooth help

### Replies: 18 Views: 1217

## \#1 Posted by: Pmac Posted at: 2018-10-08T10:30:13.704Z Reads: 224

```
Hi everyone,

I need some help with using the flipsky Bluetooth module.  I have it plugged into the Flipsky 4.2 dual ESC.

It refuses to pair with my phone and keeps giving me an error when I try.

I am unable to get it to work with the ackmaniac app.  It just won't connect.  it says it has connected but nothing happens on the app.

Due to this I tried using the standard VESC Tool and loaded the firmware to the FSESC and I can connect to the VESC Tool Android Mobile app through Bluetooth (still unable to pair the Bluetooth).  But I am unable to connect to the Bluetooth from the windows VESC Tool as windows says it has paired but the module does not appear when trying to connect through the app.

Am i doing something wrong or is the Bluetooth module from flipsky extremely limited with what it can connect to?

I really want to use the Ackmaniac app as I want to use the features of being able to switch between different configs for when newbies are trying out the board as I have friends with a terrible sense of balance who want to try it out.  It seems the VESC Tool for mobile doesn't have those features yet.

Appreciate anyones help with what they think I should do.

Cheers,
Patrick
```

---
## \#2 Posted by: chrischo1996 Posted at: 2018-10-08T13:06:10.006Z Reads: 203

```
I'm facing the same problems, as far as I know it won't connect to the ackmaniac app, you need a different Bluetooth module for that. As far as using the  VESC mobile app, you need to look at the flipsky website for the module and check that the wiring is correct. Mine came with the pins in the wrong place.
```

---
## \#3 Posted by: chrischo1996 Posted at: 2018-10-08T13:07:01.801Z Reads: 197

```
I am still having trouble properly using the Bluetooth module to connect in canbus mode to write to both escs at the same time.
```

---
## \#4 Posted by: Grozniy Posted at: 2018-10-08T16:27:03.865Z Reads: 189

```
It will not work on Android 8. You'll have to flash the firmware or use an older phone
```

---
## \#5 Posted by: Jmding Posted at: 2018-10-08T17:35:53.300Z Reads: 181

```
I was using an HM10 and ackmaniac's app, had to downgrade the vesc firmware to get it to work, apparently VESC 3.40 fw causes problems
```

---
## \#6 Posted by: Moza Posted at: 2018-10-08T18:49:15.577Z Reads: 171

```
I had everything working great on 2 x fsesc 4.12. Then last month I have stopped getting any telemetry from either of them.

When i connect it can see my motor battery limits but nothing else.
```

---
## \#7 Posted by: Pmac Posted at: 2018-10-08T22:02:57.880Z Reads: 163

```
@Grozniy I don't think the android version makes a difference with the flipsky bluetooth modules.  I am getting the exact same experience with Android 9 on a Pixel and Android 6 on a Nexus 5.

@Jmding how do you downgrade?  When in the ackmaniac app it only shows the latest firmware to load onto the Vesc?  Do I need to download an older version of the ackmaniac app?  I am a newb so any help would be really awesome.

@chrischo1996  The wiring seems fine as I can get the VESC Tool Mobile to work but nothing else.  I have some HM-10 clones around.  And I have an arduino lying around so I may try the firmware rewrite on the HM-10 and give that a go.

Thanks for all the suggestions everyone.
```

---
## \#8 Posted by: Pmac Posted at: 2018-10-09T12:28:44.619Z Reads: 146

```
flipsky has responded and they have advised their Bluetooth module will only work with the VESC Tool.
```

---
## \#9 Posted by: Andy87 Posted at: 2018-10-09T12:48:09.793Z Reads: 146

```
Did you make an update on your phone but didn’t updated your app?
```

---
## \#10 Posted by: Moza Posted at: 2018-10-09T14:15:30.694Z Reads: 145

```
Not too sure what you mean. 

Ackmaniac app is version 1.114.
Vesc tool is version 0.95

I wouldn't know how to update the vesc tool and there doesn't appear to be any updates available for the ackmaniac app so I think everything is up to date.

Someone suggested downgrading the vesc tool to version 0.91 which worked for them but I don't know how to downgrade (or upgrade lol).
```

---
## \#11 Posted by: Pmac Posted at: 2018-10-09T22:40:51.154Z Reads: 133

```
Are you using the flipsky bluetooth module or are you using a HM-10 module?
```

---
## \#12 Posted by: Moza Posted at: 2018-10-12T19:47:00.525Z Reads: 126

```
I'm using a hm-10.

I've managed to sort it by flashing the vesc with ackmaniac vesc tool. 
I was running vedders so I'm assuming an upgrade to 0.95 has made the (ackmaniac) app incompatible.
```

---
## \#13 Posted by: Pmac Posted at: 2018-10-12T22:27:31.920Z Reads: 124

```
From what I understand you can't use the ackmaniac app without having the ackmaniac software on your VESC.
```

---
## \#14 Posted by: mtuan293 Posted at: 2018-10-13T00:03:59.902Z Reads: 121

```
As far as I know most apps support HM-10 and not nrf51 - which is what your Flipsky module is based on. I think the Xmatic app by @twan supports the nrf51.
```

---
## \#15 Posted by: Pmac Posted at: 2018-10-13T03:11:29.748Z Reads: 111

```
But that is iOS only.  So useless to me.

Just swapped in a hm-10 clone I had lying around and it works perfectly.
```

---
## \#16 Posted by: Moza Posted at: 2018-10-13T09:07:26.184Z Reads: 110

```
Yes it appears you now need the ackmaniac software on the vesc. 

Although, up until a few weeks ago I was using the app without ackmaniacs extended tool.

I thought my modules where faulty because they all just stopped reading telemetry all of a sudden.

Had to install ackmaniac tool to all scooter vescs to fix the problem.

Looks like 0.95 is no longer compatible.
```

---
## \#17 Posted by: Pmac Posted at: 2018-10-14T02:43:30.990Z Reads: 100

```
I had no idea.  I had just assumed you needed the ack software to use the phone app.  I didn't realise there was a change as I din't have a bluetooth module in a board until now.
```

---
## \#18 Posted by: Jmding Posted at: 2018-10-14T03:17:59.286Z Reads: 98

```
I believe ackmaniac's app works with Vedder's FW, but vs 3.40 (the current version) is incompatible, while 3.39 works.  I wasn't able to find 3.39, so ended up flashing ackmaniac's FW.
```

---

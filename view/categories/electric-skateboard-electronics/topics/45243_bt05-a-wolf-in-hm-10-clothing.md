# BT05 a wolf in HM-10 clothing?

### Replies: 22 Views: 2705

## \#1 Posted by: DanSkates Posted at: 2018-02-01T11:56:46.046Z Reads: 226

```
Hi bluetooth aficionados!

So I just excitedly connected my FOCBOX to my bluetooth module for the very first time using this schematic:

![995016847251VESCHCconnection|594x487](upload://q3Url5ERhQG23YlHoNtY2fga0VN.jpg)

VCC - 5V
GND - GND
TX - RX
RX - TX

I got a flashing red light and all looks groovy.  However my iphone can't discover it BUT my laptop can.  When my laptop detects it and I connect it shows it as 'BT05'.

These are the modules I bought:

https://www.ebay.com.au/itm/2Pcs-BLE-Bluetooth-4-0-CC2540-CC2541-Serial-Wireless-Module-Compatible-HM-10-IOS-/201647746825

I've done a bit of research and there seems to be clones of the HM-10 called BT05 (amoung others) but they're apparently essentially the same thing.

I've triple checked my connections but just cannot get my iphone (or any iphone in the house) to see it.

Have I been duped?  The description says it connects to ios and the module looks identical to the others that people recommend on the forum but the BT05 has throw me and I'm wondering if these are the wrong thing or am I just being a dumbass?

I'll take my board in to work tomorrow and see if one of the cool kids with an andriod can detect it but in the meantime would anyone have any suggestions?  I've not come across this on the forum yet and I wondered if anyone else has encountered a similar thing?

Thanks in advance! :robot: 

Dan
```

---
## \#2 Posted by: Skitzor Posted at: 2018-02-01T12:02:15.565Z Reads: 204

```
Are you trying to connect with bluetooth directly? Don't have much ios experience. but you should try to connect with the vesc app. not ios bluetooth...
```

---
## \#3 Posted by: DanSkates Posted at: 2018-02-01T12:14:11.341Z Reads: 198

```
Hi @Skitzor - thanks for the fast reply!

Yeah I was trying with the bluetooth discovery in settings.  I've downloaded @emmaanuel's app ([eSkate VESC](https://www.electric-skateboard.builders/t/new-version-2-1-ios-eskate-vesc-app-for-standard-and-ackmaniac-fw/32340/2)) as I thought this was the only iphone version - plus it looks pretty badass!  I can't  find a way to connect directly through the app tho...
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-02-01T12:17:33.202Z Reads: 192

```
![image|281x499](upload://sNjRuJSDwtGKbPNMXdoIZpXPrqH.jpeg)
```

---
## \#5 Posted by: DanSkates Posted at: 2018-02-01T12:20:14.054Z Reads: 174

```
Thanks bud - but I get nothing but fresh air in my list:

![IMG_0226|281x500](upload://zt7e7i6JHafY3TWL2q5EAz0MG3N.PNG)
```

---
## \#6 Posted by: GrecoMan Posted at: 2018-02-01T12:24:21.075Z Reads: 161

```
ahh wait lemme take a look.

i would guess that your phone has a different transciever than your laptop, IOS is SUPER picky about bluetooth.  when i connect mine, i just plug it in, turn on bluetooth, and go into the app and it’s sitting waiting for me. 

you can find legit hm-10’s on aliexpress for about $2.50, I can link you if you want

oh yea, on the back of the module, does it say 3.3-6v?
```

---
## \#7 Posted by: DanSkates Posted at: 2018-02-01T12:33:17.145Z Reads: 155

```
Thanks for the help.  Yeah I've got the feeling that it just doesn't like them.  Yep - 3.3-6v.  They're the ones from the link above :slight_smile:
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-02-01T12:35:53.941Z Reads: 152

```
I use these ones for my modules:
https://m.fr.aliexpress.com/item/32618305048.html?spm=a2g0n.orderList.0.0.223fadaf9cVFcZ
use them daily on IOS and have 18 of them out in the wild :)
```

---
## \#9 Posted by: DanSkates Posted at: 2018-02-01T12:40:03.135Z Reads: 147

```
Thanks for the link.  Yeah I was being lazy and bought local to save on delivery time.  The description is identical to the one you sent though and they look the same.  Clearly they're not though!!  :smile:   Or I'm missing something obvious...
```

---
## \#10 Posted by: SimosMCmuffin Posted at: 2018-02-01T13:24:24.892Z Reads: 144

```
Take a picture of the module you have in hand.

HM-10 has 1 IC on the module,
HC-05 has 2 ICs on the module.

Also HC-05 if I remember correctly is Bluetooth classic/EDR
```

---
## \#11 Posted by: SeanHacker Posted at: 2018-02-01T13:32:40.579Z Reads: 144

```
@DanSkates Have you tried changing the baud rate (to 96000) in whichever vesc-tool/bldc-tool you are using to set up your vescs?
```

---
## \#12 Posted by: DanSkates Posted at: 2018-02-02T02:17:15.865Z Reads: 124

```
It's the exact module in the link - identical to that.  I'll share a pic when I get home tonight though just to be sure.

Just checked on an Android phone and it also picks up the module as a BT05.

Think I'll just buy a new module and see if that works.  This might be an intersting thread for others though if it is a case of mistaken identity so others don't make the same mistake.  Fairly inexpensive mistake to make but just annoying on postage times :thinking:
```

---
## \#13 Posted by: jmasta Posted at: 2018-02-02T02:28:16.033Z Reads: 118

```
Try the app nRF Connect.  It's a much more powerful tool for finding and diagnosing bluetooth issues on iOS.  Might help you out.  It's free, so worth a shot

https://itunes.apple.com/us/app/nrf-connect/id1054362403?mt=8
```

---
## \#14 Posted by: DanSkates Posted at: 2018-02-02T03:52:55.290Z Reads: 110

```
Wow...that's awesome! Well...it found it a found it at least:

![IMG_0229|281x500](upload://8MRpo0bRLBiQ4SNvszSyOk19fp4.PNG)

But I've no idea what to do with it 😅  It confirms my suspicions tho. 

Tried to load it into the eSkate VESC app with it connected (via the nRF Connect app) but it still doesn't see it so I'm guessing it's not compatible - also I can't pick it up in the AcKmaniac BLDC tool.  Tripled checked all my connections and ensured baud is 9600.......hmmmmmm might quickly research if the baud should be different for a BT05 module? If that fails they're going in the bin! 😂
```

---
## \#15 Posted by: DanSkates Posted at: 2018-02-02T04:05:09.423Z Reads: 103

```
"**BT05-A mini BLE Bluetooth V4.0 iBeacon**

Similar modules sold as DX-BT05. This module is based on the Bolutek CC41-A. This is the same form factor as the HM-11, however, the layout is different. The BT05 is sometimes sold as a HM-10 and regarded as a copy of the HM-10, however, I don’t see these as copies more like a different version of the same thing. Not sure where these originate from as I can’t find this version on the bolutek website nor can I find a manufacturer (didn’t spend too long looking though)."

http://www.martyncurrey.com/bluetooth-modules/#HM-10

Grrrrr...looks the same though - baud rate is the same.  Anyone else used this with success??  Am I flogging a dead horse here?  :horse:
```

---
## \#16 Posted by: DanSkates Posted at: 2018-02-02T04:30:22.242Z Reads: 98

```
Looks like it's possible to flash it with HM-10 firmware...could be worth investigating and quicker than shipping a new one if it works!  Nothing to loose so I'll let you know if I manage it...
```

---
## \#17 Posted by: SimosMCmuffin Posted at: 2018-02-02T06:23:45.558Z Reads: 94

```
I'll check what the Bluetooth services on my HM-10 modules are when I get home, so we can do a comparison.

You can then decide if you want to proceed with the firmware re-flash
```

---
## \#18 Posted by: SimosMCmuffin Posted at: 2018-02-02T06:40:16.090Z Reads: 96

```
![dsa|430x500](upload://226GigLrARMM7vxJXxCBHCGMF5o.jpg)

The BT05-module has a different form factor than the HM-10.

If you ordered the modules that you linked to the Ebay page, then most likely they are the AT-09 -module.
![dsds|392x499](upload://2hAtzYuvYBqXwOcHYUEmV3B8qk8.jpg)

Based on the info in the http://www.martyncurrey.com/bluetooth-modules/ , it would actually seem that the "HM-10"-modules that I ordered and received are actually AT-09 -modules. Based on the simple fact that there is a pushbutton footprint next to the header, where as the real HM-10 module doesn't.

But at least when I tested them, they worked as a serial-bridge, so it still fulfills it's purpose.

Also consider the possibility that the bluetooth device name could simply have been changed with AT-commands at some point in it's production/use (AT-commands in link)
http://fab.cba.mit.edu/classes/863.15/doc/tutorials/programming/bluetooth.html
```

---
## \#19 Posted by: emmaanuel Posted at: 2018-02-02T07:19:22.322Z Reads: 92

```
Strange, you should see the device when you click on "Select a VESC device". Did you click on this button ?
Another thing: Make sure your device is not already connected to your iPhone in the iOS bluetooth section.
```

---
## \#20 Posted by: ROFEN13 Posted at: 2018-03-30T21:38:55.689Z Reads: 78

```
This same thing has happened to me. My samsung S9 cannot register it, but it appears on my wife's phone as BT05. I actually purchased the same one that is listed on aliexpress from a link someone posted here, claiming it is real.
```

---
## \#21 Posted by: Acido Posted at: 2018-03-30T21:42:14.657Z Reads: 75

```
turn on location
```

---
## \#22 Posted by: Acido Posted at: 2018-03-30T21:43:16.746Z Reads: 75

```
http://www.martyncurrey.com/hm-10-bluetooth-4ble-modules/

all the same  basically
```

---

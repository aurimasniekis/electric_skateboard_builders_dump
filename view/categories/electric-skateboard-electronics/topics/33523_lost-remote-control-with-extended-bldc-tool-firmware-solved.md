# Lost: Remote Control with Extended BLDC Tool Firmware \[SOLVED\]

### Replies: 4 Views: 553

## \#1 Posted by: sprocket12 Posted at: 2017-09-19T21:45:33.219Z Reads: 70

```
Love @Ackmaniac's firmware but I've encountered a weird issue.  I am finishing a build and added Bluetooth with the Extended BLDC Tool and version 2.54 of @Ackmaniac's firmware.  Everything checked out ok.  Bluetooth connected, Android app reported data, etc.

Did a couple of test rides and went in to change battery amp settings to compensate for heat.  I connected to the VESC fine and read the current configuration.  It read settings that were not what I remember entering.  So I re-entered and started going to each page to verify my settings.

The remote showed complete defaults.  When I went in to adjust, I ran the wizard.  It doesn't see the remote at all!  I have active display on, disabled, current with brake, etc. Nothing shows the remote working.  Hand entering data makes no difference.  Android app still worked...

I checked the remote pairing- good.  It connects to the receiver when turned on.  Hmmm.  Reflashed old 2.18 firmware... (wait for it)... remote works!  Ok.  Re-re-flashed @Ackmaniac's 2.54 and loaded defaults.  Went to set up.... no remote!  

Again, went back to 2.18, and remote starts working.  What gives?  Is there an option I hit somewhere on the PPM tab that might affect this?

I'm not at my bench right now so I don't have access to the screens but if you can think of something I can look at or post, I'm all ears....

Thanks
```

---
## \#2 Posted by: Ackmaniac Posted at: 2017-09-19T21:54:28.550Z Reads: 57

```
When you change the app setings to ppm you have to select PPM or PPM and UART in the General Tab and then write the settings. Otherwise PPM won't be active. So you have to write the settings and then reboot or power on off you VESC.

Another important thing to change the mode via the app is that you have to connect to the Master VESC. If the module is connected to the master then everything is fine. If it is connected to the slave you need to activate can in the app and select the controllerid of the master.

Another important thing is that you disable "Send status over CAN" at the master. But it needs to be enabled at the slave so that the Master can change it for it's connected slaves.

<img src="/uploads/db1493/original/3X/a/6/a692cb84ef6cfdf0891a426c924c898b0bc5d63b.png" width="690" height="447">

Another possible reason could be that your smartphone doesn't have a correct bluettooth low energy integration which can be the case foe cheap phones and for Android firmware mods.
```

---
## \#3 Posted by: sprocket12 Posted at: 2017-09-19T21:59:43.591Z Reads: 47

```
Hey!  Thanks @Ackmaniac!  I'll certainly look at these points.

I have a single VESC/motor set up but I'll make sure settings are what you say.  

The Android app is not an issue at this point.  I haven't taken the board off my bench once the 2.4 GHz  remote disappeared.  I was only using it to be sure that I could see a connection to my phone.  I'm using a Samsung Galaxy S7.  I think the Bluetooth is ok.

Anyway, I really appreciate the quick response.  I fell in love with the battery/motor/etc. info at my fingertips!  I'll try these as soon as I get home...
```

---
## \#4 Posted by: sprocket12 Posted at: 2017-09-20T14:07:31.381Z Reads: 27

```
Solved!  After correcting PPM with UART, writing, and rebooting, the remote came back to life.
```

---

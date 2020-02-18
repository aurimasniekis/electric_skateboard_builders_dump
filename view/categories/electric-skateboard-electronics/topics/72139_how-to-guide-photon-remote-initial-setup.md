# \[How To Guide\] Photon remote initial setup

### Replies: 17 Views: 1306

## \#1 Posted by: Wajdi Posted at: 2018-10-24T02:25:22.333Z Reads: 202

```
Many people are asking me about how to get started or pair up their receivers, so I decided to start this guide showing the initial basics on how to set things up, without over saturating the original topic.

So you just got your hands on a new Photon remote, and are excited to start using it.
Here is a quick introduction guide on the essentials of setting things up to get you going.

![Photon|260x500](upload://4CRyp5pSjMxsneZjdvZjlSrjfMz.png) 

**1. Connecting the receiver to your VESC:**

![IMG_1414|450x500](upload://tH0bFm5i89deRtqlHOhomeVLgrr.jpeg)  

Depending on the HW version of your Vesc, look for the UART port. In this case, our VESC is a 4.12 HW. 

In case you have a **Vesc 6 derivative**, Rx and Tx are switched, carefully flip those pins on the UART cable on one end as shown in the picture below 
![IMG_1426|690x378](upload://gWx8qoqqpkiAA3ds8ucObEmwo6.jpeg) 

Every receiver should come with a UART cable, it has **6 pins**.
Carefully check your VESC UART port and make sure your connect the right pins as per the following picture:

![IMG_1415|375x500](upload://5dg6yI27ijsdbuPQim8DOddw9MA.jpeg) 

One of the pins on that port won't be used.

![IMG_1416|690x338](upload://mtVvyeNZ71GijFZbWe6uHipCIDA.jpeg) 

If connected correctly,  you should see a green LED light on the receiver.

**2. Pairing the receiver.**

**Please note:** Receivers are already paired to the remote when they are shipped out, no need to perform this step unless you have a new receiver or a new remote. Or for some reason you have to pair the receiver again after a software update.

![Photon1|260x500](upload://pEDbvG35DtqRNuaKkmVfolmVMQr.jpeg) 

If the receiver is connected and the green light is on, and you see the above display without the red dot with green circle animating, it means that they are not paired up.

![Photon2|260x500](upload://dr3VWFYfQstqsdl6mFxN50gnKSi.png) 

Go to main menu by pressing the Left button, scroll down to "Binding" and press the joystick down to enter.

![Photon3|260x500](upload://99vmnkRxF7WtYnriTXKBps2Tlle.png) 

The Photon remote supports up to 4 receivers at a time, with the first one in the list being the Master.
Select the first slot and press enter (push joystick down) if you are pairing your only receiver, or your Master.

![Photon7|260x500](upload://xnpEsAST9NDmckNjWckcyPNPxCW.png) 

A search screen will appear, looking for receivers in binding mode.
On your receiver, there is a small black push button, thats the binding button.
Press is while the remote is searching to pair it.

![Photon4|260x500](upload://9DlZwQfr8QticEpa5gsFNTbkcEH.png) 

After a successful pairing, you should briefly see this message, and then back to main screen.

![Photon|260x500](upload://4CRyp5pSjMxsneZjdvZjlSrjfMz.png) 

Now telemetry will start flowing, with your Vesc FW on top, and the red dot will now transform to green and start animating, meaning you got a connection.

Thats the basic initial configuration, more details will be posted about the other functionalities. If you got any questions please don't hesitate to ask!
```

---
## \#2 Posted by: Linny Posted at: 2018-10-24T02:42:56.185Z Reads: 157

```
If I'm using a Focbox unity, I shouldn't have to swap the wires yea? Since its not a ver 6
```

---
## \#3 Posted by: Wajdi Posted at: 2018-10-24T02:45:53.895Z Reads: 157

```
I don't have information on it's UART port pinout, if its posted somewhere let me know to take a look at it.
```

---
## \#4 Posted by: Linny Posted at: 2018-10-24T03:02:58.848Z Reads: 156

```
Sure! 

Meantime I'm using a flipsky dual 6.6. Thinking it would be better if I didn't mess with the wires and wait till the unity comes to use it.
```

---
## \#5 Posted by: danggilmore Posted at: 2018-10-24T05:22:05.416Z Reads: 146

```
I was really scared to change the wires in port and @Wajdi sent me a YouTube video and it's REALLY easy. Just need he video and a little confidence
```

---
## \#6 Posted by: DAddYE Posted at: 2018-11-25T21:43:40.473Z Reads: 115

```
Hi! 

Is it possible to configure a eSTOP when the remote loses connection?
```

---
## \#7 Posted by: danggilmore Posted at: 2018-11-26T02:15:06.174Z Reads: 108

```
This is the issue I had with remote. If it wouldn't jolt when losing connection, it wouldn't be sitting in storage
```

---
## \#8 Posted by: Goonman Posted at: 2018-12-14T23:40:40.806Z Reads: 100

```
How do you get it working once it freezes? I can't even turn it off.
```

---
## \#9 Posted by: Goonman Posted at: 2018-12-14T23:41:10.798Z Reads: 101

```
![20181215_103313|281x500](upload://hNNrlql7d5F8Q2XzPh6xX5AdjUw.jpeg)
```

---
## \#10 Posted by: mmaner Posted at: 2018-12-14T23:47:44.612Z Reads: 96

```
Take it apart, disconnect the battery, wait a few seconds then reconnect the battery, reassemble.
```

---
## \#11 Posted by: Goonman Posted at: 2018-12-15T00:02:56.383Z Reads: 95

```
Thanks yeah I managed. Fortunately it didn't come screwed together because I didn't bring a screwdriver. I managed to get the PCB out undoing it's screw with pliers. Off and on. Working. Then tape it back together.
```

---
## \#12 Posted by: directC Posted at: 2018-12-15T00:24:49.343Z Reads: 96

```
How's that meant with the master when connecting multiple vescs?
Do you just mean that I'll get the telemetry from that one?
What happens if master disconnects (no battery) and i have a slave left, does the telemetry change to that one?

Also the remote has a light control feature
Do I have to solder the leds wires as rgb to the pcb? I guess it's the 2x3 solder points under the antenna on your picture?
```

---
## \#13 Posted by: Wajdi Posted at: 2018-12-15T01:17:16.844Z Reads: 96

```
I just released an update that fixes this issue:
**-Photon Receiver: V0.4**

* **Remote has to be updated to V0.53 for this to work.**
*Fixes and improves connectivity

**-Photon Remote: V0.53**

* Fixes several software issues.
* Improves connectivity
* **Receiver has to be V0.4**

Download here http://forum.eboardshop.net/t/firmware-update-download/59

Let me know if you still need help. :slight_smile:
```

---
## \#14 Posted by: Goonman Posted at: 2018-12-28T00:05:39.922Z Reads: 85

```
Have tried to update FW. I did my best to follow the guide in the forum. Downloaded Arduino windows C++ x86 etc. Arduino file doesn't run. Remote doesn't have a driver. Computer recognises the remote is attached and has a name etc. Have tried to contact Wajdi via messenger but he isn't responding. Is there someone in Oz who is familiar with this remote and receiver who can update fw for me. 
Ideally I want to send it back for a refund but I don't know if that is going to happen.
```

---
## \#15 Posted by: Chupacabra Posted at: 2019-02-05T16:00:43.560Z Reads: 71

```
Is the remote back on sale?
```

---
## \#16 Posted by: Floyd650 Posted at: 2019-03-04T06:14:50.358Z Reads: 64

```
So I got my board up and running with the latest FW on the receiver and the remote.  Everything works beautifully, and I am ready to move on to using the LED function.  Can anyone explain what I need to do to get LED's running off the receiver?
```

---
## \#17 Posted by: MiniChopper4Me Posted at: 2019-05-03T15:09:35.868Z Reads: 46

```
@Goonman In case anyone ran into the same problem I did, posting the fix here.

I tried to upgrade my photon and receiver to the latest firmwares, but I couldn't get the updater to run successfully.  In the selection box for Port I had multiple options, including COM1 for a physical serial port on my PC.  When I would run the updater, it would communicate with the Photon on the selected port for the device (COM8 in my case) and then after starting the upgrade, I would get the following:

    C:/Users/charl/Downloads/PhotonV0.53.bin
    NoError
    Forced 1200bps success
    Closing port
    Updating…
    Error occurred
    No device found on COM1

After doing this to both the controller and receiver, both the receiver and controller would not "power up":
in the case of the controller, even if I plugged in the USB, only the orange light would come on, I could only get the screen to turn on full white (briefly) after randomly pressing a bunch of buttons on the controller.  Thankfully, it would still communicate properly with the PC.  In the case of the receiver, it would not indicate properly with the orange light on as it should.  Again, it still thankfully communicated properly with the PC when connected.

 I resolved the issue by disabling and removing COM1 from my PC and ONLY having the remote or receiver hooked up to the PC at the time of the upgrade. The flash updater then completed successfully since it had no other ports to erroneously switch to when starting the upgrade process.

The receiver has to have both the UART and USB plugged in in order to power up and be able to receive the upgrade and you will have to rebind your controller to the receiver after the upgrade.

I'm still not sure at this point whether you need to simply press the button briefly during the bind process, or you have to hold it in, but I tried holding it in a bunch of times and this never seems to work.  I think its just a momentary push while the controller is searching for the receiver.
```

---

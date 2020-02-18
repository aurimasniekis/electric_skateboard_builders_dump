# Having problems connecting bluetooth HM-10 (HMSoft) to VESC 4.12

### Replies: 3 Views: 199

## \#1 Posted by: chris96 Posted at: 2019-09-01T15:27:40.624Z Reads: 34

```
Hello guys,

i am having problems connecting my HM-10 BLE module to my VESC 4.12 (3.58 firmware).
I am using this module:
https://banggood.app.link/bSqNfuq9CZ 

I am able to connect the module with my Android 5.1 via ESC monitor (led on module lights constant), but it wont transmit data and i can not pair it with my phone. I tried it with an android 8.0 but had the same problems. The VESC app finds it, but doesnt connect to it. Every app does recognize it as HMSoft.

The module is not one of those "HM-10 compatibles/clones" like BT05/AT-09 so it should have the correct HM-10 firmware (If not pls prove me wrong!). 

The connection to the vesc looks like this:
HM-10->vesc
vcc->5v (this hm-10 has a voltage regulator)
gnd->gnd
TX->RX
RX->TX

The baud rate is set to 9600 (programmed with a cable, not with the app)

My main questions (apart from: how can i fix the problem???) are:
1) is the problem with the communication between my phone and the bluetooth module or the communication between the module and the vesc?
2) could it be that i have to change the firmware of the vesc because the esc monitor app only supports certain firmwares?
3) could it be that i have to change the firmware of the HM-10 because the hm-10 firmware are not all the same?

I would be very thankful for any ideas or suggestions you guys have!! 
Thanks!
```

---
## \#2 Posted by: deucesdown Posted at: 2019-09-01T17:06:52.514Z Reads: 29

```
My guess is incompatible firmare version. Read throgh this and try one of the listed firmware versions.

https://forum./t/how-to-ackmaniac-esc-tool/2744
```

---
## \#3 Posted by: chris96 Posted at: 2019-09-01T21:02:54.668Z Reads: 25

```
I just tried to downgrade the firmware with the Ackmaniac ESC Tool and now everything works how its supposed to. Thanks a lot for your tip, solved my problem!!
```

---

# Dual VESC CAN Problems

### Replies: 10 Views: 1574

## \#1 Posted by: notger Posted at: 2017-09-26T23:03:47.712Z Reads: 145

```
Hi,

for two days i was riding perfect in dual Motor setup with my new Focboxes.
after ride without problems i charged the battery, plugged back in and just the master was spinning.

i did not change anything in bldc inbetween.

did a firmware update and made dual settings again.
Master > ID-0, send over can-no,multiple escs over can-yes
Slave > ID-1, send over can-yes,multiple escs over can-no
PPM with UART, and can cable plugged in

still not working ?

any ideas whats the Problem ?
as solution right now i drive with PPM-Y-cable buts not at all as smooth like over CAN.

greets and thanks
Notger
```

---
## \#2 Posted by: Jinra Posted at: 2017-09-26T23:18:47.967Z Reads: 136

```
Check your connections and cables. They're particularly sensitive and can get knocked slightly loose or frayed. This is why i stopped using CAN. What do you mean Y cable is not as smooth? It's essentially the same for me unless you lose traction.
```

---
## \#3 Posted by: notger Posted at: 2017-09-26T23:36:27.607Z Reads: 125

```
in can both motors were spinning pretty similar.
with y-cable i see some offset spinning starts of both motors on the bench without load. the motos also stutter abit more on hill-start compared to can
```

---
## \#4 Posted by: Jinra Posted at: 2017-09-26T23:38:32.982Z Reads: 119

```
Sounds like a setting somewhere else for split then. There should be no difference in performance on the two control methods if you set it up correctly for each. Slightly varying trigger points for PPM signal is a non-issue as well as it affects nothing for when you actually ride it.

Make sure you turn off "send status over can" when using split ppm.
```

---
## \#5 Posted by: notger Posted at: 2017-09-28T20:47:58.065Z Reads: 102

```
went trough all the settings again, you were right, i had to make autodetect on one Motor again.
Now they work quite smooth while riding, still behave strange on teh bench.

Still:
id like to know if anyone has an solution to the "broken-CAN-issue".
I do not need traction control, but id like to have the option of using the PPM on the second VESC for cruise control (with @Ackmaniac 's BLDC-Tool) and logging via bluetooth does not allow to see the data of the second VESC if not connecte via CAN.

So ? any other ideas whats wrong
```

---
## \#6 Posted by: notger Posted at: 2017-10-03T19:36:26.742Z Reads: 92

```
? hmm did a whole Firmware flash and setting up both Focboxes up individually, still no CAN communication between both of them ?
with ppm-split they work fine ?
ideas
```

---
## \#7 Posted by: BigBoyToys Posted at: 2017-10-24T15:18:41.396Z Reads: 84

```
[quote="notger, post:276, topic:20888"]
what do you mean with "blown CAN reansceivers", do you know more about it, or know anyone able to repair it ? how does a blown CAN Transceiver look like or can you/i acutally see it ?
[/quote]

Usually its lights out when the tranceiver goes. Replacing it is easier than a drv but still requires some skill.

Sometimes it would only partially blow and lights would stay on. Have you checked for faults and tried a new can cable?
```

---
## \#8 Posted by: notger Posted at: 2017-10-24T15:50:54.887Z Reads: 71

```
[quote="BigBoyToys, post:7, topic:34035"]
Usually its lights out when the tranceiver goes
[/quote]


ähm, sorry, but what lights should be out, I'm not aware if the CAN drv would have seperate leds.

so my Dual Setup just works perfect in servo-split now, but just sponaniously stopped working when i initially used CAN.

BLDC-tool or Ackmaniac-tool do not show any faults, and yes i tried several CAN-cables and checked the solderpoints of the CAN Connector on he Focbox.

One strange effect i have is if i check "forward CAN" in one of the Tools, the VESC starts randomly disonnect its USB connection, after reconnecting it in exmpl, Ackmaniac-Tool and unchecking "forward CAN" connection is stable again.
```

---
## \#9 Posted by: notger Posted at: 2017-10-24T15:52:34.211Z Reads: 70

```
[quote="BigBoyToys, post:7, topic:34035"]
Replacing it is easier than a drv but still requires some skill.
[/quote]


Is there some " How-to Tutorial " about changing the CAN transceiver somewhere ?
```

---
## \#10 Posted by: BigBoyToys Posted at: 2017-10-24T16:34:59.368Z Reads: 67

```
Umm not specific to the can tranceiver but you can search board level soldering or reflowing on youtube then use what u learn to change it. Its U401 on the PCB I belive.

By lights out I mean no lights or response what so ever. Not always though, you issue sounds like it could be related to the CAN tranceiver but Im not an expert in diagnosing them.

If you can identify the CAN teanceiver touch it to see if its hot while the vesc is powered up. When mine failed the tranceiver was always hot compared to a a working vesc.
```

---

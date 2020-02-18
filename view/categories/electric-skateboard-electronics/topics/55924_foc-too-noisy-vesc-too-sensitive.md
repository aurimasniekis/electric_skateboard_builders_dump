# FOC too noisy / Vesc too sensitive

### Replies: 7 Views: 645

## \#1 Posted by: DAddYE Posted at: 2018-05-18T20:01:07.890Z Reads: 138

```
Hi all,

I'm converting my lovely Riptide to Vesc, and since I've laying around the 12s1p from InBoard I decided to do a nice upgrade.

I recompiled the vesc_tool for osx and did the wizards etc... I love the risk, so the first thing I did was setting it in FOC. 

The motors emit the same noise in FOC and BLDC ... is that normal?

The second issue I have is with the 2.4g Nano remote. It's way too sensitive, is there any way I can make my board not kill me? 

Here my config:

![39 AM|690x431](upload://5cozeDgY9Dy1CFxO0lE1Cf0R4Ta.png)
![41 AM|690x431](upload://u63QOBXlvpZKlIP3s8Ij72cRRxS.png)
![48 AM|690x431](upload://mQ8eOcOXC9PqBnkEjecuKLdZOkL.png)
![36 AM|690x431](upload://aacabXZpSPU2s6gei1AHtGH0ruF.png)
![19 AM|690x431](upload://3iAD2ML9gPuaiCxxCYIKZAEzzLE.png)
![52 AM|690x431](upload://nbPoFiyfuum7QOaGVMEvfdxODsq.png)
![05 AM|690x431](upload://sS8EsqxsyGOxSaCF1xKvstrt7xB.png)
![15 AM|690x431](upload://ylKXxNmSe6TTGi4TU4Vb7epWNgK.png)
![19 AM|690x431](upload://nYm30Yjz5vu1K2QoY3pCL8VDG9l.png)
![14 AM|690x431](upload://fMhctlh0JafVNFSEzJV2w6qZIJ5.png)
![23 AM|690x431](upload://2r6I6xnSUXtxVv8IiEQmdHyrlNw.png)
![49 AM|690x431](upload://zST7hKREiMvzM7HqAiPcpYjsyp6.png)
![10 AM|690x431](upload://eX4jnZQDdjfvJVMDE0xicsyp4d2.png)
```

---
## \#2 Posted by: Deckoz Posted at: 2018-05-18T20:04:25.829Z Reads: 110

```
Your boxes in the foc tab should read green even if you've disconnected and rebooted the vescs. Currently it is red with zeros. Meaning you haven't performed a FOC detection.

Redo the foc detection. Then go-to the hall sensor tab and detect sensors. Make sure you write motor config M^ on the right when you are completed...

Also the noise may be similar under no load(board upside down and throttle up). The noise difference is heard during applied load, it's different in the way it modulates torque so they sound different under load.
```

---
## \#3 Posted by: DAddYE Posted at: 2018-05-18T20:26:19.508Z Reads: 105

```
Oh, they are red because (I hope) the vescs are both ... at home right now! But I'll redo the wizard once at home! Thanks mate!
```

---
## \#4 Posted by: DAddYE Posted at: 2018-05-18T23:48:57.787Z Reads: 74

```
Hi, 

I tried to do the hall detection and got: `Status: Bad FOC Hall Detection Result Received`

Any idea?
```

---
## \#5 Posted by: ShutterShock Posted at: 2018-05-18T23:53:23.035Z Reads: 70

```
Check all your sensor wires and ensure none are broken and that they are attached in the right order
```

---
## \#6 Posted by: DAddYE Posted at: 2018-05-18T23:54:05.798Z Reads: 68

```
It doesn't have sensors
```

---
## \#7 Posted by: Deckoz Posted at: 2018-05-18T23:54:44.954Z Reads: 69

```
Then skip hall detection and on the general FOC tab switch it to sensorless instead of sensorsed
```

---

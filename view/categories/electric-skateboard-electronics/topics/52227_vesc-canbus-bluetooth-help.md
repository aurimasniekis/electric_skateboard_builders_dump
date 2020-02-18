# Vesc canbus/bluetooth help

### Replies: 7 Views: 681

## \#1 Posted by: Hatman30 Posted at: 2018-04-14T09:40:05.511Z Reads: 115

```
So I've recently received two old ollin vesc and got them set up fine (connected over canbus). They work fine however neither one has can fwd ticked in bldc. However when i go into my iphone bluetooth app, change the motor settings and upload to the vesc, only one of them is changed. Any help on how to get them both talking to each other please? many thanks
```

---
## \#2 Posted by: mmaner Posted at: 2018-04-15T00:18:11.885Z Reads: 97

```
Turn on can fwd on the slave (I think). Let me check.

Multiple ESCs over CAN should be ticked on the master VESC.  Send status over CAN on the slave VESC.
```

---
## \#3 Posted by: Hatman30 Posted at: 2018-04-21T23:22:51.056Z Reads: 76

```
Have tried that however the Bluetooth app doesn’t seem to be able to upload the motor setting changes to the vesc ?
```

---
## \#4 Posted by: skatardude10 Posted at: 2018-04-22T00:24:02.009Z Reads: 73

```
After setting "Multiple ESCs over CAN should be ticked on the master VESC. Send status over CAN on the slave VESC." ... did you set connect by CAN to ID: # in the bluetooth app?

Assuming your Master ID is set to 0 and Slave to 1 in BLDC / ESC tool, depending on which vesc your BT module is connected to, you need to set connect by CAN to ID: (other vesc's id). BT connected to master, this needs to be set to connect by CAN to ID: 1 for example and vice versa (Connect by CAN to ID: 0) if BT is connected to slave.
```

---
## \#5 Posted by: Hatman30 Posted at: 2018-04-22T00:40:07.780Z Reads: 62

```
Yeh I tried that as well . It just comes back with an upload error . I’ll screen shot my settings tomorrw .
```

---
## \#6 Posted by: Hatman30 Posted at: 2018-04-22T09:46:39.230Z Reads: 57

```
![vesc2|690x396](upload://mQYvZ1iZjNQtTipOjihUfCzm1B5.jpg)![vesc1|690x418](upload://n7kjqEIZFevg6x0pTC0a03RkWCV.jpg)![vesc3|690x421](upload://pvG05OEqwPTTEjAFZbCp3LfZMhO.jpg)
The slave has multiple esc over can disabled
Has send status over can enabled
and has controller id set as 1

Do u have a link where i can update the firmware? thx
```

---
## \#7 Posted by: strelok Posted at: 2019-03-05T18:11:47.456Z Reads: 18

```
I have the some problem.
Any solution ?
```

---

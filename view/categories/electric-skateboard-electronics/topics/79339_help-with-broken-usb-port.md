# Help with broken USB port

### Replies: 17 Views: 161

## \#1 Posted by: MustardTiger Posted at: 2018-12-29T22:54:33.244Z Reads: 64

```
So I accidentally broke off the female micro USB port on my focbox. I have a dual set up so I guess I can just make that one the slave but is there another way to connect to the vesc for motor detection? How difficult would it be to reattach the broken port?
```

---
## \#2 Posted by: pat.speed Posted at: 2018-12-29T23:19:14.827Z Reads: 57

```
If you are good at soldering and have a fine tip iron it’s not too hard. That is considering the pcb traces are still intact.

How are you going to make that the slave if you can’t connect to it lol
```

---
## \#3 Posted by: MustardTiger Posted at: 2018-12-30T00:02:06.449Z Reads: 48

```
I thought you just set up the master and connect through canbus. Not 100% since I currently use split ppm. I’m I missing something?
```

---
## \#4 Posted by: dareno Posted at: 2018-12-30T00:06:04.887Z Reads: 47

```
There is no way to do any kind of set up without re attaching the usb.  You still need to program both focboxes regardless of physical set up.  What a pain in the arse breaking that off.  If you cant do the repair yourself then someone else might be able to do it for you depending on where you are
```

---
## \#5 Posted by: MustardTiger Posted at: 2018-12-30T00:23:32.089Z Reads: 38

```
Luckily I have already programmed them I broke off the port while installing extensions so I could connect without opening up the enclosure. But I’d still like to be able to make changes. So canbus is just for the transmitter signal?
```

---
## \#6 Posted by: dareno Posted at: 2018-12-30T00:26:31.750Z Reads: 38

```
Canbus enables you to use a bluetooth module and other features like traction control once you have configured the vescs.  Your problem is you would need to set it up first and you can't.
```

---
## \#7 Posted by: pat.speed Posted at: 2018-12-30T00:29:46.820Z Reads: 34

```
He can use CAN forwarding I think meaning he can program one focbox and the other is programmed with the same setting. I think thats how it works but this must be setup first
```

---
## \#8 Posted by: dareno Posted at: 2018-12-30T00:31:18.894Z Reads: 33

```
Absolutely he can once its set up and he can't set it up without a usb port.  Catch 22
```

---
## \#9 Posted by: dareno Posted at: 2018-12-30T00:32:10.857Z Reads: 29

```
Where are you based man?
```

---
## \#10 Posted by: pat.speed Posted at: 2018-12-30T00:33:12.490Z Reads: 29

```
A local electronics shop can probs do it for you
```

---
## \#11 Posted by: MustardTiger Posted at: 2018-12-30T00:34:30.403Z Reads: 25

```
Thanks for the info! Im in AZ I think I’m going to take it to my local hobby store and see he can solder it back on for me
```

---
## \#12 Posted by: dareno Posted at: 2018-12-30T00:35:20.031Z Reads: 28

```
[quote="MustardTiger, post:11, topic:79339"]
Im in AZ
[/quote]

&lrm;Where?
```

---
## \#13 Posted by: MustardTiger Posted at: 2018-12-30T00:35:51.345Z Reads: 28

```
Flagstaff Arizona
```

---
## \#14 Posted by: dareno Posted at: 2018-12-30T00:37:04.896Z Reads: 27

```
Then the wizard can help you  @JohnnyMeduse
I hereby summon the wizard
```

---
## \#15 Posted by: MustardTiger Posted at: 2018-12-30T00:38:01.783Z Reads: 29

```
Thanks man
```

---
## \#16 Posted by: dareno Posted at: 2018-12-30T00:40:01.495Z Reads: 30

```
You are most welcome my friend
```

---
## \#17 Posted by: MustardTiger Posted at: 2018-12-30T00:44:46.877Z Reads: 29

```
So what’s the process of setting can forwarding? On the new vesc tool the input wizard just asks you if you have more than one vesc, you set up the remote and then that’s it. I’m assuming this is just for the ppm calibration and not motor values
```

---

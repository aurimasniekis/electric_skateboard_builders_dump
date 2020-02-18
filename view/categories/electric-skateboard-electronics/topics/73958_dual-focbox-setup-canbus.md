# Dual Focbox setup (canbus)

### Replies: 19 Views: 615

## \#1 Posted by: seaborder Posted at: 2018-11-08T19:51:00.422Z Reads: 133

```
Hey guys I know there a multiple threads but I dont know what Iam missing for using my dual focbox. Motor detection I did on both and everything fine everything should be configured right but the second motor isnt spinning maybe Iam missing out sth. Iam able to connect to the other focbox over can forward so there should be just a small mistake.

Maybe someone can help me out!:D Would be awesome!! 

Here are some pictures of the configuration

Master:

![focbox%20master|690x398](upload://6zDQ0Z2wC8N1qe5ky1znLikvVvV.png) ![focbox%20master2|690x410](upload://iMdnDuf66wt3W6exvztJsuGGuse.png) 

Slave:

![focbox%20slave|690x408](upload://2DaPpxnKVaC5HXIeQVR0OE3JmxK.png) ![focbox%20slave%202|690x401](upload://fNT6qNBr3BmEYCwEMtEtxWTtD3h.png)
```

---
## \#2 Posted by: L3chef Posted at: 2018-11-08T19:54:37.984Z Reads: 114

```
One the slave set it to "no app"
```

---
## \#3 Posted by: Trdolan03 Posted at: 2018-11-08T19:54:40.310Z Reads: 115

```
Try no control mode on the slave.
```

---
## \#4 Posted by: Trdolan03 Posted at: 2018-11-08T19:55:00.456Z Reads: 116

```
Damnit @L3chef you beat me to it.
```

---
## \#5 Posted by: seaborder Posted at: 2018-11-08T19:58:30.639Z Reads: 109

```
thanks for the fast answers guys!;)  I disabled control mode and made no app at the slave but still only one motor spinning
```

---
## \#6 Posted by: L3chef Posted at: 2018-11-08T19:59:16.433Z Reads: 104

```
And you reboted the vesc's? :smiley:
```

---
## \#7 Posted by: seaborder Posted at: 2018-11-08T19:59:25.939Z Reads: 101

```
do I have to set "send status over can" on both or just on the slave?:D
```

---
## \#8 Posted by: seaborder Posted at: 2018-11-08T19:59:58.058Z Reads: 99

```
yes I did mhhhhhh
```

---
## \#9 Posted by: L3chef Posted at: 2018-11-08T20:01:11.533Z Reads: 97

```
Ah, remove "multiple esc over can" on slave
```

---
## \#10 Posted by: L3chef Posted at: 2018-11-08T20:02:05.788Z Reads: 98

```
And as you allready have. Send status over can only on slave
```

---
## \#11 Posted by: seaborder Posted at: 2018-11-08T20:05:41.277Z Reads: 96

```
ok I did that so when I press the brake and try to turn the second motor I can feel its "breaking" but its not spinning somehow.
```

---
## \#12 Posted by: seaborder Posted at: 2018-11-08T20:07:12.047Z Reads: 94

```
or does the motor need some force it can work against? ^^
```

---
## \#13 Posted by: L3chef Posted at: 2018-11-08T20:07:34.820Z Reads: 91

```
Sensor or sensorless?
```

---
## \#14 Posted by: seaborder Posted at: 2018-11-08T20:08:34.109Z Reads: 87

```
sensored maybe thats why?:D
```

---
## \#15 Posted by: L3chef Posted at: 2018-11-08T20:10:34.332Z Reads: 88

```
Hmm no.. Could be you need to swap one of the phase wires and do the motor detection etc again.
```

---
## \#16 Posted by: seaborder Posted at: 2018-11-08T20:11:45.246Z Reads: 89

```
That did it! OMGGGGGG THANK YOU !!!! <3
```

---
## \#17 Posted by: L3chef Posted at: 2018-11-08T20:13:24.341Z Reads: 88

```
Ride on brother!
```

---
## \#18 Posted by: seaborder Posted at: 2018-11-08T20:15:52.195Z Reads: 91

```
Yeah so my build is nearly finished now ill post some pictures in no words just picutures soon :))
```

---
## \#19 Posted by: L3chef Posted at: 2018-11-08T20:17:09.932Z Reads: 88

```
Nice :ok_hand:
```

---

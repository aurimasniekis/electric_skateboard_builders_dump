# Diy remote from servo tester

### Replies: 7 Views: 760

## \#1 Posted by: pat.speed Posted at: 2017-07-07T06:42:27.479Z Reads: 93

```
Hey guys if anyone could give me some help with this it would be great. I have a gt2b remote that I use at the moment and it is great but it is quite big and bulky. I was thinking about making my own one using picaxe chips to send the signal over Bluetooth but then I thought I could use a servo tester. If I was to connect a servo tester to a cheap 433Mhz Rx and Tx would I be able to send the signal from the servo tester to my esc? 

Link to the receiver and transmitter

http://m.ebay.com/itm/171907284405?rmvSB=true&ul_ref=http%3A%2F%2Frover.ebay.com%2Frover%2F1%2F711-53200-19255-0%2F1%3Ficep_ff3%3D2%26pub%3D5575101368%26toolid%3D10001%26campid%3D5337582279%26customid%3D%26icep_item%3D171907284405%26ipn%3Dpsmain%26icep_vectorid%3D229466%26kwid%3D902099%26mtid%3D824%26kw%3Dlg%26srcrot%3D711-53200-19255-0%26rvr_id%3D1251259540846&_mwBanner=1&ul_noapp=true
```

---
## \#2 Posted by: wafflejock Posted at: 2017-07-07T07:12:52.985Z Reads: 81

```
There are a couple of us who have made our own controllers I did one here based on some cheap 2.4GHz Nordic RF modules and Arduino pro mini 3.3V boards https://github.com/shusain/eskatecontroller. Just got some pcbs made from pcbway so I can sandwich them together and have a receiver and transmitter.  It can be done but make sure you physically unit test the thing, unplug each part one pin at a time and make sure your receiver always goes idle or dead.
```

---
## \#3 Posted by: pat.speed Posted at: 2017-07-07T07:27:51.083Z Reads: 73

```
Ok thanks.
```

---
## \#4 Posted by: wafflejock Posted at: 2017-07-07T08:12:52.741Z Reads: 61

```
No problem search around a bit on the forum here you'll see some other (some much better) designs as well.  I stress the unit testing since i had one MOSI pin between the radio and homemade PCB come loose and the signal floated high to full throttle which is kind of the worst possible thing.  I've since patched my code and tested pulling each pin but better to do that before it destroys anything.
```

---
## \#5 Posted by: bjoern_h Posted at: 2017-07-07T13:19:16.203Z Reads: 52

```
you can simple change the case instead of buy a new remote :slight_smile:
Look at this http://www.elektro-skateboard.de/forum/eigenbauten-95/anleitung-umbau-fs-gt2b-fernbedienung-4330.php (german)

edit: Tutorial in english https://endless-sphere.com/forums/viewtopic.php?f=35&t=71922
```

---
## \#6 Posted by: rpn314 Posted at: 2017-07-07T14:01:22.174Z Reads: 48

```
[quote="pat.speed, post:1, topic:26973"]
I was thinking about making my own one using picaxe chips to send the signal over Bluetooth
[/quote]

Do not use bluetooth iteself to control your board under any circumstances. It is not a stable/reliable enough connection. You've got some great options above (you can also search for gt2b mods, there's quite a few here), just stay away from bluetooth :slight_smile:
```

---
## \#7 Posted by: wafflejock Posted at: 2017-07-07T16:30:24.814Z Reads: 40

```
I can second this I initially built mine using Bluetooth modules (HC-05 or 06 I forget).  I thought it would be convenient to be able to use a phone app or physical remote for controlling the board but the things would lose pairing constantly not to mention trying to control throttle with an app on your phone is difficult at best and puts your phone in a precarious position (serious alliteration going on there).
```

---

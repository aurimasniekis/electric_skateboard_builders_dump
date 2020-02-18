# Strange motor issue Raptor 2

### Replies: 26 Views: 301

## \#1 Posted by: Eskate444 Posted at: 2019-04-22T12:40:34.956Z Reads: 87

```
Hi all,

I am asking for help on this forum as I do not have warranty on my Raptor 2, so was wondering if you guys can help out.

The motors run fine, up hill, full throttle, anything.

Only issue is, when stationery the left motor needs me to spin it before it starts up, while the right motor moves only a little bit and when i spin the left one both work perfectly.

This means i have to push to start always, other than that the motors work fine.

Does anyone know what could be causing this?

Thank you.
```

---
## \#2 Posted by: ryansinatra Posted at: 2019-04-22T12:48:27.595Z Reads: 83

```
Sounds like a sensor issue. Maybe check the sensor cables?
```

---
## \#3 Posted by: Eskate444 Posted at: 2019-04-22T12:49:31.555Z Reads: 78

```
I was thinking this also, but i have put silicone around my enclosure to waterproof it, i might have to open it after all.
```

---
## \#4 Posted by: ryansinatra Posted at: 2019-04-22T12:50:23.308Z Reads: 77

```
Yes you will have to open it up. Could be caused by vibrations.
```

---
## \#5 Posted by: Eskate444 Posted at: 2019-04-22T12:51:24.725Z Reads: 76

```
Do you have any pictures of sensor cables? so i may know what i am looking for?
```

---
## \#6 Posted by: ryansinatra Posted at: 2019-04-22T12:59:10.256Z Reads: 71

```
![Screenshot_20190422_085722|541x500](upload://lVK9FJzl4BVNg4JzGhLPOrnn5Co.jpeg)
```

---
## \#7 Posted by: Eskate444 Posted at: 2019-04-22T12:59:43.237Z Reads: 70

```
Will do and report back, thanks man.
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-04-22T13:46:02.522Z Reads: 60

```
its hidden under a cover.... near the back trucks, the sensors connect from a extension board in that rear cover
```

---
## \#9 Posted by: Eskate444 Posted at: 2019-04-22T13:48:58.242Z Reads: 58

```
I just opened it, tried it with the sensor cable unplugged, it works fine.

When plugged in again issue comes back.

Can i just run one of them unsensored, what are the downsides?

Can i run both unsensored?
```

---
## \#10 Posted by: Touch415 Posted at: 2019-04-22T13:55:28.495Z Reads: 56

```
Just do motor dedication again ...
```

---
## \#11 Posted by: AlanZhou Posted at: 2019-04-22T13:57:07.307Z Reads: 56

```
[quote="Eskate444, post:9, topic:91404"]
Can i run both unsensored?
[/quote]

yes you can but rerun detection or else you may fry your focbox
```

---
## \#12 Posted by: Eskate444 Posted at: 2019-04-22T14:00:02.279Z Reads: 53

```
i cannot get the focbox to connect because the USB cable port is damaged.

I can do it via vesc tool (TCP) but that requires me to upgrade firmware and i am not very acquainted with that.

Via enertions vesc tool i cannot connect to Master focbox.
```

---
## \#13 Posted by: McErono Posted at: 2019-04-22T14:37:59.638Z Reads: 48

```
You can connect with the other focbox and use the can bus to get access on the focbox with the broken usb port or get a BT module like metr.
```

---
## \#14 Posted by: AlanZhou Posted at: 2019-04-22T14:41:44.114Z Reads: 45

```
um, with enertions built in BT module i think you can reconfigure the foxbox
```

---
## \#15 Posted by: Eskate444 Posted at: 2019-04-22T14:42:09.938Z Reads: 47

```
It is Raptor 2, not 2.1
```

---
## \#16 Posted by: AlanZhou Posted at: 2019-04-22T14:42:35.705Z Reads: 48

```
the raptor 2 also has a BT module i think
```

---
## \#17 Posted by: yelnats8j Posted at: 2019-04-22T14:44:32.514Z Reads: 49

```
Theres a easy solution to this problem

Step one : Throw the raptor away

Step two : Start reading on this amazing DIY forum

Step three : Build yourself a beast and forget about prebuilts
```

---
## \#18 Posted by: Eskate444 Posted at: 2019-04-22T14:45:32.113Z Reads: 48

```
Dont act like you would throw one away if you had one.

I am already building a DIY.
```

---
## \#19 Posted by: yelnats8j Posted at: 2019-04-22T14:51:39.895Z Reads: 47

```
Its just a joke man 😋🤣

[quote="Eskate444, post:18, topic:91404"]
I am already building a DIY.
[/quote]
Thats great 😁
```

---
## \#20 Posted by: Eskate444 Posted at: 2019-04-22T14:52:12.548Z Reads: 44

```
lol sorry man, its just this issue is frustrating me.
```

---
## \#21 Posted by: Eskate444 Posted at: 2019-04-22T14:52:38.116Z Reads: 43

```
Yes it has bluetooth, before i could connect via ackmanic esc android tool but now i cant for some reason.
```

---
## \#22 Posted by: yelnats8j Posted at: 2019-04-22T14:52:56.565Z Reads: 42

```
I feel you, i blew up a VESC a while back and shit that was annoying as hell
```

---
## \#23 Posted by: Eskate444 Posted at: 2019-04-22T14:53:23.477Z Reads: 42

```
I feel as if i should just leave them both unsensored? whats the worst that could happen? it seems to work fine this way...
```

---
## \#24 Posted by: AlanZhou Posted at: 2019-04-22T14:58:26.013Z Reads: 44

```
[quote="Eskate444, post:23, topic:91404"]
both unsensored?
[/quote]

nothing wrong with uncensored, it's just that you have to reconfigure the foc boxes for uncensored

or else it might blow the focbox
```

---
## \#25 Posted by: Battosaii Posted at: 2019-04-22T15:21:21.695Z Reads: 43

```
Best thing you can do is take the Focbox with the bad usb port out and send it out to be repaired. Many people fix focboxes for a reasonable price
```

---
## \#26 Posted by: barajabali Posted at: 2019-04-22T15:53:04.021Z Reads: 37

```
What happened when you tried to redo the detections?
```

---

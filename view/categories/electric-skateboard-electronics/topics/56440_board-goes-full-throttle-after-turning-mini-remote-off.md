# Board goes full throttle after turning mini remote off

### Replies: 7 Views: 330

## \#1 Posted by: 12meterkuk Posted at: 2018-05-23T04:59:07.793Z Reads: 68

```
Hi guys, I just swapped out the remote on my raptor 2 to a mini remote, did the binding and calibration on bldc tool and adjusted the trim. Now whenever I turn off the remote the board would run at full throttle until I turn the remote back on or turn off the board. Any advice? Thanks
```

---
## \#2 Posted by: PatRocks Posted at: 2018-05-23T05:01:22.723Z Reads: 68

```
Did you do a search?
```

---
## \#3 Posted by: 12meterkuk Posted at: 2018-05-23T05:02:48.239Z Reads: 66

```
I saw a thread about unplugging something before I turn it off but I don’t have the plug with me
```

---
## \#4 Posted by: 12meterkuk Posted at: 2018-05-23T05:09:01.113Z Reads: 65

```
I found the plug, but now the remote won’t bind after plugging the binding plug into ch 4
```

---
## \#5 Posted by: Ishayc Posted at: 2018-05-23T05:19:52.671Z Reads: 62

```
You need to press the bind button before you turn the remote on. After you get it to bind, you need to calibrate the remote in the vesc(assuming you are using one) tool.
```

---
## \#6 Posted by: Mikenopolis Posted at: 2018-05-23T05:23:56.027Z Reads: 58

```
Redo the whole process. Plus fail safe

Bind the remote
Pull out the bind key
Setup VESCs
Bind the remote a second time
Pull out bind key

Now test fail safe on bench. Give a little throttle, as it’s moving turn off the remote to see if the board goes full throttle

Anyone else. Correct me if I’m wrong
```

---
## \#7 Posted by: 12meterkuk Posted at: 2018-05-23T05:24:30.821Z Reads: 51

```
Thanks for the help guys, it works perfect now!
```

---

# Only one motor working

### Replies: 9 Views: 195

## \#1 Posted by: Sigorr Posted at: 2018-08-04T00:59:45.093Z Reads: 60

```
Hi guys does anyone know what I'm missing I have the can bus connector, I tried the other motor it works fine by it self. Also how do I connect the sensor wires![IMG_20180803_180033|666x500](upload://kyvR5gd6dGQuZSm6r1LDiw5ReZB.jpg)
```

---
## \#2 Posted by: dareno Posted at: 2018-08-04T01:08:58.249Z Reads: 57

```
little more info my friend and some pics of set up
```

---
## \#3 Posted by: Sigorr Posted at: 2018-08-04T02:23:51.536Z Reads: 48

```
I posted the picture
```

---
## \#4 Posted by: dareno Posted at: 2018-08-04T19:17:40.155Z Reads: 29

```
![image|666x500](upload://eh0RZW9J01hjpeD3HOioSnc7sGW.jpg)

This is where your sensors plug in.  
I can't see anything obviously wrong

That's the picture now the info.

Has it ever worked or is this the first time you've powered up?


Btw.  important 
 do not disconnect the canbus while the board is powered up ever!! 
Good idea to hot glue the connectors in.
```

---
## \#5 Posted by: Sigorr Posted at: 2018-08-04T19:32:45.972Z Reads: 27

```
If I connect the motors seperatly they work fine. I just can't get them to both work at the same time. Do I need to program the vescs?
```

---
## \#6 Posted by: Mikenopolis Posted at: 2018-08-04T19:42:23.510Z Reads: 27

```
have you ever programmed the VESCs? it's not exactly plug and play

You have to set one as the Master "ID=0"(the one with the receiver on the bottom of pix), send command over canbus and the other would be set as slave "ID=1" and receive command over canbus
```

---
## \#7 Posted by: Sigorr Posted at: 2018-08-04T19:57:55.027Z Reads: 24

```
![15334125242613369436428275757619|375x500](upload://uFNa7vnefwTBIJG0gSoJG5OFhLg.jpg)
Ok thanks I'm trying to connect but I keep on getting this any ideas?
```

---
## \#8 Posted by: dareno Posted at: 2018-08-04T20:02:02.302Z Reads: 21

```
https://www.youtube.com/watch?v=qpovd2XRKqc&t=878s

Watch this quick video and all will be revealed!!
```

---
## \#9 Posted by: Mikenopolis Posted at: 2018-08-04T20:02:46.552Z Reads: 20

```
1.) obviously, first make sure your usb cable is plugged in
2.) make sure your port com # is the correct one, that should be on the left panel, under connection, click on the down and check the other COMs
```

---

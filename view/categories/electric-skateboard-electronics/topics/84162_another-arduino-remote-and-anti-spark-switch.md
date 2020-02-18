# Another Arduino Remote and anti-spark switch!

### Replies: 5 Views: 348

## \#1 Posted by: von_p Posted at: 2019-02-14T03:32:40.651Z Reads: 136

```
Hey everybody,

I just thought I would share some pcb's I have been working on, let me know what you think!
Anti-spark switch based off of [vedder anti-spark switch](https://github.com/vedderb/SparkSwitch)![20190213_200625|690x345](upload://p7XFCiXXTjqPp24YmgYNKCMEy29.jpeg) 
Arduino remote based off of the [rolling gehcko remote](https://github.com/RollingGecko/ArduBoardControler) still a work in progress:
![20190213_200625|690x345](upload://aZQzyDehHOTNHb7xp7evKWxYpoN.jpeg) ![20190213_200651|690x345](upload://7jyVPXbNX7JQfkQSqD2zht4X7Tz.jpeg)
```

---
## \#2 Posted by: StefanMe Posted at: 2019-02-14T14:56:02.479Z Reads: 94

```
Looks cool! what chip do u use? The 16Mhz arduino `nano Chip? I cant see it on the picture
```

---
## \#3 Posted by: von_p Posted at: 2019-02-15T14:07:13.027Z Reads: 71

```
Yes, I am using the ATMEGA328P, same used on the nano.
```

---
## \#4 Posted by: StefanMe Posted at: 2019-02-15T15:27:15.824Z Reads: 57

```
Looks very cool! What software will u use? EDIT: i See... 

I think the 328p is a little underpowered for extended functionality and the huge display in respect to the framerate and cycle time. That’s why I switched to the SAMD21. 

Are I able to show a little demo already? 

Nice work!
```

---
## \#5 Posted by: von_p Posted at: 2019-02-17T01:04:08.088Z Reads: 35

```
I was trying to go for simplicity on the software side, but yes there are a lot more capable MCU's out there I agree, probably wouldn't have had to do a boost regulator to 5V either, which is the most difficult thing to  solder on this board. I tried to make it easy for anyone to build with a soldering iron. I am testing it right now and seems to be working well. The big missing link is the enclosure, as I am not very capable in that department.
```

---

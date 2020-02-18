# LiPo BMS Charging setup and questions

### Replies: 3 Views: 299

## \#1 Posted by: Flouw Posted at: 2018-12-20T13:59:57.817Z Reads: 50

```
Hey Guys, First off 
Hello this is my first post and I am glad this forum exists :grinning:
I have a few questions for my build. I want so power my board with four 5S1P LiPo batteries and use a smart BMS i bougth to track charging and discharging while driving. Now i was a bit confused about connecting the batteries balance charger cabels. As U can see in the picture I want to connect two in parallel two times and connect these 5S2P into a singel 10S2P batterie.
![BMS%20connection|690x334](upload://cb2XqZDHzrNrsqDwBcCyRumrw3O.png) 


I would apprechiate if some one would look over this diagram and could tell me if this would work cause i dont want to burn my house down :sweat_smile:. I've read in the forum that you dont necessarily need to connect the middle 
negative balance lead to the positive when u connect in series because its redundant. But what about the parallel connection? Do i have to watch out for something? 
Thanks in advance :relaxed:
```

---
## \#2 Posted by: Flouw Posted at: 2018-12-21T21:59:46.820Z Reads: 37

```
Anyone an idea? :frowning:
```

---
## \#3 Posted by: pat.speed Posted at: 2018-12-21T22:29:57.818Z Reads: 36

```
It is almost correct. This is going to be a little confusing but the series connection on the two batteries is between the wrong wires. It doesn’t usually matter which way but the balance wires must be ordered according. To make it easy we will just change the series on the main lead instead of all the balance wires. 

The way to remember is the main positive and negative wires should always be the outside leads of your balance connector and the series connection should always be between the middle two wires. This is now corrected in the diagram I’ve edited. And at the series connection only 1 wire should be connected in this case it was the red one as the black has been cut already

![image|690x334](upload://QWs8RYGqhBygvUUywzcyBWk2vS.jpeg)
```

---

# Looking for battery pack design software

### Replies: 8 Views: 1348

## \#1 Posted by: High-roller Posted at: 2019-02-08T10:21:29.441Z Reads: 79

```
As the title states, I'm looking for any kind of program that I can use to simulate a battery pack of any given configuration. You basically just select which type of cell you want to use, build or set up your configuration and then simulate it under various loads. Bonus points for open source...
I know Matlab and solidworks can sort of do this but I've never used either of them for that and I'm hoping there's a simpler solution.
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-02-08T10:48:07.419Z Reads: 74

```
If it exists, I haven't found it yet. Shouldn't be too hard to set something like that up, the math for series/parallel arrangements is pretty simple and there are discharge graphs available from several sources.

Another piece of battery design software that I wish I could find is something for solving the ideal layout of cell groups and connections for packing in weird shaped enclosures, like the triangle of a bike frame.

IIRC @b264 has a spreadsheet for determining the best cell to use for a pack, given limits such as P count, cost, and discharge current.
```

---
## \#3 Posted by: High-roller Posted at: 2019-02-08T11:13:08.972Z Reads: 69

```
Yeah, I've seen PC building Sims where you can build a custom rig from a library of real parts. I think it was meant as more of a game but the basic concept is the same. 
[quote="MysticalDork, post:2, topic:83576"]
something for solving the ideal layout of cell groups and connections for packing in weird shaped enclosures, like the triangle of a bike frame.
[/quote]
Exactly. Make the configuration as simple or complex shaped as you want, then test it to see if your connections work.
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-02-08T11:22:59.089Z Reads: 61

```
Yeah. My latest issue (I'm building an ebike with a 20s7p battery) was fitting all those 140 cells into the frame triangle, and having reasonably short connections. And since 7 is a prime and etc, it doesn't tile well unless you're using hexagonal close packing with hexagonal 7-cell groups. I've seen EV and other batteries where each P group is a different shape to maximize density and minimize resistance and connection distance, and I feel like there has to be some sort of software tool to do the same sort of optimization.

Tell it 18650s, 20s7p and a shape, and it'll try all the various orientations and connections until it finds the most efficient. Similar to autorouting for PCB layout, in a distant fashion.
```

---
## \#5 Posted by: Okami Posted at: 2019-02-08T11:37:33.447Z Reads: 48

```
I think on endless sphere forum there should be a software mentioned..

Cant remember how it might have been called, but folks there build a lot of ebikes, so they should know more about it
```

---
## \#6 Posted by: High-roller Posted at: 2019-02-08T12:17:37.261Z Reads: 44

```
@Okami is this what you meant?
https://www.ebikes.ca/tools/charge-simulator.html?ver=48&bat=cust_c26_s4_p5_l30
It's really meant for ebikes but it's a good start, it allows you to see the totals of a given pack. If there's something out there where we can simulate the connections between the individual cells that would be even better.
```

---
## \#7 Posted by: Okami Posted at: 2019-02-08T12:20:21.551Z Reads: 42

```
I remember a soft / simulator where u could enter how much space u have and then I think it modeled what layout u can use to fill that space..

Otherwise i dont have much other leads.. but i somewhat remember I took a peek at it but since i didnt need it at that time, i didnt explore it much further

---
Edit:
Here it is
---
http://epowerbikes.ru/constructor.php
---
Though it is in russian :smiley: 
Maybe translator can pick it up also

Also.. it is not as sophisticated as i hoped.. u basically upload image or maybe size layout and then just fill that space with sideways placed 18650 batteries..
```

---
## \#8 Posted by: High-roller Posted at: 2019-02-08T13:19:47.653Z Reads: 29

```
Translation worked pretty well. In soviet Russia, 30Q costs 390 rubles :stuck_out_tongue_winking_eye:
You're right about how simple it is, it's not going to help us much. I'll keep looking and post what I find here.
```

---

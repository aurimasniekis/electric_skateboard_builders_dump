# Hoverboard battery BMS

### Replies: 9 Views: 1160

## \#1 Posted by: reiko Posted at: 2018-09-07T01:21:10.581Z Reads: 133

```
Hey, 

I am looking to swap out my 6s LiPo for a hoverboard battery. I finished my attempt at building a board about 
2 weeks ago. At first I thought rolling with a 6s is fine, but as soon as I got the hang of riding I realized I would like to go faster. 

I found quite a few local used hoverboards that go for as low as 50€. Getting a 10S2P battery pack + BMS + charger + charging port for that price would be a bargain. 

I know the packs have an integrated BMS and I was wondering how are you supposed to hook up a charging port? How does it work in an actual hoverboard? Does anyone have any experience in this field? I tried very hard to find information on it, but nothing came up for me :'(

Thanks a lot!
```

---
## \#2 Posted by: Jake2k17 Posted at: 2018-09-07T03:45:23.015Z Reads: 121

```
I would recommend attatching your own charge only bms if you want to go cheap. I would recommend one like this:
https://www.mboards.co/products/10s-bms-battery-management-system
```

---
## \#3 Posted by: reiko Posted at: 2018-09-07T10:42:24.984Z Reads: 100

```
Getting a BMS would indeed be a doable solution, but I was wondering how does it work on a hoverboard battery pack. Is the charging port simply attached to the main leads of the battery? I'm still confused on that front.
```

---
## \#4 Posted by: Namasaki Posted at: 2018-09-07T11:56:07.051Z Reads: 92

```
There is loads of information about wiring a bms/battery system on this forum. 
Just type bms in the search function. 
There are loads of diagrams as well. 
Search for a thread called beautiful diagrams. 

I would think twice about using a battery pack from a cheap hover board. 
They have had a reputation of catching fire. 
I read somewhere that it was because of the Chinese companies who where making them where using counterfeit cells. 
If you want to spare expense, better stick with Lipos.  You can easily configure any voltage you want and use a bms for convenient charging.

Here is a thread about using a bms with Lipos. 
https://www.electric-skateboard.builders/t/high-power-10s-lipo-battery-pack-with-bms/10014
```

---
## \#5 Posted by: dareno Posted at: 2018-09-07T22:12:01.680Z Reads: 59

```
Definitely don not use a cheap hoverboard battery.  Those things are what caused the whole flight issues we now have to contend with.  They catch fire the old ones and for 50 euros thats what you'd be getting.
If you want a cheap 10s then go for a known brand cheap chinese manufacturer like a meepo or an ownboard 10s 2p. li ion. They are lg cells with built in bms's  Meepo even does a sanyo version but its more money.  DIYeboard is another cheap option but they have had some privacy issues lately.  They do sell the complete package though with battery enclosure charger etc.  Good cheap way of getting more power but will sag considerably. 
Not the best obviously but will give you the speed you want and won't burn your house down.
```

---
## \#6 Posted by: pat.speed Posted at: 2018-09-08T07:35:32.591Z Reads: 53

```
I think the actual reason is for them not actually using a bms, they use a “protection circuit” this does the same as a bms but it doesn’t balance the cells. This combine with cheap cells and there goes your house. 

@reiko I would probably try not to use these batteries although a few people have before and order 2 or 3 to make a 10s4-6p battery. If you do indeed buy them make sure to add your own bms that does balance
```

---
## \#7 Posted by: Blitz Posted at: 2018-09-08T08:34:55.421Z Reads: 46

```
I wouldn't recommend doing that.

You know why hoverboards are like Illegal and recalled?
The battery packs started Catching FIRE!
```

---
## \#8 Posted by: Zander8183 Posted at: 2018-09-10T00:42:16.890Z Reads: 38

```
Yes I am currently in the middle of the project.  I would strongly recommend your own bms because I am stumbling over mine. It charges through the discharge leads. On the other hand, the bms is only rated for something like 20 amps or less. I was testing my board and It would always cut out during acceleration. This is because the bms turns it off when the esc requires more than 20. What you would have to do is bypass the bms for discharging and only use it for charging which is quite risky. But I mean anything in the DIY aspect is risky.
```

---
## \#9 Posted by: reiko Posted at: 2018-09-16T11:43:28.703Z Reads: 29

```
Oh wow thanks, I didn't know about the protection circuit not having a balance feature. I will definitely keep this in mind and should I ever go through with it, check all the individual cells beforehand.
```

---

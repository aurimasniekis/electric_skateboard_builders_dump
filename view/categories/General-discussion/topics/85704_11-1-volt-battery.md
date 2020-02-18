# 11.1 volt battery

### Replies: 12 Views: 306

## \#1 Posted by: rookie_80 Posted at: 2019-02-28T23:43:23.178Z Reads: 135

```
Hey I have two 3s 11.1 volt batteries for my board, I am confused because online it says the max voltage per cell should be around 4.2 but my battery does not go to 12.6 when charging/out of the box. My understanding also with charging is that it is constant voltage and current till it reaches the max and then slowly decreases current till the battery is full. when I'm charging using the iMax b6 I select the 3s 11.1 volt battery but then once it's charging I scroll through the screens and it says the cutoff voltage is 12.6. How will I know when the batteries are done charging/will they charge all the way as I will never hit the cutoff voltage?
```

---
## \#2 Posted by: Jacobee Posted at: 2019-03-01T01:05:12.603Z Reads: 118

```
The voltage slowly increases as you charge the batteries. 12.6 volts (4.2 per cell) is full charge. 11.1 volts (3.7 per cell) is nominal voltage. The charger will stop charging the batteries once they reach 12.6 volts on its own.
```

---
## \#3 Posted by: rookie_80 Posted at: 2019-03-01T02:30:45.301Z Reads: 103

```
On my battery it says it is 11.1 volts 3s though, that isn't the max voltage? https://hobbyking.com/en_us/zippy-flightmax-5000mah-3s1p-20c.html
This is the battery it says 11.1 volts
Thanks for the reply
```

---
## \#4 Posted by: J0ker3366 Posted at: 2019-03-01T02:36:35.703Z Reads: 92

```
11.1v is nominal. 4.2v is what one cell in a 3s (and all lipos) will max charge to.

1s - 3.7 nominal 4.2 max
2s - 7.4 nominal 8.4 max
3s - 11.1 nominal 12.6 max
4s - 14.8 nominal 16.8 max
5s - 18.5 nominal 21 max
6s - 22.2 nominal 25.2 max

Mabey that helps
```

---
## \#5 Posted by: MysticalDork Posted at: 2019-03-01T03:13:06.316Z Reads: 78

```
The labels on batteries are nominal or "average" voltage, not maximum. Hence why a 10s pack might say 36 or 37v on it, not 42.
```

---
## \#6 Posted by: rookie_80 Posted at: 2019-03-01T03:21:43.532Z Reads: 75

```
Very cool thank you all for the replies I shall let the battery charge all the way
```

---
## \#7 Posted by: Slak Posted at: 2019-03-01T11:28:29.201Z Reads: 56

```
And while it is charging, read about lipos and how to use and preserve them
```

---
## \#8 Posted by: captclearleft Posted at: 2019-03-01T13:10:57.731Z Reads: 47

```
Great thoughts all.  
Also:
If you are not getting to 12.6v, and your batteries are new, and they are not puffed (they are still good batteries) - You might not be charging them at enough amps, or your charger cannot reach the needed wattage. NOTE: WARNING!: Never charge at an amperage greater than 1C.  (See notes below.)

When Charging, It's best to charge at no greater than 1c (1 times battery ah rating).  So - If you have a 5amp battery, don't ever charge at a greater amperage than 5a.  I always charge at 2amps.  This helps prolong the life of the battery.  And ... My cutoff voltage is set to 4.1v per cell.  If your charger is cheap, or not tuned and you charge to 4.2v, you may find that some of the cells are charging to greater than 4.2, and some less than 4.2.  This is quite common.  Not to big of a deal, but does shorten the lifespan of the battery.  
[NOTE: I know that it's safe to charge to 4.2v/cell at 1C.  And it probably wont make a big difference in lifespan, but I am extra cautious.]

Always charge in an area that is safe in the event of a fire.  Always keep a fire extinguisher around.  Never leave the house while charging.  Use a lipo bag properly.

Keep in mind the life of the battery.  Its best NOT to drain the batteries below 
3.2v per cell ([Check out these](https://www.amazon.com/Tenergy-Battery-Intelligent-Digital-Balancer/dp/B0178P8H9U/ref=sr_1_4?crid=2JD524BEP7B6Y&keywords=lipo+cell+checker&qid=1551444634&s=gateway&sprefix=lipo+cell+%2Caps%2C159&sr=8-4))

I have not read this, but it looked pretty good at first glance.  Always proceed with caution. :)
[Lipo Guide](https://rogershobbycenter.com/lipoguide)
```

---
## \#9 Posted by: janpom Posted at: 2019-03-01T13:26:26.816Z Reads: 35

```
[quote="rookie_80, post:1, topic:85704"]
my battery does not go to 12.6 when charging/out of the box
[/quote]

What do you mean by that? At what voltage does it stop increasing?

What kind of battery is that? Is it some kind of cheap/noname LIPO, such as Multistar?

The iMax B6 will charge to 12.6V by default and it will make very loud and annoying noise once the battery is fully charged.
```

---
## \#10 Posted by: rookie_80 Posted at: 2019-03-01T18:59:16.599Z Reads: 23

```
Yea it looked like it would continue to hit 11.1 and then go back down to 11.09 and back up so I was concerned it was trying to overcharge it. And I'm not sure if it a nock off, it is just what I bought from that link. Again thank you for the response I shall let it charge fully
```

---
## \#11 Posted by: janpom Posted at: 2019-03-01T19:58:24.270Z Reads: 20

```
Sorry, I missed the link. Zippy Flightmax are OK. Make sure you connect the balance wires. Once you start charging if you press the > button on the charger it will display individual cell voltages. You may want to check the cells are not out of balance.
```

---
## \#12 Posted by: rookie_80 Posted at: 2019-03-03T21:47:19.258Z Reads: 13

```
Awesome thank you, the battery is charging and im getting great range now!
```

---

# To what extent is the XT-90s antispark connector necessary for a 7s3p battery with an inbuilt BMS switch?

### Replies: 5 Views: 273

## \#1 Posted by: Fraserrazor Posted at: 2018-05-05T16:09:29.587Z Reads: 79

```
For one of my builds I am assessing what to use for an anti-spark method. On the market a lot of first time DIY builders choose the XT-90s loop plug as a way of preventing the intial high amperage output when plugging in the battery directly to vesc and its capacitors. I wanted ask if the 7s3p battery from https://eskating.eu/product/flat-7s3p-eskating-electric-skateboard-battery-30q/ required a form of antispark as I have tested this setup with dual motors and dual vescs and no sparking occured when using the BMS switch for turning on and off. I also need clarification as to whether I would need to switch off my BMS switch for charging but from what I have heard the actual BESTECH BMSs can be on or off during charging. Are there any component safety considerations?

I know there are a lot of questions but searching around the esk8 electronics section revealed not much information on the 7s3p setup.

P.S I got the battery brand new off an individual seller for a great price, which is the main reason not choosing a 10s2p setup.

Thanks to all those who help!
```

---
## \#2 Posted by: onepunchboard Posted at: 2018-05-05T16:42:07.921Z Reads: 72

```
aniti spark key is just to save the connector to burn or weld together when connected. it doent affect other parts. if you are using bms switch it is not needed. 

But there are thread talking about the bms failiure when regen brake go pass what bms is rated and breaks them as highend board can pass 150amp instant on brake.

personally speaking 90s is robust, but it can fall off during rough ride so it is important to make it sug feet.
```

---
## \#3 Posted by: MysticalDork Posted at: 2018-05-05T17:33:00.508Z Reads: 62

```
If your BMS has an eswitch function, then a loopkey isn't strictly necessary, but it's still a good idea to have a way to physically disconnect the battery in my opinion.
```

---
## \#4 Posted by: Acido Posted at: 2018-05-05T17:37:05.934Z Reads: 58

```
if you are going 80kmh you might get those 150amps....

also the regen amps will be limited in the vesc so...
```

---
## \#5 Posted by: onepunchboard Posted at: 2018-05-05T17:53:50.100Z Reads: 51

```
but i've seen people break the anti spark switch here rated higher than 150amp. and it is not jst occational, I forgot who he was but he broke few times so moved to 90s loop key.

not sure if bms switch fails over time, but I saw one person who broke it because of regen. 

personally I want to try, that 1 fail could've been anything.
```

---

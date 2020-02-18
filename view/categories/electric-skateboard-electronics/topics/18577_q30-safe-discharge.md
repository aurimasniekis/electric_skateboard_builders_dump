# Q30 Safe Discharge

### Replies: 3 Views: 485

## \#1 Posted by: NickTheDude Posted at: 2017-03-05T07:11:59.984Z Reads: 80

```
So I was thinking about ordering some Carvon V3 dual hubs but I wasn't sure if the Miami Electric Boards 12S2P would be able to reliably provide enough current. On their Kickstarter it says the V3 is rated for a total of 2000W so presumably that is 12S fully charged at 20A to each wheel (50.4 x 20 x 2 = ~2000). The miami battery uses Q30 cells which are rated at 15A. However I've also heard that Q30 cells are capable of 20A continuous. Do you think it would be okay to set the battery amp max to 20 or should I lower to 15A or perhaps even lower? Thanks.
```

---
## \#2 Posted by: Namasaki Posted at: 2017-03-05T08:05:49.503Z Reads: 71

```
I used to run dual Carvon V2 motors (which where Higher KV than V3) on 12s and tested total amp draw from the battery while climbing a 10% grade and the total combined current drawn by both motors was less than 20a. 
I suggest that you give it a try with your battery and your battery max set at 15a for each Vesc. This will keep you within the working range of your battery. 
And check with Jerry at Carvon for recommended motor max current. 
If your mostly riding flat, you should be fine. 
If your charging hills a lot then have a meter on top or some way to monitor your voltage sag under load. 
That will show if your battery can meet your motors demands. And if the sag is too much, you might consider a larger pack or switching to Lipos for more power.
```

---
## \#3 Posted by: Namasaki Posted at: 2017-03-05T08:21:59.881Z Reads: 61

```
Btw, referring to the 2000 watt rating of the combined motors, I believe what that means is that the motors can handle enough voltage and current to produce 
2000 watts. But the wattage produced by the motors will be limited by the current settings in the Vesc which will prevent the battery from being over taxed.
```

---

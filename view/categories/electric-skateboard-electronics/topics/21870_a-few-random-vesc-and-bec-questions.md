# A few random vesc and bec questions

### Replies: 3 Views: 1003

## \#1 Posted by: ieatflys Posted at: 2017-04-27T01:14:37.489Z Reads: 87

```
A few random questions about the vesc from diy skateboards.....     

1. what in the heck is the plug on the sensor port?? They wont tell me they just tell me to buy there adapter( 7 bucks. X4)   i thought it was a balance tap connector so i grabbed a few and there too big.  Any reccommendations?

2. Top ways of blowing up the vesc to avoid? If i set my max amps to the motor and from the battery correctly. Wont that keep it from every blowing up via hard use?

3. Is foc SAFE to use now a days WITH SENSORS? I know a while back it was more of a betta thing and blew allot of stuff up.... how safe is it to use now a days with a sensored motor? Any special order of setting it up. Or just go to foc calibrate the sensors and whatnot then change a few parameters? 

4. Im using a 12s bms from ebay(from china)  when i go to charge the batteries do i need to supply the exact voltage that i want the batteries to charge to or can i go a little over and the bms will chsrge it to the full 4.2v safely?    And how much drain will this have on my pack? Do i need to be unhooking it when its unused for a week or month at a time? It was my understanding that it kept the pack balanced 24/7... am i correct?
```

---
## \#2 Posted by: Namasaki Posted at: 2017-04-27T06:10:51.818Z Reads: 67

```
1. My recommendation is to buy the adapter for the sensor cable for a sure easy solution.

2. The most common way of burning up the vesc is to burn up the DRV chip by exceeding the erpm limit of 60k. Follow the recommendations in the thread linked below and your worries are over.
3. FOC has become a lot more reliable these days as long as you buy from a reputable vendor who sells Vesc that have the components necessary for reliable FOC operation.
4. Do not charge your 12s pack with a voltage above  50.4v which is the full charge voltage for a 12s Lipo or Li-ion pack.
Note: Cheap eBay bms's have been known to be unreliable,
It really is not a good idea to go cheap with batteries, electronics and motors.
Especially with a bms. Saving a few bucks on the bms could cost you your batteries.

https://www.electric-skateboard.builders/t/choosing-the-right-motor-kv-for-the-vesc/3125
```

---
## \#3 Posted by: ieatflys Posted at: 2017-04-27T06:38:24.397Z Reads: 57

```
thanks... id like to solder the correct connectors tothe motors so they fit the vesc so if theres anyway to find out what the plug is that would be helpful

as for the bms i could not find a 12s lipo bms anywhere else besides ebay i haven't read anything bad about them yet.
```

---

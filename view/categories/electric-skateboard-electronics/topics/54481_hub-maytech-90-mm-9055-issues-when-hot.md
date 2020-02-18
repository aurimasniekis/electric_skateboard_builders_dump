# Hub Maytech 90 mm 9055 issues when hot?

### Replies: 14 Views: 869

## \#1 Posted by: sayreul Posted at: 2018-05-05T14:07:47.929Z Reads: 160

```
hello, 

i have build a board with 2 FOC box , 1 custom 10S3P and a dual hub Maytech 9055

http://uploads.tapatalk-cdn.com/20170725/124bb485e6abd329a28e66dffb8178d2.jpg

I use it in sensored / foc mode. 

I works really well when the board is "cold" but after a few miles, I sometimes have less power or cogging at startup. 

do you think it can be a problem with sensors ? or just with the motor ? 
i will try without sensors but if you have any similar experience ... 

thanks 

Cyril
```

---
## \#2 Posted by: bevilacqua Posted at: 2018-05-05T14:17:16.519Z Reads: 149

```
do you monitor the vescs with a HM-Module (like the Metr Module)?
```

---
## \#3 Posted by: Naysh Posted at: 2018-05-05T19:24:13.235Z Reads: 132

```
What type of cells are you using?  It might just be voltage sag.
```

---
## \#4 Posted by: sayreul Posted at: 2018-05-05T20:32:03.568Z Reads: 115

```
Yes I have a Hm10 with metr app 

My battery is made of Sony VTC6 
It works really good , even with full power, when the motors are cold 

It it possible that I don’t have enough amp when my battery is around 35 V (after a ride - when motors are hot ... )
Issues are just for start , when I ride it is ok
```

---
## \#5 Posted by: Bolpix Posted at: 2018-05-05T22:29:00.366Z Reads: 109

```
I dunno how to help you but I just thought you had a really nice looking board
```

---
## \#6 Posted by: Naysh Posted at: 2018-05-06T01:35:06.981Z Reads: 97

```
What is max speed?  Is this something new that developed or a problem you've had since you built it?
```

---
## \#7 Posted by: sayreul Posted at: 2018-05-06T07:13:24.734Z Reads: 93

```
Thanks ! 

My top speed is between 35-40 km/h
I think I had the problem since beginning 

I will try without sensor and with battery discharged but motor colds  to identify the problems
```

---
## \#8 Posted by: Naysh Posted at: 2018-05-06T07:47:26.586Z Reads: 88

```
I don't own a hub motor myself and have never have tried it but from my understanding they inherently get hot because the urethane covers up the motor instead of leaving it exposed for cooling like outrunners. The design of the Maytech hubs seem to confirm this in that the heat is being trapped and when there's heat in your coils there's more resistance, slowing you down.  Other mainstream hubs like Meepo are integrated with the truck and have cone shape on the truck side for cooling as well as the truck helping dissipate the heat.  Plus they're limited to 35kph/22mph and tested at the factory to perform within these limits.

Also check the windings of the motor, a lot of times these motors rushed in mass production in China and the windings themselves are done poorly causing inefficiency.  If you have enough money to spare I would recommend buying @Hummie hub motors.  He hand winds them himself and checks that it is getting the right kv and is made of steel instead of aluminum.  If you can wait there is also Carvon direct drives which you can choose your own wheel but that is pretty much unavailable because its only 1 guy producing it and he's produced 25 in 8 months.

If I were you just go with belt driven or wait a couple more weeks for @Kug3lis to offer geared driven "direct" drives. Honestly this where the next level tech is.

If you do decide to remain in the hub motor game but just not Maytech hubs.  Raptor 2 offers hub motors but that'll cost you $800 per hub because they don't sell standalone hubs. You'll have to buy the complete then take apart the hub. You will have the best hub motors in the industry imo.
```

---
## \#9 Posted by: sayreul Posted at: 2018-05-08T19:01:21.034Z Reads: 63

```
hi, thanks a lot for your reply.
i was looking for carvon hub / direct drive. I think it is the best solution for eskate  : no pulley, no belt, but you can choose your wheels , ... 

i will try to fix issues on my maytech but I know that it is cheap quality...
```

---
## \#10 Posted by: Battosaii Posted at: 2018-05-08T19:08:44.481Z Reads: 61

```
It may be a hub motor thing cause my Raptor 2 does the same thing, when it's hot or the battery is low usually both things are happening at the same time I get cut outs  or cogging from a stop. Also brakes suck at high speed and they kick in hard at a lower speed
```

---
## \#11 Posted by: bevilacqua Posted at: 2018-05-09T09:20:13.045Z Reads: 53

```
Have you tired monitoring the Motor-Temp? 
What values do you get?

You have to take into consideration the higher Ohmic-Losses (High Amps->heat) and lack of cooling of those big Hubmotors.. 

So if the Motor-Temp limit is reached it can behave not normally.

Try limiting the Topspeed (via ERPM limit) and lower your Bat-Max, maybe that helps
```

---
## \#12 Posted by: Naysh Posted at: 2018-05-10T18:00:58.258Z Reads: 48

```
I found this thread from 2016. The hub motor looks like your Maytech ones. He had overheating problem when running an RC esc but when he switched to Vesc BLDC mode the motors ran cooler.  Try running it in BLDC and see what happens.
http://www.electric-skateboard.builders/t/electric-dual-hub-motor-disassembly-performance/2038/53
```

---
## \#13 Posted by: sayreul Posted at: 2018-05-10T20:30:40.937Z Reads: 42

```
Thanks for your reply 
It seems to be a temperature issue.  I will try to monitor motor temperature and I will check if I still have issue when I wait 20 min ...
I will keep you informed.  Thanks
```

---
## \#14 Posted by: themegak Posted at: 2018-05-10T21:27:54.187Z Reads: 34

```
it sounds like classic voltage sag.
```

---

# Breaks not working properly - vesc flashes red 3x at full break throttle - photos of vesc settings attached

### Replies: 21 Views: 1138

## \#1 Posted by: lennylogs Posted at: 2018-04-09T00:51:32.778Z Reads: 125

```
This is my first build and the breaks on my board don't seem to be working properly....they are pretty weak to begin with and when I pull the break throttle all the way, they don't connect at all. My board is a 10s4p 30q dual drive and the vescs are focboxs. 

I've attached photos of the BLDC tool settings: 

Any ideas as to what the issue is? 

Thanks 

![vesc 1|690x393](upload://v0rbiuLqo9BEhZ1meCdUtW7kg1.png)

![vesc 2|690x392](upload://5Vr3mVlpp6lTyOMffPrCJYgMm5.png)

![vesc 3|690x392](upload://6qK4YlVqp8fotITh1pBBNKs3SBf.png)

![vesc 4|690x392](upload://vE8HtPrkX4lVjyjghJ4MsQFs4ZY.png)
```

---
## \#2 Posted by: goldrabe Posted at: 2018-04-09T01:17:12.896Z Reads: 111

```
Try to up your Motor max to 60A and the Motor min to -40A.
Are you running Hubs or Belts?
```

---
## \#3 Posted by: lennylogs Posted at: 2018-04-09T01:29:13.697Z Reads: 110

```
Thanks for the response  - Im running belts - I should up the motor max to 60a even though its dual drive?
```

---
## \#4 Posted by: goldrabe Posted at: 2018-04-09T02:07:25.880Z Reads: 108

```
What kind of motors are you running? 6355? 6374?
Find out your max motor Wattage and divide that by your Battery's Voltage to find out the maximum you can go.
ex. 2500W / 10S(10X3.7)= 67.6A
I got advise to uncheck Limit ERPM with negative torque to get better braking.
```

---
## \#5 Posted by: Namasaki Posted at: 2018-04-09T04:14:28.666Z Reads: 95

```
[quote="lennylogs, post:3, topic:51634"]
I should up the motor max to 60a even though its dual drive?
[/quote]


Yes, you only need to adjust the Batt Max and Batt Min for dual drive.
Keep Motor max and Motor min same as single drive.
```

---
## \#6 Posted by: lazerusrm Posted at: 2018-04-09T12:16:31.010Z Reads: 82

```
Double Check your throttle settings / PPM as well, make sure that you've correctly followed the wizard so that you have full range on braking... Because you should have brakes even with your settings.
```

---
## \#7 Posted by: lennylogs Posted at: 2018-04-09T16:53:17.074Z Reads: 68

```
thanks for the input @Namasaki @goldrabe @lazerusrm

I'm running dual 6374 3200w motors - so i'll change the motor max and motor min to 86A and uncheck the "limit ERPM with negative torque" box, but leave everything else the same....I'll test that out tonight. That is a huge difference in motor max and motor min than what I had lol
```

---
## \#8 Posted by: goldrabe Posted at: 2018-04-09T22:08:25.204Z Reads: 58

```
Take it easy bro, don't go to the max straight away. Leave some headroom.
And as @Namasaki said the battery max and battery min settings are the more important ones, they determine how much current your battery pack delivers or receives. (regenerative braking)
```

---
## \#9 Posted by: goldrabe Posted at: 2018-04-09T22:15:21.978Z Reads: 58

```
This is a recent thread about weak brakes.I think it's a good read, with mentioning of Vesc settings.(http://www.electric-skateboard.builders/t/is-braking-force-related-to-motor-kv-or-motor-size/51496)
```

---
## \#10 Posted by: lennylogs Posted at: 2018-04-09T23:05:03.901Z Reads: 55

```
okay so i changed the settings to 75a motor max and 40a motor min. and I found that the breaks actually work really well, EXCEPT when I pull the break throttle all the way. When I pull the breaks all the way (or even just a little too far after a certain point), the board doesnt break at all the the vescs actually flash red three times.

I tried playing around with the "max ERPM at full break" and "max ERPM at full break in current control mode" values, but couldnt notice any change. also no noticeable change regardless of wether or not I checked the "limit ERPM with negative torque" box 

So the board is ridable, I just have to be careful not to pull the breaks too hard or they will totally disconnect....any one have any ideas?
```

---
## \#11 Posted by: pat.speed Posted at: 2018-04-09T23:08:21.822Z Reads: 52

```
What remote do you have?  Could it be you accidentally moved the trim knobs on the remote? 

I would redo the remote setup and turn on the real-time data so you can see the ppm pulses, if using ackmaniacs tool
```

---
## \#12 Posted by: lennylogs Posted at: 2018-04-09T23:14:26.146Z Reads: 47

```
maytech remote...I dont think I moved any trim knobs. I was thinking of re-trying to configure the vescs on ackmaniacs tool to see what happens
```

---
## \#13 Posted by: pat.speed Posted at: 2018-04-09T23:19:30.687Z Reads: 45

```
Hmm yeah that would be your best bet, it’s super easy, for some reason though the first time you do it you need to use the wizard.
```

---
## \#14 Posted by: lennylogs Posted at: 2018-04-09T23:58:08.770Z Reads: 42

```
I think it is related to the ppm pulses....Using the bldc tool i was able to make it better but still not perfect yet. Will keep playing around
```

---
## \#15 Posted by: goldrabe Posted at: 2018-04-10T00:02:29.417Z Reads: 39

```
I have seen many posts with the same issue, but mainly in foc. But no one came to a solution in the threads i am aware of.
How long are your wirings from the battery towards the VESC's?
I had the same issue in foc and switching back to bldc solved the issue.
Would be nice to hear what is causing the dropouts, one of my wild guesses is that too long wiring might cause voltage spikes during braking.
Hopefully someone more knowledgeable will chime in.
```

---
## \#16 Posted by: pat.speed Posted at: 2018-04-10T00:08:35.629Z Reads: 38

```
Try changing the minimum pulse width higher and lower and see if anything changes. I would also recommend getting Accs tool as it calculates the max and min exactly to your remote
```

---
## \#17 Posted by: lennylogs Posted at: 2018-04-10T00:22:50.187Z Reads: 37

```
I dont think its the wiring from the battery as its not that long and @barajabali made it for me. Im pretty sure its related to setting the ppm as ive gotten close to fixing it but its still not perfect. If i set to too far one way then the motor spins when im not touching the remote and if i set it too far the other way then the same breaking issue occurs
```

---
## \#18 Posted by: lennylogs Posted at: 2018-04-10T00:25:57.996Z Reads: 35

```
Thats what ive been doing but i cant get it perfect. Going to download acmaniacs tool and try there. 

On a side note, ive also learned that its best to play around with these settings while the truck/motors/wheels are secured to an upsidedown board.....
```

---
## \#19 Posted by: goldrabe Posted at: 2018-04-10T00:27:53.359Z Reads: 36

```
I had set my remote dead on when having this issues. But your battery wiring seems to be fine! If it's just ppm then it's a easy solution.
```

---
## \#20 Posted by: lazerusrm Posted at: 2018-04-10T05:19:01.179Z Reads: 32

```
Make sure you are using the latest tools from vesc-project, or ackmaniac.

In the PPM Settings you can set "Deadzone" which effectively increases your play near the center of your throttle between forward and reverse if you need to. 

If you use the input setup wizard, you should be able to see your throttle real time both forward, and brake. Make sure you apply your PPM throttle settings.
```

---
## \#21 Posted by: Edward_Spud Posted at: 2018-04-14T14:11:01.437Z Reads: 27

```
Arrrggg....Brakes not Breaks.

If the OP is intelligent enough to configure a VESC (which being honest I'm not all that confident doing myself), surely a simple spelling correction is not too much to ask ;)
```

---

# Power Cut-off with acceleration *please help*

### Replies: 61 Views: 369

## \#1 Posted by: Z4MSupreme Posted at: 2019-04-12T11:36:50.455Z Reads: 91

```
I have recently finished my board and have test ridden it briefly. i have made a 10s3p samsung 30q pack with an 80A bestech bms and a hobyking VESC. i have the max current as 45A on the vesc and the soft voltage cutoff enabled on the vesc. 

sometimes when accelerating, the power will cut off and i can see the level on my percentage indicator drop. if i keep my remote accelerating it will drop to 0% and then the power will cut off and everything shuts off, including the vesc. 

however if i stop accelerating the percentage rises and im still able to brake. there is no red light on the vesc so i dont think there is a fault. 

could it be the voltage cutoff on the vesc. (could i lower the cutoff voltage and rely on my bms??) or maybe my max current. Im able to switch my board back on and everything works, except it will cut off on acceleration again, Im guessing it is not a hardware fault but a software fault. 

any help would be much appreciated.
```

---
## \#2 Posted by: TheSebas Posted at: 2019-04-12T11:50:59.140Z Reads: 77

```
Maybe you can show your VESC settings 🧐
It is possible to set the voltage cut off lower, i had the same thing with not being able to accelerate but having the brakes.
```

---
## \#3 Posted by: Z4MSupreme Posted at: 2019-04-12T11:52:28.635Z Reads: 73

```
ok. will check now. shall i show you the baterry settings and motor settings?
```

---
## \#4 Posted by: TheSebas Posted at: 2019-04-12T11:53:29.919Z Reads: 72

```
The cut off voltages are most important, but you can show them all :)
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-04-12T11:53:43.768Z Reads: 71

```
We also need to know what motors your using and you gear ratio

Also a 10s3p with 30q you can discharge 60a through the pack no Problem
```

---
## \#6 Posted by: Z4MSupreme Posted at: 2019-04-12T11:57:12.266Z Reads: 69

```
i am using a 6374 149kv motor with 15/36 gear ratio and 100mm wheels.

i thought that the max discharge from each cell was 15A so 45A when in parallel????
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-04-12T11:58:14.269Z Reads: 68

```
[quote="Z4MSupreme, post:6, topic:90246"]
15A
[/quote]

Samsung underated them

In actuality they can do 20a per cell

And your gear ratio seems to be fine
```

---
## \#8 Posted by: Andy87 Posted at: 2019-04-12T12:07:36.719Z Reads: 65

```
where did you buy your cells from? you sure they are not fake cells?

did you check your battery and vesc connectors? If there is a bad solder join or the xt plug is not plugged fully that can happen.

is it a single drive board? I can´t see that out of your explanation.
45A for bat max is already a lot for a hk vesc.
Does the cut out come directly from the beginning if you accelerate hard, or only after some minute of driving?
```

---
## \#9 Posted by: Z4MSupreme Posted at: 2019-04-12T12:07:47.416Z Reads: 59

```
wow, didnt realise. do you suggest increasing current max?
```

---
## \#10 Posted by: Z4MSupreme Posted at: 2019-04-12T12:09:13.935Z Reads: 57

```
I bought my cells from NKON. im sure they are real cells. all connections are fine, and the electronics are fine when im lightly accelerating. it is a single drive. it cuts off after a few seconds.
```

---
## \#11 Posted by: Z4MSupreme Posted at: 2019-04-12T12:10:10.445Z Reads: 57

```
![image|690x388](upload://oCPpBGdiyxrittLop7jHctwWcP.png) ![image%20(1)|690x388](upload://vPkvvE4XAItzacgUxwN07WafuoH.png) 

here are my VESC settings :slight_smile:
```

---
## \#12 Posted by: Andy87 Posted at: 2019-04-12T12:10:11.673Z Reads: 56

```
does that happen only if you stand on the board or also without load.
like you lift up the deck and accelerate fully.
```

---
## \#13 Posted by: Z4MSupreme Posted at: 2019-04-12T12:10:55.670Z Reads: 55

```
it only happens when i am on the board. i tried doing it without load and it was fine
```

---
## \#14 Posted by: Andy87 Posted at: 2019-04-12T12:11:55.763Z Reads: 54

```
nkon cells are good.
cut off limit looks good as well.

Settings also, but i wouldn´t go higher than 35A batt max. try with 30A and look if it get better.
```

---
## \#16 Posted by: Z4MSupreme Posted at: 2019-04-12T12:17:47.578Z Reads: 55

```
by making the cut off lower would that not make it more likely to cut out? Im a bit of a noob :zipper_mouth_face:
```

---
## \#17 Posted by: Andy87 Posted at: 2019-04-12T12:17:57.216Z Reads: 57

```
I mean you should set the battery max value down to 30A.
That means that your vesc is limited to 30A current draw which result in less heat on your controler.  He just doesn´t draw more than 30A from your battery.
```

---
## \#18 Posted by: Z4MSupreme Posted at: 2019-04-12T12:19:26.104Z Reads: 56

```
[quote="Andy87, post:17, topic:90246"]
t doesn´t draw more than 30A fr
[/quote]

ok, i will give that a go later. do i had only been riding back and forth on my road for a couple of minutes. do you think it would have got that hot quickly?
```

---
## \#19 Posted by: Andy87 Posted at: 2019-04-12T12:22:09.611Z Reads: 56

```
it´s a single drive. that can be. I had once a single drive. took me 2 min driving average speed till it hit the over temp protection.

Usually the over temp protection just cut down your power output, so you feel that the acceleration will become less like the battery cut off does as well. It shouldn´t be a total shut down like in your case, but well it´s worth a try and in general not wrong to set the limit like this on this VESC.
```

---
## \#20 Posted by: Z4MSupreme Posted at: 2019-04-12T12:26:26.785Z Reads: 56

```
I understand now. So I should decrease the current to 30A to stop the over temp?? Anything else I can do to combat this?
```

---
## \#21 Posted by: Andy87 Posted at: 2019-04-12T12:28:50.462Z Reads: 53

```
air flow around the vesc or bigger heat sink helps as well.

If you would have a bluetooth module we could log your ride and look what was the reason. It doesn´t need to be overtemp. I guess it´s more likely something else.
```

---
## \#22 Posted by: goldrabe Posted at: 2019-04-12T12:36:26.984Z Reads: 51

```
I had a similar issue and it was caused by a bad P group in my battery pack which would lead to a complete shutdown. Can you check the total Voltage of your pack when fully charged? One of your P groups could have become unbalanced.
```

---
## \#23 Posted by: Z4MSupreme Posted at: 2019-04-12T14:48:26.180Z Reads: 46

```
If it were a bad cell would the board not do that as soon as i get on? i also charged it very recently so dont think its an issue......:confused:
```

---
## \#24 Posted by: Z4MSupreme Posted at: 2019-04-12T15:24:23.827Z Reads: 43

```
do you think that i should also decrease cutoff voltage to 31V and 28V?? As i also have a bms that will cut out just in case??
```

---
## \#25 Posted by: AlanZhou Posted at: 2019-04-12T15:26:29.422Z Reads: 44

```
With 3p you will sag a lot below 30v

Even though the full end discharge it the 30q is 2.5v
```

---
## \#26 Posted by: RyuX Posted at: 2019-04-12T15:27:49.560Z Reads: 42

```
I had a similar problem where my BMS would cut the power because of some random error (overcurrent or short circuit).
Does your BMS have a error log ?
```

---
## \#27 Posted by: Z4MSupreme Posted at: 2019-04-12T15:32:00.909Z Reads: 37

```
No, the bestech bms' are not smart ones so there are no fault logs :frowning:
```

---
## \#28 Posted by: Z4MSupreme Posted at: 2019-04-12T15:33:16.370Z Reads: 36

```
When researching i saw that a lot of people ran 10s3p without any problems, do you have any suggestions on how i could try and sort it out?
```

---
## \#29 Posted by: AlanZhou Posted at: 2019-04-12T15:33:46.988Z Reads: 37

```
No I'm just saying anything below 30v will sag a lot because at that point the cell has no capacity
```

---
## \#30 Posted by: RyuX Posted at: 2019-04-12T15:35:00.666Z Reads: 37

```
Can't say about 10S3P but with my 12S3P I never have any issues and I can go for around 30-40km on one charge and never face any problems with sag that will cause a cutoff.
```

---
## \#31 Posted by: Z4MSupreme Posted at: 2019-04-12T15:36:58.394Z Reads: 37

```
I think 12s would be more efficient meaning less sag but didnt think it would mean that i cant even accelerate :confused::confused:
```

---
## \#32 Posted by: Z4MSupreme Posted at: 2019-04-12T15:38:21.892Z Reads: 37

```
ok. but surely i have there is enough voltage from 4.2v to stop it from cutting out as soon as i accelerate?
```

---
## \#33 Posted by: AlanZhou Posted at: 2019-04-12T15:38:51.557Z Reads: 35

```
Yes the problem may lie in your bms or vesc
```

---
## \#34 Posted by: RyuX Posted at: 2019-04-12T15:39:06.125Z Reads: 36

```
Well.. there is another possibility.. I had a cold solder joint on my DRV8302 and it also made my board cut out while accelerating.. quite randomly. You sure your VESC is OK?
```

---
## \#35 Posted by: Z4MSupreme Posted at: 2019-04-12T15:39:45.145Z Reads: 34

```

![IMG_20190411_203437|666x499](upload://qIbo809kaxJ4CXzdqHi7urErdLi.jpeg) ![IMG_20190411_214133|666x499](upload://3bXc32SLVeFy0pTLkRjVy2iBDM6.jpeg) 

i dont have any space to add more cells as i have made this carbon firbe deck and it doesnt have enough space :expressionless:
```

---
## \#36 Posted by: RyuX Posted at: 2019-04-12T15:40:33.866Z Reads: 34

```
Do you use the BMS only for charging or also for discharge ?
```

---
## \#37 Posted by: drone001 Posted at: 2019-04-12T15:43:01.227Z Reads: 35

```
isn't the carbon fiber conductive to a certain point. I'm new but i think I read that some whwere. also what about a kickoff to get the board going before giving it juice. I also read that somewhere. Like I said I'm new so just giving my 2 cents.
```

---
## \#38 Posted by: Z4MSupreme Posted at: 2019-04-12T15:43:08.375Z Reads: 35

```
i use it for charging and discharging, it is rated for 80A
```

---
## \#39 Posted by: Z4MSupreme Posted at: 2019-04-12T15:43:29.927Z Reads: 35

```
![IMG_20190412_164148|375x499](upload://A6yQOT1448Mwtm2nlIlfcIRm5cD.jpeg) 

the solder joints seem to be ok......
```

---
## \#40 Posted by: RyuX Posted at: 2019-04-12T15:43:55.917Z Reads: 34

```
Well just for sanity check I would try to bypass the BMS for a testrun... at this point you also have to keep in mind that your problem might be hardware related
```

---
## \#41 Posted by: Z4MSupreme Posted at: 2019-04-12T15:44:36.127Z Reads: 35

```
yeah, thats what im thinking, maybe an incorrect setting in the vesc. wouldnt i fry the bms if there was too much current?
```

---
## \#42 Posted by: RyuX Posted at: 2019-04-12T15:44:56.341Z Reads: 36

```
a DRV8302 cold solder joint can't be seen with the eye - not even with a loupe.. also the DRV8302 is on the other side of the board. So is this a good known to be working, VESC ?
```

---
## \#43 Posted by: Z4MSupreme Posted at: 2019-04-12T15:46:06.744Z Reads: 37

```
thanks for the help, it shouldnt be the carbon fibre as everything is covered in heat shrink. the acceleration things happens when im already moving and accelerate more
```

---
## \#44 Posted by: Andy87 Posted at: 2019-04-12T15:46:52.862Z Reads: 36

```
Short off topic thing. You about to cut your balance wire with the nickel here.
![image|329x499](upload://q6XdpAEb550axcpjXhI7bUZKeTa.jpeg) 


I would Route that balance wire a bit different.
```

---
## \#45 Posted by: Z4MSupreme Posted at: 2019-04-12T15:47:04.841Z Reads: 34

```
I dont know if it is known to be working as i havent been able to use it on another board. should i contact hobbyking as they have a 1 year warranty?
```

---
## \#46 Posted by: Z4MSupreme Posted at: 2019-04-12T15:47:47.227Z Reads: 34

```
thanks, i will change that :slight_smile:
```

---
## \#47 Posted by: RyuX Posted at: 2019-04-12T15:48:41.282Z Reads: 35

```
Well first you have to find out if it actually is the VESC.. so try to run directly without BMS for a short test run.. then contact hobbyking
```

---
## \#48 Posted by: drone001 Posted at: 2019-04-12T15:49:17.520Z Reads: 34

```
thx...this is a learning process for me as well.
```

---
## \#49 Posted by: Z4MSupreme Posted at: 2019-04-12T15:49:18.303Z Reads: 34

```
ok, will give that a go. thanks
```

---
## \#50 Posted by: Z4MSupreme Posted at: 2019-04-12T15:49:39.154Z Reads: 34

```
me too. its a pretty steep learning curve.
```

---
## \#51 Posted by: Z4MSupreme Posted at: 2019-04-12T15:50:02.891Z Reads: 32

```
especially when things dont work :tired_face:
```

---
## \#52 Posted by: RyuX Posted at: 2019-04-12T15:50:53.315Z Reads: 32

```
Also if you feel like experimenting you could build a small "street" simulation and get something to hold back the wheel while accelerating with the remote inside your house and have the VESC Tool log the activity (if you have a bluetooth module its quite easy - otherwise connect USB)
```

---
## \#53 Posted by: drone001 Posted at: 2019-04-12T15:51:20.773Z Reads: 32

```
indeed.....I'm reading for an hour + a day on this site. It's a lot to learn sorta addictive in a way.
```

---
## \#54 Posted by: Z4MSupreme Posted at: 2019-04-12T15:52:46.767Z Reads: 32

```
great idea. thanks. i dont want to stop the motor from spinning but just slow it down right?
```

---
## \#55 Posted by: RyuX Posted at: 2019-04-12T16:01:16.918Z Reads: 32

```
You just want to build something that simulates the "street" friction... maybe build a small setup or carefully have a longer piece of wood to create friction.. I once used two unused trucks with wheels and a small break to simulate a road on my first build.. get creative but be careful that you don't hurt yourself.. those motors got power :slight_smile:
```

---
## \#56 Posted by: Z4MSupreme Posted at: 2019-04-12T16:02:49.320Z Reads: 33

```
great. thanks a lot :+1:
```

---
## \#57 Posted by: goldrabe Posted at: 2019-04-12T16:38:19.384Z Reads: 32

```
No, if it´s a bad or unbalanced P group the BMS will cut power whenever that P group reaches 2.8V.
That would explain why your capacity meter drops so dramatically. In my case the BMS cut the power at 50% or roughly 36V. 4 of my 5 P groups where at 3.8V and one group at 2.8. Just try to take measurings of your P groups at the JST balance wire cnnector of your BMS. There are plenty of videos on youtube how to do that.
```

---
## \#58 Posted by: Z4MSupreme Posted at: 2019-04-12T16:57:47.197Z Reads: 31

```
Just as you replied I figured out the problem and you are correct. I couple of weeks ago, while not riding, my vesc would not turn on because my BMS kept cutting out. I found out that I had an unbalanced cell. I charged the board and they were all balanced but the cell must've become unbalanced again. I think that is the problem I'm facing. 

So I need to replace the faulty group of cells and replace them with some new ones right.???

Thanks for your help
```

---
## \#59 Posted by: goldrabe Posted at: 2019-04-12T17:07:52.573Z Reads: 31

```
Your BMS can only balance a certain amount of difference, if your cell drifted beyond that you need to charge the P group individually. Does your capacity meter shows 42V at the end of charge? You only need to replace the P group if they are dead already. You can replace the P group if your cells are not too old.
```

---
## \#60 Posted by: Z4MSupreme Posted at: 2019-04-12T17:57:05.783Z Reads: 30

```
it shows 42v when fully charged but they seem to discharge more and become unbalanced
```

---
## \#61 Posted by: Z4MSupreme Posted at: 2019-04-17T21:55:53.437Z Reads: 23

```
I've just wired in some new batteries. Before I wired them in they were at 3.6V. I put the pack on charge but the new cells remained at 3.6v and all the others were balanced to 4.2V. do you think it is an issue with teh BMS?
```

---
## \#62 Posted by: Z4MSupreme Posted at: 2019-04-17T21:57:09.507Z Reads: 24

```
The voltmeter Alos shows the pack as 42V at the end of a charge.
```

---

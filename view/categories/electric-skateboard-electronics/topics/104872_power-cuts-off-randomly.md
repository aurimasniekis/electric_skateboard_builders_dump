# Power cuts off randomly

### Replies: 7 Views: 164

## \#1 Posted by: vmazsit Posted at: 2019-12-21T12:28:21.107Z Reads: 55

```
Hey!
I need some help for my DIY Electric Skateboard.
So the issue is my board is sometimes just stops (it's like somebody just turned off the main power...)and i need to disconnect the battery to make it run again. 

My battery is a :
![79645524_600518707444819_6327076594737217536_n|375x500,50%](upload://tWOP1iLbO9mmUd5zAaCljsoQ1yy.jpeg) 

and I have 10 of them so it's a 10S battery pack. (there is no parallel connection)

My BMS :![81491665_591422758309709_354773764757520384_n|375x500,50%](upload://liweP11KDyoH7ExMHXYRbuIP3iB.jpeg) 

And my ESC and motor are these : ![80123183_815803302218618_2152722936870469632_n|666x500,50%](upload://mrtNylRZXl0ecu8XUgO2sp4Cud5.jpeg) ![80345864_2936238143128621_3314555605263319040_n|666x500,50%](upload://n8icihtxE2cCo1qXynFY227Vtqf.jpeg) 
(Single belt motor 6354/190KV)

My ESC is works with 10S batteries.
I can't figure it out what causes the stops. I think it's the batteries or the BMS but my batteries are capable of 30A so I really don't know what to do. 

Thank you in advance for your answers. If you need more infs. or you don't understand something let me know.(English is not my native language so I apologize for that :(  )
```

---
## \#2 Posted by: Andy87 Posted at: 2019-12-22T12:55:23.473Z Reads: 35

```
Hi!
There some things to consider.
The cells are high discharge and high capacity and I have never seen them. Very likely they not what they labeled at. 3Ah and 20A discharge is pretty much top end with 18650 cells.
Next thing is your bms. Did you wire it up for charge and discharge or did you bypass the bms for discharge.
Without knowing much about your setup I would guess, either your bms cut out if it’s wired up for charge and discharge because you draw too much current, or your bms cut out because your cells sag so much that you come in the undervoltage area.
You might want to post that as well on forum. and get probably more responses to your problem
```

---
## \#3 Posted by: deucesdown Posted at: 2019-12-22T15:38:00.926Z Reads: 32

```
Keepower is a good rebrander. Or at least they were good many years ago. Not sure now because there's no 3000mah 18650 cell that can do 30a continuous.
```

---
## \#4 Posted by: Soflo Posted at: 2019-12-22T19:36:29.150Z Reads: 26

```
Dude,  you need a bigger battery.  That 10s1p isn't enough.  Go with 4p or more.
```

---
## \#5 Posted by: DucatiGuy Posted at: 2019-12-30T04:42:56.295Z Reads: 18

```
Check your power switch...
```

---
## \#6 Posted by: Wilsonliang777 Posted at: 2019-12-30T08:28:57.171Z Reads: 14

```
I think you need to build a new battery.   10s1p battery is not enough.  And the battery cell that you have is mostly fake mAh and discharge rate.
```

---
## \#7 Posted by: whaddys Posted at: 2019-12-30T08:48:51.282Z Reads: 12

```
I thought the title of this thread was referring to the esk8.builders website rather than a board at first =/
```

---

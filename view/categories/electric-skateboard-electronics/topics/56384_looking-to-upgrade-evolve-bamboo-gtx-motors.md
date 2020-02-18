# Looking to Upgrade Evolve Bamboo GTX Motors

### Replies: 20 Views: 2129

## \#1 Posted by: Scoobs Posted at: 2018-05-22T18:29:58.555Z Reads: 210

```
Hello,

I have an evolve bamboo gtx with AT wheels.  I am planning to have LHB upgrade my battery later this year to the 18650 based 10S4P lithium ion pack with 30Q samsung batteries.  With the better battery I would like to beef up the motors too for at least an extra 5 mph in top speed but I don't want to sacrifice too much torque.  Would I be better off with 190kv motors over 200kv?  Also, should I stick with 5065 motors or maybe 6355 like another member suggested?.  

I just want a little more speed but I don't want to fry the electronics and looking for a simple plug and play upgrade.  What motors do you think would work well with the better LHB battery?
```

---
## \#2 Posted by: Hummie Posted at: 2018-05-22T18:33:57.481Z Reads: 204

```
Same voltage battery?  What kv are the original motors.  ?
The speed determined by kv n voltage.   Torque by kv and what the esc sends to motor.
```

---
## \#3 Posted by: b264 Posted at: 2018-05-22T18:41:54.361Z Reads: 199

```
The original motors are dual 5065 at 150kv
```

---
## \#4 Posted by: Hummie Posted at: 2018-05-22T18:44:29.736Z Reads: 189

```
So if u went up to 190kv ull go way up in speed but down in torque. Can u adjust the esc output?  Otherwise it's torque OR speed choice

Might as well just get diff pulley n save bucks.

Without controlling esc output...the new battery...doesn't have much point.
```

---
## \#5 Posted by: b264 Posted at: 2018-05-22T19:17:41.865Z Reads: 176

```
I don't know of any way to adjust the ESC.  But you can use one 140kv and one 200kv motor....
```

---
## \#6 Posted by: Scoobs Posted at: 2018-05-22T19:23:28.828Z Reads: 171

```
I'm a novice and not sure what can be adjusted.  So the battery mod basically only increases my range and reduces battery lag?  Well I still plan on upgrading the battery for those reasons.  

So when you say get a different pulley are you talking about for instance changing to the boardbumpers 58T drive gear or something else?  This seems like the simplest way to increase the top speed but again I lose torque.  Without building a DIY board I was hoping there were some simple tweaks I could make for higher speed without losing too much torque.
```

---
## \#7 Posted by: Hummie Posted at: 2018-05-22T19:37:40.647Z Reads: 167

```
Yea as u say ull get more range n less sag but unless u can alter the esc output its going to be a trade of speed for torque.  Maybe u could add another cell in series n that would get u more speed.   I bet if u look other people have tried to increase esc output or the extra cell.
```

---
## \#8 Posted by: Scoobs Posted at: 2018-05-22T20:06:37.503Z Reads: 161

```
Would I need a larger enclosure to add an extra cell in series?   I was thinking about asking LHB if this is a viable option for my board.  I don't care if it no longer looks stock.  I'm also not sure about shaving down more of the board to fit the battery mod.  I guess I'd have to find an enclosure that had the same holes so I don't have to drill more holes into the board which may not even be available.  This seems like shit Evolve should offer.
```

---
## \#9 Posted by: Lumaci Posted at: 2018-05-22T20:46:50.958Z Reads: 154

```
You can buy a spacer you can install onto the enclosure so you wont need to do anything to the deck, its 50 bucks theres a link somewhere on the forum about it.

One made out of foam or anything else will also work no need to replace it :-)
```

---
## \#10 Posted by: Jesk8 Posted at: 2018-05-25T03:13:36.748Z Reads: 131

```
I'm actually thinking about doing the same not sure yet though. I have a bamboo gtx AT set up and i'm doing a 10s4p Samsung 30Q battery upgrade that i'm finishing up tomorrow. Everyone above is correct, higher KV means more top speed but lose out on torque. However, if you want both high speed and high torque you'll need to upgrade the diameter size of your motors (essentially bigger motors). I found that UNIKBOARDS(https://www.unikboards.com/en/boutique/motor-mount-for-evolve/) actually has a custom motor mount that allows you to mount 63mm motors.

Btw adding more cells in series will not give you any speed boost only range really and DON'T DO THIS if you plan on using Evolve's stock BMS. The BMS only recognizes 10s4p pack or anything of same voltage, the BMS will not function with a 10s5p pack or anything of different voltage.
```

---
## \#11 Posted by: Scoobs Posted at: 2018-05-25T17:45:05.705Z Reads: 122

```
Lumanci, a spacer sounds interesting.  Hopefully LHB agrees.

Also, thanks Jesk8 for the input on the motors.  Which 63mm motors were you looking at?  Do you already have them installed and if so, how are they working out?  I'd like to hear how they work with the battery upgrade.
```

---
## \#12 Posted by: egzplicit Posted at: 2018-05-25T17:58:48.081Z Reads: 117

```
[quote="Jesk8, post:10, topic:56384"]
The BMS only recognizes 10s4p pack or anything of same voltage, the BMS will not function with a 10s5p pack or anything of different voltage.
[/quote]

:smile: 

10s99999p is same voltage. Series increases voltage not parallel.

Bigger motors won’t work with original Evolve esc, those mounts are made for people doing diy builds based on evolve trucks.
```

---
## \#13 Posted by: Jesk8 Posted at: 2018-05-25T17:59:30.577Z Reads: 115

```
I actually haven't looked into any details on motors or anything I still have the stock motors on right now cause I want to just focus on the battery upgrade.
```

---
## \#14 Posted by: Hummie Posted at: 2018-05-25T17:59:53.529Z Reads: 113

```
in theory a bigger motor shouldnt give you more torque or top speed.  maybe you could get a bit more but it's power that wouldve been lost in the motor to inefficiency and cant be much

you should get more speed with more cells..if it blows up your stuff that's something else
```

---
## \#15 Posted by: Jesk8 Posted at: 2018-05-25T18:00:26.825Z Reads: 107

```
Yeah you're right mb. Something like a 12s4p pack wouldn't work
```

---
## \#16 Posted by: mechanicalturkey Posted at: 2018-07-24T19:15:38.168Z Reads: 93

```
[quote="Hummie, post:14, topic:56384"]
you more torque or top speed. maybe you could get a bit more but it’s power that wouldve been lost in the motor to inefficiency and cant be much

you should get more speed with more cells…if it blows up your stuff that’s something else
[/quote]

Hey jesk8,

I'm also looking into these 63mm motor mounts. Did you ever pull the trigger on these? I'm wondering if the stock motor controller will work with these.
```

---
## \#17 Posted by: Hummie Posted at: 2018-07-24T19:22:38.206Z Reads: 89

```
i just read what i wrote and its confusing

you could get more speed if the esc can handle more cells in series (should be able to find this out from people who tried)
you could get more torque if you can adjust the esc setttings and maybe also probably need adjust the bms too and be problematic if you cant find someone who has figured out how to do it already

but just putting different motors on ...there would be difference in speed or torque solely depending on the kv of the new compared to the old motors, similarly if you were to put a different pulley on, trading torque for speed or vise versa

other than that trading with different kv.....you will only get a hair more power with a bigger motor and only because a bigger motor is a bit more efficient.  you might not even notice.
```

---
## \#18 Posted by: brenternet Posted at: 2018-07-24T20:11:49.319Z Reads: 82

```
Not sure if you got this done but the most common motor replacement for the GTX is racerstar 140kv's and to a lesser extent 200kv's. 

People who are fed up with Evolve prices generally use these as a replacement when theirs eventually shit themselves. Plug and play.
```

---
## \#19 Posted by: craigthemachine Posted at: 2018-07-24T22:36:55.289Z Reads: 76

```
Yup, i have both sets of motors. I’ve tried both. The 200kv is way more fun.( speed) not healthy in the battery.

140kv, better torque , easyier on the battery. And not as fast.
```

---
## \#20 Posted by: craigthemachine Posted at: 2018-07-24T22:40:03.744Z Reads: 77

```
To add, the 200kv racerstar motors Runs the BMs kinda hotter than the 140kv, obviously due to more amps being pulled.
```

---

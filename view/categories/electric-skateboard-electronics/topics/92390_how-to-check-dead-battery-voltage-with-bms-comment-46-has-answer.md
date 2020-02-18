# How to check “dead battery” voltage with BMS (COMMENT 46 has answer)

### Replies: 56 Views: 882

## \#1 Posted by: DEEIF Posted at: 2019-05-01T02:02:16.951Z Reads: 182

```
Okay, so I haven’t used the battery in awhile but was planning on selling it to a friend so I went and looked at it and realized it was “bricked” I think.... here’s a pic of it, I tried charging it but nothing happens. Anyone know what’s wrong/how to fix? ![image|375x500](upload://osLX4bDPqdxrlgvHUmBKdSWExYf.jpeg)
```

---
## \#2 Posted by: threebysix Posted at: 2019-05-01T02:22:37.556Z Reads: 171

```
Get a volt meter and test to see if u have a voltage reading from the charging cable's barrel connector when plugged in to a outlet. 

Also, check to see what the voltage of the battery is. The pack might have over-drained due to lack of use.
```

---
## \#3 Posted by: Eboosted Posted at: 2019-05-01T02:34:19.682Z Reads: 167

```
Did you store it fully charged? That's the main reason batteries go dead after some time
```

---
## \#4 Posted by: b264 Posted at: 2019-05-01T02:35:59.292Z Reads: 167

```
[quote="threebysix, post:2, topic:92390"]
Get a volt meter and test to see if u have a voltage reading from the charging cable’s barrel connector when plugged in to a outlet.

Also, check to see what the voltage of the battery is. The pack might have over-drained due to lack of use.
[/quote]

Just to be clear, never stick voltmeter prongs in a charge port.  NEVER.

(I don't think that was suggested, but I want that to be clear :slight_smile: )
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-05-01T02:36:12.990Z Reads: 152

```
Uh oh you just alarmed @b264

@b264 thought you were gonna say, if the board ain’t stored at 100% then it ain’t a real means of transportation
```

---
## \#6 Posted by: threebysix Posted at: 2019-05-01T02:38:32.010Z Reads: 145

```
I was definitely not suggesting to do that (you were correct on your assumptions) :joy:
```

---
## \#7 Posted by: RedBaron Posted at: 2019-05-01T04:41:53.695Z Reads: 144

```
This is like the 5th battery I've seen in the past month made by tb with the same issue. I even tried to fix one but the cells were shot.
```

---
## \#8 Posted by: DEEIF Posted at: 2019-05-01T05:14:43.247Z Reads: 145

```
@Eboosted Battery was at 50% which I was told was a good storage charge.

@b264 Definitely getting a volt meter to test later this week or next
```

---
## \#9 Posted by: legend27 Posted at: 2019-05-01T05:32:30.161Z Reads: 145

```
[quote="b264, post:4, topic:92390"]
Just to be clear, never stick voltmeter prongs in a charge port. NEVER.
[/quote]

Just to make it clear, you are talking about the red circled one?

Haven’t had any issues yet doing it with the blue circled one. Just don’t think it’s recommended to do though lol

![image|672x500](upload://twjFK7DDPOyc3kuqcKToqIPOOmf.jpeg)
```

---
## \#12 Posted by: b264 Posted at: 2019-05-01T06:04:30.730Z Reads: 134

```
Correct<foobar>
```

---
## \#13 Posted by: chaka Posted at: 2019-05-01T12:54:07.208Z Reads: 123

```
> Just to be clear, never stick voltmeter prongs in a charge port. NEVER

Ahh c'mon, how about just the tip? Promise to pull it out before it explodes! 😘
```

---
## \#14 Posted by: L3chef Posted at: 2019-05-01T13:03:31.839Z Reads: 125

```
That's how I start every morning. No coffee needed
```

---
## \#15 Posted by: chaka Posted at: 2019-05-01T13:05:49.291Z Reads: 128

```
I should probably add something helpful too. 😁

From my expirence, a dead battery after it has been sitting idle for a season can be caused by the BMS powering its circuit from the 2nd cell in series. One of the main reasons I only use balance boards or no bms at all on my builds now. But I still wouldn't go without a bms on a small pack.

Ussually, if the cell has not been drained too low it can be revived by charging the cell individually.
```

---
## \#16 Posted by: banjaxxed Posted at: 2019-05-01T14:03:18.795Z Reads: 118

```
A second loop key is needed then? drat
```

---
## \#17 Posted by: chaka Posted at: 2019-05-01T15:21:08.176Z Reads: 110

```
If you did that you would need a piano type switch to disconnect the balance wires from the BMS too.

It would be cool if we all standardized an aux port with pinouts to diagnose and charge individual p groups. Then we could use a hobby charger or other DIY methods involving a lab power supply to bring a pack into balance without removing an enclosure. This would also allow us to bottom balance a pack if we wanted.
```

---
## \#18 Posted by: banjaxxed Posted at: 2019-05-01T15:23:10.325Z Reads: 104

```
Surely the BMS cannot drain if the switch is between the BMS and the - pole of the battery?
```

---
## \#19 Posted by: chaka Posted at: 2019-05-01T15:25:03.079Z Reads: 100

```
You can drain individual cells via the balance wires. I have had BMS's fail and drain a single p group before.
```

---
## \#20 Posted by: mikenyc Posted at: 2019-05-01T15:25:25.112Z Reads: 103

```
SuPower BMS?
```

---
## \#25 Posted by: DEEIF Posted at: 2019-05-02T05:02:54.174Z Reads: 86

```
Also, @b264 and @legend27 According to my dad he’s got a volt meter!
```

---
## \#26 Posted by: legend27 Posted at: 2019-05-02T05:18:28.801Z Reads: 84

```
Dad saves the day!

Remember to swap the batteries if it’s really old or have been siting for a long time because some people have experienced incorrect voltages caused by that.
```

---
## \#27 Posted by: DEEIF Posted at: 2019-05-02T05:31:20.276Z Reads: 80

```
Ok thanks! What’s the “save zone” that battery voltage should be at for a 12s pack? (Sage zone meaning not dead)
```

---
## \#28 Posted by: DEEIF Posted at: 2019-05-02T05:32:57.759Z Reads: 83

```
[quote="legend27, post:26, topic:92390"]
Dad saves the day!
[/quote]

I got to get you a pic of his “workshop” next time I’m their lol... He pretty much has every tool I could need come to think of it... (besides dang soldering and spot welding stuff tho 😢)
```

---
## \#29 Posted by: legend27 Posted at: 2019-05-02T05:44:35.166Z Reads: 82

```
I honestly got no idea, but pretty sure 3V is the lowest a cell should be discharged to. Don’t think it’s recommenced though. So 36V would be my guess.

Remember to measure all the voltages of each individual p-group. Remember when measuring B1 you need to put the negative prong on the B- part of the BMS and the positive prong on the first balance connector spot. Afterwards it’s just measuring from the balance connector. BE CAREFUL!!!
```

---
## \#30 Posted by: davidwilliams Posted at: 2019-05-02T11:56:42.260Z Reads: 74

```
good idea! Thanks
```

---
## \#31 Posted by: chaka Posted at: 2019-05-02T13:25:16.693Z Reads: 71

```
I salvaged 18650s from laptop batteries for my first few builds. If they still show a voltage they can be revived. Anything below 2.5 volts and they need to be trickle charged back to 2.5 volts and then they can be charged at 1c, ussually around 2 amps.

These packs are still in service after 3 years of use.
```

---
## \#32 Posted by: mmaner Posted at: 2019-05-02T13:26:57.776Z Reads: 72

```
[quote="chaka, post:13, topic:92390"]
> Just to be clear, never stick voltmeter prongs in a charge port. NEVER

Ahh c’mon, how about just the tip? Promise to pull it out before it explodes! :kissing_heart:
[/quote]

ROFL, I'm sitting at my desk laughing like a 12 year old and everyone is looking at me funny, thanks for that :slight_smile:
```

---
## \#33 Posted by: mmaner Posted at: 2019-05-02T13:28:16.916Z Reads: 72

```
[quote="chaka, post:15, topic:92390"]
One of the main reasons I only use balance boards
[/quote]

I've been looking into this, which balance boards are you using?
```

---
## \#34 Posted by: chaka Posted at: 2019-05-02T13:33:52.559Z Reads: 70

```
I made them. Super simple design with adjustable voltage.
```

---
## \#35 Posted by: mmaner Posted at: 2019-05-02T14:02:34.192Z Reads: 72

```
That sounds really usable, if you decide to sell any let me know.
```

---
## \#36 Posted by: chaka Posted at: 2019-05-02T14:04:53.118Z Reads: 74

```
I already have you and Tim on the books for beta testing. 🤫
```

---
## \#37 Posted by: mmaner Posted at: 2019-05-02T14:07:30.381Z Reads: 74

```
SWEET! :slight_smile:, I appreciate it brother.
```

---
## \#38 Posted by: DEEIF Posted at: 2019-05-02T14:14:01.435Z Reads: 71

```
Do you take the enclosure off every time to charge or...
```

---
## \#39 Posted by: chaka Posted at: 2019-05-02T14:28:01.703Z Reads: 71

```
No, I use a fused charge port but you need to check your balance connector to be sure everything is staying balanced. In the RC world this is standard practice but most rc pilots get into the technical side pretty deep. Most eboard riders want nothing to with all that. They just want "plug and play" so a bms is still the best option for the masses.
```

---
## \#40 Posted by: IndyPilot Posted at: 2019-05-02T22:10:12.660Z Reads: 58

```
Why not? Serious question, want to learn.
```

---
## \#41 Posted by: DEEIF Posted at: 2019-05-02T22:13:24.412Z Reads: 58

```
Alright so just for checking and being serious these are what I should/how I should check the voltage

Stick voltmeter into the CHARGERS connector, the one that @legend27 circled blue.

Then, stick voltmeter into the XT90 connector in the battery or is there another way to do this part...

@b264 @chaka @legend27 @AlanZhou
```

---
## \#42 Posted by: b264 Posted at: 2019-05-02T22:17:04.107Z Reads: 57

```
It's nearly impossible to do so without causing a short.  It's like the old "Operation" game except the consequence of a short is much worse than a red light and buzzer.
```

---
## \#43 Posted by: chaka Posted at: 2019-05-02T22:28:17.370Z Reads: 57

```
I'll be honest, not much can be gained by checking the total voltage. If you can get access to the balance connector then you can check each p group individually.
```

---
## \#44 Posted by: DEEIF Posted at: 2019-05-02T22:29:37.064Z Reads: 60

```
Alright so to check the balance boards voltage for each p group it would be a prong on the one numbered B and so on adding the voltages together correct?
```

---
## \#45 Posted by: pookybear Posted at: 2019-05-02T22:31:10.514Z Reads: 64

```
https://medium.com/@esk8life.orders/checking-and-correcting-voltage-drift-in-a-battery-pack-616e139d2e3b
```

---
## \#46 Posted by: chaka Posted at: 2019-05-02T22:36:15.565Z Reads: 66

```
I check the first cell in series by probing the battery neg and the first pin on the balance harness. Your bms may be different.
![20190502_163255|406x500](upload://251liJ8UB2fw6UegWCdAkZEfV3q.jpeg) 

The next cells can be checked by keeping the neg probe on the battery negative and adding voltages or you can probe eack p group individually like this.
![20190502_163236|356x500](upload://tEbslb6iVampf4wG1ZOh2mr0QMS.jpeg)

Do you see the burn marks on my probe @b264 :smirk:
```

---
## \#47 Posted by: DEEIF Posted at: 2019-05-02T22:38:23.655Z Reads: 59

```
Thanks @chaka ! So for the first part I can just put the negative probe into the negative side of the xt90 connector?
```

---
## \#48 Posted by: accrobrandon Posted at: 2019-05-02T22:39:15.039Z Reads: 60

```
Finally this tid bit has been posted and with pics lol this bit right here was mentioned when i was a newbie but had to figure it out on my own really after building my first pack and understanding wiring...hope this post help more future peeps beyond the op.
```

---
## \#49 Posted by: DEEIF Posted at: 2019-05-02T22:40:23.921Z Reads: 59

```
Definitely will! I’m gonna change the name in a sec to “How to check “dead battery” voltage with bms...
```

---
## \#50 Posted by: chaka Posted at: 2019-05-02T22:41:23.754Z Reads: 57

```
Yeah, ussually this is how it is done. The first balance wire is most always the positive terminal on the first p group so we probe the battery neg to check cell #1
```

---
## \#51 Posted by: DEEIF Posted at: 2019-05-02T22:42:26.774Z Reads: 58

```
Thanks! @chaka
```

---
## \#52 Posted by: b264 Posted at: 2019-05-02T23:21:57.414Z Reads: 59

```
[quote="chaka, post:46, topic:92390"]
Do you see the burn marks on my probe @b264
[/quote]

How do you think I know to tell folks not to do that :smirk: :rofl: I've burnt a few myself

... and to [fuse](https://www.mouser.com/ProductDetail/576-099707.5WXN) their charge ports ...
```

---
## \#53 Posted by: chaka Posted at: 2019-05-02T23:43:16.907Z Reads: 60

```
Im just glad you didn't call me out for how far up the shaft those burn marks are after I promised to use "just the tip."
```

---
## \#54 Posted by: brenternet Posted at: 2019-05-03T00:36:56.078Z Reads: 60

```
I was about to mention your lack of sleeve on that bad boy. Shame on you.
```

---
## \#55 Posted by: DEEIF Posted at: 2019-05-06T00:49:45.825Z Reads: 61

```
Sadly the battery was completely dead... 3.691 volts. 😢

@chaka @b264
```

---
## \#56 Posted by: banjaxxed Posted at: 2019-05-06T00:53:30.480Z Reads: 58

```
Curiosity killed this cat
https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words-2/88821/845?u=banjaxxed
```

---
## \#57 Posted by: bluegreen Posted at: 2019-05-06T01:18:20.246Z Reads: 57

```
[quote="banjaxxed, post:56, topic:92390"]
Curiosity killed this cat
[/quote]

Careful... careful.. dont short the... POP!ZZZZZZFFFFFFFFFFF

[quote="b264, post:42, topic:92390"]
It’s nearly impossible to do so without causing a short.
[/quote]

In my case, I didn't even make contact with anything, the probe being close was enough for the spark to air gap and blow up.
```

---
## \#58 Posted by: banjaxxed Posted at: 2019-05-06T01:26:31.430Z Reads: 53

```
I was just walking past holding the multimeter and that lightening just jumped into my probe...sure buddy sure 😁
```

---
## \#59 Posted by: bluegreen Posted at: 2019-05-06T01:29:08.846Z Reads: 50

```
It was only a mm or 2 away, but it did not touch. I guess trying to convince people online it is kind of pointless if they are just going to make fun of me, but whatever. Air gap sparks are a thing at this voltage.
```

---
## \#60 Posted by: banjaxxed Posted at: 2019-05-06T01:30:07.406Z Reads: 51

```
Uh-oh I iz in trouble

Just poking, just earlier I rubbed my head with a ballon and it pulled my toupee clean off

I make fun

But a 2mm gap should require about 5000v to run the gap afaik, if you live in a wet hot humid environment maybe less. Maybe the socket is faulty
```

---
## \#61 Posted by: b264 Posted at: 2019-05-06T01:53:18.163Z Reads: 52

```
I'm not sure which part of

[quote="b264, post:42, topic:92390"]
It’s nearly impossible to do so without causing a short.
[/quote]

is unclear :stuck_out_tongue:


https://www.electric-skateboard.builders/t/barrel-connector-goes-what-is-the-best-charge-connector/92895/9?u=b264
```

---
## \#62 Posted by: monsterbuilder Posted at: 2019-05-07T18:25:17.072Z Reads: 30

```
Oh man.  The same shit happened to me Friday night.  Hadn't even contacted the charge port and it arced.  Glad to see I'm not the only one.
```

---

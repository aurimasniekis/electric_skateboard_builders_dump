# &ldquo;A Treatise on Belt Sizes,&rdquo; Or &ldquo;Is HTD3M Really All That Bad?&rdquo; Or &ldquo;Some Thoughts on Belts&rdquo;

### Replies: 44 Views: 857

## \#1 Posted by: faithfulpuppy Posted at: 2018-06-05T15:17:33.334Z Reads: 242

```
I've recently been having some trouble with belt skipping during hard braking, and it got me thinking about different belt pitches and why we use 5m pitch over 3m pitch.

As many of us know, the standard belt size we use is 5mm HTD, where each tooth is 5mm tall (?) and the teeth are spaced 5mm apart. However, Boosted, probably the earliest brand to make a super reliable, (relatively) high-performance board, uses 3mm. I think it's safe to say that the boosted board has really powerful brakes that are extremely reliable, and i rarely if ever hear about bboard owners having belts skip while braking. Either way, if 5mm is so much stronger (what seems to be a safe assumption given the larger teeth), why don't they use it?

A thought occurred to me: Each 5mm tooth can individually bear more load, but if you have 3mm teeth, *you have almost 67% more teeth in mesh at a given time* because they each take up less space (1.666 times more teeth, to be exact). Therefore, if each 3mm tooth can withstand at least 3/5ths of the load of one 5mm tooth, it stands to reason that 3mm belts can transmit more power. I checked spec sheets from the same manufacturer for [HTD5M](https://www.tyma.cz/files/remeny/e-05m-en.pdf) and [HTD3M](https://www.tyma.cz/files/remeny/e-03m-en.pdf) to find out what the exact numbers were. Guess what? a 5mm tooth

![Screenshot%20(35)|415x151](upload://gFdZSF45LdfemFCQyOu5NsEDGLT.png)

Has a shear strength of about **27.21 N/cm** (with the cm representing the width of the belt of course) at 0 RPM, meaning that for the 3mm belt to be "stronger" it would have to have a shear strength of  at least **16.326 N/cm**. So, I checked the 3mm belt spec sheet and

![Screenshot%20(36)|398x149](upload://aAF7TdETyvNI77ClcwLxLUWL57s.png)

it has a shear strength of **17.30 N/cm**, which is actually an **improvement of about 5%** over what would be expected of a 5mm belt of the same dimensions. Additionally, this spec sheet lists the minimum number of teeth per pulley for both of these belt sizes to be 16, but i'm running 15 and some people on this forum go as low as 12. With smaller teeth, i could run 20 or something and still have a smaller pulley than I have now (i'm trying to push my max speed down to about 25mph with 190kv, 12s, and 107s and just keep the torque to tow my friends around). This makes sense, because 3mm belt should be more flexible, which in theory means we won't have to pull it as hard to keep it meshed with as many teeth as possible so lower belt tension should be possible, because it won't naturally curve away from the pulley as much. Especially for how small our motor pulleys are, i think running 3mm belts might actually be better than 5mm belts.

In conclusion: I think there might be some advantages to running 3mm belts like boosted does instead of 5mm belts like basically every other belt drive on the planet. Namely, I think flexibility, size, straight-up shear strength, number of teeth meshed, noise, and belt tension could all stand to benefit from a *down*size in our belt pitch. I think 5mm belt probably wins on durability and ease of creating pulleys, but we should seriously consider 3mm as an option.

What are your thoughts on this? Did i miss something? Anyone have experience with both belt sizes want to comment? Thanks guys!
-
-- Joe
```

---
## \#2 Posted by: drassak Posted at: 2018-06-05T15:25:49.456Z Reads: 217

```
intersting question. I feel that 3m belt would be good especialy for +12mm wide puleys.

I upgraded my board to a 5m 15mm wide but quickly came back to the original 5m 9mm belt because it was quieter and more efficient (more flexible).
```

---
## \#3 Posted by: Cobber Posted at: 2018-06-05T15:29:17.037Z Reads: 214

```
tldr: 9mm not enough, 15mm too much: try 12mm? :thinking:
```

---
## \#4 Posted by: GrecoMan Posted at: 2018-06-05T15:30:35.768Z Reads: 207

```
the boosted board doesn’t output nearly the amount of power that most of our boards do. i have trouble with my benchwheel skipping too. 3m is much easier to get a hold of and much cheaper too, that’s my suspicion on why they used it
```

---
## \#5 Posted by: faithfulpuppy Posted at: 2018-06-05T15:33:26.205Z Reads: 203

```
That's true, but I've ridden boosted boards and they seem to brake much harder than my board without slipping. Could that be the gearing ratio, the wheel pulley size, and the belt width (mine are dual 9mm because i can't fit 15mm)?
```

---
## \#6 Posted by: GrecoMan Posted at: 2018-06-05T15:34:56.768Z Reads: 193

```
i’ve never had skipping issues with full -120a braking (-60a motor min and -12a batt min per vesc) with properly tensioned 15mm belts and 15/36.
```

---
## \#7 Posted by: faithfulpuppy Posted at: 2018-06-05T15:37:09.567Z Reads: 189

```
interesting. I guess the solution for me has to be dual 15mm. Still, I want to explore this whole 3m thing, there could be something to it
```

---
## \#8 Posted by: GrecoMan Posted at: 2018-06-05T15:37:39.755Z Reads: 183

```
eh i guess
you need tighter tension and a steeper reduction
```

---
## \#9 Posted by: Pedrodemio Posted at: 2018-06-05T15:38:28.412Z Reads: 183

```
The main problem with 3M is alignment, if any of your pulleys it's a little bit of center the tension will change as you ride, and since the tooth is smaller it will skip easier

My first board was 3M, since the motor pulley was drilled a bit off center is was unriadeable

But the drag was way way lower than with 5M, if you can guarantee that your mount is solid and everything is almost perfect aligned it would be possible
```

---
## \#10 Posted by: Cobber Posted at: 2018-06-05T15:38:31.692Z Reads: 178

```
3mm v 5mm is good for lower power set ups...
```

---
## \#11 Posted by: Jedi Posted at: 2018-06-05T15:39:45.393Z Reads: 171

```
Good research. You may be on to something. I think (no data to backup) that 3m belts require more tension than a 5m belt. I run my 5m belts pretty loose, for free rolling. My friend has a boosted and his belts are pretty tight, but it doesn't coast nearly as far as mine. And he rarely has skipping. Actually the only time I've heard his skip, is yesterday. He hit the brakes hard to avoid a car, and broke a belt. They were only like a month old. I've never broken a 5m belt, over 2000 miles.
```

---
## \#12 Posted by: GrecoMan Posted at: 2018-06-05T15:44:34.113Z Reads: 164

```
boosted doesn’t coast because they use duty cycle. if you’re not throttling you’re braking.
```

---
## \#13 Posted by: Jedi Posted at: 2018-06-05T15:48:00.851Z Reads: 160

```
I wonder what their range could be without the drag brake.
```

---
## \#14 Posted by: BoostedBuilder Posted at: 2018-06-05T15:49:56.323Z Reads: 152

```
Is that a guess or you know about that? When I had a Boosted, releasing the throttle would not result in braking.
```

---
## \#15 Posted by: onepunchboard Posted at: 2018-06-05T15:59:18.667Z Reads: 147

```
I think he meant that regen switch. it technically does brake when u press it while cost. I feel not much difference on normal use , but on flat road it is really annoying.

or if he meant duty cycle in general brake when neutral he is wrong. it does not

in my experence it honestly feel like a toy. sorry guys but acceleration is just not there. 25% hill claim is not that good, i can run faster than the board. 

it just not have the Ump, which is the best part of the esk8. speed also is too slow. belt get loose when u go fast and running hot. thats why 3m is enough for them.

one thing about the sound, 
I prefer bit of noise because people doesnt notice it. i have to say excuse me like 100 times a day. 
I can make my board dead silence with belt spray, lubed bearing, foc. U won't hear me until 1 m from behind.

lastly belt eat through the pulleys, and with smaller pitch it will wear down quickly. boosted is no exception although steel pulley will hold for yrs, but my buddy's v1 is suffering this and rips belts once a month.
```

---
## \#16 Posted by: BoostedBuilder Posted at: 2018-06-05T16:22:09.397Z Reads: 132

```
[quote="onepunchboard, post:15, topic:57916"]
in my experence it honestly feel like a toy.
[/quote]

The Boosted Board? You serious?
```

---
## \#17 Posted by: onepunchboard Posted at: 2018-06-05T16:25:31.533Z Reads: 134

```
yeah I havent tried the new stealth but I tried boosted v2 plus. maybe extended battery will be better. I'm putting 100amps per motor and speaking from diy perspective, but I can't quite get the torq Im looking for.
```

---
## \#18 Posted by: mmaner Posted at: 2018-06-05T16:58:57.147Z Reads: 130

```
The key to 'No Belt SKip' is teeth in mesh and belt tension.  Its a job sometimes to find the perfect combination of motor mount length to increase the mesh and running belts loose to avoid motor bearing damage and wasted energy.  A properly tensioned HTD5m belt at 12 or 15mm width will almost never skip.

The difference in Evolve and Boosted is when you slam the brakes on a dual vesc with dual 15mm belts and a 10s/12s 30q pack, you are typically exerting a lot more force than you will with a boosted or evolve board.  So your more likely to skip.  Just use proper belt lengths and tension and those issue will go away.
```

---
## \#19 Posted by: Deckoz Posted at: 2018-06-05T17:30:52.912Z Reads: 129

```
[quote="BoostedBuilder, post:16, topic:57916"]
The Boosted Board?
[/quote]

I kind of slightly agree. The boosted board and the app are super polished. But for almost 3 years, Boosted didn't support Android, I waited and waited, and then the boosted left me. 

As well the advertised milage of 7-8 miles really was 4 miles with heavy riding(who doesn't ride hard?). The torque is lacking compared to most DIY builds. While I do think it has a place, they no longer have a place in my home or esk8 arsenal. Especially after, cracked trucks, and the BMS on original battery going bad - even though they were warranty. 

Boosted is a nice entry level board, but with the range and size and lack of power, it can't fit into the "last mile" category. Android support was non-existent throughout my ownership. It's hard to categorize a proper place for it. Especially after I sold it, and DIY'd a vanguard that killed it in every aspect except having an odometer. 

Anyway back on topic:
20mm belts or bust. can run them superloose for almost no rolling resistance, and they will never skip ever.
```

---
## \#20 Posted by: b264 Posted at: 2018-06-05T17:37:11.793Z Reads: 124

```
Good luck finding those metal 20mm wheel pullies ;-)

I'd run 20mm in a heartbeat if it was an option.  Finding 15mm ones is like pulling teeth, especially if you need more than 36 teeth.  @dickyho has some good ones
```

---
## \#21 Posted by: Deckoz Posted at: 2018-06-05T17:44:11.499Z Reads: 120

```
just run metro pulleys with a smaller motor pulley @b264 

standard 12 or 15mm ratios
16/36 - 2.25:1 
16/40 - 2.5:1 CANNOT USE ON 83mm wheels
16/44 - 2.75:1 CANNOT USE ON 83 or 90MM wheels
16/48 - 3:1 97mm or 107mm only

20mm belts on 36T metroboard, with any size flywheel... and no belt skip
16/36 - 2.25:1 
15/36 - 2.4:1 
14/36 - 2.57:1 
13/36 - 2.77:1 
12/36 - 3:1
```

---
## \#22 Posted by: b264 Posted at: 2018-06-05T17:54:35.732Z Reads: 116

```
That's the whole fkn problem is that I refuse to use less than 15 teeth

So I need bigger wheel pullies because I only use 107mm wheels (and one set of 100mm)
```

---
## \#23 Posted by: Deckoz Posted at: 2018-06-05T17:55:37.758Z Reads: 115

```
Yea I refuse to use less than 15teeth on small belts too..  but my 250lb buddy couldn't make 12t on 20mm belts skip Soo... It kind of negates itself with friction
```

---
## \#24 Posted by: BoostedBuilder Posted at: 2018-06-05T17:59:43.509Z Reads: 112

```
You agree with me or with that it's more of a toy?

Because you pretty much summarized what I feel. It's just a polished **product**. Like it's fucking beautiful. I put 800 miles on my board in 2 months last summer (my first board btw), and it was the best experience I've ever had. I enjoyed it better and used it more than a car. I had an iPhone last year, so the app was amazing. Torque is enough for a person who never skated before, but ofcourse after time you want more. Hence my switch to DIY.

But I really can't call it a toy. For 50mm motors, it's a powerful board. Just comparing to DIY, it's really behind because we have the option for 63mm+ motors and 400Wh+ batteries.

Anyways, I need to start making build threads for my boards : )
```

---
## \#25 Posted by: BoostedBuilder Posted at: 2018-06-05T18:00:29.032Z Reads: 109

```
If you're so desperate, why don't you just make your own? It's not hard what so ever.
```

---
## \#26 Posted by: b264 Posted at: 2018-06-05T18:01:41.712Z Reads: 109

```
I live in a high-rise downtown with no CNC mill up here.  Also I did get some from @dickyho but they are 15mm.  20mm ones are unobtainium.
```

---
## \#27 Posted by: Deckoz Posted at: 2018-06-05T18:02:41.091Z Reads: 110

```
[quote="BoostedBuilder, post:24, topic:57916"]
You agree with me or with that it’s more of a toy?
[/quote]

I agree with you more that it is a polished product.. just the range feels toy like. I play with toys for a few minutes... Like drones and then the battery dies.. I was killing my boosted battery in about 15-20 minutes... Then waiting an hour to charge. That's the "toy like piece" for me I think.

Makes it hard to justify buying another.. for 1500 when my Evo with ~40 miles of range cost me 1900. I dunno i can be on both sides... And it makes it even harder when the board is large and not a short deck so can't fit in the last mile category even though it's range is last mile type range...
```

---
## \#28 Posted by: BoostedBuilder Posted at: 2018-06-05T18:09:02.490Z Reads: 104

```
I got a solid 5mile ride on a full charge, it's not toy like to me because I understand the idea behind using LiFePo4 batteries, but I'm not saying it's enough either! That's why I made a Vanguard build too!

Love you Evo btw!

@b264 I thought so too until I actually searched. Believe me you'll find a shop with a mill within a 5mile radius.
```

---
## \#29 Posted by: Deckoz Posted at: 2018-06-05T18:16:03.913Z Reads: 105

```
Yea man.. I dunno I ordered a boosted mini. Because I feel like that actually will fit the category quite well. Half the price of the original boosted, same range, short deck. I'm actually really excited for it. 

It's just hard to be excited about almost any production longboard in the 36"+ length. As the cost/range per ride makes me feel cheated.

The boosted mini costs about the same as my 🥔, and will have almost identical ranges, and 50mm motors. The boosted mini seems justifiable In my head.

I know this isn't coming out right...but maybe you get what I guess I'm trying to say?
```

---
## \#30 Posted by: BoostedBuilder Posted at: 2018-06-05T18:33:47.104Z Reads: 101

```
I get exactly what you're trying to say 😜Why did you get the mini if you're already making the :potato:?

Metro pulleys fit on 218 TB trucks, right? And they are 20mm, not 18mm?
```

---
## \#31 Posted by: Bjork3n Posted at: 2018-06-05T18:34:07.253Z Reads: 101

```
I use Dual 12mm and 5m pitch with 16/36 on 90mm wheels. (6355 x2 motors)
I run my belts very loose so there is almost no drag from the belts. The belts will skip when i brake very very heavy but still stops quite well. The pros with loose belts is that i can coast forever, and my range is also increased cuz of this.
On normal riding the belts never skips on my setup.


On my previous board i ran 3m pitch... they skipped like crazy and when i tightened the belt so it wouldn't skip the belt would be destroyed after 3-5 charge cycles.

5m pitch is my choice! :)
```

---
## \#32 Posted by: Deckoz Posted at: 2018-06-05T18:40:12.097Z Reads: 101

```
[quote="BoostedBuilder, post:30, topic:57916"]
Why did you get the mini if you’re already making the :potato:?
[/quote]

Mostly because I have a locker at work, and plan on leaving it in my locker(potato doesn't fit....oops lol) so I'll have a board at work, and then another last mile board to take from the house when I feel I need it.

[quote="BoostedBuilder, post:30, topic:57916"]
Metro pulleys fit on 218 TB trucks, right?
[/quote]

Yea metroboard pulleys are actually 21mm and fit on 218 trucks.
```

---
## \#33 Posted by: Jumpman Posted at: 2018-06-05T18:40:35.082Z Reads: 97

```
Hobbyking wheel pulleys are at least 20mm, but only 36T.
```

---
## \#34 Posted by: BoostedBuilder Posted at: 2018-06-05T18:41:07.297Z Reads: 95

```
He likes those with bearings!
```

---
## \#35 Posted by: Jumpman Posted at: 2018-06-05T18:41:38.805Z Reads: 97

```
Sorry, didn’t read!
```

---
## \#36 Posted by: BoostedBuilder Posted at: 2018-06-05T18:42:43.492Z Reads: 95

```
Haha really? I thought the mini is longer then the :potato:,

EDIT: I confused the Potato with the Spud, forget it 🤦‍♂️
```

---
## \#37 Posted by: Battosaii Posted at: 2018-06-05T18:48:15.943Z Reads: 96

```
I'm 300ish and I cant make my 12mm belt skip and I can slam the brakes as hard as they can with -65 motor amps.
```

---
## \#38 Posted by: Deckoz Posted at: 2018-06-05T18:49:35.786Z Reads: 96

```
[quote="Battosaii, post:37, topic:57916"]
12mm belt skip and I can slam the brakes as hard as they can with -65 motor amps
[/quote]

But on a 12T motor pulley? 12mm on duals is typically fine on 15T or higher.. but 12-14T start having skipping issues with lack of width
```

---
## \#39 Posted by: Battosaii Posted at: 2018-06-05T18:50:26.057Z Reads: 97

```
Actually not I run a 16t motor pulley
```

---
## \#40 Posted by: onepunchboard Posted at: 2018-06-05T19:43:16.401Z Reads: 90

```
I'm sorry if I upset you by my words. I just think price per performance is not there.
```

---
## \#41 Posted by: BoostedBuilder Posted at: 2018-06-05T19:44:19.976Z Reads: 85

```
Why would you upset me? My name is in no way related 🤣 😂

I was just curious!
```

---
## \#42 Posted by: b264 Posted at: 2018-06-05T20:39:41.494Z Reads: 80

```
[quote="Jumpman, post:33, topic:57916, full:true"]
Hobbyking wheel pulleys are at least 20mm, but only 36T.
[/quote]

If it's not metal and 20mm and 40T or more, than it doesn't matter to me :smiley:
```

---
## \#43 Posted by: Pedrodemio Posted at: 2018-06-05T23:08:41.246Z Reads: 77

```
I used 12T with an idler in my previous setup, never skipped a teeth, but the diameter of the pulley is too small and stress the belt too much, I was destroying belts all the time

With 14T I’m fine for now
```

---
## \#44 Posted by: faithfulpuppy Posted at: 2018-06-05T23:09:31.559Z Reads: 77

```
i might put an idler on my setup, if i can figure out how to fit one on.
```

---

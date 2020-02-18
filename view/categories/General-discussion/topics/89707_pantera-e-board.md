# Pantera E-Board?

### Replies: 8 Views: 460

## \#1 Posted by: Fingerbang Posted at: 2019-04-07T15:19:24.924Z Reads: 141

```
![image|374x500](upload://42icH3rDs6THNWMIXLYXSsXXpWf.jpeg) ![image|666x500](upload://5NUMjCPKhfR3EnzumUiSkwneF3.jpeg) ![image|666x500](upload://sE50oSPaJYfwcqxb2UdLzqqZLK6.jpeg) Hi.  Totally new to electric boards but have ridden since the late 80s.  I came across this beast and Paid next to nothing for it.  It doesn’t have a charger.  I’m pretty sure someone has bent the nose ‘flat’ but other than that it appears to be all there.  Anyone got any info on what this is?  How old it is etc??  It has 2 x 12v 7amp batts in it but they appear to be dead.  Multimeter gives a reading of 6.4 on 1 and 1.6 on the other.  I’ve tried to put power through the circuit with a 12v 10amp batt from a kids quad bike but it didn’t turn or light up the on switch.  I put the batt direct to the motor and it spun so am thinking something funky going on with the electrc circuit?   Any help with this would be greatly appreciated!
```

---
## \#2 Posted by: High-roller Posted at: 2019-04-07T16:01:37.512Z Reads: 128

```
Hello @Fingerbang and welcome! 
The Pantera was a copy of the BMW streetcarver (look it up), it was made around 2003-2005 give or take.
If you want to see what you can do with one, you can check out my build log. It's still a work in progress but coming along.
If you're using the original motor I'm a little surprised it's held up this long. Didn't it use a brushed motor?
Likewise the batteries. Even if they where new you wouldn't get much out of them by today's standards.
Are you trying to upgrade this or just get it back in working condition? What's your budget?
Can you please show some pictures of how the trucks are bolted to the deck? I've been having trouble with mine stripping out of my wood deck (9-ply maple) so I'm debating getting a CF one. How light is that aluminum deck?
```

---
## \#3 Posted by: Fingerbang Posted at: 2019-04-08T21:22:17.109Z Reads: 98

```
Hi @High-roller.  I bypassed the circuitry and got the motor spinning.  It’s extremely smooth.    Although old I don’t think it ever had any real use.  The wheels look pretty clean and all the bushings / runners are, surprisingly, in really good condition.  I’ve multimetered the circuitry and can’t find any faults within the wiring although the battery’s are dead.  I tried to charge them up thinking they may have just deep discharged given the length of time it’s stood (many a cobweb) but nope - they are shot.  So all in, to get this thing rolling, I think all it needs is two 12v 7ah batts - that was what was inside when I cracked it open.  

I bought it as it was an oddity.  I’ve kept my old boards (Powell Peralta mainly) and longboards and this just looked like a future piece of skate history to add to the collection.  I knew of the BMW street carver (and the price tag) and always wondered what the trucks would actually ride like. 

£20 got me the board as it sits now.  I thought it was worth a punt.  Initial thoughts were to just get it back to as it should be.  New lead batts and some fresh grip.  Bats equate to roughly £35 and a bit of grip which I’ve already got makes it a £60(ish) outlay.  That said - if there was an alternative to the heavy lead batts and it wasn’t to pricey I’m all ears.  Oh and I’ll be heating and gently bending the nose back as it should be.  

Weight wise it’s ridiculously heavy.  40lbs plus.  The trucks are bolted by way of 3 bolts.  If yours are pulling through a good option would probably be to place a thin metal plate underneath to spread the tension or some nice wide washers.  👍🏻
```

---
## \#4 Posted by: Fingerbang Posted at: 2019-04-08T21:24:42.043Z Reads: 84

```
![image|666x500](upload://cm3IpiacUf7ha5J7NReDdZHWOg2.jpeg) ![image|666x500](upload://hbFYdIASNGazfA03g7C4V9Cmvvx.jpeg) ![image|666x500](upload://qDsblMGRS9LVwCVncBmxXzXoIoG.jpeg) ![image|374x500](upload://tPie4jyfssqhGplOvFLjFyimnxo.jpeg)
```

---
## \#5 Posted by: Fingerbang Posted at: 2019-04-08T21:25:49.808Z Reads: 78

```
Has anyone heard of Federal as a brand for this sort of board?
```

---
## \#6 Posted by: High-roller Posted at: 2019-04-09T08:36:50.142Z Reads: 58

```
Okay, short answers first: I have never heard of federal brand skateboards, maybe it's just a logo decoration?

So it sounds like the two bottlenecks are the battery and the ESC. It would also help to know your motor Kv so let's do that first. Based on your pictures and info I am making a few assumptions, please correct me if I'm wrong:

Motor is 150 watt, 24VDC. Your wheels are 107mm (I have the same ones). Your two 12v batteries are connected in series, giving you 24v and 7000 mAh.
Using this post as a guide:
https://www.electric-skateboard.builders/t/can-i-calculate-the-kv-of-this-motor/88519/15
And assuming a top speed of 35 kmh I calculated a motor kv of approximately 72 kv which is very low. You'll get tons of torque (which you'll need in order to move 40+ pounds :wink:) but low speed, and it will almost certainly need a push to start rolling.
The quick fix for this is to replace the dead batteries with Lipos, probably a 6s pack. This will give you 22.2 volts and a higher capacity in a considerably lighter pack. The question is whether your ESC can handle lipos, and I suspect that it won't, at least not easily. Nicad or Nimh batteries might work, but will likely have lower stats for the money.  

[quote="Fingerbang, post:3, topic:89707"]
If yours are pulling through a good option would probably be to place a thin metal plate underneath to spread the tension or some nice wide washers. :+1:t2:
[/quote]

This is indeed one of the ideas I'm considering. I'm also talking to a local skateboard deck manufacturer about a carbon-fibre deck since plain wood doesn't seem to be enough to handle the stress.

[quote="Fingerbang, post:3, topic:89707"]
I knew of the BMW street carver (and the price tag) and always wondered what the trucks would actually ride like.
[/quote]

I've only had a brief test ride on mine, as in 10 meters, before the the bolts on the front truck pulled out of the threaded inserts in the deck. It's possible they just weren't long enough, but since one or two of the ply layers were stripped around the holes I'd rather not risk it with this deck anymore.
I can tell you that the steering was nice and easy, you don't have to lean too much to get a good turning radius, but you do have to be firm when you push with your feet to steer. Bindings like the freeboard or similar ones are a huge help for this.

Let me know what you decide to do, I'm curious to see how it turns out!
```

---
## \#7 Posted by: Fingerbang Posted at: 2019-05-09T19:55:02.754Z Reads: 39

```
Hi there!  Been a bit manic hence the delay with this project.  Ok so I decided I wanted to put it back to its original state.  So I bought some batteries and got a click coming from the deck foot button so proceeded to attach motor and has partial success.  In spun, stopped, spun a bit more then stopped.  Sensing a probable shirt somewhere set about finding it.  A good friend took a look at the motor and declared it shot so I bought another.  Whilst we were ‘messing’ with it attempting to make the circuit board work constantly as opposed to when it felt like it I managed to connect the batts incorrectly creating a small spark - now I’m not sure the circuit was attached but from this day on lost the click coming from the circuit board when the foot button is pressed.  Equally when running a multimeter across it I’m not getting a reading from wires that go to the motor.  So I think we shafted the circuit.  Which is a monumental issue as that ain’t a part I can easily find - unless you got one?! 😂.  So - new motor, new batts, no circuit.  Figured I might get a cheap scooter esc and cannibalise that?  Not ‘board or age  specific’ but at least I could get the wheels turning.  I did find I could buy the switch that solder to the board for a couple of quid so might try that just in case that just gave up the ghost but it’s a long shot!
```

---
## \#8 Posted by: High-roller Posted at: 2019-05-10T10:17:10.687Z Reads: 19

```
It does indeed sound like your ESC is dead. Okay, first of all, what kind of batteries and motor do you have? These will both impact the performance the most.

For a single motor build you should be fine with a standard 4.12 vesc, any reputable name brand will do. I don't know much about scooter esc's so I can't really help you there.

Controlling with a footswitch is not for everyone, it sounds like you'll have to be extra careful when adjusting your ESC settings.
```

---

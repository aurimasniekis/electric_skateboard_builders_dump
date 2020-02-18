# Hello i&rsquo;m new and i&rsquo;m craving for power

### Replies: 10 Views: 1748

## \#1 Posted by: Sebastiaan Posted at: 2016-01-03T03:12:41.709Z Reads: 105

```
Hello, i'm new, i lurked through this entire forum for days reading threads on how to build (or buy) my electronic street rollercoaster.

So i far i've dived deep inside the terminology and "how-to's" on tinkering, electronics and mechanics.

Soooo without any knowledge of anything into RC, motor's and electronicshizzledizzle i came up with this.

I have a Riviera longboard gathering dust, tired of pushing (manually)
So here is my (maybe) "buy list"

Okay we are going fully bonkers on this one so i planning on :
The dual motor mount from Enertion with the fittings motors.
I guess the 190kv 6355's will do, as recommended, i do not know the difference (for now)
(If Enertion could deliver this in a neat package with a fair price, i'm game) (Still waiting for updates on their webshop) (PRESS F5 EVERYDAY)

I'm gonna need two VESCs right? Any updates on the dualvesc ?

I will need to power this baby up with some sparkly sparkly aaaand i saw a thread here combining 2 x 6c cells of 20000mah into a total of 12s for apocalyptic power) (THEY ARE EXPENSIVE oO)
So maybe 2x6s 10000mah would suffice. 
The thing is, i want an easy switch between parallel and serie's (So i can choose between durability and insane mode. Where can i get those? The space cell which Enertion is selling won't do for my setup i think.

And my final question of this wall of text where i think i will stuggle the most with... wiring *badum tsssss*

Is it hard to connect everything to.... everything, I do not want to solder, (electric shortage trauma)
And is there a wire plan somewhere around here?

Thanks, i should get into bed now, it's about 04:00 in the morning here in Belgium. oO
```

---
## \#2 Posted by: lox897 Posted at: 2016-01-03T05:02:03.293Z Reads: 95

```
@chaka Sells dual VESCs.
He can also do custom connectors that he solders there. It's easy to connect everything but configuring the VESC is where it gets harder. If you don't want to start with a vesc and want something simpler get torqueboards esc that supports up to 12s or a hk 150amp esc. Hobbywing and castle also have some ESCs that work. There was a thread by @cmatson that had his wiring diagram. Just search google for "series and parallel wiring of batteries" the rest is pretty much plug in and is self explanatory. The ESC servo wire usually goes into channel 2 or 3 (not sure exactly which one because I'm not at home) others know this.
```

---
## \#3 Posted by: cmatson Posted at: 2016-01-03T06:02:14.957Z Reads: 93

```
[quote="lox897, post:2, topic:877"]
The ESC servo wire usually goes into channel 2 or 3
[/quote]

channel 2 :wink:

Any reason why you say the space cell won't work? I know you are going for simplicity (no complicated wiring/soldering) and the space cell was made for just that. 

it will have a connector that matches exactly to the type of connector on your VESC, which will then have the same bullet connectors as your motor! the receiver will have a standard servo cable going to it(again, no soldering!) so the only thing you'd have to focus on is mounting the components to your deck!

@psychotiller makes some sweet ABS cases for space cell and VESC builds, so you could have everything plug and play except actually mounting the enclosure onto your deck.
```

---
## \#4 Posted by: Sebastiaan Posted at: 2016-01-03T14:46:40.459Z Reads: 88

```
I see the space cell has a 10s rating, that will do for now !
I just saw someone is willing to  sell their enertion raptor dual board here on this forum, and it's in my price range... Someone is also selling (i think) their custom board called starlet cruiser, i'm looking into that to.
Either way if none of these options work out, i will build my board, thanks for the info, i will look into the different ESCs that are available. And maybe stay in the 10s flow, i think on 12 i have the potential to cause serious injuries :P
```

---
## \#5 Posted by: psychotiller Posted at: 2016-01-03T15:28:00.370Z Reads: 86

```
6s has torque and speed capable of killing us...
```

---
## \#6 Posted by: laurnts Posted at: 2016-01-29T12:51:11.781Z Reads: 75

```
@Sebastiaan Everybody think they require 8s - 10s - 12s and reaching the highest speed possible. But longboard at least normal longboard are not qualified for high speed transportation. @psychotiller is right about 6s, I have 6s my self and I barely hit full throttle as stones / passing cars / pot holes might instantly throw you off with serious injury.

[quote="Sebastiaan, post:1, topic:877"]
The thing is, i want an easy switch between parallel and serie's (So i can choose between durability and insane mode. Where can i get those? The space cell which Enertion is selling won't do for my setup i think.
[/quote]
For switching between parallels and series, hmm that actually doesn't differ so much in terms of deliverable power (Watt / Energy). The only reason I could think off when switching from series to parallel is to increase distance travelled and this is not necessarily the case if you think that way. Because the energy being stored in the battery stays the same amount. So it all depends on how much your motor would draw the power. If you ride 12s for 5 min that most likely equal to use 6s for 10min distance. And each motor has their own rpm of efficiency yet what I know and feel about brushless motor is that they are more efficient at higher speed.
```

---
## \#7 Posted by: trbt555 Posted at: 2016-01-29T13:29:56.344Z Reads: 75

```
Higher voltages are not only useful for higher top speeds, it makes sense from an efficiency perspective.
At 12S you'll have half the current you'd have at 6S and only 1/4 of the heat.
Or in layman's terms: less risk of frying anything.
```

---
## \#8 Posted by: laurnts Posted at: 2016-01-29T13:58:05.512Z Reads: 73

```
Never heard of this before, but it does make sense.
Lessons learned.
```

---
## \#9 Posted by: Sebastiaan Posted at: 2016-01-29T15:33:28.359Z Reads: 69

```
Thanks all for replying and giving advice, I will start a new thread following the forum rules at making a fitting topic title. I'm gonna reverse engineer a electric board i bought from the owner from aliendrivesystems.com

I've had an accident involving a small puddle of water. The ESC needs to be replaced as well as some BECs and maybe the receiver.. I'm planning to mount the whole system to a new custom made board i made when sulking and grieving over the expensive units i broke. 

This topic can be closed if needed.
```

---
## \#10 Posted by: chaka Posted at: 2016-01-29T16:06:45.604Z Reads: 66

```
You can go too far with voltage and over saturate the stator resulting in a loss in performance. Best to give your motor a small buffer based on the ratings.
```

---

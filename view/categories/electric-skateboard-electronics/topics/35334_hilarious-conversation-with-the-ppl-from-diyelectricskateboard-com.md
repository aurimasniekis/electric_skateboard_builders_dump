# HILARIOUS conversation with the ppl from diyelectricskateboard.com

### Replies: 16 Views: 1158

## \#1 Posted by: nordlicht Posted at: 2017-10-11T20:40:28.296Z Reads: 294

```
So heres the thing:
I wondered that both, the single and the dual HUB motors of torque are rated with 50A max current and Peak Rated Power 
of 1800W. Voltage obvously stays the same, since they are used in parallel, but 2 motors draw double the current and provide double the power - so that can't stay the same.

I tried to get that information from the customers service, but they tried to tell me, that the current stays the same, no matter how many motors I use. 
Enjoy:


----------
**You** — Please update your info
Hi

**Ralph** joined the chat

**Ralph**
Hello.
**You** — Please update your info
the single torque and the dual torque HUB motors have both the max current of 50A

but if I use a single motor in parallel (which i have to obviously) the current would double

so is the max current of 50A for dual or single setup?


**Ralph**
Yes.

You can set it to 50A max.

That is fine.
**You** — Please update your info
you dont understand me

how high is the maximum current of one single torque HUB motor?

50A?

than the current of the dual setup is 100A?


**Ralph**
What KV?
**You** — Please update your info
doesnt matter, stays the same

talking about HUB motor


**Ralph**
Yeah.
**You** — Please update your info
your peak rated power is also the same for dual and single setup


**Ralph**
We have 75 and 130KV. Anyway, I do not have the info, but you can just set the VESC to max 50A.

Doesn't matter

As our VESC is compatible with all our setups.
**You** — Please update your info
you still dont understand my question

single motor: Peak Rated Power - 1800W / 50A
dual motor: Peak Rated Power - 1800W / 50A

that cant be


**Ralph**
I mean, for our VESC.

You can just set it to max 50amps.

Either belt drive or hub motor.

Does not matter

Since our VESC can draw 50amps continuous.

So it is safe to just set it to 50.
**You** — Please update your info
what if i dont sue your vesc


**Ralph**
Directly.
**You** — Please update your info
butr want to use the motors to the limit?


**Ralph**
Hmmm, let me check.

Please hold.
**You** — Please update your info
thanks!

and if I WOULD use your vesc, I still need to know if 2 Motors draw 50A or 100A current to design the batteries. I'm actually stunned that I seem to be the first person asking those questions :x

is there a datasheet for the motors?


**Ralph**
I am sorry but we do not have that info.
**You** — Please update your info
YOU DO NOW KNOW HOW MUCH CURRENT THE MOTORS DRAW YOU SELL?

gimme the datasheet please!


**Ralph**
Like I said we do not have that information.

I am still checking with our team.

And waiting for a response.
**You** — Please update your info
thanks

whereever you buy the motors, they provide a datasheet


**Ralph**
Either Single or Dual.

That is 60amps.
**You** — Please update your info
my name aint maxwell

but that cant be


**Ralph**
Either SIngle or Dual, either 75KV or 130KV. Same.

60amps.

----------

Apparently they really do not have a clue what motors they sell and how much current they actually draw.
IF anyone has current clamp which stores data, I would HIGHLY appreciate information about the current of those motos.

Cheers
```

---
## \#2 Posted by: yummyblobs Posted at: 2017-10-11T21:06:03.571Z Reads: 265

```
Bro, I understand that you had questions that weren't answered in a way that clarified your understanding, but you need to take time in understanding the description. Here's what it says on the site for the Dual Hubs,

TORQUE HUB MOTOR SPECS

Tested on 6S. Results will vary with higher voltage but this is provided as a general guideline.
Motor Size:63mm * 50mm
Stator Size - 52.8mm * 30mm
Wheel Size - 90mm Diameter 52mm Wide 90A Duro
Magnets - N42SH
Maximum Heat - 50-60°C, Max 80°C / 122-140°F, Max 176°F
Voltage - 6S-12S
Peak Rated Power - 1800W
Continous Output Power - 500W
Max Current - 50A

It pretty much says it in the title, "TORQUE HUB MOTOR SPECS" which pretty much infers that it is the spec for ONE hub. Also note, these are BLDC motors, they don't necessarily DRAW current, they have no current limiting resistance so theoretically they draw what ever you throw at it. They must be controlled by the ESC and thats what the CSR is stating, (Mind you that he is referring to the VESC) just set the ESC to 50amps motor max and your golden.
```

---
## \#3 Posted by: yummyblobs Posted at: 2017-10-11T21:11:45.243Z Reads: 254

```
You should also remember, you can only control ONE motor at a time with ONE ESC. I think you should spend more time on this forum and research other people builds and you'll really figure everything out. Questions are much better answered on this forum than a simple CSR chat.

DIY's CSR is probably more geared towards answering question pertaining to stock availability.
```

---
## \#4 Posted by: mmaner Posted at: 2017-10-11T21:13:03.684Z Reads: 241

```
I love it when new guys start jumping on vendors after they've been here less than a month.  Just chill and the stuff will make sense eventually.  If you have questions, ask them in a respectful manner and you'll get good answers.  

I would also point out that you said in your second sentence "you dont understand me", I would argue you weren't making yourself clear...but the whole conversation went downhill from there anyways, so whatever.  So blue ribbon for being a dick, good job.
```

---
## \#5 Posted by: chaka Posted at: 2017-10-11T22:01:28.376Z Reads: 222

```
https://www.youtube.com/watch?v=M3fSDtJgAas
```

---
## \#6 Posted by: onepunchboard Posted at: 2017-10-11T22:42:55.369Z Reads: 199

```
sounds like u r the one who have dumb questions
```

---
## \#7 Posted by: nordlicht Posted at: 2017-10-12T13:26:56.054Z Reads: 166

```
Well alright, thanks for correcting me on the fact that BLDC motors draw "unlimited" current - but it's still pretty bad service that the CSR can't tell me that ...
But there needs to be a technical limit where more Amps only result in molten isolation of my wires - is there any information on that?

[quote="yummyblobs, post:3, topic:35334"]
You should also remember, you can only control ONE motor at a time with ONE ESC.
[/quote]
Thanks I'm 100% aware of that fact ;)

I plan to use 18650 30Q's. 12S4P. They have a constant discharge current of 15A, 4 parallel would make it 60A.
This means I can only give each motor 30A.
I try to figure out if thats enough torque, the maths I did:

ke (it may be some german abbreviation, dunno :x) = (1/kv) *9.5 [Nm/A]
With this "ke" can I calculate the torque, depending on the Amperage, which is 60Amps.
=> 1/(130)*9.5 * 60A = 4.4 Nm.
This doesnt sound like much tbh.

Whats your experience on them? should I search for new Batteries to get the full 100amps?

Cheers
```

---
## \#8 Posted by: mmaner Posted at: 2017-10-12T13:43:33.039Z Reads: 148

```
If you don't get enough torque using 12s4p on 130KV motors then get the tank off the board :).  You are looking at peak, look at constant and you will see more reliable info.
```

---
## \#9 Posted by: psychotiller Posted at: 2017-10-12T14:03:12.702Z Reads: 142

```
Not really that hilarious being that you were given correct information that you don't understand..Maybe read a little (lot) more before you start condescending members of the community here.
```

---
## \#10 Posted by: evoheyax Posted at: 2017-10-12T14:06:09.290Z Reads: 145

```
Pretty funny conversation TBH. Surprised he could just set you straight. Your questions were enough to understand what you were asking for in my mind. It seems like you lost your patience mid way through though, and that never helps. 

[quote="nordlicht, post:1, topic:35334"]
so is the max current of 50A for dual or single setup?

Ralph
Yes.

You can set it to 50A max.

That is fine.
[/quote]

What? Is this a bot or a person responding? It's as if the question was totally ignored.

In general though, your cells are rated to 60 amps con between the 2 motors, but I wouldn't even pull that if I were you from those cells. It will sag like a mofo. Maybe 20 amps per motor (battery amps). Motor amps, you can set a little bit higher, 60 or 70, each.

IF these are 130 kv, your not getting good torque ever from a hub motor that high in kv. 130 kv is meant for speed freaks, not people who want torque.
```

---
## \#11 Posted by: longhairedboy Posted at: 2017-10-12T14:18:42.253Z Reads: 129

```
[quote="evoheyax, post:10, topic:35334"]
130 kv is meant for speed freaks, not people who want torque.
[/quote]

truth. 

Also this is yet another fine example of why vendors should be able to just say "go somewhere else." and not fear backlash from the consumer hoard citing terrible customer service or some other such nonsense.
```

---
## \#12 Posted by: Deckoz Posted at: 2017-10-12T14:26:28.305Z Reads: 127

```
I mean ive had hilarious convos with them to.

What are your wheel Duro's? No clue. What is a wheel durometer? Couple weeks later they update them to say 76A(they're a lot harder then that)

When I ordered a kit they sent one motor with 4mm bullets, one with 5.5, and two vescs with 5.5 bullets. I asked for them to send me three 5.5 bullets, they kept saying I need to spread the bullet out, even after showing pictures of the bullets being measured with a micrometer. Lol.

When I had three vesc die within days of receiving them and inquire about them they declined to offer support. When I asked about purchasing a warranty they only allow warranty purchase with the vesc. And the little they did say was did you plug it in and wait for the flashes, lolol(its dead dumb ass no flashes)

When we had the antispark die literally on plugin, they asked for video. Of course it doesn't show anything as it failed open(on). They kept saying push the button lolol. And didn't understand the button does nothing because their antispark is a POS

Either way Mary and Ralph are useless, if you want any real answers email or ask for Dexter directly.
```

---
## \#13 Posted by: longhairedboy Posted at: 2017-10-12T14:41:40.107Z Reads: 124

```
I couldn't get the total length from hole to hole of the 12mm pulleys out of them recently. I don't think they, the people answering questions, have parts on hand or have measurement devices. When i finally received the pulleys, it took me about 10 seconds to get the number i needed.
```

---
## \#14 Posted by: nordlicht Posted at: 2017-10-16T17:15:54.250Z Reads: 86

```
I've never used the VESC before, so I dont exactly know what you mean.
> Maybe 20 amps per motor (battery amps). 

Alright, so I'll set the current limit of the VESC to 20 Amps - sounds reasonable.

> Motor amps, you can set a little bit higher, 60 or 70, each.

How do you mean that? If I draw 2*20A from the batteries, how do the motors get 60-70?

Cheers
```

---
## \#15 Posted by: longhairedboy Posted at: 2017-10-16T18:03:13.097Z Reads: 78

```
motor amps aren't the same as battery amps. Somebody else here can probably explain it better than that, but battery max amps is actual amps and motor amps is some kind of weird pole math amps.
```

---
## \#16 Posted by: nordlicht Posted at: 2017-10-16T18:32:09.034Z Reads: 67

```
Alright, that has something to do with converting DC to 3phasish AC, if I recall correctly.
But I can only set the current limit from batteries to VESC in the options of the vesc, right?
```

---

# I&rsquo;m Confused.. About Fusing

### Replies: 10 Views: 280

## \#1 Posted by: walleywalker Posted at: 2018-08-10T04:50:06.486Z Reads: 152

```
How does fusing make a battery pack safer - When you essentially have a large number of heating elements only a few amps away from melting trapped in a nearly sealed compartment with no way to exchange heat outwards? 

Also, doesn't it defeat the purpose of using nickel strips that are capable of handling your intended amperage? If the whole point of piling multiple nickel strips atop one another is to prevent heating right? 

This causes me a headache.
```

---
## \#2 Posted by: Eboosted Posted at: 2018-08-10T05:13:55.400Z Reads: 142

```
A fuse will help you in case of a sudden rush of current a lot more than intended for a normal output of motors.

For example if you short the positive and negative leads of a motor controller, however if the short occurs within the battery itself no fuse or BMS will keep your cells from shorting and probably venting. The second problem with fuses is if you blow them on a high speed ride you will have no brakes, scary sh!t
```

---
## \#3 Posted by: lrdesigns Posted at: 2018-08-10T05:36:02.984Z Reads: 133

```
Yeah its tricky because a main fuse needs to never go off under "normal" ridding conditions. But blow if there is a short circuit from a crash, wear and tear or user error. 

If it blows while ridding the sudden stop in acceleration will most likely throw you on the road, so no need to worry about no breaks :sweat_smile: 

For this reason many riders don't use a main fuse. They build in other safety measures and say a board fire is slightly less bad then being thrown on the road at top speed.

If your batteries are getting hot they are too small or low performance for your setup.
```

---
## \#4 Posted by: dareno Posted at: 2018-08-10T05:58:35.641Z Reads: 115

```
The only way to safely fuse a battery is to install a fuse on every bank, so all your p packs.  this will at least stop one cell from taking down your whole board but the logistics of that kind of set up is what stops most people.  There are a number of non solder options out there and some can be fused.  Myself I don't use a main fuse because I like my face and care for it more than my board and secretly would enjoy watching the fireworks but I'm getting therapy for that.
```

---
## \#5 Posted by: Andy87 Posted at: 2018-08-10T06:08:27.090Z Reads: 107

```
Just don’t get that. Why I can’t use like let’s say a 120-150a fuse on a dual set up for example.
Usually for dual the setup is limited by 80-100a by the vesc.
So in real life situations the fuse never can blow, even not on high speed or steep hills. But if you short the battery which would led to flow a way much higher current they would blow.
For me would be interesting who already had an blown fuse and what was the setup of the board and the size of the fuse. 
Sure if I run with a 60-80a fuse it’s likely that one day it just blow on a high load.
```

---
## \#6 Posted by: sztamas Posted at: 2018-08-10T06:09:30.616Z Reads: 105

```
As I saw the short circuit amperage for 30Q is about 130A. The max continuous you should get is 30A. If your cell level fuses are rated about 60A it should protect you when shorting happen. But yor battery will function perfectly. But if you don't replace it, it would have less cycle, because the parallel cells has to add more amperage.
```

---
## \#7 Posted by: walleywalker Posted at: 2018-08-10T16:46:44.656Z Reads: 73

```
This was the type of fusing I was referring to. It made sense to me that the filament gauge has to be very close (just above) the max amperage that the cell was capable of putting out, otherwise it's not much of a safety feature? If that case is true, does it not mean that all the filaments (fuses) themselves would run hot even under constant standard load?  Concern being for evacuating heat from the closed battery case. 

[img]https://i.imgur.com/l2RKJoc.jpg[/img]
```

---
## \#8 Posted by: sztamas Posted at: 2018-08-10T16:51:49.837Z Reads: 71

```
That is why you should use a fuse double as the rated amps. If there is a short it will be much more then that.
```

---
## \#9 Posted by: deucesdown Posted at: 2018-08-10T17:03:53.088Z Reads: 66

```
IMO cell level fusing sounds good but doesn't make sense in electric skateboards. A single blown cell fuse is actually quite terrible, but your board may continue to run. You need to be able to inspect and/or measure every connection. Maybe combined with a very sophisticated BMS it would ease the burden of constant monitoring.

I think it makes sense in bigger chassis like cars or even bikes, and in stationary installations without all the environmental issues we have.

Pack level fusing is almost mandatory :)
```

---
## \#10 Posted by: Brdchris Posted at: 2018-08-10T18:14:56.279Z Reads: 56

```
I’m no expert, but I used 20 awg copper for my fuses. It is supposed to pop around 58 amps. So if I have a short circuit it should blow, but also not add much resistance for normal use. I know normally we fuse maybe 25% above max rated current but I’m only concerned about short circuits. Not overloads.
```

---

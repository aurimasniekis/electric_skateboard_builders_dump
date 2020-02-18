# Why are my brakes so bad?

### Replies: 9 Views: 326

## \#1 Posted by: macodrick Posted at: 2019-06-29T20:22:57.439Z Reads: 99

```
I am using the cheap, ebay chinese ESC and remote bundle with a 280kv sk3 motor, running on 6s battery setup. My brakes are underwhelming and dont work very well. Other than that, the esc and remot seem to work really well. is there a way to make my brakes better and modify the ESC to achieve this, that anyone knows of? not sure how it all works but ready to learn if possible
```

---
## \#2 Posted by: ZachTetra Posted at: 2019-06-29T20:36:36.790Z Reads: 96

```
The brakes suck when the battery is full, I think they behave more at 10s but not sure.  If you change the gearing for more torque then the brakes are stronger
```

---
## \#3 Posted by: Qpus Posted at: 2019-06-29T21:16:33.180Z Reads: 77

```
When you brake, your motor turns in to a generator. You should be able to program the brake power in your esc. You can adjust the current that is produced from the generator, higher current -> higher brake torque. 
The problem for strong brakes is that the current you produce while braking is charging your battery. So you can just brake with the maximum charging current of your battery.
```

---
## \#4 Posted by: AlanZhou Posted at: 2019-06-29T21:17:17.273Z Reads: 73

```
[quote="macodrick, post:1, topic:97553"]
is there a way to make my brakes better and modify the ESC to achieve
[/quote]

Nope, because you brought an unconfigurable esc, what size is your sk3 motor and what voltage are you running at.

[quote="Qpus, post:3, topic:97553"]
You should be able to program the brake power in your esc
[/quote]

his esc is not configurable
```

---
## \#5 Posted by: Qpus Posted at: 2019-06-29T21:18:06.722Z Reads: 65

```
That’s true. The bms won’t charge the full battery
```

---
## \#6 Posted by: ZachTetra Posted at: 2019-06-29T21:20:32.779Z Reads: 63

```
If you have a discharge BMS, redo it as a bypass and the brakes are a bit better
```

---
## \#7 Posted by: AlanZhou Posted at: 2019-06-29T21:20:33.794Z Reads: 63

```
[quote="Qpus, post:5, topic:97553"]
The bms won’t charge the full battery
[/quote]

it will, till a certain point, the overcharge detection is usually kick in at 4.25v per cell and if you pass that voltage than the bms will cut off and you will be left without brakes....

^this only applies if your bms is setup for discharge
```

---
## \#8 Posted by: AlanZhou Posted at: 2019-06-29T21:21:52.311Z Reads: 59

```
pretty sure its an esc thing, but I don't think esc substitutes are smart enough to lower brakes when the battery is almost full

when I had an esc substitute brakes  felt weaker when the battery was discharged.
```

---
## \#9 Posted by: Sick Posted at: 2019-06-29T21:58:03.079Z Reads: 52

```
Sounds like my old slick revolution, absolute crap of a board. I needed to setup the brakes everytime before i started using the skateboard. If i didnt it was like they wouldnt break...
```

---

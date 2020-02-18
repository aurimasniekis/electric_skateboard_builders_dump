# Could I wire this Ebay ESC to theoretically work

### Replies: 6 Views: 683

## \#1 Posted by: marcus Posted at: 2017-06-06T01:01:33.674Z Reads: 85

```
Ok,

I've got a totally random idea. So I came across this Ebay ESC and others in the forum have said that it has worked quite well: 
http://www.ebay.com/itm/Dual-motors-longboard-skateboard-controller-with-remote-ESC-Substitute-/302332736118?var=&amp;hash=item46646f7276:m:mfx-qzZdIxn8ZrfP1Gbxebg

However,

The single motor one is only rated to 1300 watts. Yet, the double motor ESC is rated up to 2600 watts (1300 on each motor). What if I wired the matching wires on each side into one female bullet (so the six total wires would be soldered into 3 bullet plugs). Could this theoretically then run a single motor up to 2600 watts? 

Maybe it will explode X)

I'm still a noob in the electronics department..
```

---
## \#2 Posted by: JLabs Posted at: 2017-06-06T01:18:36.392Z Reads: 76

```
No, no, no, no, just no. Lol. If you're trying to use two motors with one ESC it will not work
```

---
## \#3 Posted by: marcus Posted at: 2017-06-06T01:27:59.640Z Reads: 76

```
but I would be using one motor! I want to use a 190kv turnigy which can draw well over 1300 watts. However, as I said, in the description it says that this dual board is rated up to 2600 watts (1300 watts for each output from the board because it is technically a dual motor board). Ill draw up a diagram
```

---
## \#4 Posted by: JLabs Posted at: 2017-06-06T01:49:46.936Z Reads: 71

```
Oh ok. No that won't work. Just save up a little and get a VESC. It will be well worth it in the end
```

---
## \#5 Posted by: Rinzler Posted at: 2017-06-06T01:50:45.562Z Reads: 68

```
PLEASE DONT EVEN TRY THIS! The esc reads the position of the rotor via back emp which was generated when the rotor magnets passed over the stator winding.If both channels are out of sinc they will create a **short circuit** in the stator which will fry your esc and even your motor.If you try this you may end up hurting yourself and the eletrical components of your board.If you didnt understand what i just wrote doesnt matter, just dont do it. :worried:
```

---
## \#6 Posted by: marcus Posted at: 2017-06-06T02:18:17.798Z Reads: 59

```
I completely understood. Like I said, I he a feeling it would blow up....
```

---

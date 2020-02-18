# Dc socket wiring help

### Replies: 22 Views: 556

## \#1 Posted by: red Posted at: 2017-12-28T17:40:42.982Z Reads: 74

```
hello i have a dc socket but no idea how to wire it up or if i need a cable for it. there is just 3 pins on the back do i solder straight to them or is there a cable with connectors on one end.Any help would be greatly appreciated<img src="/uploads/db1493/original/3X/4/9/49c3de9899e98b774c709fb36d42f267afa6e6f2.jpg" width="281" height="500">
```

---
## \#2 Posted by: faithfulpuppy Posted at: 2017-12-28T17:47:42.553Z Reads: 69

```
if you have a multimeter you can figure out which tabs correlate to the pin on the inside, and to the outside bit using the continuity function.
```

---
## \#3 Posted by: red Posted at: 2017-12-28T17:55:45.656Z Reads: 63

```
ok thanks but even so when i figure that out  am i soldering wire to it or am i connecting cables to them
```

---
## \#4 Posted by: faithfulpuppy Posted at: 2017-12-28T18:06:37.644Z Reads: 55

```
what do you mean "connecting cables"? i would assume you're going to be soldering wires to the tabs.
```

---
## \#5 Posted by: red Posted at: 2017-12-28T18:18:54.795Z Reads: 50

```
thats what im asking do you solder wires to them. what size wire would i use
```

---
## \#6 Posted by: faithfulpuppy Posted at: 2017-12-28T18:24:15.228Z Reads: 47

```
well this connector won't be carrying much current (probably 1-5a max) so more or less any wire you have laying around should work unless its really, really tiny.
```

---
## \#7 Posted by: red Posted at: 2017-12-28T18:28:57.108Z Reads: 41

```
ok thanks for the help.they look very small to be soldering to is there clamps or something you can get to create more surface area
```

---
## \#8 Posted by: red Posted at: 2017-12-28T18:31:53.266Z Reads: 40

```
so i am get a current flow on the 2 outsid ones but nothing on the middel one so would i just leave that one alone
```

---
## \#9 Posted by: faithfulpuppy Posted at: 2017-12-28T18:32:08.439Z Reads: 37

```
see those holes in the tabs? you can wrap the wire through that hole and around the side of the tab. That'll give it some more purchase while you solder it on.
```

---
## \#10 Posted by: faithfulpuppy Posted at: 2017-12-28T18:32:55.388Z Reads: 39

```
if the 2 outside ones are continuous/connected to each other, then don't use both as that would just create a short.
```

---
## \#11 Posted by: SilentException Posted at: 2017-12-28T18:33:05.838Z Reads: 38

```
Just a word of advice, get some proper sockets. Metal ones, like [this](https://www.banggood.com/55mm-x-21mm-DC-Power-Jack-Socket-Female-Panel-Mount-Connector-p-931397.html).

As for soldering, put the jack in the socket while doing anything. Otherwise you will probably move the inner part and perhaps even ruin the socket.
```

---
## \#12 Posted by: red Posted at: 2017-12-28T18:42:52.275Z Reads: 37

```
so when i am using the multimeter to check current flow i put red on one of the small pins and the black on the other small pin.the multimeter says current can flow this way your saying it cant?what?
```

---
## \#13 Posted by: red Posted at: 2017-12-28T18:44:25.095Z Reads: 36

```
so id use the big middle one and one small one witch one is+ and witch -
```

---
## \#14 Posted by: faithfulpuppy Posted at: 2017-12-28T18:48:05.485Z Reads: 38

```
if current can flow freely from point A to point B, and you connect the positive to A and the negative to B, you will effectively be connecting the positive directly to the negative. this will create a short. can you show a picture of the two parts you say are connected?

as for which is positive and which is negative, it doesn't technically matter. all that matters is that it matches your charger. I recommend you check your charger to see which part (inside or outside) is positive, and connect your battery accordingly
```

---
## \#15 Posted by: bigben Posted at: 2017-12-28T18:51:49.358Z Reads: 33

```
[quote="SilentException, post:11, topic:42101"]
Just a word of advice, get some proper sockets. Metal ones, like this
[/quote]


This is sound advice. The ones in the original post are not ideal. I had them sparking every time they plugged in.
```

---
## \#16 Posted by: faithfulpuppy Posted at: 2017-12-28T18:57:54.460Z Reads: 31

```
those look good. can you slide a link for a matching male connector? the ones i bought on ebay don't quite fit together and i want to get my board to a point where it almost resembles a complete product
```

---
## \#17 Posted by: red Posted at: 2017-12-28T18:58:47.982Z Reads: 31

```
ok thanks ill do that they look bit more straight forward to solder
```

---
## \#18 Posted by: bigben Posted at: 2017-12-28T19:02:12.814Z Reads: 29

```
Where are you? I've got some of the better ones if you're busting to get going?
```

---
## \#19 Posted by: red Posted at: 2017-12-28T19:05:28.377Z Reads: 29

```
im in ireland
```

---
## \#20 Posted by: SilentException Posted at: 2017-12-28T19:13:08.764Z Reads: 26

```
You didn't mix and match 2.5mm and 2.1mm socket/plug? :slight_smile:

There are no matching plugs AFAIK, only the regular ones. You probably have one already installed on your charger anyhow?

But yes, sometimes due to crappy tolerances, even the matching ones (2.1mm or 2.5mm) are not really tight fit. It's just trial and error. Buy few from one seller, few from other...
```

---
## \#21 Posted by: faithfulpuppy Posted at: 2017-12-28T19:30:18.622Z Reads: 23

```
my charger currently has an xt60 soldered on to it, i lopped off the original connector (like an idiot) and lost it, so i'm looking for a replacement.

the plugs i got were listed as the same size, but the pin in the socket was a little too big for the ID of the barrel jack
```

---
## \#22 Posted by: SilentException Posted at: 2017-12-28T19:40:28.261Z Reads: 22

```
[quote="faithfulpuppy, post:21, topic:42101"]
the plugs i got were listed as the same size, but the pin in the socket was a little too big for the ID of the barrel jack
[/quote]

Might be the tolerances but if it wouldn't fit at all maybe you got wrong plugs after all. Get some Vernier calipers. Mitutoyo or some cheep and cheerful China ones :)
```

---

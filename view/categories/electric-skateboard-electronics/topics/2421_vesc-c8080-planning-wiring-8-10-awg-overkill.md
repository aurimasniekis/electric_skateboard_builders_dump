# VESC &#124; C8080 &#124; Planning wiring - 8/10 awg overkill?

### Replies: 15 Views: 2967

## \#1 Posted by: jaybird Posted at: 2016-04-18T00:27:21.865Z Reads: 209

```
I am still awaiting packages of 8/10/12awg wire, connectors, vesc, etc. In the meantime, plan the layout. 

I know much of what I have here is over sized for the limits of the vesc. But not so overkill if I end up swapping out the current vesc in the future for something that can push my 80mm motor up to its 18s maximum.

Are there any disadvantages to over sized wiring on the vesc, other than weight or wire maneuverability? 
Also, is the xt90 anti-spark connector enough? I have seen loop keys put in the jumper, it this advisable or unnecessary?
Any problem with wiring it how it is shown here?

<img src="/uploads/db1493/original/2X/f/fddb657e937bd28f2c68f18ceda51b3f3c05d3e3.jpg" width="690" height="371">
```

---
## \#2 Posted by: onloop Posted at: 2016-04-18T00:57:50.626Z Reads: 202

```
this will be awesome! how will you fit an 80mm motor?
```

---
## \#3 Posted by: laurnts Posted at: 2016-04-18T00:58:21.817Z Reads: 203

```
I have to say 8awg is an overkill. I never have my cables hot (10AWG all the way).
The idea of cabling for me is that the lower number awg should be on the battery side until it reaches the VESC. So there will be enough room for current to flow no matter how much the VESC is pulling.

If you mix match wire AWG, only the highest AWG is effective. So if you use 10AWG and 12AWG, it's practically just 12AWG.

From your diagram, my recommendation is to remove the 10AWG wire from VESC - battery side and use the 8AWG. It's actually not entirely necessary as you have your batteries connected in series, higher AWG is not needed. Higher AWG cable is only needed / useful when you use your batteries are connected in parallel as their total discharge rating is increased 2x.

Also use 12AWG wire from VESC to motor side as it doesn't get effected with 10AWG wire in between.
```

---
## \#4 Posted by: jaybird Posted at: 2016-04-18T01:05:42.619Z Reads: 194

```
Ok, thanks @laurnts :) That is is the advice I was hoping for. I will go with the 10awg/vesc/12awg and save the the 8awg for building a new harness if and when I need it.
```

---
## \#5 Posted by: lowGuido Posted at: 2016-04-18T01:06:30.476Z Reads: 190

```
I would remove the 8AWG and just go 10AWG all the way. there is really no point to having 8AWG if the battery cables themselves are only 10AWG and then you go back into 10AWG at the VESC.. its pointless.
```

---
## \#6 Posted by: jaybird Posted at: 2016-04-18T01:11:55.918Z Reads: 188

```
@onloop  It fits easy on top ;) 

<img src="/uploads/db1493/original/2X/4/4936a0a8ba9e401c4c056e8796636f7b6e4c860a.jpg" width="690" height="352">
```

---
## \#7 Posted by: jaybird Posted at: 2016-04-18T01:17:36.603Z Reads: 181

```
I know it is pointless, for the vesc. I was considering doing it for the upgrade-abilty. ie, larger controller in the future...
```

---
## \#8 Posted by: lowGuido Posted at: 2016-04-18T01:18:57.190Z Reads: 180

```
well there is no such thing as too big..  unless you can't fit it on your board....

its just sensible to keep everything the same size.
```

---
## \#9 Posted by: jaybird Posted at: 2016-04-18T01:28:33.756Z Reads: 178

```
yeah, but if there is no advantage like laurnts said, I might as well do this one in 10/12awg and do up an new one with the 8awg when needed. My soldering skills could use the extra practice anyway.
```

---
## \#10 Posted by: onloop Posted at: 2016-04-18T01:36:45.810Z Reads: 172

```
awesome!............. please makes some vids when done
```

---
## \#11 Posted by: DougM Posted at: 2016-04-19T06:12:53.865Z Reads: 149

```
Keep in mind that on the motor side your duty cycle is not 100% so the wires can be smaller.  I run 10AWG on the battery side and 12AWG on the motor side.  Run length is the bigger issue - if you are doing long runs, like on a dual motor board, then 10 AWG is preferable, but for short runs you could almost get away with 12AWG all around

DougM
```

---
## \#12 Posted by: barajabali Posted at: 2016-04-19T13:56:48.189Z Reads: 139

```
this this always cool no matter how many times i see it.   I'd love to see a hub motor on it.
```

---
## \#13 Posted by: jaybird Posted at: 2016-04-19T17:12:52.944Z Reads: 139

```
Thanks :) I did a hub motor one a few years ago. I have an old build thread on endless-sphere. [3 wheel Version.2](https://endless-sphere.com/forums/viewtopic.php?f=12&t=53348&p=795206&hilit=smokee#p795206)
<img src="/uploads/db1493/original/2X/a/a9bcd4d1b79be45dacaf7ee6c9a4c21d1eb5fb1b.jpg" width="497" height="360">
```

---
## \#14 Posted by: longhairedboy Posted at: 2016-04-19T18:05:28.894Z Reads: 135

```
I use 10awg on power leads and 12awg on phase leads. 8 is total overkill and would make things more difficult to work with, even on 6S where you have more heat from lower voltages and higher currents.
```

---
## \#15 Posted by: Kmurr Posted at: 2016-08-26T19:46:22.021Z Reads: 102

```
Hay Guys,

Im new to all of this and planning a dual motor set up, Ive herd that the best way to get two VESC power connectors to one battery is to solder two 10awg wires (-- , ++) and then connect to the raptor battery cell.

Does anyone have any good links on how the soldering should be done in this case?

appreciate any guidance given.
```

---

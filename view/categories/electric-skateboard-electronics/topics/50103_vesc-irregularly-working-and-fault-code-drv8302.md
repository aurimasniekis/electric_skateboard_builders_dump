# VESC irregularly working and FAULT_CODE_DRV8302

### Replies: 11 Views: 449

## \#1 Posted by: drassak Posted at: 2018-03-25T18:13:24.538Z Reads: 65

```
Hello all,

My vesc has a wierd behaviour : 
it will work for 20 sec then blink red for 5 sec and log a FAULT_CODE_DRV8302 then come back to normal and so on...

I can comunicate with the vesc using the BLDC tool, write and read configuration without issue. From the outside the DRV looks OK.

is the VESC dead or still there is some troubleshooting option?


<a href="https://www.noelshack.com/2018-12-7-1522001574-capture.png"><img src="https://image.noelshack.com/minis/2018/12/7/1522001574-capture.png" border="0" alt="1522001574-capture.png - envoi d'image avec NoelShack" title="1522001574-capture.png"/></a>
```

---
## \#2 Posted by: RedEagle Posted at: 2018-03-25T18:15:50.303Z Reads: 63

```
What brand? What firmware? When does it occur?
```

---
## \#3 Posted by: GrecoMan Posted at: 2018-03-25T18:24:57.168Z Reads: 57

```
the vesc is dead.
```

---
## \#4 Posted by: drassak Posted at: 2018-03-25T18:29:13.637Z Reads: 58

```
DIYelectric skate, i have been using it for 2 years, 2.54 ackmaniac a couple of weeks ago i rode on wet pavement. 
Since then I get this, can ride my board but I will lose connection 20% of the time : the vesc blink red for a while then back to normal for some seconds the fail again.
```

---
## \#5 Posted by: drassak Posted at: 2018-03-25T18:33:38.092Z Reads: 53

```
I dont have a electronic background but i though electronic componants where quite binary when it comes to functioning. Shouldn't it stop for good once i get the blinking red light?
```

---
## \#6 Posted by: GrecoMan Posted at: 2018-03-25T18:35:16.455Z Reads: 50

```
nah,  the blinking red light is what it does when it restarts, it’s just constantly restarting.

oh btw, i don’t have an electronics background either, I like to think I know the vesc pretty well tho
```

---
## \#7 Posted by: RedEagle Posted at: 2018-03-25T18:51:35.487Z Reads: 49

```
You then most likely have water damage. I'd buy a new one if I were you. This vesc is beyond repair. 
It'll continue behaving like this and when you least expect it it'll stop functioning altogether. 
You could do it but I don't think it's worth the time. Even after you have replaced the drv there could be loads of other damaged parts.
```

---
## \#8 Posted by: drassak Posted at: 2018-03-25T18:56:17.406Z Reads: 49

```
yeah i would put any effort into changing the DRV. 

How would yo explain that I can still make it work in between the intermittent faults? I mean in these phases i can go full speed, uphill etc... it just doesnt last.
```

---
## \#9 Posted by: drassak Posted at: 2018-03-25T18:57:47.826Z Reads: 47

```
would not*
```

---
## \#10 Posted by: RedEagle Posted at: 2018-03-25T18:58:07.920Z Reads: 49

```
Water damaged electrical components. They work fine for a while and then BOOM. 
Apply enough load on a faulty system and it WILL fail.
```

---
## \#11 Posted by: threebysix Posted at: 2018-03-26T01:24:33.460Z Reads: 34

```
I had the same symptoms as you before but I never checked my error log cause I knew I toasted my vesc. It was caused by me riding in the rain and getting water into my vesc.

An easy way to check for damage is do a visual check on your vesc and its components. 

Looks for components that look:
-burnt
-charred
-green rust/oxidation
-white dusty residue 
-bulging capacitors
-funky charred/plastic/smell in general when u sniff the vesc
```

---

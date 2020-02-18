# Vesc Tool doesn´t show any faults, what i‘m doing wrong

### Replies: 6 Views: 195

## \#1 Posted by: Andy87 Posted at: 2018-12-09T11:09:34.517Z Reads: 55

```
I have a faulty focbox.
If I open the terminal in push the menu print faults here
![image|469x500](upload://rK71ToFIckBMnaHUNJ75jEXcKSp.jpeg) 

I don’t get any results. 
Just written „no faults from start up“
I know that I have a DRV fault on the focbox, so it should be listed there.
Do i need to make any updates or push another button to get the fault listed?

Just don’t understand why I don’t get any readings.
```

---
## \#2 Posted by: Bjork3n Posted at: 2018-12-09T11:58:42.835Z Reads: 46

```
Try a motor detection and the fault should show up.
```

---
## \#3 Posted by: Andy87 Posted at: 2018-12-09T12:10:23.275Z Reads: 43

```
Thats not work too.
The motor detection just don’t start without any diagnostic
```

---
## \#4 Posted by: Andy87 Posted at: 2018-12-11T06:54:05.586Z Reads: 21

```
still nobody who can help me?
why my faults not displayed in the terminal.
it should be something easy i´m missing, i´m sure...just what?
```

---
## \#5 Posted by: Bjork3n Posted at: 2018-12-11T06:59:07.529Z Reads: 19

```
I'm sorry but what do you mean that the detection won't start without diagnostics? 
 
I had a vesc a while ago and the drv fault didn't show until I did detection (it failed) or if I would try to spin the motor with the arrow keys on the keyboard.
```

---
## \#6 Posted by: Andy87 Posted at: 2018-12-11T07:06:27.177Z Reads: 15

```
i start the wizzard.
doesn´t matter if FOC or BLDC mode selected, if i push the button for motor detection nothing happens. no red "faulty detection" in the right down corner, nothing. I also can´t rotate the motor with the arrows.

The thing is, if I connect my DaveGA to the focbox it directly show that there is a DRV error on the focbox. I just want to get a diagnostic log in the terminal too.
```

---

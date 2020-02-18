# Just checking my wiring diagram is correct

### Replies: 4 Views: 644

## \#1 Posted by: jason3w Posted at: 2016-11-28T23:56:06.703Z Reads: 74

```
Hey Guys!! 
I've read a fair bit on here and come up with this diagram as a result. 
If any more experienced people can weigh in on this it's would be greatly appreciated. 
I think i've got it right, but first time doing this so just wanted to double check! :slight_smile:

 <img src="/uploads/db1493/original/3X/3/7/3762c467a7fd6731d6444eedb31af85889a84de2.jpg" width="431" height="500">
```

---
## \#2 Posted by: jmasta Posted at: 2016-11-29T01:46:12.496Z Reads: 57

```
I recommend you do NOT connect the red (+) balance wire of your first battery with the black (-) balance wire of your second battery in series.  Technically IF the batteries are hooked up correctly, it would not matter because they are the same voltage.  But if you have the main power leads wired A+B, and you accidentally hook up the balance connectors as B+A, you will short out an entire battery.

Also, I don't know what kind of on/off switch you are planning to use. Make sure it's a mosfet switch, such as those made by Olin or DIY.  A normal switch won't work correctly


**EDIT:  Looking closer at your balance leads, you will short out a battery as you have it pictured now!  The balance leads are reversed.  Easiest fix for your digram is to swap the polarities of your main power leads (make them red, black, red, black.. reading right to left)**
```

---
## \#3 Posted by: VladPomogaev Posted at: 2016-11-29T01:56:09.351Z Reads: 46

```
I agree. The balance leads are backwards, and the easiest solution is to switch the main wires.
```

---
## \#4 Posted by: jason3w Posted at: 2016-11-29T04:49:41.898Z Reads: 36

```
Thanks guys! I've just ordered this https://hobbyking.com/en_us/twin-pack-charge-lead-2-x-3s-6s-w-xt60.html
So hopefully this takes out the errors i was going to make :stuck_out_tongue:

Thanks again. This forum is a great help so far!!
```

---

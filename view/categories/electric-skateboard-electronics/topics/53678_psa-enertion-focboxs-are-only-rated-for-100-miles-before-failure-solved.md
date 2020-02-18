# PSA, enertion FOCBOX&rsquo;s are only rated for 100 miles before failure -solved

### Replies: 18 Views: 380

## \#1 Posted by: ggalisky Posted at: 2018-04-27T18:30:38.745Z Reads: 114

```
This is solved, thank you
```

---
## \#2 Posted by: Acido Posted at: 2018-04-27T18:32:11.044Z Reads: 114

```
send your focbox for repair its like 40$(to a guy on the forum @Martinsp fir EU and @JohnnyMeduse US  )
only vesc that has warranty is the one from HK i think
```

---
## \#3 Posted by: wafflejock Posted at: 2018-04-27T18:37:22.623Z Reads: 113

```
Small clarification regarding power coming from the batteries just because the batteries are rated to be safe up to some amperage doesn't mean that's all you can ever possibly draw from them (it's just as much as you should ever draw), unlike voltage it isn't a hard limit, the voltage is basically fixed on the batteries since you can only overcharge the cells so much before you will have exploded cells.  The max amperage the batteries 'can handle' is based on their IR and heat build up in the cells.
```

---
## \#4 Posted by: barajabali Posted at: 2018-04-27T18:40:21.292Z Reads: 103

```
You don’t think it’s at all possible that the failure is not due to manufacturing defects? 

You rode for 100 miles before anything happened. I can understand if you just installed it and it didn’t work but at what point is Enertion liable. 


There is no reason the focbox would just crap out on you after 100 miles, must be an outside variable
```

---
## \#5 Posted by: ggalisky Posted at: 2018-04-27T18:40:46.095Z Reads: 98

```
Can you give me a example with some number so I can understand this better?
```

---
## \#6 Posted by: ggalisky Posted at: 2018-04-27T18:43:14.536Z Reads: 94

```
I have another one right beside it that is working fine. The phase wires on both FOCBOXs was heatshrinked, and then electrical taped on top of it. The settings on both FOCBOXs are the same, so shouldn't both of them have failed if it was my settings?
```

---
## \#7 Posted by: squishy654 Posted at: 2018-04-27T18:44:06.568Z Reads: 89

```
I had one blow up in my face on the bench..during auto sensing..it attempted to spin a motor and blew..never even got to see it go close to 100 miles...and I didn't even make a giant whiny post either..found some debris had gotten into the case and shorted it out somehow...if anything it should be sealed better if you wish it to last a long time..
```

---
## \#8 Posted by: barajabali Posted at: 2018-04-27T18:44:38.876Z Reads: 87

```
Not necessarily. Do you run in can or split ppm?
```

---
## \#9 Posted by: barajabali Posted at: 2018-04-27T18:45:46.965Z Reads: 91

```
I think I’ve blown up more vesc based hardware than most/many people. For pretty much every reason. And they don’t fail for no reason, the reason may be unknown but there is a reason.
```

---
## \#10 Posted by: ggalisky Posted at: 2018-04-27T18:46:13.466Z Reads: 90

```
https://enertionboards.zendesk.com/hc/en-us/articles/333757028475-How-to-connect-dual-Focboxes

this is what I did. I think you made this diagram too
```

---
## \#11 Posted by: barajabali Posted at: 2018-04-27T18:46:52.147Z Reads: 88

```
Yea there is nothing incorrect of how it is connected if you followed that guideline.
```

---
## \#12 Posted by: wafflejock Posted at: 2018-04-27T18:47:05.762Z Reads: 87

```
As a trivial example say you have a 10V battery (not common but keeping the numbers simple) if you put that 10V across a 1 Ohm resistance you get 10V/1Ohm = 10A current.  If you double the resistance then you half the amperage, with numbers 2 Ohms and 10V still then we have 10V / 2Ohm = 5A.  So depending on what resistance and voltage you will get some particular amperage of flow (Ohm's law).  Batteries also have their own resistance inside of them that causes heat build up in the battery and resists the flow of current so at some point it will limit the current but typically the current values supplied by manufacturers are safe operating limits to avoid overheating the battery and causing degradation of the components:

"The resulting number is the maximum sustained load you can safely put on the battery. Going higher than that will result in, at best, the degradation of the battery at a faster than normal pace. At worst, it could burst into flames. So our example battery can handle a maximum continuous load of 250A."  https://rogershobbycenter.com/lipoguide/

Not saying this is a reason for early failure but just good to know it's not a hard limit when you're reading those values off the battery hence good to limit things on the ESC.
```

---
## \#13 Posted by: mmaner Posted at: 2018-04-27T18:52:02.319Z Reads: 79

```
I just wanna put this out there...

_If you run over 60k ERPM you are taking a risk, regardless of what Enertion says.  The contact AMP value of a battery is not its capability, its what you SHOULD run._  

Those 2 facts are really important if you wanna keep your VESC based speed controllers running.
```

---
## \#14 Posted by: barajabali Posted at: 2018-04-27T18:56:36.383Z Reads: 75

```
@ggalisky  I made the call to reject your case, but I'm willing to have it repaired free of charge. Just send it to me. Give your information to Eric in the thread you have been communicating on.
```

---
## \#15 Posted by: mmaner Posted at: 2018-04-27T18:58:29.774Z Reads: 73

```
thats cool of you bara, good man.
```

---
## \#16 Posted by: ggalisky Posted at: 2018-04-27T18:59:09.337Z Reads: 74

```
Thank you, this is appreciated.
```

---
## \#17 Posted by: barajabali Posted at: 2018-04-27T18:59:43.621Z Reads: 75

```
My pleasure. Eric will rely the ship to address.
```

---
## \#18 Posted by: barajabali Posted at: 2018-04-27T19:00:11.033Z Reads: 73

```

```

---

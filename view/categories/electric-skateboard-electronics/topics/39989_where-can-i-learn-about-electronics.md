# Where can i learn about electronics?

### Replies: 10 Views: 680

## \#1 Posted by: Proxy Posted at: 2017-12-03T05:00:00.393Z Reads: 138

```
The electronics part of building an eskate is confusing me and is the only part thats stopping me from finishing my build. Are there any electronics sources that explains in full detail?

Discharge?
nominal voltage?
Charge voltage?
Amps?
Max amps?
What does the "s" on lipo batteries stand for? i know it means voltage, but how many?
Cells in battery?
and so on....
```

---
## \#2 Posted by: Namasaki Posted at: 2017-12-03T05:24:08.333Z Reads: 134

```
S stands for Series so S = the number of cells connected in series.
P stands for Parallel so P= the number of cells connected in parallel
Putting cells in Series adds their voltage together 
Putting cells in Parallel adds their capacity together
Example:
two battery packs that are 6s 5000mah
Put them in series, you get 12s 5000mah
Put them in parallel you get 6s 10000mah
Lipo cells:
Nominal voltage is 3.7v
Storgage voltage is 3.8v
Full voltage is 4.2v
Discharge voltage is debatable. I personally would consider 3.4v to be a safe min voltage however I usually don't take mine below 3.6v
C rating is very important factor with Lipos. It determines their max discharge amps
Unfortunately, C rating have been blown out of proportion by the battery industry and are only good as a relative guide.
I recommend using Lipos that are 60C or higher.
Besides Google, you can use the search function in this forum.
Best of luck with your build.
```

---
## \#3 Posted by: Proxy Posted at: 2017-12-03T05:56:05.506Z Reads: 113

```
The more i learn the more questions come up. I been using the search function but dont find much on what i want. I already the starter beginner guides pinned to the top. Thats why im asking for sources not answers because i know no one here can give me a satisfying answer (unless they can explain everything like im a 5 year old). Currently researching on youtube but they take forever to get to the point so i guess i have to learn everything from the bottom up.

Nominal voltage is 3.7v?
Storgage voltage is 3.8v?
Full voltage is 4.2v?
Discharge voltage?
Do each type/brand of battery have their own rules/standards?

What the hells does each of these mean?
```

---
## \#4 Posted by: Exiledd_Top Posted at: 2017-12-03T07:27:22.957Z Reads: 104

```
You need to learn about lipos ... not electronics I'll try to exsplain it basically lipos or any cell goes up to 4.2 volts and  that's the Max volts (fully charged )
Nominal voltage is like  the operating volts it was meant to stay at before the cells drop drastically. Storage volt is basically if your not going to use your batteries for let's say a week lipo chargers have a storage setting were they'll charge and or discharge your batteries too 3.8 because that's the manufacturer recommendation to keep them safe if not going to be touched for a while.
Most lipos are the same the only thing that may vary is the cells and c rating the about of Amps may discharge . So if it was a 5s1p that would be 5 cells in one pack 3.7 X 5 = 18.5.v that's not the total  but volts fully charged battery would be 21v
```

---
## \#5 Posted by: davidbonde Posted at: 2017-12-03T07:51:16.700Z Reads: 92

```
For batteries this book is amasing for learning from scratch.

https://www.amazon.com/DIY-Lithium-Batteries-Build-Battery/dp/0989906701

Also check his website and videos on youtube they are also great resourses.

http://www.ebikeschool.com


https://www.youtube.com/playlist?list=PLPqn8bOJKP_nYD-BAKxJHOYovjickM3wD
```

---
## \#6 Posted by: lowGuido Posted at: 2017-12-03T10:36:15.331Z Reads: 71

```
[quote="Proxy, post:3, topic:39989"]
The more i learn the more questions come up. I been using the search function but dont find much on what i want. I already the starter beginner guides pinned to the top. Thats why im asking for sources not answers because i know no one here can give me a satisfying answer (unless they can explain everything like im a 5 year old). Currently researching on youtube but they take forever to get to the point so i guess i have to learn everything from the bottom up.
[/quote]

electronics is pretty complicated, you can spend years studying it. 
however the questions you are asking seem to be related to lithium batteries more than electronics itself.
just keep searching and keep reading.
it's ok to ask questions.
```

---
## \#7 Posted by: Proxy Posted at: 2017-12-05T06:51:44.692Z Reads: 37

```
Thank you David, your post was really helpful.
```

---
## \#8 Posted by: Proxy Posted at: 2017-12-05T06:57:46.200Z Reads: 39

```
Thanks for the help.

When im charging lipo in the future, am i not suppose to charge them completely? Is there a limit of how long i can keep them plugged in? For the example you gave, "**3.7 X 5 = 18.5.v that's not the total but volts fully charged battery would be 21v**", what happens if i plug the fully charged 21v into my board?

Also, does discharge mean to "let out"/"to use the electricity? "

Okay, last one promise.
When you mean "Cell" are you refering to the little "double A" looking batterys within the lipos?
Thanks in advance!
```

---
## \#9 Posted by: Exiledd_Top Posted at: 2017-12-05T16:06:53.695Z Reads: 35

```
When your charging lipos u most likely allways want to charge them fully so they can balance the cells. Your lipo chargers if you have a good genuine one will stop on it's on as long as you put the right settings on the lipo charger as what cell/voltage battery it is . Having a fully charger batteries doesn't hurt as long as it's not over 12s in lipos it, in lipos if you have 12s and fully charged it's over 50v and you exceed the rpm limit but there so many factors that prevent u from exceeding it but just keep that in mind so you don't just spin it  at Max throttle fully charged without load (u on it ).
Discharge means the output so yes what it let's out 
Lipos usually don't like like double a batteries they look like a phone in shape comparation and there stacked in the lipo pack there thin and long usually
```

---
## \#10 Posted by: Yaboiwenis Posted at: 2018-10-27T17:22:47.494Z Reads: 15

```
cheers for the help :grinning:
```

---

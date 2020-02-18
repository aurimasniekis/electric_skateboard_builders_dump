# Help with hollowing-out 3D model

### Replies: 20 Views: 1049

## \#1 Posted by: ikjahaa Posted at: 2017-12-26T16:33:34.479Z Reads: 182

```
So i'm finally down to the enclosure on my build...
Its nearly finished, only need to find how to hollow it out. Cant seem to find it :confused:

Could someone hollow it out with 5mm thick borders for me ? please ? pretty please ? :blush: 
I made it in inventor, but i can export it to a different format if needed.

https://hddemonie.myqnapcloud.com/share.cgi?ssid=0SEAxs6
```

---
## \#2 Posted by: kyletrainy Posted at: 2017-12-26T16:37:40.540Z Reads: 179

```
Try to use the shell function
```

---
## \#3 Posted by: PXSS Posted at: 2017-12-26T16:49:54.769Z Reads: 177

```
Shell,
Move surfaces,
Create the enclosure body and then substract the inside,
There are many ways to do it, you got it!
Shell is definitely the easiest way
```

---
## \#4 Posted by: ikjahaa Posted at: 2017-12-26T16:50:12.881Z Reads: 163

```
I tried it but i cannot get it to work for 5mm borders, i have to use 20mm.....
```

---
## \#5 Posted by: FredrikHems Posted at: 2017-12-26T17:05:28.913Z Reads: 153

```
Is there an offset function? Thats What i use in F360
```

---
## \#6 Posted by: kyletrainy Posted at: 2017-12-26T17:24:25.162Z Reads: 140

```
That’s weird I swear I have made it thinner than that. I feel like a constraint might be doing something there but idk.
```

---
## \#7 Posted by: ikjahaa Posted at: 2017-12-26T18:26:44.090Z Reads: 131

```
Could you possibly do it for me ? :smiley:
```

---
## \#8 Posted by: ikjahaa Posted at: 2017-12-26T18:29:22.101Z Reads: 126

```
I've been tinkering again, somehow it does it on 1mm, 2mm and 3mm but not my desired 5mm arghhh haha
```

---
## \#9 Posted by: GrecoMan Posted at: 2017-12-26T18:34:55.647Z Reads: 122

```
hold on i’ll try in a few minutes
```

---
## \#10 Posted by: GrecoMan Posted at: 2017-12-26T18:46:41.014Z Reads: 122

```
its because the flanges. i added 1mm to the thickness of both of them and was able to shell it
https://drive.google.com/file/d/10LqTXVyhPtAqPnPX8JjtCWkxACzmEBFP/view?usp=sharing

you gotta shell it before adding the flanges if you dont want the flanges to effect the shell
```

---
## \#11 Posted by: wmj259 Posted at: 2017-12-27T04:14:32.745Z Reads: 99

```
I assume the problem has been solved?
```

---
## \#12 Posted by: ikjahaa Posted at: 2017-12-27T10:32:22.821Z Reads: 85

```
Nope, i just checked the model.. first off, thank you for your effort, really appreciate it. But there are some weird circle thingies in that flanges.

Also, I might need some thicker borders to be able to print it in nylon..
```

---
## \#13 Posted by: wmj259 Posted at: 2017-12-28T03:07:41.846Z Reads: 73

```
It does't let me open the file in Inventor, I've tried importing to Solidworks but still nope.
```

---
## \#14 Posted by: ikjahaa Posted at: 2017-12-28T11:12:27.326Z Reads: 65

```
Prob a dumb question, but just to be sure. Did you use the .ipt file ?
```

---
## \#15 Posted by: MrLayton Posted at: 2017-12-28T11:44:35.704Z Reads: 66

```
I just uploaded a model where i hollowed it out. Not sure if it is done well cause I resently began to work with inventor.

wmj259 I don't know if this matters but maybe it is because it is made in 2018 version or something. I can open the file without any errors.
```

---
## \#16 Posted by: GrecoMan Posted at: 2017-12-28T13:28:13.381Z Reads: 52

```
ooooh you want the flanges solid?
```

---
## \#17 Posted by: ikjahaa Posted at: 2017-12-28T15:34:33.401Z Reads: 46

```
yea :smiley:
```

---
## \#18 Posted by: ikjahaa Posted at: 2017-12-28T15:34:46.130Z Reads: 47

```
Thanks mate !
```

---
## \#19 Posted by: wmj259 Posted at: 2017-12-28T16:13:32.821Z Reads: 45

```
That maybe the reason, for some reason I have AutoCAD 2018 installed but Inventor is at 2016... :angry:
```

---
## \#20 Posted by: BenTheBarre Posted at: 2018-03-04T21:55:07.386Z Reads: 35

```
I actually use designspark mechanical. Totally free and has a fully functional shell tool. Check it out.
```

---

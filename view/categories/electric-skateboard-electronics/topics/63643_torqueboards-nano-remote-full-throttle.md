# TorqueBoards Nano Remote full throttle

### Replies: 21 Views: 519

## \#1 Posted by: fredrikinn Posted at: 2018-08-02T20:45:36.691Z Reads: 150

```
Hi, i know there is alot of posts about this but i cant find one with my exact problem.(soory if there is a post with the same problem)

When i turn my board on without connecting the remote the motor goes full throttle until i turn it off again.
If i plug out the controller reciver and turn the board on it donst do anything.
if i turn on the board and connect the controller, it works fine. But when i turn off the controller the motor starts throttleing up. 

i tryed everything i cound find on fail safe here on the forum but nothing works.
Does anyone have an idea about what i can do? Thanks
```

---
## \#2 Posted by: accrobrandon Posted at: 2018-08-02T20:49:56.953Z Reads: 135

```
U sure in your ppm settings its on "current no reverse" ?

and you have either just ppm or 
ppm and uart selected if using BT
```

---
## \#3 Posted by: mccloed Posted at: 2018-08-02T21:09:16.822Z Reads: 125

```
Did you try this already? https://www.electric-skateboard.builders/t/2-4ghz-nano-remote-sold-out/5017/83
```

---
## \#4 Posted by: fredrikinn Posted at: 2018-08-02T21:12:16.681Z Reads: 122

```
Setting are on current no reverse and just ppm
```

---
## \#5 Posted by: fredrikinn Posted at: 2018-08-02T21:14:09.204Z Reads: 112

```
Yeah, with no luck
```

---
## \#6 Posted by: bigben Posted at: 2018-08-02T21:18:38.995Z Reads: 107

```
Have you set up the dead band on the vesc tool?
```

---
## \#7 Posted by: fredrikinn Posted at: 2018-08-02T21:24:44.453Z Reads: 103

```
Set to 0,15
![image|666x500](upload://xcn8k5jHkFR9wu9YGg4yNk5Y9UG.jpeg)![image|666x500](upload://fZaD6j8XqyA3OP2JgTXde4N3uyR.jpeg)
```

---
## \#8 Posted by: bigben Posted at: 2018-08-02T21:34:36.283Z Reads: 99

```
Sorry, someone will be able to explain this better than me. When you run through the app wizard you set up the parameters of your controller?
https://www.youtube.com/watch?v=v1glLDO-EjA&t=694s
About 14 minutes in is what I mean. Pulsewidth?
```

---
## \#9 Posted by: fredrikinn Posted at: 2018-08-02T21:48:23.048Z Reads: 94

```
If youre talking about pulsewidththen yes. But the vesc program in the video is that a new one? And will it wwork on mye old vesc
```

---
## \#10 Posted by: bigben Posted at: 2018-08-02T22:04:11.411Z Reads: 90

```
Yes it should do.
It's the new vesc tool.
```

---
## \#12 Posted by: fredrikinn Posted at: 2018-08-02T23:23:47.527Z Reads: 85

```
When im connected to BLDC tool and turn off the remote controller this  happens

![image|320x385](upload://hllZVdaWsNl34pxeljh0eXIQtMI.gif)
```

---
## \#13 Posted by: fredrikinn Posted at: 2018-08-03T09:33:46.266Z Reads: 71

```
Any ideas? Will it help to buy a new reciver maybe?

Bump
```

---
## \#14 Posted by: Andy87 Posted at: 2018-08-05T09:24:28.942Z Reads: 62

```
Your failsafe is set wrong
Pair you remote new with the trigger centered.
After it should be fine
```

---
## \#15 Posted by: fredrikinn Posted at: 2018-08-05T10:27:43.768Z Reads: 61

```
How do i pair it new? Feel like i tryed everything
```

---
## \#16 Posted by: fredrikinn Posted at: 2018-08-05T12:13:17.353Z Reads: 54

```
@torqueboards
```

---
## \#17 Posted by: Andy87 Posted at: 2018-08-05T15:46:07.639Z Reads: 52

```
Plug in your pairing brige on the receiver.
Remote switched off
Turn on your board
Press the pairing button on the remote and hold it
Than switch on your Remote still holding the pairing button.
Take care that the trigger is in center position while doing this.
Switch off everything 
When you now switch on everything, all should be good
```

---
## \#18 Posted by: torqueboards Posted at: 2018-08-05T15:50:18.058Z Reads: 51

```
@fredrikinn I told you how to solve it. Same thing Andy87 is mentioning to you.
```

---
## \#19 Posted by: fredrikinn Posted at: 2018-08-05T15:53:22.669Z Reads: 49

```
@torqueboards @Andy87 tryed that 10-15 times now, still no luck 😕
```

---
## \#20 Posted by: Andy87 Posted at: 2018-08-05T16:24:02.971Z Reads: 47

```
One thing I could imagine it could be too.
Look in your ppm settings.
Is there some break current defined in case of signal loss?
Usually it would only break but look if there is written 0a
```

---
## \#21 Posted by: Andy87 Posted at: 2018-08-06T07:40:58.888Z Reads: 39

```
You managed?
```

---
## \#22 Posted by: fredrikinn Posted at: 2018-08-06T10:23:10.906Z Reads: 37

```
It was set to 0A, but didnt help changing it 😕 looks like i need to get a new remote and reciver. Think im going to try a different one this time, have been some problems with torqueboardes remote. Have problems with pair the remote to the reciver aswell now.

But thanks for all the help, good to know i tryed everything i could before i get a new remote.
```

---

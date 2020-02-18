# NEED HELP! Board won’t turn on

### Replies: 15 Views: 189

## \#1 Posted by: Sk8technica Posted at: 2019-04-06T03:11:12.785Z Reads: 67

```
Any help would be appreciated. So here’s my build, diyeboard dual belt drive kit. V2.1 Dual Belt Motor FOC ESC with custom battery 10s3p 8.7ah Korean LG MG1 2900mah. 
Upon setting up the board and tested on smooth road it runs fine, until going through a bump on asphalt pavement the board shuts down and wouldn’t turn on. Board was fully charged.
What seems to be the problem? 

![image|375x500](upload://cm6DfttS3RVUt4MfFnMnHe2JiAh.jpeg) ![image|666x500](upload://l8zESoxURyE4GAuC6WwGTY4HEt9.jpeg)
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-04-06T03:57:05.642Z Reads: 57

```
Go through the list of what could be wrong:
Is there voltage from the battery? 
Is the antispark plugged in all the way?
Are the other connectors plugged in all the way?
Is there voltage to the ESC?
Does the ESC show any signs of life?
etc
```

---
## \#3 Posted by: Sk8technica Posted at: 2019-04-07T00:19:04.729Z Reads: 45

```
Yes there’s voltage on the battery (40.1V), anti spark plug in all the way, every connectors are plugged in correctly, when disconnecting battery and ESC xt60 there was voltage on ESC but goes down to 0V over time, there’s life on ESC. 
I’m guessing problem is battery or BMS?
```

---
## \#4 Posted by: MysticalDork Posted at: 2019-04-07T00:22:23.794Z Reads: 41

```
If you've got voltage to the ESC, I'd guess it's an issue with the ESC.
```

---
## \#5 Posted by: RedBaron Posted at: 2019-04-07T00:29:19.174Z Reads: 40

```
If it cutt off durring a bump and you don't visually see a loose connection with ur hardware then the problem is most likely a broken weld or a week series connection inside the battery between the cells.
```

---
## \#6 Posted by: maxchilton Posted at: 2019-04-07T00:34:22.024Z Reads: 39

```
lol @ the shred or die sticker, i guess your board chose to die. :joy:
```

---
## \#7 Posted by: Sk8technica Posted at: 2019-04-07T02:03:32.266Z Reads: 33

```
How do you define a faulty ESC? Picture below shows no voltage
[image|375x500](upload://7AvCuIxHKrIUOLgZBNK3sGNUB7W.jpeg) 

[image|375x500](upload://1CgJWdV3ovUkh4j1Bt1ZENMsZ5X.jpeg)
```

---
## \#8 Posted by: Sk8technica Posted at: 2019-04-07T02:05:33.000Z Reads: 33

```
Could be. I’ll have to check
```

---
## \#9 Posted by: MysticalDork Posted at: 2019-04-07T02:49:07.515Z Reads: 30

```
[quote="Sk8technica, post:3, topic:89545"]
when disconnecting battery and ESC xt60 there was voltage on ESC but goes down to 0V over time, there’s life on ESC. I’m guessing problem is battery or BMS?
[/quote]
Does this mean when you have the ESC plugged in it has voltage, but when you **disconnect** it the voltage goes down slowly, or that the voltage goes down **while it's plugged in**?
```

---
## \#10 Posted by: Sk8technica Posted at: 2019-04-07T03:13:15.213Z Reads: 26

```
When I **disconnect** voltage goes down slowly
```

---
## \#11 Posted by: Wilsonliang777 Posted at: 2019-04-07T03:21:06.778Z Reads: 24

```
Remote got unpaired?   Maybe try pairing the remote again?
```

---
## \#12 Posted by: MysticalDork Posted at: 2019-04-07T03:37:00.115Z Reads: 22

```
Yeah, that's normal. Capacitors. If the voltage dropped while plugged in, I'd suspect BMS. But it doesn't, so I suspect ESCs.
```

---
## \#13 Posted by: Sk8technica Posted at: 2019-04-07T03:52:15.974Z Reads: 21

```
I don’t think so. If the board wouldn’t turn on how will the remote pair
```

---
## \#14 Posted by: Sk8technica Posted at: 2019-04-07T03:53:52.540Z Reads: 21

```
So when it’s plugged in, board turns on runs fine. Over bumps it shuts off. Then I have to repeat the whole process again of plugging and unplugging the xt60 to have the board running. 

I should probably do that test, voltage drop when plugged in

*Update*
I tested voltage drop when plugged in and it maintained at 40.1V. Is this the ESC problem then?
```

---
## \#15 Posted by: MysticalDork Posted at: 2019-04-07T08:03:26.840Z Reads: 12

```
That would be my guess. Only real way to be 100% sure unless you can see a physical defect anywhere, is to start swapping parts. Swap the ESCs, and see if it works. If not, then it's probably the battery. Swap the battery, and see if it works. If not, then it's probably something else. Basically, think yourself up a flowchart of everything that has to go right for the board to work, and start replacing one chunk at a time until the problem goes away.
```

---

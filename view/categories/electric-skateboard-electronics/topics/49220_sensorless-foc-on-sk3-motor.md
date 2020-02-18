# Sensorless FOC on SK3 motor

### Replies: 8 Views: 621

## \#1 Posted by: HCWH97 Posted at: 2018-03-15T22:00:04.006Z Reads: 161

```
Hello 
I want a new VESC since I hate the ESC I am using now. 
I have a tunigy SK3 280kv motor and it has no sensor wires. Is it possible to run FOC on that motor sensorless? Could a FOCBOX do the job or is a maytech okay?
```

---
## \#2 Posted by: rok Posted at: 2018-03-15T22:12:24.832Z Reads: 160

```
Yes, you can run sensorless FOC and yes, FOCBOX :wink:
```

---
## \#3 Posted by: HCWH97 Posted at: 2018-03-15T22:22:28.071Z Reads: 154

```
thx :) do you know where i can find the setting for that?
```

---
## \#4 Posted by: FredrikHems Posted at: 2018-03-15T22:31:47.159Z Reads: 146

```
What voltage are you running? 280kv isnt optimal..
```

---
## \#5 Posted by: Jammeslu Posted at: 2018-03-15T22:46:37.041Z Reads: 138

```
He would have to limit erpm, or is that even possible on foc?
```

---
## \#6 Posted by: FredrikHems Posted at: 2018-03-15T23:00:07.740Z Reads: 132

```
Nope. Not that I am aware of at least
```

---
## \#7 Posted by: onepunchboard Posted at: 2018-03-16T02:15:25.171Z Reads: 109

```
u can limit erpm at ppm section on foc. 
for 280kv u wont get much torq.
cuz 6s esc usually have 120a~150a where as even focbox only go up to 100a.
I strongly advise u to get bigger motor for low kv
it will suffer at hill for both going up and down because motor won't brake the board either.
```

---
## \#8 Posted by: HCWH97 Posted at: 2018-03-16T07:49:50.033Z Reads: 85

```
thanks for the reply. Makes sense bc. i have had problems with breaking...
```

---

# 6s battery voltage per cell difference

### Replies: 11 Views: 503

## \#1 Posted by: s00cl0se Posted at: 2017-11-08T23:19:08.774Z Reads: 48

```
Hi all , so i balance charged my new 6s (3sx2 8000mah) battery @ 2.0-2.2A  , almost full , to 24.6V. these are the voltages, are these within range of each other , if not how to fix it
4.07
4.11
4.12
4.11
4.12
4.09

24.6V

resistance is
032
001
001
001
002
024
```

---
## \#2 Posted by: MysticalDork Posted at: 2017-11-08T23:29:17.839Z Reads: 45

```
Looks like the first and last cells have much higher internal resistance than the others, and they're also the ones with the most voltage difference. This may indicate that those cells are damaged, faulty or older than the others. 

You should be balance charging them if you aren't already, and for the first few rides you should check the voltages often, and not discharge them too far. 

They may break in and become more even as time goes on. If not, you may want to consider replacing the cells or the pack.
```

---
## \#3 Posted by: s00cl0se Posted at: 2017-11-08T23:32:31.525Z Reads: 43

```
okay kool , this is the first time i charged them full btw, tomorrow i will do the full run , and see if they stabilize. is it okay to run it full without load, as i want to do that , then charge them to storage and put them back as i dont have much time nor i have the motor mount, the motor is mounter on a peice of 2mm aluminum.
```

---
## \#4 Posted by: MysticalDork Posted at: 2017-11-09T00:02:10.381Z Reads: 35

```
What sort of battery charger do you have? Most have a discharge function. That would be easier and safer than using the board to drain them, and allow you to monitor the voltage as it discharges.
```

---
## \#5 Posted by: s00cl0se Posted at: 2017-11-09T00:09:42.218Z Reads: 33

```
imax b6 ac v2
```

---
## \#6 Posted by: s00cl0se Posted at: 2017-11-09T00:10:15.890Z Reads: 32

```
at full cahrge they are 4.13 4.20 , 4.2 4.2 4.2 4.16
```

---
## \#7 Posted by: s00cl0se Posted at: 2017-11-09T00:20:56.346Z Reads: 32

```
so i basically stary the battery storage function now? or battery discharge fnction
```

---
## \#8 Posted by: MysticalDork Posted at: 2017-11-09T00:22:45.789Z Reads: 31

```
I'd do a storage, then check them and balance charge them again. Emphasis on balance charge, not fast charge.
```

---
## \#9 Posted by: s00cl0se Posted at: 2017-11-09T00:24:30.149Z Reads: 32

```
so  is it fine to storage charge them instantly after full balance charge, sorry i am noob
```

---
## \#10 Posted by: s00cl0se Posted at: 2017-11-09T00:25:57.173Z Reads: 31

```
also i can storage charga at 1a  or 2a , what do u suggest
```

---
## \#11 Posted by: MysticalDork Posted at: 2017-11-09T01:46:51.597Z Reads: 23

```
Whatever is the fastest the charger can handle. Usually there's a limit with high voltage batteries (>12v) because the discharge circuitry dissipates a lot of heat.
```

---

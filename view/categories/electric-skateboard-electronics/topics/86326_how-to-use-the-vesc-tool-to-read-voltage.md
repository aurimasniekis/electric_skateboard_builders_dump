# How to use the vesc tool to read voltage

### Replies: 3 Views: 314

## \#1 Posted by: humanisticnick Posted at: 2019-03-06T16:49:09.530Z Reads: 62

```
I am going back and forth with TB about a battery purchase and I don't have a multi-meter to test the battery. I am wondering if I use the battery to power a vesc and I connect to it via USB to the VESC tool on windows is there a way I can see the actual live voltage available coming from the battery? Forgive my ignorance lol.
```

---
## \#2 Posted by: olestra Posted at: 2019-03-06T19:50:15.913Z Reads: 48

```
Images should explain... connect, click stream realtime data and stream realtime app data, then go down to data analysis and select realtime data

On the bottom right you'll see the total voltage from your pack. there is no display for individual cell voltage since the balance leads don't connect to the Vesc.

![image|123x500](upload://f3ET5BFaBgk1TUzIpI7O1b01AhL.png) 
![image|241x483](upload://cwIJXImOE2zTkFEuNHpQ2H5dDmF.png) 
![image|690x116](upload://ywIHXtsjx1zTYBMnItwwHQpcEtW.png)
```

---
## \#3 Posted by: humanisticnick Posted at: 2019-03-06T20:36:29.702Z Reads: 43

```
Thank you very much
```

---

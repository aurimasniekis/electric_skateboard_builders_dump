# VESC tool setup

### Replies: 2 Views: 429

## \#1 Posted by: KeivanM Posted at: 2018-09-20T22:15:53.421Z Reads: 63

```
Hello all, sorry to bother you guys but I just wanted a quick opinion on my setting for my board and to see if I can improve performance and or safety! By the way my setup is:
12s4p on samsung 30qs
192kv sk3 6374 ( Max Loading:  **80A**  Max Power:  **4032W**  )
97mm flywheels
36T/18T ratio
345mm belts 12mm 5M
218mm trucks
![image|472x500](upload://iJS2DLmIeiP7zkyRDJVx7PLoBjR.png) 

![image|494x500](upload://9CGNp7JwS1E8CeoABp6lN1qyK1o.png) 

![image|498x500](upload://pSyxHlanvhT2mHD0x6Z3RDGCiQd.png) 

![image|495x500](upload://us2sq39z0IB0umjMMt993AUeghA.png) 

![image|493x499]

![image|493x500](upload://nonGPh9wE7n8Jhk5wVVOoyv4rhN.png) (upload://vZA8I1IShXatUZQuF5D22CVdP6L.png) 

![image|492x500](upload://dDMwTkoDAyY59SrdDkuJ3SdRH9j.png)
```

---
## \#2 Posted by: mynamesmatt Posted at: 2018-09-20T23:14:59.643Z Reads: 44

```
Your motor doesn't have hall sensors so change to bldc mode. 
your motor settings are fine, just expect a shit load of torque. 
i personally would up the battery amps to 30a.
id make the battery cutoff start at 40.8V, and the cutoff end to 38.4V, just helps with longevity of the pack a lil
```

---

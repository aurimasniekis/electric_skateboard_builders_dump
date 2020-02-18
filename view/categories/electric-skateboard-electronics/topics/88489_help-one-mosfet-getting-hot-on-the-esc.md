# \[HELP\] One MOSFET getting hot on the ESC

### Replies: 7 Views: 210

## \#1 Posted by: reiko Posted at: 2019-03-27T17:58:34.011Z Reads: 38

```
Hey,

I am rebuilding my old board for the now very near esk8 season and noticed something that raised some concerns.

I am using the dual ESC substitute, bought it nearly a year ago from @dickyho on eBay. I connected a battery to it and even without needing to spin the motors, one MOSFET on the board started warming up. It never reached a temperature that I couldn't touch it, but it was still considerably hotter than other parts of the controller. I connected the motor phase + sensor wires and tried spinning the motors and everything seemed to work great.

I'll post some pictures to give you an idea, which MOSFET thinks it deserves to be hotter than others. Circled with light blue to illustrate hope.

![Inkedphoto_2019-03-27_19-33-08_LI|375x500](upload://wjb2iLNPNYnlhxTEXng2icSgExO.jpeg)

Here are some close up pictures from different angles.

![photo_2019-03-27_19-34-07|373x301](upload://1TbsCvkxNt2Jepc8UorNcRZmKZf.jpeg) 


![photo_2019-03-27_19-34-07%20(2)|302x191](upload://6Wy11jWQfeurfVd2v2rmJzv4rFR.jpeg) 

As seen on the last image, the type(?) is 78M05. Not sure if it means anything though.

- What are your thoughts?

- Is this ESC safe to use?
- Is it normal behaviour for a MOSFET to heat up like that?
- If not, what could I do to fix it?

I do want to upgrade to VESCs, but I can't afford them at the moment. VESC swap is high on my list of upgrades however. I just want to start riding again, really :confused:
```

---
## \#2 Posted by: Blasto Posted at: 2019-03-27T17:59:43.265Z Reads: 35

```
7805, that's a 5V LDO. By nature, they get hot
```

---
## \#3 Posted by: Sn4pz Posted at: 2019-03-27T18:02:54.451Z Reads: 33

```


[quote="Blasto, post:2, topic:88489, full:true"]
7805, that’s a 5V LDO. By nature, they get hot
[/quote]

maybe slap a little cooling fin on it :) 

https://www.amazon.com/Cosmos-Copper-Cooling-Heatsinks-cooler/dp/B00637X42A/ref=pd_lpo_vtph_147_bs_t_1?_encoding=UTF8&psc=1&refRID=KR9EA669MH6ECKQVBCH8
```

---
## \#4 Posted by: banjaxxed Posted at: 2019-03-27T18:27:40.355Z Reads: 30

```
Think top is plastic, so may not help
```

---
## \#5 Posted by: AlanZhou Posted at: 2019-03-27T18:29:11.722Z Reads: 30

```
Thermal pad 😉
```

---
## \#6 Posted by: Sn4pz Posted at: 2019-03-27T18:29:18.210Z Reads: 26

```
woops, oh well
```

---
## \#7 Posted by: Gamer43 Posted at: 2019-03-27T21:55:16.332Z Reads: 15

```
What's your battery voltage?

If you really want, you could by bypass it with a 5V BEC xD.
```

---

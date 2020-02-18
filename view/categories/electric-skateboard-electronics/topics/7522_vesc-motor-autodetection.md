# VESC motor autodetection

### Replies: 5 Views: 469

## \#1 Posted by: petmakris Posted at: 2016-08-11T22:50:30.621Z Reads: 67

```
I successfully blew up my first VESC when I tried to autodetect in BLDC mode a motor with 149KV (this motor in particular  http://www.hobbyking.com/hobbyking/store/__18184__Turnigy_Aerodrive_SK3_6374_149kv_Brushless_Outrunner_Motor.html)

I used 12s fully charged and the bam was quite good. 

Now I am testing the same motor with a 3A - 19V power supply and a new VESC ofcourse and either in BLDC and FOC mode detection fails.
In FOC only the R & L seems to succeed.

Any recommendations, on what PS supply to use for motor detection? What should be the minimum A/V specs for a PS to use?
```

---
## \#2 Posted by: hugohammarstrom Posted at: 2016-08-11T23:18:30.966Z Reads: 59

```
Check if you have the battery cutoff set properly for your voltage, motor detection doesn't work if the battery cutoff is active.
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-08-11T23:29:13.052Z Reads: 58

```
where did u get your vesc from?>
```

---
## \#4 Posted by: petmakris Posted at: 2016-08-11T23:30:28.414Z Reads: 56

```
I bought the vesc from enertion last batch , it's v4.12.

Please, what is a properly set battery cutoff for my voltage?
```

---
## \#5 Posted by: hugohammarstrom Posted at: 2016-08-12T00:16:15.510Z Reads: 51

```
The battery cutoff trigger points should be lower than your voltage, so in this case lower than 19v [quote="petmakris, post:1, topic:7522"]
3A - 19V
[/quote]
```

---

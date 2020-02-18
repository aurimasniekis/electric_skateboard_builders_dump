# Vesc Slow Take off

### Replies: 3 Views: 465

## \#1 Posted by: crisonix01 Posted at: 2017-06-08T12:34:13.336Z Reads: 91

```
Hi, I recently acquired a vesc, but my board accelerates really slowly, it can push me fine even from a complete stop but it goes the same speed for like 4 seconds and then picks up, it's really annoying to start up. I like how smooth it is id just like a bit more kick, I use a 12s 5000mah lipo battery, sk3 149kv 6374 motor, vesc. My battery and motor max amp is set to 60. Does anybody knows how to fix this issue?
```

---
## \#2 Posted by: chaka Posted at: 2017-06-08T13:11:26.309Z Reads: 82

```
C̶h̶e̶c̶k̶ ̶y̶o̶u̶r̶ ̶l̶o̶w̶ ̶v̶o̶l̶t̶a̶g̶e̶ ̶c̶u̶t̶-̶o̶f̶f̶.̶ ̶I̶t̶ ̶i̶s̶ ̶p̶r̶o̶b̶a̶b̶l̶y̶ ̶s̶e̶t̶ ̶f̶o̶r̶ ̶a̶ ̶1̶0̶s̶ ̶b̶a̶t̶t̶e̶r̶y̶.̶ ̶

Edit, now that I am fully awake I realized you are rocking a 12s battery. . You could be experiencing some heavy voltage sag since 5000mah is too small.

You might get better performance from that pack if you lower your motor and battery amps down to 30.
```

---
## \#3 Posted by: Jinra Posted at: 2017-06-08T14:50:27.282Z Reads: 61

```
Keep in mind he's using prismatic lipos. He should be getting at least better performance than he's currently getting. 

As you originally mentioned, it's perhaps the low voltage cutoff. @crisonix01, Please post your vesc settings
```

---

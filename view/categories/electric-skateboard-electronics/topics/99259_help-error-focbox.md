# Help error focbox

### Replies: 5 Views: 106

## \#1 Posted by: Djawho Posted at: 2019-07-28T13:47:54.930Z Reads: 40

```
hi guys
i have a problem with my focbox (last ackmaniac) and an new sk8 6374 149KV (battery 10S 4P 10A, Bms bestech hcx d223 v1) . When i brake i lost the connection , whitout capacity of brake or accelerate .
 And subaltern problem , the connection with the app android ackmaniac , work 1 time to 10...
Do you have an idea ??? thx![Screenshot_20190728-114926|281x500](upload://stBTNKqvzkH5zxOCk8CISJnhaV6.png) ![Screenshot_20190728-152810|281x500](upload://gZE7Dvoa8C1Wq77MaoXyOPSOWYi.png)
```

---
## \#2 Posted by: L3chef Posted at: 2019-07-28T21:38:10.924Z Reads: 27

```
You are getting over voltage fault. Start by checking every wire in your setup
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-07-29T00:12:06.492Z Reads: 25

```
@Djawho  I've never used this specific BMS, but the specs say maximum 20A charging current and you're running 24 for regen (12 per vesc). That charge rating is usually through the C- connection rather than P-, so I can't be sure how it'd behave, but I'd suspect your BMS is shutting off due to excessive charge current and that's causing a voltage spike that's causing the vesc to throw an error. Try setting your regen to 10 or less per side, and see if the problem persists.
```

---
## \#4 Posted by: Djawho Posted at: 2019-07-29T00:35:07.287Z Reads: 24

```
thx , but it's not that . I have only one motor and focbox
```

---
## \#5 Posted by: sayekim Posted at: 2019-07-29T10:00:04.080Z Reads: 19

```
I think your bms is cutting you off due to braking on a full battery which makes you hit the over voltage cut off. 
Your esc will do the same as soon as it sees more than 57V.
```

---

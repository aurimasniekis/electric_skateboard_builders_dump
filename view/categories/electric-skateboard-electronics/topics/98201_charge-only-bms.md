# Charge only bms

### Replies: 6 Views: 138

## \#1 Posted by: JoelMatousek Posted at: 2019-07-10T15:40:50.479Z Reads: 47

```
This may have been talked about before, but I couldn't find anything.  I got a charge only 10s bms. It says that you don't use pin 1. I feel like I should connect it to the battery negative but I'm not sure![Screenshot_20190710-113918_Chrome|243x500](upload://4q5korTmuKsifpUt9tcxlTqDluU.jpeg)
```

---
## \#2 Posted by: accrobrandon Posted at: 2019-07-10T18:12:15.351Z Reads: 40

```
depends how many wires are on the pigtail... i literally JUST installed a 12s one an hour ago... had 13 wires.... first one goes to battery negative... if you only get 10 then u know what to do... i bet youll probably have 11 tho.... on the pcb the slot without a line says battery negative...
```

---
## \#3 Posted by: bsancken Posted at: 2019-07-10T18:38:05.391Z Reads: 38

```
Use a multimeter and check if there is continuity between common ground and that first pin. I bet they're connected internally making that redundant.
```

---
## \#4 Posted by: JoelMatousek Posted at: 2019-07-10T18:38:25.332Z Reads: 36

```
I didn't even think of doing that
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-07-10T18:47:40.325Z Reads: 35

```
If you have d140 bms, and same amount of balance wires as S in your battery, start with first balance wire between 1st and 2nd group. That means, no balance wire goes on battery - . You can see that nothing is soldered on pcb where first balance wire should be.
```

---
## \#6 Posted by: JoelMatousek Posted at: 2019-07-11T11:58:01.676Z Reads: 18

```
I checked, they are both connected. So I guess it doesn't matter. Although just as a precaution I'll use it
```

---

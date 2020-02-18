# Battery Safety - Balance Cable Adapter 3S to 6S

### Replies: 1 Views: 151

## \#1 Posted by: HillRipper21 Posted at: 2018-08-06T01:19:09.123Z Reads: 25

```
Tldr: don't be an idiot with lipos, made this post so other beginners who don't know much about electronics don't do what i did

I don't have much electronics background and i imagine anyone else in this position can get easily confused with this. If you have the 3S to 6S balance cable adapter this applies. There is nothing stopping you from connecting them backwards and causing a short.

Using a multi-meter, start from the end and measure each individual voltage ALL THE WAY DOWN do not stop after the first one if its ~3.7V and you think its good. They should increment up to about 23V for 6S. When you get to the 4th pin, if it is a negative reading, this means its shorted, switch them around. 

Personally I was confused by this because there's no safety mechanism to tell you they are on wrong. Luckily it only cost me a $2 adapter and 1 port on a parallel charging board. 

See pics below: 
Good: ![20180805_204546|374x499](upload://bM8ncWO9zP66kVLSuLWnBGRU6gg.jpg)
Good: ![20180805_204409|374x499](upload://ytIGJWl8YGemz3Q23MeXSf2Rp6g.jpg)
BAD: ![20180805_204601|374x499](upload://3LkAMyxCVXZK3lJ9VtyFYm9U42U.jpg)
BAD: ![20180805_204554|374x499](upload://ysmDsFk0v7jN0TauCjAZABtUaGG.jpg)
```

---

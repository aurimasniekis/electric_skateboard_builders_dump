# 192kv 6374 Sk3 &#124; 5 x 2s 5000mAh 20C &#124; BLDC settings

### Replies: 3 Views: 335

## \#1 Posted by: usual Posted at: 2017-07-09T09:29:55.507Z Reads: 62

```
Hey there, 

I have a setup without BMS. 
Are these settings okay? 

Motor max/min:  60A/-40A
Batt max/min:.    30A/-20A

Maximum input voltage: 42V
Battery cutoff start: 33V
Battery cutoff end:. 30V
```

---
## \#2 Posted by: Achmed20 Posted at: 2017-07-09T11:24:18.021Z Reads: 57

```
motor OK but i can handle up to 80A max if i remember correctly
batter can do 100A so 100A should be max

voltage seems completely off.
Max input voltage can/should be the default which is 52. there is no need to mess with this value
cutoff start doesnt realy matter as long as its heigher then the min voltage (tbh thats more a guess).
Cutoff end is way to low. this would mean that the board will shutdown down when each cell is at 3V which kinda killed the battery allready. you should not go lower then 3.2V per cell which means cutoff end is 32V.
```

---
## \#3 Posted by: usual Posted at: 2017-07-09T16:16:59.995Z Reads: 29

```
Thank u! 
I've set the battery cutoff start to 35 and end 33. 
One question, with an 77A BMS would the batt max be 77A?
```

---

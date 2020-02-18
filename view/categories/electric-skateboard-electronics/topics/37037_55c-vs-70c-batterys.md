# 55c vs 70c batterys

### Replies: 8 Views: 347

## \#1 Posted by: lunasicc Posted at: 2017-11-01T05:06:57.907Z Reads: 63

```
Currently running dual 4s 5ah in series(70c) 5000mah 8s 70c. I'm looking to get more packs soon. The same battery in 55c is like $20 cheaper. Would I see any power differences if I swapped to the 55's? I don't want to spend extra money if there is no advantage. Only reason I went with the 70's was cause they were insanely cheap.
Setup is a mtb with dual direct drive, 240kv 6374's, 8s with max 6
```

---
## \#2 Posted by: ShutterShock Posted at: 2017-11-01T06:26:09.505Z Reads: 57

```
Do you have any idea how much current you draw at max load?  Bluetooth monitor or anything?  70C is crazy high but it kind of makes sense for a mtb because sometimes the battery manufacturers talk up there batteries a lot.

IMO 55C will probably still be enough, I would imagine you don't draw anywhere near the max amperage output, but it is hard to say without an actual value from the board
```

---
## \#3 Posted by: Cobber Posted at: 2017-11-01T06:43:40.151Z Reads: 53

```
Mixing lipos is not a good idea as discharge/charge speed/rates will vary (I'm not talking C rating). Even just mixing new with old batteries of same brand/type can cause issue. You will need to be monitoring individual cell charge and discharge to make sure you do not destroy some cells or worst case cause catastrophic failure (fire).

I would guess if you are asking, you do not have the knowledge to safely try... best practice is to buy and use your lipos in sets at one time.
```

---
## \#4 Posted by: lunasicc Posted at: 2017-11-01T06:57:38.827Z Reads: 43

```
I honestly don't know what it draws, that's why I just gave hardware specs. no watt meter hooked up. 

@Cobber I'm fully aware man. I think you may have misunderstood. I was talking about running identical 55c battery's with each other, just comparing the power delivery compared to my 70's. I have 4 of the same battery's and even keep them isolated and only ran with each other.
```

---
## \#5 Posted by: Cobber Posted at: 2017-11-01T07:03:22.091Z Reads: 37

```
ah I see said the blind man

most cheap lipos are over rated
40c of a good lipo is plenty
most people seeing sag are using less than 20c

55c/110c even at 1p should be ample
what is the mah?

so we can calc. the C rating x Mah = ???
```

---
## \#6 Posted by: lunasicc Posted at: 2017-11-01T07:27:15.624Z Reads: 31

```
Lol! And ya that's kind of what I thought. 70c has to be overkill. So it would be a 5000mah 8s. Two 5000 4s in series. At 55c that would be 275amps?! Is that right? My esc is 160amp max. So basically I wouldnt notice one bit of difference? Even voltage sag wouldn't change anything I don't think
```

---
## \#7 Posted by: ShutterShock Posted at: 2017-11-01T07:28:12.532Z Reads: 30

```
Yeah I agree here, I have 25C on my street build and it sags just a little bit but I think I would use 40C at least for a mtb
```

---
## \#8 Posted by: ShutterShock Posted at: 2017-11-01T07:28:44.636Z Reads: 29

```
Yeah I doubt you would notice any difference.  I barely even pull like 50 battery amps at maximum acceleration
```

---

# Battery voltage issue

### Replies: 14 Views: 660

## \#1 Posted by: jga Posted at: 2017-06-28T09:41:53.872Z Reads: 75

```
I have an issue with my battery currently under construction.
As you can see on the photo, two series of 4 cells have been spot welded in parallel.
<img src="/uploads/db1493/original/3X/8/9/898af97f5ee707a5f5237a403b67b019e144f1a2.jpg" width="690" height="388">
Now when I put the multimeter on both side of one pack of cells, it only reads 3,4V
<img src="/uploads/db1493/original/3X/b/a/bac95b2994bd53b984823e520dfa6ec2347f02fb.jpg" width="690" height="388">
I have two nickel strips welded on the cells on each side. Same problem with other group of cells already done.
```

---
## \#2 Posted by: Maxid Posted at: 2017-06-28T09:58:01.277Z Reads: 73

```
You have 4 batteries connected in parallel in a 1S configuration - of course they will only show 3.4V.
It also looks like you have the second group of 4 in the same position as the first - if you connect them like this you will just add more cells in parallel
```

---
## \#3 Posted by: memesupreme Posted at: 2017-06-28T09:58:17.948Z Reads: 73

```
3.4 seems a bit low for even 1s, did you check the voltage of each cell before connecting them?
```

---
## \#4 Posted by: Maxid Posted at: 2017-06-28T09:58:53.890Z Reads: 72

```
What? 3.4 is perfectly fine for a Liion cell.
They are usually "empty" at 2.5V and their nominal voltage is 3.6V
```

---
## \#6 Posted by: memesupreme Posted at: 2017-06-28T10:11:45.274Z Reads: 65

```
yeah 3.6 sounds better, my voltmeter measured mine to be 3.6-3.7. so are you holding the black probe on the very negative and the red on the very positive? that's the only thing I can think of besides not pure nickle
*edit. nevermind someone put a diagram  aha
```

---
## \#7 Posted by: jrpwit Posted at: 2017-06-28T10:17:55.498Z Reads: 64

```
You're testing the voltage like this right? <img src="/uploads/db1493/original/3X/3/a/3a9ac107952edc56697d114bc90a66ca888411c4.png" width="690" height="460">

Oops voltage will appear negative cause probes backwards but just try this
```

---
## \#8 Posted by: SirDiff Posted at: 2017-06-28T10:39:14.405Z Reads: 63

```
Did you check all the cells before connecting them? They should all be at 3,4V
If you connect them in parallel, of course they will remain at 3,4 V
If you don't understand this, you should study a bit more before building your own battery pack, you could risk a lot. Batteries are dangerous.
```

---
## \#9 Posted by: Maxid Posted at: 2017-06-28T10:59:17.151Z Reads: 58

```
I have no idea what you are talking about. What has polarity to do with anything here?
So you measured yours at a different charge level to get 3.6V - now what does that have to do with anything?
When full you'll see them at 4.2V
```

---
## \#10 Posted by: memesupreme Posted at: 2017-06-28T11:51:11.624Z Reads: 53

```
you have 2 groups in series, if you put the black probe of your voltmeter on the negative end of one group and the red probe on the positive of that same group, youll get the voltage of that one group, not the entire series group. If you put the red probe on the positive end of the second group then your voltmeter will read about 6.8. If its still reading 3.4 then either you haven't connected them in series, or your nickle is not conducting
```

---
## \#11 Posted by: jga Posted at: 2017-06-28T11:56:04.777Z Reads: 49

```
Of course! What a joke! I must have been very tired last night...:grin: 
Thanks for the answer anyway. By the way the two groups are not connected together, they are just glued and will be connected with another group of four each as in the 10S4P modular battery configuration of @Eboosted The connections between each group are through XT60.
```

---
## \#12 Posted by: jga Posted at: 2017-06-28T11:58:13.648Z Reads: 46

```
No the two groups are not connected at all
```

---
## \#13 Posted by: memesupreme Posted at: 2017-06-28T11:59:40.849Z Reads: 49

```
ahhh, yeah once they're connected in series you'll get a higher voltage
```

---
## \#14 Posted by: Maxid Posted at: 2017-06-28T12:09:48.771Z Reads: 47

```
I am not the initial poster - not sure why you refer to me as the one that should measure anything :confused:
```

---
## \#15 Posted by: memesupreme Posted at: 2017-06-28T12:13:17.994Z Reads: 46

```
that's entirely my bad aha, i didn't read the names :sweat_smile: welp that's embarrassing
```

---

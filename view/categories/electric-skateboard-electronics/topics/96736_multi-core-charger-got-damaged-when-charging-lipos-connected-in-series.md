# Multi core charger got damaged when charging lipos connected in series

### Replies: 4 Views: 150

## \#1 Posted by: DavidC Posted at: 2019-06-16T16:32:25.709Z Reads: 35

```
![IMG_6730_K|666x500](upload://37S2B5BWI9T3t8lTXoZh4mC3KZ1.jpeg)

![IMG_6729|666x500](upload://mv9qVTvgiK9ShqSPwrLKZNwccQy.jpeg)
```

---
## \#2 Posted by: anders Posted at: 2019-06-17T06:56:08.453Z Reads: 22

```
These chargers have common ground for each channel, so if you connect in series it will short out. I have a 12s pack made up of 6x2s packs and I charge them as 2 6s packs split in the middle with an xt90 antispark. https://www.electric-skateboard.builders/t/remover-of-obstacles-first-build-rayne-amazon-sk3-6374-149kv-12s-graphene/86399/8?u=anders 
Got the idea from here https://www.electric-skateboard.builders/t/beautiful-diagrams-no-words-just-pics/3179/7?u=anders
Not sure how many cells each channel can charge on your charger? correct me if I'm wrong but it looks like your battery is 8s, if your charger have 6s/channel then you can split it in the middle with an xt90 for charging, but if you forget to disconnect the loop key you will fry the charger. Otherwise get a bms and monitor cell voltage actively.
```

---
## \#3 Posted by: DavidC Posted at: 2019-06-17T07:10:09.345Z Reads: 21

```
Thanks. I also fried a HobbyKing Safe 40A Parallel Charge Board first. 

![](https://cdn-global-hk.hobbyking.com/media/catalog/product/cache/1/image/660x415/17f82f742ffe127f42dca9de82fb58b1/legacy/catalog/36007.jpg)

In spite of the fuse the track on the PCB was burnt.
```

---
## \#4 Posted by: anders Posted at: 2019-06-17T07:20:01.353Z Reads: 19

```
At least no fires, be careful, never rush when charging, do lots of research, monitor cell voltage.
Your series connection soldering on your battery looks nice and tidy but can the cell move individually? if not something could break over time.
```

---

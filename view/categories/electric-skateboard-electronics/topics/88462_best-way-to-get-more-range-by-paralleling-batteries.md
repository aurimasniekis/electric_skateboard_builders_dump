# Best way to get more range by paralleling batteries?

### Replies: 6 Views: 258

## \#1 Posted by: skaterscooter Posted at: 2019-03-27T11:51:54.366Z Reads: 92

```
![21v%20_Ah|666x500](upload://beE1CG8sFlLOeRki7FXs9SfYKDq.png) ![21v%209Ah%20Diagram|666x500](upload://2w4evBHZSvaicRiYECYutGHvIof.png) ![21V%206Ah%20Diagram|666x500](upload://1KhO8QwHVnTi9YLgw7heWMuFFuw.png) 


I'm trying to expand my ebike battery (yes i know it's technically an esk8 forum but i thought someone could help) and basically want great range not more power. As my 3rd crude diagrams show, I have a 10s 2p pack at the moment to give me 42V and 6Ah. If I connect three batteries on each side to make it a 10s 3p, I would get 9Ah right?. However what would happen if I had 4 on one side and only two on the other? Would I get 6,9, 12 Ah? Any help appreciated

1st diagram is 4 on the top 2 on the bottom
2nd diagram is 3 on each side
3rd diagram is my current setup
```

---
## \#2 Posted by: venom121212 Posted at: 2019-03-27T11:58:59.420Z Reads: 88

```
Diagram 1 is a HUGE no no. You should always match your parallel groups (you currently have a 4p and 2p in series in diagram 1)

The problem is in charge and discharge. Your 2 series packs will drain to different levels, charge equally to different levels, and cause imbalances in your cells. This will most likely lead to a large fire shooting out of the 2p pack.

Parallel adds range

Series add voltage

Stay at 10s and get as many p groups as you can fit if range is your goal.
```

---
## \#3 Posted by: skaterscooter Posted at: 2019-03-27T12:11:47.236Z Reads: 78

```
Thanks for clearing that one up :)
```

---
## \#4 Posted by: venom121212 Posted at: 2019-03-27T12:16:21.418Z Reads: 71

```
No problem man. Glad to have you here. Stay awhile and check out the [pictures thread](https://www.electric-skateboard.builders/t/no-words-just-pictures-delete-words/2992?u=venom121212) if you dare. Careful, you will be instantly in love with esk8 and this wonderful community and need to build your own :wink:
```

---
## \#5 Posted by: Narnash Posted at: 2019-03-27T12:37:09.691Z Reads: 61

```
The safest and easiest way would be to build another 10S2P (or 1P if the cells can handle your load) and make them samewhat swapable. Because venom is right it's not worthwhile nor safe to use well used cells with added new cells in the same battery. 

As he said the resistance of the cells is drifting (a bit) by time and use, mixing them with new ones will lead to a unbalanced load on the older cells (since the heat "loss", voltage sag and power delivery are all effected by the resistance) till they can't handle that load whithout overheating leading to thermal runaway (thus fire or cell venting). The less fatal case would be extra strain on the older cells making them age faster till they die or can't hold up an enjoyable capacity anymore.

A easy to swap new battery would do the trick, a XT90-s plug or similar and some kind of latching mechanism or case where you but the battery and you are fine. But you have to disconnect the discharged battery when you swap in another one otherwise your full battery will try to charge the discharged one without any Amparege limitation (in case the battery itself has no BMS) which could kill (heat up) both oth them very quickly.
```

---
## \#6 Posted by: janpom Posted at: 2019-03-27T12:56:45.379Z Reads: 46

```
The diagram 1 would actually work as long as you don't overcharge/overdischarge, but it doesn't really make sense. You would start off with 6 Ah in your 2P pack and 12 Ah in your 4P pack. Both would discharge at roughly the same rate so after discharging 1 Ah you would have 5 Ah / 11 Ah remaining and after discharging 6 Ah you would have 0 Ah / 6 Ah remaining, i.e. your 2P pack would be completely empty while your 4P would still have ~6 Ah, which you however wouldn't be able to use.

The diagram 2 is what you want to aim for.
```

---

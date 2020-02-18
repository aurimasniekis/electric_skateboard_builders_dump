# Weird BMS balance port

### Replies: 12 Views: 299

## \#1 Posted by: ShakeNBake7000 Posted at: 2018-08-26T19:49:19.681Z Reads: 82

```
Hello, just got back to upgrading my board and got really confused with the BMS, let me explain:
I have two 6s batteries connected in series, and I bought a 6s 10A BMS for easier charging (charge only) but after soldering everything and trying to connect the balance cable to the BMS port, I couldn't get it in there, and then I noticed that it wasn't the "normal" 6s port, it was smaller. 

So my only way of connecting a balance cable to the BMS is connecting the one that came with the BMS, but that one has no connectors on the other side, and I don't want to start soldering tiny balance cables.
What are my options here? should I just get a different BMS with a full-size port? Is there any adaptor from the smaller 6s to the standard one?
I took some pictures to make it clearer:
![34|375x500](upload://aLVbUGqlATlJHEyZg9Vsr18KqxJ.jpeg)

![34%20(1)|375x500](upload://hgQFdaUWbbDcZPYL7MzWIlyLtq0.jpeg)

![34%20(2)|375x500](upload://yld48ZE7szzNKaWeVXagkrEY8sC.jpeg)

Hope you can help me
Thanks!
```

---
## \#2 Posted by: TowerCrisis Posted at: 2018-08-26T21:00:55.211Z Reads: 72

```
It's possible that they use the same pin size and socket, so it might be possible to just switch the white housing and keep the cable.

Try taking a pin out from each and compare. Careful though, it's live 😂
```

---
## \#3 Posted by: ShakeNBake7000 Posted at: 2018-08-27T14:11:47.015Z Reads: 49

```
Just checked, pin sizes are also smaller, so I can't swap them out manually
```

---
## \#4 Posted by: TowerCrisis Posted at: 2018-08-27T14:34:42.286Z Reads: 44

```
That's a shame. Sounds like a solder job then.
```

---
## \#5 Posted by: ShakeNBake7000 Posted at: 2018-08-27T16:44:21.044Z Reads: 31

```
Welp. 
Mabye I'll just get another BMS with a normal sized port, they're like 5$.
Thanks for trying
```

---
## \#6 Posted by: TinnieSinker Posted at: 2018-08-28T07:36:45.889Z Reads: 23

```
The larger one is JST XH and the smaller one is JST PH series
```

---
## \#7 Posted by: ShakeNBake7000 Posted at: 2018-08-28T09:24:39.364Z Reads: 20

```
[quote="TinnieSinker, post:6, topic:66158"]
JST PH
[/quote]

Oh, I tried looking up a balance cable with the PH one but couldn't find anything, any recommendations on where i should look?
```

---
## \#8 Posted by: TinnieSinker Posted at: 2018-08-28T09:29:18.223Z Reads: 22

```
something like this?

https://www.banggood.com/10Pcs-Mini-Micro-JST-2_0-PH-6Pin-Connector-Plug-With-30cm-Wires-Cables-p-1147297.html?rmmds=search&cur_warehouse=CN
```

---
## \#9 Posted by: ShakeNBake7000 Posted at: 2018-08-28T09:34:46.100Z Reads: 23

```
[quote="TinnieSinker, post:6, topic:66158"]
XH and the smaller one is JST PH series
[/quote]

Yeah, but with the other side as two 3s balance cables, like this one:
https://hobbyking.com/en_us/6s-battery-pack-balance-charge-adapter-lead.html
```

---
## \#10 Posted by: TinnieSinker Posted at: 2018-08-28T09:55:52.005Z Reads: 18

```
oh hmmmmmmm cant say i've seen much in that size.

buying another bms might be easier but if you want to make your own adapter, rs-online has all the connecters

https://au.rs-online.com/web/p/pcb-headers/8201431/
```

---
## \#11 Posted by: ShakeNBake7000 Posted at: 2018-08-28T10:18:15.048Z Reads: 16

```
Thanks for all the help, I'll probably get a bms.

Edit:
Do you think this bms has the XH port or the PH one? I can't really tell and its not specified in the specs.
https://www.ebay.com/itm/6S-22-2V-Li-ion-18650-Lithium-Battery-BMS-Charger-Protection-Board-with-Balance/202309446114?hash=item2f1a9529e2:g:4iEAAOSwWqNa8~mw
```

---
## \#12 Posted by: TinnieSinker Posted at: 2018-08-28T11:04:03.580Z Reads: 8

```
the little fin things on the top of the plug look like XH
```

---

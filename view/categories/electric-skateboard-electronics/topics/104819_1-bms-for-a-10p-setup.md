# 1 BMS For A 10P Setup

### Replies: 6 Views: 150

## \#1 Posted by: AK1 Posted at: 2019-12-19T01:34:24.741Z Reads: 46

```
I have been lurking in the forums for quite a while now. Recently I have begun purchasing all of the parts required for my mountainboard. I am stuck on making a decision for my BMS system and was wondering what you guys think.

The planned battery will be 10s10p using Samsung 30q cells. I will be using 10mmx.2mm nickel strips to wire the battery together(using 10 strips parallel to handle the amperage, and 10awg wire on the entire positive and negative side). I am also planning on using the BMS for charging/balancing only, and bypassing it for discharging. I understand the risk with this, however I am using a the dual vesc 6.6 and will monitor the voltage properly. (as a side note, if there are any problems with this setup let me know. I have heard that nickel strips are not the best with this many p groups, however I will be using 10 parallel strips to handle the current which should be within spec)

The question is, can I use a single BMS to manage this many cells without problems, or should I create two 10s5p packs which each have their own BMS in parallel and have them share the charging port. I am currently under the impression that 1 BMS which is bypassed will fulfill all my needs as I can charge at 8A max(though I will use 4A or 6A), and will balance the cells if given the time(I charge overnight so Ill have the time)

The BMS in question will be [this one](https://www.amazon.com/Akozon-Protection-Balance-Li-ion-Battery/dp/B07FX7DRXP/ref=sr_1_4?keywords=42v+BMS&qid=1576718747&sr=8-4)

TL;DR: do you guys recommend I use one or two BMS chips in a 10s10p BMS bypassed pack?
```

---
## \#2 Posted by: Tinp123 Posted at: 2019-12-19T06:55:38.493Z Reads: 39

```
Welcome! don't forget to join news forum too!

when you say using 10 strips parallel, I guess you mean 1 strip on top of each cell and they will connect two parallel groups? so those strips will make series connection, right? if that's the case, that is actually best solution, I'd say even better than silicone wires because your battery will be in top mounted box so there won't be any flex in there. 

you can setup cut off voltages in vesc settings, so there is no fear that you will ever over discharge your battery. 

you don't need two bms, you will make thing unnecessary complicated that way. use one bms on whole battery, but get some better bms than that from amazon. I can not say for certain it is bad bms, but it is not tested like bestech or Daly red aliexpress bms are. Daly for example is cheap (under 20$), but you will have to wait some time to arrive. 

which charging port you want to use?
```

---
## \#3 Posted by: webst Posted at: 2019-12-19T07:14:54.998Z Reads: 35

```
Cells balance themselves in parallel so just make sure voltages are equal when you put battery together. Bms acts on parallel groups connected inseries so there should be no problem with your setup, it might just take longer to balance eventually when batteries degrade.
```

---
## \#4 Posted by: AK1 Posted at: 2019-12-20T05:23:11.573Z Reads: 25

```
Im going to be using a female 2.1mmx5.5mm charger. I currently have a 2A charger that will fit this though it will take ~14 hours to go from 0% to 100%. For now it will do until I order a higher amp charger.
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-12-20T06:51:15.078Z Reads: 25

```
be aware that some 5.5x2.1mm ports are rated up to 3A and some up to 5A. If you want to go over 5A, consider going to different charging port.
```

---
## \#6 Posted by: mynamesmatt Posted at: 2019-12-25T20:28:11.642Z Reads: 19

```
I would not use 2x bms' instead of 2 like as said up there, it'll make things unnecessarily confusing.

I would however go for a BMS with a higher balance current. Your amazon BMS (for a eskate i don't understand why anyone would buy anything from amazon (except a unity)) only has a balance current of 56ma. Some bms have a balance curret up to 120ma which helps keeping your cells balanced that little bit easier.

Some i'd recommend would be the bestech d140, the bestech hcx-d223v1, the diebiems, or even any of the SuPower battery BMS'. They're also pretty good.

Hope this helps :)
```

---

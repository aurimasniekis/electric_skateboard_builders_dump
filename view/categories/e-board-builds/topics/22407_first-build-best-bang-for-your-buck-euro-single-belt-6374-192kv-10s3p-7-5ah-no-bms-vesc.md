# First Build &#124; Best Bang For Your Buck &#124; Euro &#124; Single Belt 6374-192kv &#124; 10S3P 7.5Ah &#124; No BMS &#124; VESC

### Replies: 3 Views: 1478

## \#1 Posted by: Jap Posted at: 2017-05-04T19:52:01.809Z Reads: 189

```
# Best Bang For Your Buck Build [Euro]

Hi all, I'm trying to get together my first electric skate build! I'm from Europe and trying to go for a cheapish but decent spec build :)

The general idea is single motor **SK3-6374-192kv**, powered by 18650 **10S Samsung's 25R 2500mAh** cells. All mounted on chinese hardware, similarly to [BEST VALUE](https://www.electric-skateboard.builders/t/best-value-under-650-murdered-out-vanguard-boosted-clone-deck-10s4p-jlabs-dual-6355-dual-vesc-black-90mm-carbon/18782) and [CHINESE BUILD](https://www.electric-skateboard.builders/t/chinese-build-10s3p-maytech-vesc-maytech-6374-190kv-mono-drive-boosted-board-deck-97mm-wheels-winning-remote/14040) builds from around here.

Let me know your thoughts about the parts, and help me with some questions down below please!

# Main Parts

  - **Boosted Board clone deck** - https://world.taobao.com/item/536855694383.htm?fromsite=main&spm=a312a.7700824.w4004-14838118875.2.l7tyh8
  - **Turnigy SK3 - 6374 - 192kv motor** - https://hobbyking.com/en_us/turnigy-aerodrive-sk3-6374-192kv-brushless-outrunner-motor.html
  - **Maytech VESC** - https://world.taobao.com/item/536720652464.htm?spm=a312a.7700714.0.0.skowvc#detail
  - **Trunks, Wheels (83mm), Motor mount, Drivetrain** - https://world.taobao.com/item/545683147963.htm?id=545683147963&scm=1007.12006.46753.i548257582108&pvid=776683d7-bb68-4c0f-9bb6-0c6e45ee77fc
  - **INR18650-25R batteries 10S3P** - https://www.nkon.nl/rechargeable/18650-size/samsung-18650-inr18650-25r.html



# Battery pack
Plan is to build the battery pack just like in the one in the image below. Since I have (two!) iMax B6 chargers, I'm thinking to instead make two balance plugs, from leads 1,2,3,4,5 for the first one, and 6,7,8,9,10 for the second one, so that I can charge the pack with the charger, and not require any BMS to run.
Any flaws with this approach? Am I correct to assume charging the first 5 packs from the series like that won't interfere with the rest of the cells?

![battery scheme](https://www.electric-skateboard.builders/uploads/db1493/original/2X/3/3d5bec9f703b91c87c83f215be6c2d2126d05195.png)


# Questions

So I think that covers the core of the build, if you need any clarifications let me know!
Btw I weigh ~72kgs, and spots I am planning to ride at don't have steep hills. So with those battery specs, I should be getting around 27km of range, and some quite good speeds, which is very nice :)

However I have some questions, which I hope you can help me out with!
1. TaoBao shipping to Europe via Superbuy : what are people's experience with shipping cost? I also assume I will have to pay import taxes when they arrive here. Also what kind of shipping time to expect?  Wonder if it would be cheaper to exclude the deck and try to find some used one locally, as If I understand there might be some issues with shipping the item of such a relatively big length.
2. If I were to get this [Battery Display](https://world.taobao.com/item/524929127650.htm?spm=a312a.7700714.0.0.idmlv8#detail) , what option should I pick for my batteries (**10S 3P cells**)? Is it 12 or 13 string lithium?
3. The [trunk/pulley/drivetrain combo I posted above](https://world.taobao.com/item/545683147963.htm?id=545683147963&scm=1007.12006.46753.i548257582108&pvid=776683d7-bb68-4c0f-9bb6-0c6e45ee77fc) :
a) Any guess on the width of those trunks? I don't have experience with longboards, but I've heard people recommend 180mm, so I would shoot for those.
b) Belt width? I'd like to have 15mm belt to have extra longevity on it, though I think it's either 12mm or 9mm in this kit. Do you think it would handle my setup alright? I would be fine with spending more on a better quality drivetrain, but not sure which one to get, and how to make sure it would fit the wheels or motor mount? (Also I'd need to get some extra belts in advance, where can I find those?)
c) Talking about motor mount, will the provided kit be able to accomodate the **SK3 6374** turnigy motor? And will the motor pulley fit on the 8mm motor shaft?
d) Another option for a drivetrain could be a 15mm kit from [BangGood](https://www.banggood.com/DIY-Electric-Skateboard-Kit-Parts-Pulleys-And-Motor-Mount-For-80MM-Wheels-p-1146629.html) for ~19 euros. However the specs mention **5065/5055** size motors, which I think is different size than the **SK3 6374** I am planning to get. Also the mount looks a bit thin, but it's hard to tell.
4. [Maytech VESC](https://world.taobao.com/item/536720652464.htm?spm=a312a.7700714.0.0.skowvc#detail) : I've read good things about it, what are your thoughts? Seems like a way better option than car ESCs, and paying ~150 euros for a non-chinese ESC seems a bit steep for this build, so I'm thinking of taking a chance at it. Will it be configurable with the same software as all other VESC's popular around here?
5. For the remote control I was thinking of going for this one from [BangGood](https://www.banggood.com/2_4GHz-Radio-Remote-Controller-Receiver-Transmitter-For-Electric-Skateboard-p-1125575.html?rmmds=mywishlist) (~18 Euros), small form factor and 2.4ghz for a stable connection.

So I think that's pretty much it! If you have any thoughts on the parts or the questions that I asked you are very welcome to share your opinion!
Also if you are from europe and have some spare parts that relate to the build for an OK price I'm open for suggestions :)

Thanks for looking!
```

---
## \#2 Posted by: Maxid Posted at: 2017-05-04T20:41:50.957Z Reads: 154

```
Don't use 25Rs but 30Q cells instead.
Maytech VESCs cheap out on the bootloader - you will not be able to update the firmware or will have to upload a bootloader yourself
```

---
## \#3 Posted by: Jap Posted at: 2017-05-04T21:13:48.836Z Reads: 151

```
Thanks for the tip about VESCs, I've got an st-linkv2 programmer laying around, I assume that's all the hardware I'd need to upload the bootloader?

Are you suggesting 30Q cells because of their increased capacity? I was considering HG2 from [Gear Best](http://www.gearbest.com/batteries/pp_242228.html) with the current sale going on, but I'm not sure on the import taxes that I'd have to pay and how much it would affect the price.
```

---

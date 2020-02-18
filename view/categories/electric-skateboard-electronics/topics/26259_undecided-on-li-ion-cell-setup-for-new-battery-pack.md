# Undecided on Li-ion Cell Setup For New Battery Pack

### Replies: 14 Views: 640

## \#1 Posted by: darkkevind Posted at: 2017-06-27T10:38:34.997Z Reads: 101

```
Can anyone help me decide please?

I'm not sure whether to make up a 6s or an 8s 4p pack for my board. I'm running a single 230kv 5065 SK3 with a VESC. I've been running 2 x 3s 5000mah 25c Li-pos in series for a while now and I was happy with speed and torque.

Why should I go with 8s over 6s? Reason for asking is that I'm finding it hard to find a reasonably priced 8s 60A BMS but 6s 60A BMS's are ten a penny!

Any help appreciated...
```

---
## \#2 Posted by: Martinsp Posted at: 2017-06-27T10:42:14.516Z Reads: 99

```
Generally speaking higher voltage at same power means lower amperage which means less heat. Speed and torque can be lowered to what you were used to with 6S pack in BLDC tool when using 8S.
```

---
## \#3 Posted by: darkkevind Posted at: 2017-06-27T10:46:33.543Z Reads: 93

```
Ok I get that, thanks. Although I'll be sticking with 60A motor max whichever battery pack I go for as that's my motor's actual maximum.
```

---
## \#4 Posted by: Martinsp Posted at: 2017-06-27T10:48:51.252Z Reads: 92

```
Im glad i could help :) Yeah most people use the 60A max and min for motor because it is a pretty safe number for most of the motors out there.
```

---
## \#5 Posted by: darkkevind Posted at: 2017-06-27T10:48:58.025Z Reads: 94

```
My li-ions are HG2's @ 20A so whatever pack I make will be an 80A pack, but the BMS will limit it to 60A output, if I go for 6s or 8s will that still have an effect on the heat generated like for like?
```

---
## \#6 Posted by: darkkevind Posted at: 2017-06-27T20:03:17.290Z Reads: 73

```
[quote="darkkevind, post:5, topic:26259, full:true"]
My li-ions are HG2's @ 20A so whatever pack I make will be an 80A pack, but the BMS will limit it to 60A output, if I go for 6s or 8s will that still have an effect on the heat generated like for like?
[/quote]

Does anyone have any feedback on this at all? @Martinsp  ?
```

---
## \#7 Posted by: Martinsp Posted at: 2017-06-28T07:23:27.327Z Reads: 51

```
Well if you are ok with using more cells for the 8S pack (8S4P to achieve the 80A you mentioned) It would generate less heat therefore you would be able to get away with smaller or even no heatsink.
The heat is related to the battery voltage (heat from the VESC not the batteries themselves) in a way that higher voltage means less heat... If you look at it from kind of mathematical point of view the power P equals voltage V multiplied by amperage I so the formula is P=V*I
What this means is that you will get the same power with 6S and 8S but the difference will be the amperage.. less amperage with 8S to achieve the same power 
More amperage through the VESC means more heat and you would not gain any difference in power when going 6S just more heat.
**If you use 60A on 6S that is maximum power of 1512W and a lot of heat**
**If you wanted to achieve the same power (1512W) on 8S you would only need 45A so result would be less heat with same power**
```

---
## \#8 Posted by: darkkevind Posted at: 2017-06-28T07:53:31.908Z Reads: 45

```
Great explanation! Thanks so much! I think I'll stick with 8s as I want the batteries to last as well as the VESC! :slight_smile:

I've just found and ordered a reasonably priced 8s BMS too
```

---
## \#9 Posted by: Martinsp Posted at: 2017-06-28T08:39:28.542Z Reads: 41

```
I am glad I could help you! I have my BMS from batterysupports.com and it has worked great for about half a year now.
```

---
## \#10 Posted by: Challlsss Posted at: 2017-06-28T13:17:51.055Z Reads: 32

```
Also you can always bypass the BMS to save monays $$$
```

---
## \#11 Posted by: Martinsp Posted at: 2017-06-28T14:27:20.843Z Reads: 30

```
I dont know if saving 38 USD on BMS is worth potentially destroying 100*USD battery :D  :D
```

---
## \#12 Posted by: Challlsss Posted at: 2017-06-28T14:38:40.727Z Reads: 30

```
it wont destroy the battery.
```

---
## \#13 Posted by: Martinsp Posted at: 2017-06-28T14:45:24.019Z Reads: 28

```
With lipos it might especially with the cheaper ones because the internal resistance of the batteries is different and the cheaper batteries are not matched meaning that in say a 3S pack the individual cells might not have the same internal resistance and therefore if you leave them without a BMD for longer period of time with eskates for example winter some of the cells will discharge faster then others.

**Keep in mind i am not talking about the BMS that most people including me use... those are pure s**t when in comes to balancing. Because the balancing current is not even 1mA** I use BMS only to cut off my battery at certain voltages. say one cell reaches 2.9V and others dont the BMS should disconnect the load, same goes for overcharge.
```

---
## \#14 Posted by: Martinsp Posted at: 2017-06-28T14:48:11.301Z Reads: 28

```
The voltage limits are managed by VESC i know but VESC only monitors the voltage of the whole pack and not individual cells so if for example an 18650 pack is vibrating on the bottom of your skateboard and one cell comes loose after a couple of months of stress and you dont notice it you will discharge the rest of the cells in that parallel bank faster because there will be one battery unconnected. And that is what i have BMS for... worst case scenarios.
```

---

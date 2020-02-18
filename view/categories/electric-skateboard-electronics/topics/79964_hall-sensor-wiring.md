# Hall sensor wiring

### Replies: 8 Views: 492

## \#1 Posted by: Shaz Posted at: 2019-01-05T09:02:37.814Z Reads: 78

```
I bought some 6368 motors from AliExpress and the hall sensor connectors dont match up to the connector PCB headings on my FSESC V4.12.

Does it matter which pinout the hall sensor wires get connected to as long as the VCC and Ground are correct?
```

---
## \#2 Posted by: Shaz Posted at: 2019-01-05T09:03:16.281Z Reads: 77

```
Pinout for motor hall sensor here:

![08|516x486](upload://idjPYSiWwstZxBk7KYBypSGDiuk.png)
```

---
## \#3 Posted by: hyperIon1 Posted at: 2019-01-05T09:04:33.093Z Reads: 76

```
Yes it matters. If you get it wrong you can fry a sensor
```

---
## \#4 Posted by: hyperIon1 Posted at: 2019-01-05T09:04:54.548Z Reads: 77

```
Let me look at my diagrams
```

---
## \#5 Posted by: hyperIon1 Posted at: 2019-01-05T09:10:01.084Z Reads: 71

```
Ok, the motor doesn’t have a temp sensor. So you will be a pin short. 
5v-5-v +
Temp- nothing 
H1-U
H2-V
H3-W
G-ground -
```

---
## \#6 Posted by: Shaz Posted at: 2019-01-05T09:18:24.876Z Reads: 66

```
thank @hyperIon1, just to confirm, the H1, H2, H3 relates the to below image?

![03|690x156](upload://7bbu3fwmB1FHujCR0F5pvokZ5c7.png)
```

---
## \#7 Posted by: hyperIon1 Posted at: 2019-01-05T09:26:51.150Z Reads: 64

```
Correct, as long as power is correct and you have hall sensor in sequence front or back it’s fine. There is no way to get hall sensor out of sequence because of number 3 and triangle configuration
```

---
## \#8 Posted by: Shaz Posted at: 2019-01-05T09:28:34.569Z Reads: 62

```
Awesome thank you! 
My first build is now on the home straight! :grinning:
```

---

# BMS Boards, Need some clarification

### Replies: 4 Views: 1048

## \#1 Posted by: g4tv4life Posted at: 2016-11-08T04:45:42.765Z Reads: 102

```
Hey everyone, I'm looking to use a 4s bms with balancing for a project, pretty much one of these
http://www.ebay.com/itm/4S-14-8V-Li-ion-Lithium-Cell-8A-18650-Battery-Protection-BMS-PCB-Board-w-Balance-/122078036751?hash=item1c6c6b030f:g:nDwAAOSwZVlXpWY4

But with every BMS I'm seeing, they overdischarge protection kicks in at around 2.7volts.
Even this one which I see around here alot kicks in at 2.9volts
http://www.batterysupports.com/36v-37v-42v-10s-60a-10x-36v-lithium-ion-lipolymer-battery-bms-p-267.html

Im using 18650 cells and I know going that low will kill them, but every bms I've found has the overdischarge set to
around 2.7volts. Am I missing something here? or do all these bms boards allow the cells to kill themselves.

Thanks everyone
```

---
## \#2 Posted by: Jinra Posted at: 2016-11-08T06:14:07.264Z Reads: 87

```
It's best to manage cell voltage by checking them yourself. Your BMS will let your cells go low so you dont get stranded when you still have power. 18650's are tested to go as low as 2.5v. You won't kill them going this low, you'll just drastically impact its cycle life.
```

---
## \#3 Posted by: treenutter Posted at: 2016-11-08T23:55:39.846Z Reads: 60

```
You can customize the LV threshold on VESC.
```

---
## \#4 Posted by: Namasaki Posted at: 2016-11-09T11:51:27.943Z Reads: 48

```
Bestech Bms's can be ordered with low voltage protection as high as 3.0v
They also sell Bms's with communication ability that can be connected to a computer and custom programed with software that is included with purchase.
http://bestechpower.com/products/

As Jinra mentioned, it is still best to monitor battery voltage.
At least with an inline volt meter for the total pack voltage. (with this option, you'll need to keep a safe margin during discharge)
```

---

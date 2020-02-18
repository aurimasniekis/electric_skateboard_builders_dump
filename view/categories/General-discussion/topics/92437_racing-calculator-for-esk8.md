# Racing Calculator for ESK8

### Replies: 1 Views: 199

## \#1 Posted by: professor_shartsis Posted at: 2019-05-01T13:42:24.400Z Reads: 63

```
I've made a couple of racing calculators which show "how fast you could go" on a given uphill slope and the gear ratio required to go that maximum possible speed.

The first version is a Mac/PC excel spreadsheet - you enter the 13 values on the top left and it tells you the max possible speed & necessary gear ratio on the top right:

https://files.secureserver.net/0fT5HhdTQhpC24

https://forum./uploads/default/optimized/2X/d/daf33cba802352e9f9581f5d01388274107a25ca_2_1380x644.jpeg

The second version is a Mac only numbers spreadsheet with charts - you fill in the numbers at the top and it makes the chart:

https://files.secureserver.net/0fhemIK29ta5TN

https://forum./uploads/default/optimized/2X/6/6ad8f5964d87eaa70159d0a2704eaaa60300533c_2_1060x1000.jpeg

Some early results:

Comparison of theoretical performance of some typical hub motors compared to gear reduction drive…

Geared: (2) 190kv, 0.05ohm motors w/ 42v &amp; 100mm tires

Hubs: (2) 73kv, 0.07ohm motors w/ 42v &amp; 84mm tires

https://forum./uploads/default/optimized/2X/9/97cd2cde4b2d17806940f8afdd09e5e2ade6af78_2_1054x998.gif

geared:

https://forum./uploads/default/optimized/2X/5/5aed27a7d2993033bd7487fbb1c4b79af78da299_2_1026x1000.jpeg

hubs:

https://forum./uploads/default/optimized/2X/e/e9f459ad44024822dc1b4393ff75c20c9d76a789_2_1050x1000.jpeg

Conclusions:

left chart shows “how fast you could go” in miles per hour after you choose a battery current limit and a slope (colored lines - 0% - 25% grades).

right chart shows what gear ratio you need to reach that max possible speed on that slope. since hubs don’t have gears, if the ratio for the chosen slope &amp; battery current limit (on the right chart) shows less than “1.00” you need bigger tires to go as fast as shown on the left chart— but putting bigger tires will reduce the efficiency in the same manner as lowering the gear ratio.

in other words in many situations the hubs could propel a rider faster with bigger tires, but the bigger tires would also make the board less efficient.

also there appears to be what I’d call a sort of “sweet spot” as far as gear ratio as long as the battery voltage is around 42v and using 2 motors…

setting the gear ratio such that the no load wheel speed is about 34mph (regardless of kv, tire size but having 42v and 2 motors) gives both maximum possible hill climbing speed up 25% slopes at 60a battery current limit per motor (~31-32mph), and maximum possible flatland speed with only 10a battery current limit (also about 32mph).

https://forum./uploads/default/optimized/2X/b/baaaf110e9988b1063889b36ad7af891961c61c2_2_1026x998.jpeg
```

---

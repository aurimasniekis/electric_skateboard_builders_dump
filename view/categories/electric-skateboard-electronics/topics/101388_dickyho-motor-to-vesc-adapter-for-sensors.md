# DickyHo motor to VESC adapter for sensors

### Replies: 11 Views: 307

## \#1 Posted by: esk8snith Posted at: 2019-09-05T16:27:36.889Z Reads: 101

```
I have purchased 2x 6374 170kV motors (https://www.ebay.com/itm/6354-6364-6374-6384-150-170-200-230-270KV-High-Efficiency-Brushless-motors/303074535503?hash=item4690a6684f:m:mUObW1iCo0TOBEwqaQQ1qXQ&var=602007163507) 

from @dickyho 
from previous purchases i know his motors sensor port is not a direct fit into the VESC port. Is there an adapter out there that will make it plug and play?

Thanks!
```

---
## \#2 Posted by: Grozniy Posted at: 2019-09-05T17:03:14.577Z Reads: 96

```
No idea but check with him what pin is it and maybe this works
https://s.click.aliexpress.com/e/3MEx5mUC
```

---
## \#3 Posted by: accrobrandon Posted at: 2019-09-05T20:50:41.646Z Reads: 80

```
https://flipsky.net/products/flipsky-esc-sensor-wires?gclid=Cj0KCQjw9ZDeBRD9ARIsAMbAmoZUggzQnmCZwXfK9oa6tzx3vmsdhGhFfxhzGVgw9Awl7QWmUcsxI9IaAvV5EALw_wcB
```

---
## \#4 Posted by: esk8snith Posted at: 2019-09-06T00:15:57.437Z Reads: 66

```
thanks. are you sure about this? Do you know if there is anywhere I can buy this from in the US?
```

---
## \#5 Posted by: accrobrandon Posted at: 2019-09-06T03:05:12.047Z Reads: 59

```
u could search the domestic sellers.... torque boards has em... sensor wires alone might cost a bit, but coupled with a purchase may make it more reasonable..... never found em on ebay....
```

---
## \#6 Posted by: esk8snith Posted at: 2019-09-06T03:16:00.379Z Reads: 56

```
okay thanks. are those adapters proven to work w dickyho motors? did you ever try it?
```

---
## \#7 Posted by: accrobrandon Posted at: 2019-09-06T03:27:20.370Z Reads: 55

```
no, but most motors are 6pin....ask him, he responds quickly.... but I have yet to find a motor (knock on wood) that didnt use these connectors... option B would be to run them sensorless unitll you get connectors... no biggie just give the board a light push like it wasnt electric and all runs smooth.
```

---
## \#8 Posted by: silverr1 Posted at: 2019-09-07T11:03:25.182Z Reads: 43

```
I had the same problem. Its not a 1.5mm 5 pin connector. Its closer to a 2mm 5 pin connector. I had Flipsky make a special one for me. It would connect but not keep a reliable connection. I ended up just cutting the ends and soldering the wires.

Here is pic of what flipsky made for me. 

![image|412x500](upload://4LV1WhQrntQlvEnojJYotgEYjJJ.png)
```

---
## \#9 Posted by: esk8snith Posted at: 2019-09-07T15:21:56.417Z Reads: 36

```
ahh thanks for sharing. i might have to end up doing that same thing. would you mind sending me the schematic for the the wire order that you used to connect to the VESC?

also which one of dickyHos motor did you use?
```

---
## \#10 Posted by: esk8snith Posted at: 2019-09-07T18:02:59.865Z Reads: 31

```
also here are pictures from his 6354 200kV motor, i’m assuming the 6374 170kV will have similar connectors.![image|375x500](upload://aZLJUG6O3xT3to5rWVZ65gk5Bbx.jpeg) ![image|375x500](upload://2bSy1FhXWjVdMXxvV9qVwFScLLk.jpeg) ![image|375x500](upload://yZt8Lqxq8xp8MIz5fofrvkfn1qP.jpeg) ![image|375x500](upload://jFhVd18Q3t2im5DE6nDaryqZSaf.jpeg) ![image|375x500](upload://xhSAZXuAUEfEUzmsE2Y6IwNxj9d.jpeg)
```

---
## \#11 Posted by: silverr1 Posted at: 2019-09-08T09:54:46.231Z Reads: 25

```
I've got the same motor as you. I did not use a schematic. Just match up the cables in the same order as they would be when using the connectors. They both won't use the same color. I started with the black wire on both and went in the same order as the pins. 

Here is an an example of the flipsky connector

![Screenshot%20from%202019-09-08%2005-48-48|591x330](upload://q9Dc4oN3B3s0vvdPHFZHDiaCevX.png) 

And this is the one from the motor

![Screenshot%20from%202019-09-08%2005-50-48|417x500](upload://kCTFPpykHGwANcO2mmJW0AMlKCP.png)
```

---

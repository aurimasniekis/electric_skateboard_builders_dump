# ESC Substitute(ebay) VS FVT120A

### Replies: 3 Views: 401

## \#1 Posted by: MonkeyFist Posted at: 2018-05-06T13:20:21.753Z Reads: 86

```
ESC Substitute(ebay) VS FVT120A

Rest of hypotetical setup:
Racerstar 280kv 6368
FVT120a/ESC Substitute
15/36 gearing
83mm wheels
6s Battery

Which will have more power/torque?
The Esc substitute is rated for max 35A vs the Car esc 120A.
Does this mean more power?
```

---
## \#2 Posted by: Quezacotl Posted at: 2018-05-06T14:16:48.890Z Reads: 73

```
35A controller gives 900W on 6S battery. On 10S it's 1500W.
And if it's a ESC substitute, make sure it is for brushless 3-phase motor(your racestar) and not just 2 lead DC.

But only in the end, it's just up to you what you want to try. If the substitute supports more than 6S, then it's better to use bigger battery.
```

---
## \#3 Posted by: Namasaki Posted at: 2018-05-06T17:10:10.293Z Reads: 44

```
 Hobby ESC's like to FVT and other similar ESC's  only run in duty cycle mode. 
This means that voltage to the motor increases and decreases with the amount of throttle applied. 
The amount of current will depend on the amount of mechanical resistance or Load applied to the motor. 
For example, during hard acceleration or when climbing hills. 
If your ESC is only rated for a max of 35a. And 6s voltage, you will be lacking power and you will likely have trouble with overheating and will probably wind up burning the ESC down. 
A 150a car ESC would be the minimum and even then you ar compromising brake quality. 

This is why the majority of diy'ers are using the Vesc. 
It delivers full voltage constantly and controls current proportional to the throttle with adjustable current limits. 
Delivering maximum power with minimum heat. 
And it offers adjustable brakes that are smooth and predictable.
```

---

# What&rsquo;s more efficient?

### Replies: 8 Views: 1177

## \#1 Posted by: SageTX Posted at: 2017-02-04T22:46:10.045Z Reads: 147

```
So I'm  wondering -  with the exact same batteries, I can set them up 8s or 12s is there an advantage to either? 
<img src="/uploads/db1493/original/3X/d/c/dcb60f5206bcd80b9086ed85610c9899f0d67469.png" width="690" height="406">
Setup - 
2xVesc  2x190kv6355  lipo 20c batteries.  
Identical setup on the same board  
Watt hours are the same for 12s or 8s. 
LIMITING THE SPEED to 22mph, what is the better way to go, and why?  
Considering - 
  Range 
  Battery heat 
  Motor heat 
  Vesc components
```

---
## \#2 Posted by: Alextech Posted at: 2017-02-04T23:00:33.626Z Reads: 135

```
Typically the Higher the Voltage the better, Keeps components cooler, Yet Despite this Esk8 in terms of being efficient is more a matter of Mechanical efficiently , The setup will essentially be the same, because in the end the same amount oh WH is being used no matter 8s or 12s, You wont see the benefits of 12s Speed so you might as well use a 8s to preserve cell life by lowering the amount of Amperage stress on individual batteries.
```

---
## \#3 Posted by: Ackmaniac Posted at: 2017-02-04T23:59:23.516Z Reads: 127

```
If you want to reach the same speed with both battery setups the 12S would be more efficient because could use a 33% lower gearing compared to the 8S. But i guess your gearing would be the same in both cases so you can reach a 50% higher top speed with the 12S. 

With the same gearing the 12S would be still a bit more efficient because of the lower amps and that means less heat losses but only between the battery and the VESC. I guess in real life you wont feel that difference.
```

---
## \#4 Posted by: Hummie Posted at: 2017-02-05T02:15:40.948Z Reads: 113

```
 given two identical hub motors except one wound to 50kv and the other 100kv, would there be a decrease in efficiency running the higher kv compared to the lower kv at slow speeds?  it seems like with pwm the motor can get any mix of amperage it needs and they would be similar, no?  i mean in the motor efficiency mainly but also the esc
```

---
## \#5 Posted by: saul Posted at: 2017-02-05T04:24:57.500Z Reads: 95

```
I have a 12s 5200mah and a 8s 10ah battery. I've used both with a single 190 6355 (among others).
Since you only want 22mph. I say 8s.

The real world efficiency gains are pretty small. with 8s its a bit simpler to wire and keep slim. and you can use an 8s balance charger.

Then, if you decide you want more speed one day. just swap in a 10 or 12s battery. No need to change anything else :sunglasses:

also is that range you calculated? seems a bit high
```

---
## \#6 Posted by: SageTX Posted at: 2017-02-05T06:53:30.814Z Reads: 85

```
Yes, it was range, but just estimated at 10wh/mi. Also I used max voltage, instead of nominal. But was really just looking at WattHours. 

Thanks peeps.  I was just seeing if I should  to rewire to 12s. 

Conclusion - not really necessary unless for top speed increase.  😎
```

---
## \#7 Posted by: Ackmaniac Posted at: 2017-02-05T12:04:42.884Z Reads: 69

```
It's 10 Wh a km. So it would be 16 Wh a mile. But that is really for a chilled cruise, but possible.
```

---
## \#8 Posted by: SageTX Posted at: 2017-02-06T22:06:56.444Z Reads: 52

```
[quote="Ackmaniac, post:7, topic:17217"]
It's 10 Wh a km.
[/quote]

thats what I meant :confounded: And that's what the spreadsheet cutout is calculated to.
```

---

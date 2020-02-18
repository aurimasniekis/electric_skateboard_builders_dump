# Why does the vesc run so poorly on 6s?

### Replies: 6 Views: 295

## \#1 Posted by: Dariks Posted at: 2018-07-26T02:41:06.385Z Reads: 144

```
Hi I'v been using a vesc x on 6s for a while and have noticed it runs significantly worst on 6s. Has anyone else seen this happen?
```

---
## \#2 Posted by: Colson003 Posted at: 2018-07-26T02:52:15.088Z Reads: 143

```
Because you have to pull a lot more amps causing it to heat up faster compared to higher voltages.

That’s just the simple answer.
```

---
## \#3 Posted by: lrdesigns Posted at: 2018-07-26T07:06:00.691Z Reads: 119

```
  6s 3.7*6=22.2 Volts x 45amps  =  1000w
12s 3.7*6=44.4 Volts x 22.5amps =1000w

Provided equal top speed with either different kv motors or gearing the 12s _"should"_ run less hot due to lower amps.
```

---
## \#4 Posted by: Maxid Posted at: 2018-07-26T07:54:32.816Z Reads: 96

```
Especially with P=I²*R you have 4 times the loss when using double the amps.
```

---
## \#5 Posted by: Bataleon Posted at: 2018-07-26T08:11:17.464Z Reads: 85

```
What are your motor KV and low voltage cut-off parameters looking like? A 140KV motor is never going to work as well on 6S as it is on 12S.

I don't think the performance difference you're seeing is strictly due to higher amps being pulled.
```

---
## \#6 Posted by: Dariks Posted at: 2018-07-28T23:19:59.590Z Reads: 42

```
After further inspection I'm actually noticing that I'm hitting the rmp limit on the vec this Chinese motor is mislabeled as 260kv its more like 360kv yeahh... Thanks For The Explanation.
```

---

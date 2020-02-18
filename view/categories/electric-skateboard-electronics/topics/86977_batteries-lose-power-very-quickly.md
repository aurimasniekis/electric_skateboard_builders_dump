# Batteries lose power very quickly?

### Replies: 4 Views: 158

## \#1 Posted by: skaterscooter Posted at: 2019-03-12T19:23:23.008Z Reads: 70

```
At the moment, I'm using 4 lipos to power my electric bike - 2 in series and 2 in parallel to give me 42V and 6Ah. Normally they give really punchy acceleration and good top speed with my vesc set to 65A max. Recently however, they are punchy as usual for about the first 2-3 minutes of riding but then acceleration slows down as well as the top speed. They still provide power but it's certainly not as fun to ride! I'm aware that this is probably a sign that there is something wrong with them but am unsure exactly what the issue is. I briefly did some analysis with the vesc tool and the voltage didn't drop too - 36v at 100% throttle. (this test wasn't particularly accurate as I was only riding for 3 minutes). Any thoughts on what the problem is and if there is any way to revive the batteries or whether it's gonna be a blow to my wallet!
```

---
## \#2 Posted by: Andy87 Posted at: 2019-03-12T19:28:59.122Z Reads: 68

```
If acceleration slowing down it can be the power restriction of your vesc.
Most likely when the vesc hit 80 degree.
As you mentioned in the other thread you don’t have over heat issues.

I would check the capacity of your packs with a Hobby charger, maybe also internal resistance if you can measure that. 
If both in normal values than the battery is not the issue.

Edit: check that all your power connections are plugged together and you don’t have any broken solder joins. That can cause a powering down as well.
```

---
## \#3 Posted by: skaterscooter Posted at: 2019-03-12T19:45:32.323Z Reads: 60

```
Ok thanks - I'll do some more tests and measurements when I can. Will post an update in a few weeks.
```

---
## \#4 Posted by: skaterscooter Posted at: 2019-03-15T21:49:19.649Z Reads: 30

```
Actually I think I might have solved it. After looking back at some of the recorded data, the VESC hits 80oC just as I begin to notice a loss i power. I've recently put it in an enclosure with little ventilation so I'll need to address that and hopefully won't need new batteries... 

Will update next weekend.
```

---

# How to charge 8000mah 3s lipo batteries

### Replies: 6 Views: 1043

## \#1 Posted by: luhulu Posted at: 2017-06-26T22:06:14.675Z Reads: 59

```
Hi,
I bought myself three 8000mah 3s lipo batteries from hobbyking and now i would
like to know how I can charge them?
Can I charge one battery at the time with the imax b6 charger? (https://hobbyking.com/en_us/imax-b6-50w-5a-charger-discharger-1-6-cells-genuine.html)
And if this works, what are the settings to charge one battery?
Thanks in advanced!
```

---
## \#2 Posted by: wafflejock Posted at: 2017-06-26T22:11:04.998Z Reads: 57

```
Yeah most of these chargers use the same interface just select lithium battery, plug in your balance leads (white connector cable) and the main power cable to the charger.  On the next screen when you hit okay you can change the chemistry type just make sure it says LiPo then hit okay, for amperage you can up the value some but depends on the W of the charger and V of the battery how high you can bump the amperage before it's  a problem up to 1C is usually deemed safe from what I've seen so 8A would be fine if your charger can handle it without overheating (typically they just restart if they overheat but might want to check the manual on that one, think you can do the charger wattage divided by the battery voltage to get the amperage you can push with the charger without it overheating, be a bit conservative).

Once you put in the amperage and chemistry type you hold the okay button and it will check the battery and show you it is a 3S hit okay again and it will start to charge.  While charging you can hit the arrow keys to get details on the individual cell charges.
```

---
## \#3 Posted by: luhulu Posted at: 2017-06-26T22:35:20.132Z Reads: 51

```
Thanks for the quick answer. But the charger can only charge with 5A, not 8A. Is it a problem or does it just take longer to charge? So the highest amperage is 5 on the charger and the battery has 8, right? So does it still work ? Or do I need a charger that charger up to 8A?
```

---
## \#4 Posted by: sl33py Posted at: 2017-06-26T22:38:45.454Z Reads: 52

```
Yes, you can charge individually.

You can also charge in parallel w/ a parallel board.  It's good to charge individually every once in a while and make sure all are working ok, but i frequently charge good packs in parallel.  

B6 will work fine, but you won't be able to charge 1c, since it maxes at 5A (1C would be 8A).  That's ok, i frequently charge at .5C to get better battery life anyway (when you aren't in a rush).  

Basically you should be able to charge full tilt 5A w/o issue.  Always inspect your packs for damage before charging.  If puffed or damaged - don't charge.  I think they also recommend waiting 15-30 min after use before charging, and another 15-30 min after charging before use.

Always balance charge!  and some cheap pyrex is a nice if you don't want to get charging bags.

GL!
```

---
## \#5 Posted by: wafflejock Posted at: 2017-06-26T22:40:05.737Z Reads: 43

```
Yeah no problem it just takes longer.  Basically you have 5Ah to fill up so if you go at 5A it would take 1 hour to fill that up (plus some time for balancing), typically even though it says 5A it's going to have a lower limit depending on the voltage of the batteries you're charging and wattage of the charger, with 3S it might be able to keep charging at 5A but it might overheat as well.  The one I have is slightly different but same LCD and controls and all so I assume yours also probably has the thermal cut off where it'll just switch itself off if it gets too hot and beep at you.  When it gets done charging it will beep as well but will show FULL on the screen, if it resets because of overheating you'll be back at the main menu, just let it cool off and start again (lower the amperage charge rate maybe or throw a fan on it).
```

---
## \#6 Posted by: luhulu Posted at: 2017-06-26T22:52:07.135Z Reads: 42

```
Thank you both for your helpful and quick answers! Thanks a lot!
```

---

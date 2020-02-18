# Using a 6s cell-meter on a 10s pack

### Replies: 3 Views: 460

## \#1 Posted by: mt37 Posted at: 2017-03-08T07:34:09.255Z Reads: 53

```
I'm building a 10s3p battery pack, with its own el-cheapo chinese BMS.

I don't fully trust the thing, so I'd like to monitor the cells myself with this cell meter [1].

Here is the kicker : that cell-meter doesn't support 10s. So I'd like to make two clusters of 5s to plug in the meter.

The question is : Do I need to physically separate my 10s pack into two 5s packs (break the serial connections) for this to work ?
Or can I just have the negative terminal on the cell reader be the 5th cell in series (positive of the 5th, or negative of the 6th), in order to get a reading on cells 6 through 10 ?


[1] https://www.amazon.com/Tenergy-Intelligent-Capacity-Discharger-Resistance/dp/B0178P8H9U
```

---
## \#2 Posted by: krloz Posted at: 2017-03-08T11:11:53.520Z Reads: 41

```
This IS exactly what i am planning on doing as soon as i upgrade my 6s to 10s. Two lipo alarms. One with its negative To the battery negative reading the first 5s and the second alarm with its negative to the 5-6 cell wire. A Two circuit switch to cut off both of those alarm negatives, turning both alarms off at the same time.
This should work as you can Connect the alarm anywhere on the balance cable, aslong as you respect polarity and It Will show the levels of only those connected cells. It would be as having Two independent 5s packs (at least for the alarms)

Be sure you dont Connect the alarms between them in Any way (IE. I am switching their negatives through 2 independent circuits(of the same switch)):)
```

---
## \#3 Posted by: mt37 Posted at: 2017-03-08T22:13:36.460Z Reads: 24

```
Thanks for confirming @krloz !

While I'm in there I may actually break the 10S into two 5S'es by adding an xt60 connector in the middle.
But it's great to know that I can still use the cell meter, or voltage alarms while that connection is active.

My goal ultimately is to use two cheap imax b6 hobby chargers instead of a BMS that does god knows what and has no readout. This is inspired by this video :

https://www.youtube.com/watch?v=pljSZcEwc8Q
```

---

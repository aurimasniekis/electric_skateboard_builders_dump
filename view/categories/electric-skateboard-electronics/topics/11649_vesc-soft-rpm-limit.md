# VESC - Soft RPM Limit

### Replies: 5 Views: 2492

## \#1 Posted by: yaca Posted at: 2016-10-21T22:44:19.171Z Reads: 306

```
Did anybody try to set the Soft RPM Limit at "App config" - "PPM"?
Is it right to set "Soft RPM Limit End" to the desired max ERPM for example 25000? Should it be the same number as in "Motor config" - "Motor" - "Max ERPM"?
And what do I have to set at "Soft RPM LIMIT Start"? Is 20000 a good number?
How does it feel compared to drive without Soft RPM Limit?

BTW I drive Dual Hub Motors with 10s Lipo.
Thank you for your answers!
```

---
## \#2 Posted by: chinzw Posted at: 2016-10-22T00:02:42.087Z Reads: 294

```
Im using Soft RPM limit in the PPM App. You set the limit end to your desired rpm you want to limit to, then you set the start to something lower, i have 10k start and 20k end. If the start and end are to close, you will feel and mainly hear the "pulsing" of the limiter (think car rev limiter).
It feels pretty much the same as using it without, just that you dont go as fast of course, but acceleration is the same.
I haven't played with Motor Max ERPM, so i cant tell you how it compares, but i believe motor max erpm is actually a cuttoff limit.
```

---
## \#3 Posted by: yaca Posted at: 2016-10-27T10:27:40.707Z Reads: 257

```
I wanted to limit the top speed of my first build because I have to get used on the speed and I don't trust the winning remote. At first I tried just to do it with "Max ERPM" at the Motor tab. But it behaves a bit strange when you reach full speed. Now I got it with "Soft RPM Limit" at PPM tab. At Start I have 20,000 and End is 25,000. That's on Jacob's Dual Hubs 28 km/h. Till 20,000 it accelerates stronger and then it accelerates slower before you reach full speed. I tried also with 15,000  - 25.000 but I wanted more acceleration, so 5,000 difference I like. "Max ERPM" at the Motor is now at 50,000. It's more then I can reach with a 10s battery. I think the maximum is about 33,000 ERPM.
```

---
## \#4 Posted by: sandrewvdv Posted at: 2016-10-27T10:53:00.262Z Reads: 233

```
I also am interested in knowing what the best way is to set a limit to your ERPM. Is setting the Soft RPM limit to 60000 enough to protect your hardware?
```

---
## \#5 Posted by: yaca Posted at: 2016-10-27T11:54:20.329Z Reads: 217

```
To protect your hardware set the "Max ERPM" in the **Motor Tab** to 60,000. The "Soft RPM Limit" - "End" in **PPM  tab** is just for to set your desired Top Speed and "Start" is for the Speed where the acceleration should start to be softer. You can see your MAX ERPM at "Realtime Data" - RPM"
```

---

# Found max current specs

### Replies: 4 Views: 353

## \#1 Posted by: Jmding Posted at: 2018-09-23T07:11:20.360Z Reads: 128

```
I found some good information on max motor currents for various SK3 motors. Apparently they are produced by SunRay, an OEM in China. Some guys on a RC forum dug this up. These numbers look a LOT more sensible than the ones provided by HobbyKing. For example, you’d think that a 200 Kv 6374 would be able to handle roughly twice the current as a 200 Kv 6354, given that the 6374’s stator is about twice the length of the one in the 6354. But Hobby King lists the SK3 6374 200 Kv at 80A, and most 6354 200 Kv motors are listed as 70A. But if you look at the table below for “60-size motors,” the 6374 200 Kv (listed as a 5035 195 Kv) is rated to 75A, while a 6354 260 Kv (listed as a 5020 225 Kv) is rated to 45A.

You have to convert the listed sizes to our typical naming convention, since the spec sheets refer to the motors by their stator dimensions, i.e. 6374 = 5035, 6354 = 5020, and 5045 is probably either 4020 or 4025.

Check out how max motor current is higher for motors that have higher Kv windings, confirming the idea that you always want to pick the highest Kv you can subject to erpm limits, and your ability to fit more extreme gear-ratios on your board.

Since max rated current is basically the only important spec when it comes torque, having reasonable ratings based on a actual tests is incredibly insightful.

![60-size%20motors%2C%20SunRay%20Technology%2C%202012-04-18|690x400](https://www.electric-skateboard.builders/uploads/db1493/original/3X/1/6/162c8a670a69a25f11b3d1e2382de4091087c8eb.jpeg)

![50-size%20motors%2C%20SunRay%20Technology|690x360](https://www.electric-skateboard.builders/uploads/db1493/original/3X/f/9/f93951d967575916a3556a2b28f2399d53f610d6.jpeg)
```

---
## \#2 Posted by: Pmac Posted at: 2018-09-24T06:11:44.530Z Reads: 70

```
That's some good info.

I have the SK3 6354 which as per your document is the 5020/26T

HK say it is 2360w and 70amp but the document says it is 1600w and 55amp.  I have run 70amp through the motor without an issue but it did get very very hot on hills where it would be pushing the max through (with my weight being 110kg).  and this clearly explains why.

I am going from a single drive to dual drive so running them at 55 amp max should mean they stay cooler and i still should have heaps of torque with 2 of them running.

Thanks for the info.
```

---
## \#3 Posted by: pat.speed Posted at: 2018-09-24T07:23:29.599Z Reads: 62

```
We should see if they would be willing to sell us some discounted ones if we got a gb going🙃
```

---
## \#4 Posted by: xilw3r Posted at: 2018-09-24T10:31:19.030Z Reads: 46

```
would be awesome, and we could get specifications we want for the shaft. Perhaps they would even do custom lamination thickness, or use other magnets/ bearings etc.

Only issue, I imagine that at the scale these guys are working, the minimum order quantity might be rather high, perhaps a few hundread units
```

---

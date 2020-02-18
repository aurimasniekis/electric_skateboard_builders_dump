# Help with Debugging the Vesc Failures

### Replies: 1 Views: 354

## \#1 Posted by: Ixf Posted at: 2017-12-31T17:15:59.724Z Reads: 41

```
Hey guys would love the communities help on debugging a problem I am having.
I just installed 2 new focboxes onto my built yesterday.  
Went out for a 5 minute test ride to a dunks, picked up coffee and the board first refused to start then started with only one motor.

The build is 12s4p running on BLDC hybrid with 6374 190KV.

Pictures of config:
<img src="/uploads/db1493/original/3X/b/7/b70c5a69dc3a2f9b1e200efa1f52adf46d617d76.png" width="690" height="331">

Following is what I had done to debug

>remove can bus + remote module so we have single vesc setup
>boot up shows only power LED no blinking redlights
>running motor detection returned Bad Detection Result
>swapped motor same results
>swapped phase wire same result
>removed sensor wire same results
>faults in terminal returned no faults
>motor spins up fine on other vesc
>Checked bullet connector to vesc connection as I had swapped out the connector, theres clear current
>DRV chip looks like it has a small bubble on it

<img src="/uploads/db1493/original/3X/5/b/5bcae0739c8a25c641a24b189e2bdd7704ce5efd.jpg" width="666" height="500">

Appreciate everyone's help on this.
This would be the third vesc that failed on me, I am at wits end on whats causing it. (could it be a bad motor??? evil spirits?????)
```

---

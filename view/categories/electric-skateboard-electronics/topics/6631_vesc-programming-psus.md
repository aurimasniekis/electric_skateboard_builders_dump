# VESC Programming PSU&rsquo;s

### Replies: 6 Views: 1094

## \#1 Posted by: dstnceswmer Posted at: 2016-07-26T15:18:26.373Z Reads: 96

```
Hi, just puchased a vesc from Ollin boards. Have seen a lot of posts warning about frying the vesc during programming due to wrong power supply being used. I have read that Ollin VESC's can just use batteries? also I have an old ATX PSU from a computer kicking around, would this be suitable? Or do I need to go out and buy a Bench supply(I'd rather not if I don't have to)?
```

---
## \#2 Posted by: Kaly Posted at: 2016-07-26T15:23:11.305Z Reads: 95

```
With that VESC you can plug into your battery an will be ok. @Chaka already set that up before leaving his shop.
```

---
## \#3 Posted by: Pablo_702 Posted at: 2016-07-26T17:57:55.987Z Reads: 77

```
@chaka 😍 
10 characters
```

---
## \#4 Posted by: dstnceswmer Posted at: 2016-07-27T14:19:53.531Z Reads: 58

```
So based on this video, https://www.youtube.com/watch?v=5HLZaMcYRuY, do I still follow all of these steps from the beginning (Firmware Update, motor detection) if I have an Ollin Boards VESC?
```

---
## \#5 Posted by: chaka Posted at: 2016-07-27T15:18:33.983Z Reads: 48

```
Here is Vedder's tutorial. You can run detection at your required system voltage for detection unless you are using a motor that is outside of the recommended kv range and size. Your VESC is loaded with v2.18 firmware so you will not need to update the firmware with the most current version of the bldc-tool.

https://youtu.be/17CSl1iXYE8?t=449
```

---
## \#6 Posted by: dstnceswmer Posted at: 2016-07-27T15:55:50.115Z Reads: 40

```
Cool, thanks! by "system voltage" are you referring to the battery voltage I'am using to drive my board? (just triple checking, it's ok to use my LiPO battery packs, I do not need a lab bench supply?)
```

---

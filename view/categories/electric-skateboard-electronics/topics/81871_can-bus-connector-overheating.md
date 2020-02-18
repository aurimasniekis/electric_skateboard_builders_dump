# Can bus connector overheating?

### Replies: 8 Views: 245

## \#1 Posted by: Noob-at-building Posted at: 2019-01-24T00:20:02.708Z Reads: 83

```
I recently solders all my parts together and got my board running with the help of @AdamE3399
But when I ride the board for more than a minute the vesc shuts off for safety because of the canbus connector overheating
Any one know how to shut the canbus connectors off in the vesc tool since I am ppm splitting
And I reconnected  the anti spark and it sparked just then
```

---
## \#2 Posted by: Noob-at-building Posted at: 2019-01-24T00:25:52.626Z Reads: 78

```
@JohnnyMeduse
Any ideas?
```

---
## \#3 Posted by: Noob-at-building Posted at: 2019-01-24T00:28:45.537Z Reads: 76

```
Is there any way to disable it?
```

---
## \#4 Posted by: JohnnyMeduse Posted at: 2019-01-24T00:28:54.439Z Reads: 76

```
Sound like an Issue with the tvs Diode... does one of the vesc as a dime blue light at the start?
```

---
## \#5 Posted by: Noob-at-building Posted at: 2019-01-24T00:31:17.044Z Reads: 73

```
I think it's fine cause we just removeds solder from the connector that was creating a short circuit but is there a way to disable the can bus on the vesc tool settings?
```

---
## \#6 Posted by: JohnnyMeduse Posted at: 2019-01-24T02:24:30.791Z Reads: 61

```
The chip is always activated I think, but you can try uncheck in "app configuration" "send status over can"
```

---
## \#7 Posted by: Noob-at-building Posted at: 2019-01-24T03:26:08.809Z Reads: 53

```
okay thanks ill try
```

---
## \#8 Posted by: Noob-at-building Posted at: 2019-01-24T10:38:18.210Z Reads: 40

```
Thanks you so much i disabled it in the app setting, general, Send Can status to false
![91|690x388](upload://cBUIZFjkmEwXlaHlpwZqYLKzNE.png)
```

---

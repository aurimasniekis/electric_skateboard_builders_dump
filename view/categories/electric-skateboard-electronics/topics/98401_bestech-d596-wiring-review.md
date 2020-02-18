# BesTech D596 wiring review

### Replies: 6 Views: 182

## \#1 Posted by: zenobios Posted at: 2019-07-13T21:41:28.191Z Reads: 34

```
Hi guys,

could you please take a quick look at my wiring diagram below and check if I made any mistakes? 

![ES8%20Board%20-%20Electric%20Setup-Page-2%20(1)|690x425](upload://nYNh1aG3xnSSs8VewmRbXYYrxHy.png) 

Here is the BesTech D596 datasheet for reference: https://www.litechpower.com/htmledit/uploadfiles//20190320041544395.pdf
```

---
## \#2 Posted by: MysticalDork Posted at: 2019-07-13T21:49:09.059Z Reads: 30

```
Looks OK to me. I'd add a physical switch to the negative wire between the BMS and the vescs (An XT90 loopkey), just as an extra layer of redundancy on top of the eswitch, just to have a physical way to disconnect stuff hsould the BMS decide not to turn off for whatever reason.
```

---
## \#3 Posted by: Tinp123 Posted at: 2019-07-13T21:53:10.873Z Reads: 28

```
D596 has 13 balance wires, first balance wire (B0) goes to battery main negative (in your diagram, bottom unused balance wire)
```

---
## \#4 Posted by: zenobios Posted at: 2019-07-13T22:01:27.719Z Reads: 29

```
Interesting! I updated the diagram. @Tinp123 but all other wiring stays the same?

@MysticalDork In this case I would also need to make the loop key accesible from outside the enclosure. Did you ever hear about problems with the e-switch? Or are you just some kind of overcautious :slight_smile:
```

---
## \#5 Posted by: Tinp123 Posted at: 2019-07-13T22:04:39.452Z Reads: 27

```
Everything else looks good!

I would not go with loop key, there is just no need for it. Okay, if you want to be extra safe. But no need for it.
```

---
## \#6 Posted by: MysticalDork Posted at: 2019-07-13T22:09:10.532Z Reads: 27

```
I've never heard of issues with that specific e-switch, but antispark switches in general have a reputation of frying after some use. I prefer to have a physical I-can-yank-this-if-everything-goes-to-shit option. It's like the battery disconnector loop that Teslas have so that emergency services people can disconnect the HV traction battery in the event of a crash/fire/accident.

If you're worried about waterproofing, you can always use some silicone sealant around and/or dielectric grease in the loopkey that will break away if you ever need to pull it.
```

---

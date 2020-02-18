# Hall sensor pin numbers

### Replies: 4 Views: 2029

## \#1 Posted by: Maxid Posted at: 2017-01-11T20:06:52.757Z Reads: 146

```
I have bought one of those 5065 140kv motors that look like the Evolve ones.
They come with a sensor cable with a 5pin plug.
My car ESC however has a 6pin plug and since it is a HK ESC I can't find a manual that would explain this.

Has anyone an idea as to what I need to do in order to connect the 5 wires to the ESC?

http://img.banggood.com/thumb/water/oaupload/banggood/images/37/DF/d047af1f-c351-4d91-b7b2-ec54fece8316.jpg
http://img.banggood.com/thumb/water/oaupload/banggood/images/E7/A8/5a2ad49f-53a5-47c9-8463-7f92db55003f.jpg
```

---
## \#2 Posted by: barajabali Posted at: 2017-01-12T05:20:43.316Z Reads: 130

```
The 6th is a temp sensor which some motors don't have. There is a thread by @Jinra that goes through how to connect the 5pin motor lead to the Vesc.
Search it
```

---
## \#3 Posted by: Maxid Posted at: 2017-01-12T07:34:23.690Z Reads: 122

```
So you mean this one?
http://www.electric-skateboard.builders/t/ollinboardco-om5065-200kv-sensored-motor/3409/397?u=maxid

Looks like it is just the same as this then:
<img src="/uploads/db1493/original/3X/6/4/6458c5e4626c3b62d40140ea7d40a061287884ce.jpg" width="690" height="414">
From https://endless-sphere.com/forums/viewtopic.php?f=30&t=9061&start=225#p327960

That means I'll need to find out polarity on my ESC and then just connect the +5V to the 6th instead of the 5th pin - should be doable.
```

---
## \#4 Posted by: Okami Posted at: 2017-01-12T07:37:39.225Z Reads: 116

```
@Maxid please post some feedback once you have tested them ;)

Yes, i think you will need to make some sort of adapter so one pin (the temp one) is left out.
```

---

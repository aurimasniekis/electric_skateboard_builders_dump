# Motor detection failure when my battery is at %100

### Replies: 3 Views: 400

## \#1 Posted by: Chris604 Posted at: 2016-10-13T15:13:23.615Z Reads: 48

```
Hey,  so my board started not detecting my motor when charged fully.  If I get it down to %95 it starts to work again.  I'm sure it's the settings in BLDC.  Does anybody have an idea what's going on? 

I have:
Pro 4 space cell 
Vesc updated 
190kv R-spec 
Gt2b Mod
```

---
## \#2 Posted by: Blasto Posted at: 2016-10-13T15:14:11.378Z Reads: 48

```
Did you change the max input voltage? Leave it at 57V
```

---
## \#3 Posted by: Chris604 Posted at: 2016-10-13T15:33:00.304Z Reads: 42

```
@Blasto I think that fixed it,  I wrote the default settings by accident the other day and messed it all up..  Thank you!
```

---

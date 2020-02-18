# How do I power aux electronics off the main battery?

### Replies: 3 Views: 148

## \#1 Posted by: ZachTetra Posted at: 2019-01-17T00:45:42.342Z Reads: 67

```
I'm making my board with neon underglow and 5 highbeams, both run off batteries but I want them to be tied into the main power, how do I run them?  The underglow is a 12V 1A LED strip powered through a controller and the highbeams are 4.5V 1A a piece flashlights, the main battery is a 12s4p lipo flat pack.
```

---
## \#2 Posted by: J_Dizzle Posted at: 2019-01-17T00:47:34.220Z Reads: 65

```
You will need a 12v step down converter, just search on ebay
```

---
## \#3 Posted by: MysticalDork Posted at: 2019-01-17T01:03:43.038Z Reads: 60

```
For the lights on my board I bought dedicated LED drivers from DigiKey or Mouser. They're small, very efficient, and can be controlled via PWM if you wish. 

If your lights have their own regulation circuitry, then you can get  DC-DC converters in just about any voltage and current rating from DigiKey or Mouser too, and they'll probably be smaller and more efficient than the Chinese ones that are all over eBay. (Not saying the eBay ones are useless, but if you're really trying for minimum space and maximum efficiently, there are some great ones at the big electronics suppliers.)
```

---

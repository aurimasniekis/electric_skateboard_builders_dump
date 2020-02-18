# eRPM max for my build

### Replies: 3 Views: 119

## \#1 Posted by: Aeorbis Posted at: 2019-08-28T22:19:06.128Z Reads: 54

```
Ok, so Im a bit confused here. I have read 190kv on 12s is fine and others that its a no go. However calculating max eRPM for my setup i get : Min 47,880 Max 67,032

My build is:
 12S6
TB 6374's
16T Motor
36T Pulley
97MM Wheels (Alternating between 107s)

Is this old news and no longer a problem? I found a post from Enertion claiming they tested the Unity to 130K eRPM. Also if it is a problem my understanding is that the Unity will set the eRPM limits automatically during calibration. Lastly, how does this effect top speed?
```

---
## \#2 Posted by: Saturn_Corp Posted at: 2019-08-29T00:54:38.931Z Reads: 45

```
eRPM scales with speed so you can limit it in the settings to cap off your top speed. If you're too lazy for math, here's a calculator https://codesandbox.io/s/vue-template-jikph?fontsize=14. 

Not sure what the Unity's eRPM limit is but I have heard it was safe up to 120,000 or so. Most older vescs were around 60,000. Thinking about that now It humors me to think wonder not just marketing material for 2x vescs on the same chip lol. IDK though. 67k on unity though I think is probably fine.
```

---
## \#3 Posted by: Andy87 Posted at: 2019-08-30T09:52:27.146Z Reads: 24

```
It’s only an issue with hw 4.12 based vescs
```

---

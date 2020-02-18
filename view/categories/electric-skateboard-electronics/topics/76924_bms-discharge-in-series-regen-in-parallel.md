# BMS discharge in series - Regen in parallel?

### Replies: 5 Views: 195

## \#1 Posted by: rlynd Posted at: 2018-12-03T17:17:55.896Z Reads: 60

```
I'm wanting to make a few modular 6S5P liion packs to power a couple different builds. For my longboard I'd like to run 2 packs in series (12s5p) but charge on-board in parallel (6S10P). I've got the wiring of this figured out with a way to isolate the charger port so I don't create a short but I'm not sure if I can configure a the VESC so that I can still use Regen in this configuration. So I have a couple questions for the experts here...

1. Can the VESC output and Regen at different voltages?
2. Can I just pump back a higher voltage to the BMS during Regen?
3. Do I need separate charge port on the BMS and use a stepdown to get to the proper 25v?
4. Anyone else doing this that has some tips/tricks?

The cells in using are 30Q and the BMS I'm considering is this one: http://www.bestechpower.com/222v6spcmbmspcbforli-ionli-polymerbatterypack/PCM-D345.html

Thanks in advance for your help!
```

---
## \#2 Posted by: longhairedboy Posted at: 2018-12-03T17:53:00.149Z Reads: 49

```
The VESC draws power and throws power back from regen through the same wires. I don't see how this is possible without some kind of intelligent switching circuit that likely doesn't exist.
```

---
## \#3 Posted by: linsus Posted at: 2018-12-03T18:11:41.851Z Reads: 43

```
[quote="rlynd, post:1, topic:76924"]
* Can the VESC output and Regen at different voltages?
* Can I just pump back a higher voltage to the BMS during Regen?
* Do I need separate charge port on the BMS and use a stepdown to get to the proper 25v?
* Anyone else doing this that has some tips/tricks?
[/quote]

You are over complicating things. Use XT connectors to wire them into go between parallell and serial "mode". Youll endup with 2 XT connectors and one charge port. And an on/off Button.
```

---
## \#4 Posted by: rlynd Posted at: 2018-12-03T21:28:41.061Z Reads: 29

```
Thanks that makes sense. Not sure why I was under the impression they were separate connections but that answers my question on separate charge port vs integrated on the BMS.

Maybe I'll just make life easier and get a 12s and 6s BMS to attach to the configurable battery based on application and gaurd each cell pack with a 80A fuse in case something shorts while mixing up the packs.

Was planning to use 2 Bestech BMS but has anyone used these? I like that they are already enclosed.
BMS 12S 60A: https://s.click.aliexpress.com/e/bncSXoRI
```

---
## \#5 Posted by: rlynd Posted at: 2018-12-03T22:35:58.676Z Reads: 22

```
I'll try and make a schematic tonight so it's more clear what my plan (now) is... Is it best to post that here? Or is there already a "Please check my wiring to help prevent fires" section that I should post in?
```

---

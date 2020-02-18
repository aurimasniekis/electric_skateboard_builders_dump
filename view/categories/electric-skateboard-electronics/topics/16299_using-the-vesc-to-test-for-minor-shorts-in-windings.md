# Using the vesc to test for minor shorts in windings

### Replies: 4 Views: 608

## \#1 Posted by: Hummie Posted at: 2017-01-19T00:37:56.153Z Reads: 68

```
I was riding with 3 motors on my board and just one of them powered.  The two unpowered got a bit warm from eddy currents just spinning around.  Not a surprise but one was 10f hotter than the other and it's either due to smeared laminations in the stator  and laminations losing their isolation and further spreading eddy currents or I have a minor short in the winding.  Is it possible to use the vesc's resistance tool to check INDIVIDUAL windings as apposed to the single number it gives which is an average for all three phases?
```

---
## \#2 Posted by: devin Posted at: 2017-01-19T02:27:31.411Z Reads: 60

```
<p>This post was flagged by the community and is temporarily hidden.</p>
```

---
## \#3 Posted by: PXSS Posted at: 2017-01-19T02:42:18.287Z Reads: 53

```
I would not do this. That is how you demagnetized your motors...

E: I know because I've demagnetized a few motors by mistake while testing regen brakes
```

---
## \#4 Posted by: Hummie Posted at: 2017-01-19T02:55:45.716Z Reads: 46

```
connecting the motor and vesc to the pc and running the ap isn't going to demagnetize magnets if that's what you're saying.   don't know what you mean but only way I know to demagnetize magnets is with a lot of heat beyond their curie temp or exposing them to an extreme magnetic field.


**if there's a slightly different magnetic field strength coming from the magnets it could produce a bit different eddy currents in the stator but I imagine it'd be a pretty insignificant difference.   the windings are not connected to anything, just wires, and any voltage built in them from passing magnets will not be expressed as a current....unless theres a short, and that's the possibility.  there should be no current in the windings otherwise.  if there were a minor short each passing of the magnets would produce a current..heat...and also  I think it would produce a back force to the magnets motion as well.  At least if i make a big short by connecting two phase wires there's a lot of resistance.  not sure on exactly what the resistance is in a short

it could be from scratching the rotor and connecting a bunch of lams and allowing greater eddy currents to flow.  i think it has to be this or the minor short in the windings but my multimeter won't do such small resistance and the vesc is super accurate..if only it could do the single windings and not average them either the resistance or inductance numbers would reveal
```

---

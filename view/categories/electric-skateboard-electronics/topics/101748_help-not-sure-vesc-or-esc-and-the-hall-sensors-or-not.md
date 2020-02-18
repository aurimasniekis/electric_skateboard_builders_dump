# Help! Not sure Vesc or esc, and the hall sensors or not

### Replies: 11 Views: 215

## \#1 Posted by: t.arrieta Posted at: 2019-09-13T22:06:02.382Z Reads: 51

```
Hi, i'm new here. I brought a Chinese electric skate, that for the moment goes good. I'm try to improve the skate, changing the motors, and brought two sk8 Turnigy of 130 kv to gain some  torque, and works really good ( a little bit abrupt at start and braking ), looking inside the connexions, it seems like have a dual vesc with sensors, but the problem is that doesn't fit the connectors. Somebody Can help me, and tell me if it's for sensor or not, and if that's it how can connect the hall sensors to the vescs?

Thanks so much for your help.![IMG_20190913_193859|666x500](upload://bdnh3Fbxjkaru56DL2585wFQyJv.jpeg) ![IMG_20190913_193831|374x500](upload://trUlyYjgnA66NHVV1aVXZQLDGiB.jpeg) ![IMG_20190913_194153|374x500](upload://6Db2R6KY4rl8fLzVGzI1swu26pv.jpeg) ![IMG_20190913_194111|374x500](upload://bdBnM0Hp3zPxnh1lQQx6dUMKV4W.jpeg) ![IMG_20190913_193949|666x500](upload://5lfMybrx0ZAyZFgWqIVDjq1DJMi.jpeg)![chrome|240x500](upload://jszjRmRdhxRRnVF1pMefa2aXMje.jpeg)
```

---
## \#2 Posted by: Santino Posted at: 2019-09-14T07:34:24.311Z Reads: 39

```
Hola amigo,

It looks like the hall does not have the temp sensor (5pins instead of 6pins). You could buy a jst conector for that module, and leave the temp sensor aside. You will run the motors with no temp readings, therefore you could program the vesc to shut down under determined temps. I use those motors, and set the cut of at 100C...Just in case try to put the esc brand and model, to help you in a certain way. Tambien hablo español, por si necesitas una mano.
```

---
## \#3 Posted by: t.arrieta Posted at: 2019-09-14T07:53:34.443Z Reads: 38

```
Buenos días Santino, muchas gracias por responder tan rápido!! He estado revisando por todos los lados las placas, pero no veo la marca o modelo por ningún  sitio... Sabrías decirme cuál de los dos conectores es el hall sensor? Y el otro conector, entiendo que sería para configurar el vesc? Son 4 en total, 2 por placa. Intentaré hablar con el vendedor chno para que le pregunte al fabricante qué modelo de vesc es el que lleva. En el caso de que no obtuviera esa info como se llaman esos tipos de conectores y dónde podría encontrarlos? ( Para buscarlos y comprarlos ) y que he de comprar para la configuración? ( Solamente un conector y salida USB para conectarlo al ordenador? 

Por cierto el vendedor es de Aliexpress y se llama Daibot Scooter Store'.

Muchas gracias de antemano Santino!!
```

---
## \#4 Posted by: Surfer Posted at: 2019-09-14T08:00:39.147Z Reads: 36

```
Eso no es un vesc....🤔
No es programable, probablemente no te funcione bien del todo, por qué no puedes ajustar el esc a tú nuevo motor. ( Motor detection in vesc tool)
Es importante el orden de los sensores que sea el mismo que el motor antiguo que tenías, ya que no puedes cambiarlo en el esc. Si tienes 6 cables, 2 son positivo y negativo, 3 los sensores, 
Y el sexto si tienes sensor de temperatura en el motor.
También es probable que pueda funcionar medianamente bien sin sensores, solo funcionan para arrancar, hasta 1000rpm más o menos, luego el esc ya no los tiene en cuenta.
```

---
## \#5 Posted by: t.arrieta Posted at: 2019-09-14T08:35:50.935Z Reads: 36

```
Buenos días surfer, los motores originales no llevaban sensor, cuando comprè los Turnigy los compre con sensor por si acaso en el futuro compraba un dual vesc. Pero al cambiar otra cosa Vi èstos dos conectores ( dos por placa ) y me entró la duda de si era o no, entrada para el sensor, y como soy novato en èsto no tenía muy claro si eran para ello o no. De ahí la consulta. Ójo! que sin los sensores la potencia de los motores es brutal, pero siempre se intenta mejorar.
```

---
## \#6 Posted by: Surfer Posted at: 2019-09-14T08:51:35.281Z Reads: 32

```
Ese tipo de esc es muy común en skate chinos, casi todas las marcas llevan ese modelo, imagino que será fácil encontrar información.
Yo creo que ese conector es la entrada para los sensores.
Seguimos en inglés
Get a set of vesc when you have the opportunity,   is really nice upgrade, no just power but smoothness
```

---
## \#7 Posted by: t.arrieta Posted at: 2019-09-14T13:39:19.008Z Reads: 27

```
Ok thxs so much for your help.
```

---
## \#8 Posted by: Santino Posted at: 2019-09-14T20:03:37.322Z Reads: 21

```
Agree with @Surfer , Chinese cheap esc...I just recommend you to buy 2 escs, good ones, compatible with Vesc6 hardware. I think that it is the most important investment on a eboard. I use Trampa Vesc. Expensive though, so Flipsky, Focbox, maybe the new Torqueboards escs, would be a great option too...Then you could upgrade everything that you want during time....Batteries, motors, boards....etc....
```

---
## \#9 Posted by: t.arrieta Posted at: 2019-09-15T01:08:04.690Z Reads: 16

```
Ok, I'll do it. So what it's recommend? Thanks so much Santino!
```

---
## \#10 Posted by: Santino Posted at: 2019-09-15T05:25:00.907Z Reads: 15

```
Just depends on how much money your are willing to spend...Top end Vesc6+ from Trampaboards; Mid to high end Focbox, Flipsky (there might be others but I do not know the reputation); low end esc with 4.2hw (which I do not recommend). If you do not live at the EU, you will save VAT from Trampa 20% off (I did that). The best thing to do is to read a lot and learn. You should also check up https://forum. , builders and vendors are there too. Saludos amigo...
```

---
## \#11 Posted by: t.arrieta Posted at: 2019-09-15T22:57:11.056Z Reads: 12

```
I read a lot but, my English level not the best. I understand that I need to buy two vesc or a dual one, the problem is that I'm live in EU and the tax are a lot of money, but I'm sure that sooner or later I must buy it the trampa ones or other one that I saw a little bit expensive. 
Thanks for your help!
```

---

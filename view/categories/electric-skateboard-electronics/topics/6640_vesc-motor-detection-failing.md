# Vesc motor detection failing

### Replies: 50 Views: 8097

## \#1 Posted by: ikjahaa Posted at: 2016-07-26T18:10:55.116Z Reads: 644

```
So,
I'm using a  VESC 4.12 (Enertion), 2ea Zippy 5000mah batteries in series and a SK3 245Kv motor.
I connected my vesc to the motor, vesc to the computer and finally i connected my vesc to the batteries.

I used the BLDC tool (v2.18 2.17) .

Whenever i do a motor detection my motor starts spinning, then stops and i hear a beep while the green led from the VESC blinks brighter (once, 1x short blink). The blue led stays on. After this i get an error "bad detection result received" and the motor detection says "Detection failed".
```

---
## \#2 Posted by: lox897 Posted at: 2016-07-26T20:08:31.726Z Reads: 619

```
@onloop may be able to help you. Have you tried to reflash the firmware?
```

---
## \#3 Posted by: ikjahaa Posted at: 2016-07-26T20:11:29.996Z Reads: 603

```
I do hope so, no I haven't.... the BLDC toold does get the right motor parms though (read configuration)
```

---
## \#4 Posted by: ikjahaa Posted at: 2016-07-26T20:23:51.819Z Reads: 594

```
So I flashed my firmware, now my vesc isn't copatible with the bldc tol anymore :confused: Weired since i used the firmware folder from the bldc tool dir
```

---
## \#5 Posted by: ikjahaa Posted at: 2016-07-26T20:25:24.802Z Reads: 569

```
I downloaded BLDC tool v2.15, it workes now, strange....
```

---
## \#6 Posted by: b-rad Posted at: 2016-07-26T21:08:30.706Z Reads: 557

```
Always also make sure that there is no load when doing a motor detection such as having no wheel or belt attached to the motor when you are doing a motor detection
```

---
## \#7 Posted by: lox897 Posted at: 2016-07-26T22:27:50.708Z Reads: 546

```
The motor detection works?
```

---
## \#8 Posted by: ikjahaa Posted at: 2016-07-26T22:44:06.228Z Reads: 536

```
Yea I think Vedder mentions this in his video.
```

---
## \#9 Posted by: ikjahaa Posted at: 2016-07-26T22:44:27.241Z Reads: 529

```
Yes luckily it does
```

---
## \#10 Posted by: lox897 Posted at: 2016-07-27T04:07:48.533Z Reads: 519

```
It seems that anyone having issues with motor detection has fixed it by reflashing the firmware.
```

---
## \#11 Posted by: Rick Posted at: 2016-08-03T23:40:54.033Z Reads: 508

```
Hi, I'm getting the same problem as you. I installed version 2.15 and its corresponding firmware and I'm still getting "detection failed" and everything happens like you said "my motor starts spinning, then stops and i hear a beep while the green led from the VESC blinks brighter (once, 1x short blink). The blue led stays on. After this i get an error "bad detection result received" and the motor detection says "Detection failed".

I also reflashed the fw when using bldc v 2.18 and still the same results.

I have the motor attached to the motor mount and to the truck but with no load on it.

I'm running the r-spec big motor (the one for mono-drive boards), the battery I connected the VESC to is a zippy flightmax 5000mah 25C 4s and these are my motor parameters before running detection.


<img src="/uploads/db1493/original/2X/4/46ba427e83fd85e444d18f0d5297a677532537f6.png" width="690" height="379">
```

---
## \#12 Posted by: sl33py Posted at: 2016-08-03T23:48:13.677Z Reads: 445

```
any time you are having issues - also try a different and shorter USB cable.  I recall Vedder mentioning this way back as a troubleshooting step.

worth a shot - GL!
```

---
## \#13 Posted by: hugohammarstrom Posted at: 2016-08-03T23:48:20.303Z Reads: 442

```
You might need to change the battery cutoff. This happened to me when doing motor detection and changing the cutoff fixed the "bad detection result received" error.
```

---
## \#14 Posted by: Rick Posted at: 2016-08-03T23:50:30.570Z Reads: 429

```
That fixed it!!! Thank you! :DD
```

---
## \#15 Posted by: Dunmer Posted at: 2016-09-06T07:04:46.695Z Reads: 405

```
This also worked for me! I used a 12v lead acid battery and my cutoff was on 33v and end was on 30v. I changed this to 10v and 8v and then it worked like a charm. Entered the right values after motor detection and then changed it back to 33v and 30v.
Thx a lot!
```

---
## \#16 Posted by: JamesNothing Posted at: 2016-09-25T17:15:03.201Z Reads: 346

```
I signed up to the forum after months on ninja reading only to thank you for this post that saved me from a HUGE headache!
```

---
## \#17 Posted by: yippie Posted at: 2017-07-18T10:39:46.328Z Reads: 232

```
+1
Changing battery cutoff solved "bad detection result received" error.
Thank you!
```

---
## \#18 Posted by: darkkevind Posted at: 2017-07-18T10:56:07.152Z Reads: 218

```
If none of these solutions work try upping the amps for the detection. Mine wasn't detecting at 6A but I upped it to 8A and it worked like a charm.
```

---
## \#19 Posted by: thetechtrader Posted at: 2017-07-29T14:26:12.017Z Reads: 202

```
Great post,  I just had same issue... motor detected before, then I changed some settings with volts and it would not detect... I reset to default, disocnnected, reconnected and it worked. Then I made my setting changes and saved.. hope this does the trick!
```

---
## \#21 Posted by: noble Posted at: 2017-12-05T01:16:49.185Z Reads: 158

```
Sorry guys,

but after extending these cables the engine stopped working. Is it because I have not sold them? Now i connect for fist time to bldc tool, update to 2.18 and try detection motor but dont move.

https://youtu.be/WKO3kuqBjgc

Im from spain. Sorry for my english

Thanks
```

---
## \#22 Posted by: Eboosted Posted at: 2017-12-05T01:31:26.193Z Reads: 143

```
Tienes que hacer motor detection otra vez.

Descarga el BLDC tool y conectalo a tu computadora, setea los límites de corriente nuevamente, y has motor detection en BLDC.
```

---
## \#23 Posted by: noble Posted at: 2017-12-05T01:34:18.930Z Reads: 138

```
Voy volando, gracias.
```

---
## \#24 Posted by: Eboosted Posted at: 2017-12-05T01:46:14.101Z Reads: 138

```
Esos cables no pueden estar así puenteados ni siquiera para probar, debes soldarlo y usar tubo termocontraible, si alguno llega a tocar vas a tener que comprar un VESC nuevo, estás poniendo en riesgo una pieza muy cara.
```

---
## \#25 Posted by: noble Posted at: 2017-12-05T01:49:09.683Z Reads: 138

```
Entiendo perfectamente, he ido con mucho cuidado. Tras cambiar los valores como el compañero sigue sin funcionar. Detection failed. He encargado un soldador en amazon. Funcianaba perfecto. Desconecte bateria, corte cables y ya no va. Sera por que no he soldado no?

Muchisimas gracias por tu interés, en serio, no tengo ningun amigo que entienda de esto. La vesc sigue funcionando.
```

---
## \#26 Posted by: noble Posted at: 2017-12-05T02:06:34.131Z Reads: 135

```
Te expongo la situación, muchas gracias.

https://youtu.be/tWzmUw_0OCs
```

---
## \#27 Posted by: Eboosted Posted at: 2017-12-05T02:24:59.373Z Reads: 126

```
Anda BLDC tool trata de hacer motor detection, inmediatamente luiego que te de "detection failed" anda a terminal y escribe "faults".

Uno nunca debe hacer funcional el motor si has cambiado los phase wires de posición, eso es lo que creo que has hecho, primero debiste hacer "motor detection".

Por último, postea un screenshot de cada una de las pantallas de BLDC tool, probablemente hayas seteado algo incorrectamente.

Actualiza la última versión del firmware correspondiente a tu hardware version, tu hardware parece ser un V4.12 pero no estoy seguro.

Mide el voltaje que llega de la batería al VESC y postealo
```

---
## \#28 Posted by: noble Posted at: 2017-12-05T02:31:46.428Z Reads: 123

```
Gracias.

Mi vesc es una 4.10. Ya he actualizado a 2.18. No se si los phase wires es la posición de los cables pero te aseguro que no he tocado nada. Solo cortar y empalmar. 

De hecho nunca lo habia conectado al ordenador hasta ahora.

Voy a ver si encuentro el terminal y hago lo que me has dicho.

Gracias de nuevo.
```

---
## \#29 Posted by: noble Posted at: 2017-12-05T02:40:01.003Z Reads: 121

```
Terminal me dice 'No faults registered since startup'
```

---
## \#30 Posted by: Eboosted Posted at: 2017-12-05T02:41:23.490Z Reads: 120

```
Definitivamente te has equivocado en la posición de los cables, es mas que seguro, cuando empezo a girar mal nunca debiste forzarlo, sino hacer motor detection.

Este es la pestaña de terminal:

<img src="/uploads/db1493/original/3X/2/0/2033de17407c934f8ac5cfd64ce0912146e09dde.png" width="690" height="337">

Antes de grabar tienes que hacer read configuration, pero si ya has escrito un nuevo firmware todos los valores se resetean a default, significa que debes configurar todas las opciones nuevamente:

- Motor configuration: motor y bldc
- App configuration: general y ppm
```

---
## \#31 Posted by: noble Posted at: 2017-12-05T02:52:55.639Z Reads: 110

```
Madre mía, gracias. 

https://imgur.com/3tYE5pG

https://imgur.com/Hajxkd4

https://imgur.com/DRqTGyM
```

---
## \#32 Posted by: Eboosted Posted at: 2017-12-05T03:00:26.441Z Reads: 111

```
Aquí debes seleccionar PPM, está en No app

[img]https://i.imgur.com/Hajxkd4.jpg[/img]

No veo nada en terminal, le pusiste "faults" luego de hacer motor detection?

Para configurar todas las opciones debes saber:

1. Qué batería tienes, cuántos amps puedes suministrar máximo
2. Qué motor tienes? cuántos KV y qué potencia máxima soporta?
```

---
## \#33 Posted by: noble Posted at: 2017-12-05T03:16:01.216Z Reads: 108

```
He hecho un video, ahora te lo adjunto.

Bateria: 5000 mAh lipo

Motor: 2000W

Skate: bolt, bolt motion

Que nervios, sino fuera por ti estaría colgado del techo.

https://youtu.be/h_L6fWNKLao

Te paso el realtime data

https://youtu.be/ExkTcacXhCs
```

---
## \#34 Posted by: Eboosted Posted at: 2017-12-05T04:13:57.470Z Reads: 103

```
Dejalo en PPM y UART

Batery cut off start significa que por debajo de ese voltaje no funcionará a full potencia, por ejemplp si tu bateria es una de 10S deberías tener ese valor en 30V (10*3=30v) y no en 10V (por ello nunca funcionará), el cuttoff end debería ser 28v. Si tu batería es un 6S el cutoff start debería ser 18V (6*3=18v), si es 8S (8*3=24v)

Debes saber qué S number tiene tu bateria, en caso no sepas debes medir su voltaje directamente usando un voltímetro
```

---
## \#35 Posted by: Eboosted Posted at: 2017-12-05T04:14:54.763Z Reads: 104

```
Usa este video para setear PPM

https://www.youtube.com/watch?v=OtuofrQr3F8
```

---
## \#36 Posted by: noble Posted at: 2017-12-05T04:28:45.673Z Reads: 102

```
He hecho todo, lo del mando correcto.

No sera que los cables no están soldados? No se la información de las baterías, y no tengo el medidor.

El cuttoff start es 33 y el end 30. Has visto el video del realdata time del comentario anterior?

Es tan raro. Gracias

Edito xq no me deja escribir mas replicas

He encontrado esto,

In Motor the fields should be 14, 14, 32, 72.
In Battery: Li-Ion, Voltage S: 6.
Now you can go in the Realtime tab and get instantaneous information or go to the Record tab and record your rides.

Si, lo he puesto en 18 y el end en 16 y nada.

https://youtu.be/QaP3iPmEgLc
```

---
## \#37 Posted by: Eboosted Posted at: 2017-12-05T04:30:53.542Z Reads: 97

```
Busca un voltímetro o saca la información de la batería,
```

---
## \#38 Posted by: Eboosted Posted at: 2017-12-05T04:34:26.728Z Reads: 98

```
Tu bateria esta en 25V segun el real time data, si está al 100% cargada entonces tienes una 6S, si está casi completamente descargada tienes un 8S, si tienes el cutoff start seteado en 30v nunca va a funcionar.

8S (cutoff start 24v)
6S (cutoff start 18v)
```

---
## \#39 Posted by: noble Posted at: 2017-12-05T21:49:07.179Z Reads: 101

```
Hi, i have the same problem. But when I spin the motor with my hand I see I have response from realtime data.

https://youtu.be/xu5f0Dp7DGY

https://youtu.be/gOq-kCeyo-I

Thanks to all
```

---
## \#40 Posted by: Blasto Posted at: 2017-12-05T22:15:56.710Z Reads: 96

```
this thread is actually very hard to follow.

from what i see, you may have 1 or 2 disconnected phases (inside the motor or somewhere)

quick test to figure that out, run a FOC R&L detection. that will give us the internal resistance of the windings, if the resistance is very high or induction very low... you have a motor problem

<img src="/uploads/db1493/original/3X/6/7/67bdb5df882dfaa59001eaa5cc0a3865d5d9b845.png" width="532" height="500">
```

---
## \#41 Posted by: noble Posted at: 2017-12-05T22:37:07.752Z Reads: 100

```
Thanks. This is the reult;

https://youtu.be/nj9P36_gm48

Thanks
```

---
## \#42 Posted by: Blasto Posted at: 2017-12-05T22:50:49.338Z Reads: 94

```
ok so your vesc disconnects when you run a detection. you probably have a blown mosfet, the fet creates a dead short on your input sagging your batteries to the point of disconnecting.

to confirm this you can check the continuity of the Drain-Source of each fet, should be high impedance (resistance)

now i understand why this thread is hard to follow, it's high jacked half in spanish lol
```

---
## \#43 Posted by: noble Posted at: 2017-12-05T23:05:20.783Z Reads: 97

```
Thanks Blasto

https://youtu.be/iRvYHSaYNiQ
```

---
## \#44 Posted by: Blasto Posted at: 2017-12-05T23:13:27.775Z Reads: 96

```
<img src="/uploads/db1493/original/3X/0/4/04b72fe3efa05f54e292373167ce11967e6d0fe1.png" width="400" height="296">

those solder joints look quite messy, maybe a high resolution picture of them, may have a short on the gate of a fet
```

---
## \#45 Posted by: noble Posted at: 2017-12-05T23:32:10.280Z Reads: 95

```
Thanks

https://youtu.be/pxWSczluCyI

https://youtu.be/hSnF9dSm8Fc
```

---
## \#46 Posted by: Eboosted Posted at: 2017-12-06T05:29:48.377Z Reads: 90

```
I'm sorry to say but your VESC needs to be replaced.
```

---
## \#47 Posted by: noble Posted at: 2017-12-06T17:51:54.457Z Reads: 89

```
Thanks! There some way to kmow if my motor die?
```

---
## \#48 Posted by: Eboosted Posted at: 2017-12-06T18:08:59.355Z Reads: 93

```
Do the procedure described by @blasto

You could also disconnect the motor, short two phase wires and try to turn the motor by hand, if it brakes then it's good
```

---
## \#49 Posted by: noble Posted at: 2017-12-06T18:27:25.700Z Reads: 90

```
Lorenzo from Bolt Motion send me setting

https://ibb.co/c6YCVG

Im going to try. If dont work I will send to Lorenzo to repair.

Thanks to all

Yes, when I put two cables together the motor slows down
```

---
## \#50 Posted by: noble Posted at: 2017-12-07T21:36:34.032Z Reads: 88

```
Lorenzo Cella from BoltMotion ( Bolt skateboard ) disappeared. It already seemed strange to me to attend. I give up, nobody in Spain is going to help me. Now I have a charger of about 800 euros. The worst business of m life hahaha
If someone knows someone in Spain who could change my VESC and configure it to tell me. Surely it is broken because never turn on any red light, or updating, or plugging, never, although everything else seems correct. I think it does not send energy to the engine. Anyway, I wanted to thank everyone who has tried to help me. Thank you
```

---
## \#51 Posted by: MarcB Posted at: 2018-07-22T16:49:14.321Z Reads: 53

```
Thanks man, had the same issue. I however will write the Cutoff back to what I think was the right values.

Start 36V (instead of 34 V)
End 35 V (instead of 31 V)

Do you see any issue there? I run a 10S 5Ah 20 C.

Thanks anyway already ! :slight_smile:
```

---

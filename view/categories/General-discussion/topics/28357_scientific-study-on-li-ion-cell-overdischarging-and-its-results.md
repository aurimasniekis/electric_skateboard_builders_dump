# Scientific study on Li-Ion cell overdischarging and it&rsquo;s results

### Replies: 2 Views: 581

## \#1 Posted by: SimosMCmuffin Posted at: 2017-07-23T08:25:16.470Z Reads: 86

```
Came across this video on my recommended feed on YT. I have watched a lot of bigclivedotcom's teardown videos and this particular topic interests me, as I'm building my own BMS module. I thought it would interest other people here also.

Interesting stuff starts at 1:10, but there is a lot of good stuff overall.
https://www.youtube.com/watch?v=sRwoYJyjZNo

Here's the link to the scientific study, which is also mentioned on the video. https://www.nature.com/articles/srep30248


**Watch the video first and check the research article and then continue below for discussion.**
----------
**Study abstract**
> Lithium-ion batteries connected in series are prone to be overdischarged. Overdischarge results in various side effects, such as capacity degradation and internal short circuit (ISCr). However, most of previous research on the overdischarge of a cell was terminated when the cell voltage dropped to 0 V, leaving the further impacts of overdischarge unclear. This paper investigates the entire overdischarge process of large-format lithium-ion batteries by discharging the cell to −100% state of charge (SOC). A significant voltage platform is observed at approximately −12% SOC, and ISCr is detected after the cell is overdischarged when passing the platform. The scanning electron microscopy (SEM) and X-ray diffraction (XRD) results indicate that the overdischarge-induced ISCr is caused by Cu deposition on electrodes, suggesting possible Cu collector dissolution at the voltage platform near −12% SOC. A prognostic/mechanistic model considering ISCr is used to evaluate the resistance of ISCr (RISCr), the value of which decreases sharply at the beginning of ISCr formation. Inducing the ISCr by overdischarge is effective and well controlled without any mechanical deformation or the use of a foreign substance.

_So TLDR, what are they testing?_
They are testing the effects of "extended" overdischarge, which none or very few other studies have done. In normal discharge cycle you're going from full 100% SoC (State-of-Charge) to empty 0% SoC. In the study they actually continue from 0% SoC to -100% SoC, and yes that's a minus. This can only happen on multi-cell series packs and they have shown their test setup in Figure 8.

https://images.nature.com/m685/nature-assets/srep/2016/160722/srep30248/images/srep30248-f8.jpg

So they have already discharged one cell by it's nominal capacity, in this case 25 Ah. It is put in a pack with other cells with charge still left in them. This means that even though that one cell might hit 0 Volts, the total pack voltage is still >12 Volts with 4 charged cells, so they can still pull current through the discharged cell, discharging it even further.



----------
**Weird curves (and maybe vibrations)**

0% SoC has terminal voltage of 2.75 V, so in normal use the cell voltage would stay between 4.20 V and 2.75 V
So what happens to the cell voltage when it's below 0% SoC? Well, pretty weird things. They have logged the cell voltage on figure 1, in different states of negative SoC.

> The overdischarge profile can be approximately divided into 3 stages according to the characteristics of the voltage variations. In Stage I (−11% < SOC ≤ 0%), the voltage dropped rapidly from 3.4 V to the minimum voltage of approximately −2.19 V, following a clear platform at approximately 1 V. In Stage II (−20% < SOC ≤ −11%), the voltage stopped declining and rebounded gradually with several fluctuations. In Stage III (−100% < SOC ≤ −20%), the voltage underwent a monotonic gradual increase asymptotically to 0 V without fluctuations.
https://images.nature.com/m685/nature-assets/srep/2016/160722/srep30248/images/srep30248-f1.jpg

So, if a cell is discharged after hitting 0 % SoC, it will quickly drop to significant negative terminal voltage and then rise up towards -0.3 V the further it is discharged



----------
**So what are the effects on the cell when it is overdischarged?**
The study found that the cells ISCr (internal short circuit resistance) started to significantly decrease, if the cell was discharged further then -12% SoC. Basically the cells would become damaged and if charged up again to 4.20 V, they would then self-discharge at much higher rates then healthy cells due to the decreased ISCr. This is due to copper dissolution and deposition, which happens after -12% SoC and forms internal short circuits in the cell. 

> The cells under overdischarge that were terminated in Stage I exhibited no discernible changes in properties, whereas in Stage III, the voltage increased slowly asymptotically to 0 V, suggesting the occurrence of severe ISCr.
https://images.nature.com/m685/nature-assets/srep/2016/160722/srep30248/images/srep30248-f2.jpg



----------
**What does this mean in practical setup?**
Well there are couple important finds in the study. First of which is, that even if a cell is discharged to 0 Volts it still falls in the Stage 1 at which:
> The cells under overdischarge that were terminated in Stage I exhibited no discernible changes in properties
<img src="/uploads/db1493/original/3X/1/5/15570eccd29f2fdb312e432ef97fc80188eb4d97.jpg" width="277" height="377">

So there shouldn't be any real damage to a cell even if it has been discharged to 0 V.

This also means that no damage should be done to the battery pack if the BMS cuts off the load at more sensible 2.5 Volts for example. and this is easy to detect.

**TLDR**
No damage if cell discharged to 0 Volts.
If a charged cell self-dicharges then it's bad.
```

---
## \#2 Posted by: Okami Posted at: 2017-07-24T21:57:52.390Z Reads: 29

```
Good stuff. I should go over this when i have anow bit more time about battery stuff again :)

Thanks for posting @SimosMCmuffin
```

---

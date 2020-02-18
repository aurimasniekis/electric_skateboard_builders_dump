# Active Balancers? New smart BMS? Ooooh

### Replies: 9 Views: 1888

## \#1 Posted by: deucesdown Posted at: 2019-04-27T04:28:39.721Z Reads: 167

```
Looks like a bunch of new stuff! I know aliexpress bms vendors sometimes list stuff that's not actually in production, to see if there's interest. But at least some of this stuff has sold through and has ratings. This particular vendor is one of the trusted ones at ES.

This first listing is 4s, but has graphs and shows the principle of operation. Looks like energy from high cells goes to low cells.

https://www.aliexpress.com/store/product/5A-8A-Active-Balancer-Equalizer-4S-Lipo-Lifepo4-Li-ion-Battery-BMS-High-Large-Blance-Current/2856009_32964854259.html

Dumb versions, I think has LED indicators.

https://www.aliexpress.com/store/product/Li-ion-Lipo-Lifepo4-LTO-Lithium-Battery-Active-Equalizer-Balancer-Energy-Transfer-Board-BMS-1-2A/2856009_32982883973.html

https://www.aliexpress.com/store/product/1-2A-Balance-Li-ion-Lipo-Lifepo4-LTO-Lithium-Battery-Active-Equalizer-Balancer-Energy-Transfer-Board/2856009_33002903687.html

https://www.aliexpress.com/store/product/3A-Li-ion-Lipo-Lifepo4-LTO-Battery-Active-Balance-Board-BMS-Balancer-Energy-Transfer-Equalizer-3S/2856009_32963936728.html

Smart ones, with bluetooth and ability to configure/monitor:

https://www.aliexpress.com/store/product/eBike-Bluetooth-Lithium-Battery-Active-Equalizer-1A-Balance-2S-24S-BMS-Li-ion-Lipo-Lifepo4-LTO/2856009_32945565819.html

https://www.aliexpress.com/store/product/2A-Active-Equalizer-High-Current-Bluetooth-Display-APP-2S-24S-BMS-Li-ion-Lipo-LTO-Lifepo4/2856009_32988078902.html

And a new smart bms? Looks bigger, HUGE current (300A only a few bucks more) versions listed. The series count seems all software configured, and has more balance current. No screenshot of app though, might be vaporware?

https://www.aliexpress.com/store/product/Smart-7S-20S-ANT-Lifepo4-li-ion-Lipo-LTO-Battery-Protection-Board-BMS-400A-300A-100A/2856009_32997552090.html

And this is interesting, looks like a big current drain-down balance board. @Hummie 

https://www.aliexpress.com/store/product/3S-16S-High-Current-Lithium-Battery-Balance-Board-60V-48V-1-5A-balancing-current-Active-Equalizer/2856009_32947962896.html
```

---
## \#2 Posted by: deucesdown Posted at: 2019-04-27T04:37:10.084Z Reads: 145

```
I'm looking at the 2A active balance board with bluetooth. I think it would work very well with ditching BMS, charging to 90% routinely, and once a month opening up the enclosure to check/balance the pack, and check inspect everything else.
```

---
## \#3 Posted by: Hummie Posted at: 2019-04-27T04:48:32.436Z Reads: 144

```
https://m.aliexpress.com/item/32863964045.html?trace=wwwdetail2mobilesitedetail&productId=32863964045&productSubject=2pcs-Chargery-BS12-Microprocessor-controlled-Monitor-Reader-Saver-Watcher-TFT-LCD-Display-2S-12S-Lipo-Li&gps-id=storeRecommendH5&scm=1007.18500.102169.0&scm_id=1007.18500.102169.0&scm-url=1007.18500.102169.0&pvid=7144d7a7-2bae-4e21-aaa8-52b0e2503459&_t=gps-id:storeRecommendH5,scm-url:1007.18500.102169.0,pvid:7144d7a7-2bae-4e21-aaa8-52b0e2503459&spm=a2g0n.detail-amp.store-card.32863964045&aff_trace_key=&aff_platform=msite&m_page_id=6794amp-EZou2dxKLxy-rE27dxTnOw1556340236773

25$ for an over voltage and under voltage alarm for each cell.  I like it 

How does the high power balancer work with those big inductors?
```

---
## \#4 Posted by: deucesdown Posted at: 2019-04-27T04:53:10.371Z Reads: 140

```
I believe SkaterBoy58 used these in his lacroix builds with external balance charger. I need 13s! (and 15s lifepo4)
```

---
## \#5 Posted by: deucesdown Posted at: 2019-05-02T00:31:19.347Z Reads: 99

```
So searching ES came up mostly dry, but youtube has some stuff on the active balancers

https://youtu.be/uDvS5alGH6w?t=209

https://www.youtube.com/watch?v=LIaYDqBu9Vk

https://www.youtube.com/watch?v=9aHrhjSn6rw

https://www.youtube.com/watch?v=DX4fVaY7K80

It can balance any series count 2s to 24s. Great for me because I have 10s, 12s, 13s, 15s, with maybe 11s coming.

It needs 40v to power itself (last contact on left is the VCC). If your pack has less than 40v like a partially depleted 10s pack, you can wire a dc dc boost inline with battery, or a power supply.

It works just as I thought, and is really perfect for those who have trouble trusting BMS. It looks like a fantastic diagnostic/maintenance tool all around.

I also found some more intensely priced stuff.

https://www.aliexpress.com/item/3S-to-9S-lithium-battery-balancer-which-keep-voltage-difference-within-10mV-the-best-solution-to/1950876697.html

Looks like 1s balancers that daisy chain. They sell boards that have many of these hooked up in series (4s, 8s, etc). $82 for the 4s one! 3A balance current. No bluetooth or display, but it looks like high quality stuff used in electric buses and the like. Too much for us IMO.

I'll probably pull the trigger on the 2A version. I have to find a robust multipin connector (JST XH is not rated for many cycles).
```

---
## \#6 Posted by: deucesdown Posted at: 2019-05-02T00:34:41.297Z Reads: 90

```
Links with more English description for the active balancers with bluetooth:

https://greatpow.com/product/bluetooth-balancer-battery-active-equalizer-for-large-capacity-series-lithium-battery-packs-management-system/

https://yiruikeji.en.alibaba.com/product/60813074849-810825950/12S_24S_1A_Lithium_Battery_Protection_Board_Active_Equalizer_Balancer_For_Li_ion_Lipo_LiFepo4_LTO_With_Bluetooth_APP.html
```

---
## \#7 Posted by: pakue Posted at: 2019-05-02T01:43:59.124Z Reads: 72

```
These active balancers are quite an interesting EE problem to design. Those things use a ton of switches to interconnect 2 cells via a DC-DC converter and need to actively compare each cell to select the right ones to balance.

Some academic research can be found on passive-active (for the lack of a better word) equalizer circuits that don't need a micro to match the cells. Here is one that is based on an isolated Cuk-converter: https://www.intechopen.com/books/energy-storage-technologies-and-applications/single-and-double-switch-cell-voltage-equalizers-for-series-connected-lithium-ion-cells-and-supercap

I haven't played around with these but it's definitely on my todo list.
```

---
## \#8 Posted by: visnu777 Posted at: 2019-05-05T16:11:15.599Z Reads: 55

```
Interesting, right now I'm balance charging with a 6s balance charger one half after the other because I couldn't find one for up to 12s...
```

---
## \#9 Posted by: deucesdown Posted at: 2019-05-05T16:18:19.759Z Reads: 50

```
Right so I think you can just bulk charge and the balancing portion will be very very fast without burning off excess as heat. With bluetooth monitoring.
```

---

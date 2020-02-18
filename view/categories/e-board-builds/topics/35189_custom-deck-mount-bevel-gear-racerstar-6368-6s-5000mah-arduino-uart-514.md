# Custom Deck / Mount &#124; Bevel Gear &#124; Racerstar 6368 &#124; 6S 5000mAh &#124; Arduino Uart &#124; 514$

### Replies: 14 Views: 1501

## \#1 Posted by: florr Posted at: 2017-10-09T18:04:20.836Z Reads: 253

```
In the last weeks, i've build my first electric longboard.
I didn't know, that there is such a huge community, so i've calculated and selected most parts by myself.
For example, i've used a bevel gear - just because they are really cheap.
I also chose a potentiometer, which seems to be uncommon (Can anybody tell my why? i don't see, why nunchucks are better..)
The controller-board communication is handled by an arduino over a nrf24l01
The Arduino runs a modified version of RollingGeckos Uart Controller.
I still need to 3D print a case for the controller, and for the gears (maybe with an oilpath - but mainly because i don't want to crush stones while driving )
Partlist:

[Racerstar 6368 280kv](https://www.banggood.com/de/Racerstar-6368-BRD6368-280KV-6-12S-Brushless-Motor-For-Balancing-Scooter-p-1117657.html?rmmds=myorder) 43€
[axis and 70mm wheels](https://www.amazon.de/RAM-UB-Truck-Longboard-Achsen-Griptape/dp/B01END2WRS/ref=s9u_simh_gw_i2?_encoding=UTF8&pd_rd_i=B01END2WRS&pd_rd_r=2G9BYN5NA6G7Z8ZF5T80&pd_rd_w=rHcuy&pd_rd_wg=e7qQu&pf_rd_m=A3JWKAKR8XB7XF&pf_rd_s=&pf_rd_r=G3HSKVEN0T8TNF52KMNC&pf_rd_t=36701&pf_rd_p=b9192609-35a1-4877-9094-5ab9bc159b27&pf_rd_i=desktop) 60€
vesc + antispark switch 180€
[lipo charger](https://www.aliexpress.com/item/Free-Shipping-Original-Skyrc-Imax-B6-Mini-60W-Professional-Balance-Charger-Discharger-Lipo-Charger-With/32273113863.html?spm=2114.01010208.3.10.uAUy9V&ws_ab_test=searchweb0_0,searchweb201602_5_10152_10065_10151_10068_10084_10083_10080_10082_10081_10177_10110_10136_5100019_10137_10111_10060_10138_10112_10113_10062_10156_10114_10056_10055_10054_10059_10099_10078_10079_10103_10073_10102_10096_10070_10148_10123_10147_10052_10053_10124_10142_10107_10050_10143_10051-10110,searchweb201603_4,afswitch_1,ppcSwitch_2&btsid=24916255-1883-43a0-b7fe-19b544e0b1aa&algo_expid=c034a074-c3a4-4897-94bb-e12e85cbe8df-1&algo_pvid=c034a074-c3a4-4897-94bb-e12e85cbe8df) 40€
[2*5000 mAh 3S Lipo](https://de.aliexpress.com/item/New-11-1V-5000mAh-50C-Max-55C-3S-3Cells-11-1-Volt-RC-LiPo-Li-Poly/632383559.html?spm=a2g0s.9042311.0.0.60DOLp) 60€
Electric parts (Arduino, xt60, switches, potentiometer , cables etc..) ~50€
[bevel gear 1:2.4](http://www.ebay.de/itm/262940636926) 5€
The Rest(wood, steel etc) i had already laying around.
**Total: 438€ (514$)**

As you may already noticed - my english isn't that good. But images are more informative anyway - so i'll show you my build process
(Feel free to ask questions)
<a href="https://photos.app.goo.gl/MIGwYXsnuXtesn2k1"><img src="https://lh3.googleusercontent.com/L9R3bj52D4DfNYtAlBjRAMrIc-I-53IT8-6xZQBaszOD9uu1KnplHB1879lQDkNTHGhxjbgD6fqlo4Fffr_tYNJwiZMge2sIQA2VZm2_SRUIqTBQupA9EtKLx43wtayF1MbOUO_6ruObEj6HFhicm2BUeA_vEQDg5FtHr1iO1VS7WJD09UaORRl8AQYJhtPetQMF4uwSmD0-hwmgLgVkEVnd3sc4NHaxMvDbGckImuI4nqotR2B0v01hGDNY8SZZlAbwId-JA3pcXjXX4SoX9H_3C2vOKPMKDczGYq1GI_fBHapwCdLNdwWLZCnlbfqi7-dbXjheg6SUqICnxCWmNAKMH5nKHyeSDGBPHwhWtUfzoNiH7kdFNJ7w1_uDL1BaNoVWQ7Ci3RB9qL2xfax9eXWmhQ_k8Octm3S7C-aCavsa6IslVJiLNG3wN-TRy3nT-no5TBum4ttM_RiU0wDEEBfQvnoqNBkUJxftbXD5sA1ilsUSn-juZSGmolub95ZQishUYb0Y7VypMxpf1bOtQYFjM8MUCyr-35msNdGKDtzcsK7CLR2cGB6drlF07zLbOvXvHVTq6u4OaQ55Xax1U72xWmyNOl9A99j-SbilpAdW79ADdJ_-bBCtH_4BatcfCYaqKTMouObX5t2zFx_vsjos7g7fG6okN6g=w731-h974-no" border="0"></a>
<a href="https://photos.app.goo.gl/AnXr9TcbZxl1jqmr1"><img src="https://lh3.googleusercontent.com/AZOJ5ha3krx5HU_v6FNAn1suSc2EyZVdVcaiBrgyfgRodb67U-UcqN5PUgD1ge9Bj8jVB4D6j6G66Y_u8Dgf5AidMVPsAxVfNd3-2oxAFl2mO90j3QuZeuY4GqOGiKxwcFsuD44M-aQFGwBkk5VNbW0yKdBa3siPk6Kh2eM64dVKkuWMC_Q5IskRlp-yykfozMNpBYbIrPxOnHhRRuKZOWV8pMZV5AyyTb8UtYR99lkZQMFE_YaZCyeiQFr03qBMyR5on3x63J6D-ZGy4TbRtQxPgd37jBgjzNhQzsiaIZHKCWYcE6rx8GASHKChF1hdj57JbSnTWIrcW_bfy0hghGCpgCh1zkgTC3iAEJ-ETPytaA-Xa57qr_ONVktb-RRiBqMAbjo986P-Ho07cDbk-aSSPmB6qpvN-KAH7YN86YQmnlQxsrzTEhDeM1dvHoPWhc-fTZuMXidrpIBdGrt6eidb3Vydmj3KeQQ_xSR8UZa9ilui6CQPqT_8ue6FN92BIyPHX3WRHkdAHWEwaM53588oSzHKmx19Ls2VbChGys4AvGNKvFa7ZEDnQsy9ozFYfl_EHPKpasKET55BDabPn4bq7_ipAD8_e_zN9LLNDg-5SGcUTko5OWIhfkeVBJA75VtEdCKad2GPSnl86J0s53a9CMoMnH45gLE=w731-h974-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/Oz4IfgNJJYBiYn4o1"><img src="https://lh3.googleusercontent.com/eeK43SduuLwFNgMEtTNHRoqslszLo0L94TYo0_90qjUeqViMOlvrz1mojZQrMnWhFbmeR4EA2oVbsJaUKz_EAH_6hOnYZniO3XGf_49kcEEbaVmcqOCvqn7Im1gudhS9ppchQ09qZ1Xr1rhMYfgs2P3u0gR6uHQJtcND3rWIXloUn82qk0eHrdvzekWyydT2qJSFdjJwrgqpUpvEb0lHBeIiTHJrPADQHoBeIkG-p39t91DR-SRsZAib2PfwloAfhthLJkb0P1lLOlgt8LF_VzJmqdLuG2EM2Y2VfaQu1gFI5_ffyEs8piyR1JDRUt_8KBKjksPMU4hlsADKNeZV_A-vAporOSl4J_1mBL_pOWlSyPc_6lK147gvjZnQck5Q0Hit66ZRndRc7Ane8U0iytGStEl8GTtIJDLLvSmQoKuYF7_5acaMUuMGZ3yMClt4-bjZnPPO1v_h_jnQPwlLYi8Z2gZFLDgB5mp4K8JDEbQcJZuZn_qRjle2H-7oAOi23lL7lxMoG0TCJ7XpVvxpd0j7hJvMdAml2OIKtV4HjKFz2WAdvNH5dxZB16hR9Bc8hzv0c0dcsFomt7qCz5TWahlvt1raobnMk13L5kcr9qr_0o-6GfBUE6iINVBGQKcFT9OOJYtQCXUvk3LgnzP79Sf_jzlIBqJgmVo=w1299-h974-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/u1VEKqTRVX6ZlJvD2"><img src="https://lh3.googleusercontent.com/71XHqR317D6v2zM8BARhmuvTnFZuSwT5E2dZlQNAJZ6F0cam3KGNye8DzcE-6_uBuDlXzvs0XG_FrmnhP6pAW0Rv_dEqpSw4VKS_DddP9fLz-HKip5g1_TtLgiu-8N8uFs3mww9ngJfJo_v8paW5O7B3rg4MGSteZ7VWwLYQQzy6kJk5sJmYB-tNeDb4t8rEfW4ad1wQj8b4gyJP_q0mPp_-4tYQGKup6pGkDdt_4QEa13zYAThvyR1ImMw_ZSBnoyLB8Cpp0PGX10xq2xI3LbsUzyYxN3ngQSSMyXeP638qZUG8LtqNhYfxESLud3RkaVjcmoSEmc6VR0QvJf9VL2kgD6MH4t2wVw444G-25rkJzUzSMGNpDP2p5jfWiuzA9n3ZTBlLFSC4DIuVlgj7j6_WcGNHxwGr_cq0ZkDahA_sQqxBemrmbgby7iWLHhh_IxXMc045kb4qgL61xsluzL1Etcu2c_1OWMwBz53cWgJeUuvSejufhn5sVZ30SXAAHjGH7efLmBvhElUHzHiy1p5IhPt0u0fCQIxy64QFPGnN-mD9l2M3jGqSLzQFlOuYtR-1brlvEcg6lTadlJ2veQZ3ZmKFewyBVosRD1zW3Sxk45Nj7W8h7keXYb-Da_rR_ZQbytEGdr17X64aXgG1YJSMj3Ce6eD0Akg=w731-h974-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/u1VEKqTRVX6ZlJvD2"><img src="https://lh3.googleusercontent.com/71XHqR317D6v2zM8BARhmuvTnFZuSwT5E2dZlQNAJZ6F0cam3KGNye8DzcE-6_uBuDlXzvs0XG_FrmnhP6pAW0Rv_dEqpSw4VKS_DddP9fLz-HKip5g1_TtLgiu-8N8uFs3mww9ngJfJo_v8paW5O7B3rg4MGSteZ7VWwLYQQzy6kJk5sJmYB-tNeDb4t8rEfW4ad1wQj8b4gyJP_q0mPp_-4tYQGKup6pGkDdt_4QEa13zYAThvyR1ImMw_ZSBnoyLB8Cpp0PGX10xq2xI3LbsUzyYxN3ngQSSMyXeP638qZUG8LtqNhYfxESLud3RkaVjcmoSEmc6VR0QvJf9VL2kgD6MH4t2wVw444G-25rkJzUzSMGNpDP2p5jfWiuzA9n3ZTBlLFSC4DIuVlgj7j6_WcGNHxwGr_cq0ZkDahA_sQqxBemrmbgby7iWLHhh_IxXMc045kb4qgL61xsluzL1Etcu2c_1OWMwBz53cWgJeUuvSejufhn5sVZ30SXAAHjGH7efLmBvhElUHzHiy1p5IhPt0u0fCQIxy64QFPGnN-mD9l2M3jGqSLzQFlOuYtR-1brlvEcg6lTadlJ2veQZ3ZmKFewyBVosRD1zW3Sxk45Nj7W8h7keXYb-Da_rR_ZQbytEGdr17X64aXgG1YJSMj3Ce6eD0Akg=w731-h974-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/ZNOpf4ELbK3ZM67F3"><img src="https://lh3.googleusercontent.com/gZMbC_bJK6xGsgMyJJunUJMgUPu15kyemVzvOd4y__tdDzk6nii1PXnme6EuW5pGT-S04zWqcib220N1iqVznEHTE85qN7WP6Mxnh0Fu6xoo1y57ZOl239nE3yoqgFV1__ePPHVOvK0BjDyJnhGCkxhgAs8YAQ4cyKuMV_ojrY5jHP-taIsdtdTDKfqELmKilTvmgmD4njeNuH5rRTrml0bjFams_X3juy3fI7JDb0cH8TKcLjqH1lRfMjgd93ktM1xaAYegUXNu0uXk8tKSheQyuSrlaHRYF5eeypKVnoizTJLcFG_SdqqwEhFcS8nyaj8sr0R-lBykzdJF0AvzYSHbr4cIvznyipHPWUfCoA5FhiOmmfqzOktk_impeYsAebPjXJgB4NCdyKGmdI5tKIM7GcRtaAMldgQ8mPSljueMyuCYyZMjAU8FqWZUqcbFSnWeg6fShdCABy6TThiFWlbKaoi9h47M_8_kBYhjHFOW24BVh2m4yLfUgHlzWeMmH03tPEOaGblKDTT_7Q2uY4vzTkrbGJqIie-2uUsuCxRppmrrqTb2PR3f6GWZCQnO67CAZDC63Gsvcw2exTN_1id9PjjdzE4mYztBif4hUrPYbCY0CEydyXjjgCF1fxYMHZ080I9B7V3Cx4gzbt82CCqF4jHPJyTS_ck=w1039-h779-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/rpSppLaIZLblCzZo2"><img src="https://lh3.googleusercontent.com/fic2MJdeszRup3d6Vfs1qFrpIOrB1_uAKvcEwY8vDy_z3H_lo_7JPEovwaL13RAaTOIS6OlxqDu320k_o4CPDDkVuJ0cV4B4C0KrdOpwMrcoKBBhz_pfCTIoORHyyPx5E2sVvr-xwhs_aiuBR9MMc3sDBTj8RBiTAHW5by3j3Ne1Pf79uEgxOZ9fipWXHfeipgcVFlsUaeSMPXGbPboHJFDmt0MkQlW4VvtLklUhrbIsKXABzgP_jt7jiN_0-2d4_m6Ti1ufMQJqcW8JoPTZwkdHscShAN2hZ5Z36cYF0XlZz1FdnjAin2DCyNw5l1qXGsp2uRupR3zXaQwOdIH7Ddg7pKpFptUO5ednbOIqImg1wM2YHWwrsjum6VxlmV4JJ88oyvuCUBcZhc3cIAU74rSGfw_TN6SkqjcupFo9BRY8iP_uC1nyg2K4eLr2T6y2UJXqiW0QkpiKn6I3vT-9nNvAk0NU1-sdZGfKE7TxJhgkkHVs6zq7UT2qXX3LFAZQ7tjmJJ_F9EOBnAhDV_vP-c5MU4VO7mcLW0CJbeLRGWTv2z5Xkxc5ZXA2daqTqav0O5s5NDCSXBMZEik9-U8D-gSo5mzA447tYDmGnmKiN_tsMsz8AaB76c4uWi3n7kIkuLanYO5MmRv3InH4dpFby7bH2pzDghkI0h8=w584-h779-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/1RYYV3NYbNPSj1D43"><img src="https://lh3.googleusercontent.com/lbEJYi_l2REE3FU_0O0kl6pkj1hOxdedw5NglBa_hZzPCXhJuiBneQrliUomcRmSg7Cab3YEzh0ZqzQSeMEiLShz77IdKSeCTiqg7X7eqbw3n_uil1lLA9S6-I3I8J9CW3i-mzeFuwH3RmYxHCAGcL0BTiZgs_iGAfqrM-7K1zdjepCZbk7_uOmY9G78LvQC37yFnU7qZqJOXNyR8bdra4Zz-G6gpkeOF7iKpzhJkg1obhix44UNbgAeumr7kBsVLy_NJOLJDOZWA_hxVo87lpTfAVcB88LZPjUmoCtrNIOzLefWYIfF8iRlJw5GbZAPDFT3_DmiZV17siSaPKMYHrKYkkaz1Pe4NufPJmJa7hD2EwnA28GdH6XwO4Sjbrfy8w7MqV3NTtHv-Yt1_4dFU_EaZyatglCO9jKul6NpHJuLKd3omuUcCqQeP5O6RGjUSAsOP48s7eT8CoGInojMnexe9eHorKP6l5TdeMjj3kFSQR-xKI4PdwydLNFFJF3jzLGYh35mOgArPjQmbR6PZrLon15MJ0BOx0elrxnPSun2w8nwZv5GO2hzcLFIgrWyDLjfSk_OZ3PsltLKyHWwxwfBTrp6N8y_um8dDIpcFxTNsgcce1gtmjx4XUDKzFoh59AWoJxNUWimCqxGU7FcPqcIAd0CSTIirNE=w1299-h974-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/n0KqQ2uQCIj16aXC3"><img src="https://lh3.googleusercontent.com/lkll4sTe7slC9vwQVfOV8Omenvg7WHnJI5r09BCNsw1Tn5pvPMB5zmimfJPYvZH4uQxY04GgXzH6oPVxYEPbYbk2v3kzxq0QwOHu9M02F06ZT3xehyTUkanQAwCXcPIajJz6_zWy4tBoAGJ_MKD9MLEFKKA_Dv5ZJD5WDKzWYA331HuHcTGiK1-42wO7a0_WDGwSfoYwc0-FrnO-XfUCsJotmTo5mKfTsra2TT3CyfzunYUzObVQIj259U4XtnTqQwy-YIh3Twr9EThxxxItmOEkxYfM1_t3vamuAFbQX_bb-w3NcsM-2TXFCnaj-6PtBJNkyONBHcq8C3ALEDXmGhOuQN_l_hmkolMBDXs6MAIuP8JazsEie4VZRSPiMc50vZlXlKhKD_ySdV49_1ARMJ85ElAag7mOd209kQVj98DSaS7a0icC2WVtyy8yTt_bx4sJ1YowEubsgsZ_ZpHnl7NhuzsgWX4mO0gGaxNWB9schN6SxxMANa15kb4J78FyW5-LkukqhsZNwcHjwBaBb8wAuCCDRX24ZS9tceLO9TPwrJ2rf56Y5980IkbQE-a19gkg0wAnKbUoEwxYASBcZWmr2p8k6KDBkDY_y0hDErjHNyKBJ6mPMcXdeFfICt_Cq6PCzZFr5FaLBAF35h2iBZPQAQb6DqD3qLQ=w584-h779-no" alt="IMG_20171006_180648" border="0"></a>
<a href="https://ibb.co/isJxVb"><img src="https://preview.ibb.co/cTDWqb/IMG_20171006_180648.jpg" alt="IMG_20171006_180648" border="0"></a>
<a href="https://photos.app.goo.gl/4JYTkkIn4eU7Ohcw2"><img src="https://lh3.googleusercontent.com/y_sDe5NOApcZp1YPBoWewShoeSyAsCKVljtGeDzHbeQAie5lO-mkR0SWtuXdk3TSNNFIcPakdeGoiLzmykAq4A6ISgef7sMHsYV9lxo-XZUZkNOwiXQXoaQ3xfnRX_SmNPpzT-iwAsuiTYpc9VzLOgGbhFeUF1k5Nsdmtn_p5bPvcdZ1hGdGjPJC4q8AdDN3CdS8d9PwRtK14Ifh53t8K6OxstMiUYXE2KRYG2ECGIdM8isJ3KYC7zKOEB9BjJmPD0ETX8tFPPogipcZEwNXaFIVUxwPL7GnsrwTcJ0MnlMjuFaH3mUaciht4xXMv6Uo6k4D6gIgRORcYHZ25s4_ETZg4TXF62jCDNwV2qL8zBdnTaS8t0IoE4CqQl_bvofxCEy_5Gef1Pt8gdEGvpepVfdb52qteC2F4BNq2EAzUNhAd0-NxzPtfqxyprvlLnjxF8JWN2dVJcaj03KOhvUaRKbBBe5E-By7sSSxl5EB4x7VTFzy3TMc6FcKQFjypslwcuBb48OhfWU2xjUtZjwTT4QtCfi2yZghcmMJurdsaRAGYTj7DE1Zpfd7sB2Xy8VFsqmnpE6vO_il7L4K7w4dqalU9KptPwvfW2YPrsxzVP4b2CeyKeyfNmwQE90m5sN44TNew4L9P0LPL2uKOYCJKWAu33PWxQZZpLI=w1299-h974-no" border="0"></a>
[Google Gallery](https://photos.app.goo.gl/jEzj6aZdxqA3cyso1)


I don't know yet, how fast and far it can go, because I don't want to ride that far before i've closed up the gears..

PS. As you may noticed - there is space for a second motor ;)
```

---
## \#2 Posted by: JohnA Posted at: 2017-10-09T18:17:14.134Z Reads: 230

```
Sweet build! @GrecoMan seems to be heading down the same direction.
```

---
## \#3 Posted by: GrecoMan Posted at: 2017-10-09T19:14:04.731Z Reads: 221

```
we have already chatted through pm about his failures and suggestions :wink:

Ive got something huge in the works right now
```

---
## \#4 Posted by: Okami Posted at: 2017-10-09T22:57:14.424Z Reads: 191

```
Cool approach. I think this is first build where.i see.something like this, if u paint the mount (and it is sturdy enough as of.now, it might look way more refined :) 

though as i understand this is just first prototype as u are planning to seal the gears too
```

---
## \#5 Posted by: florr Posted at: 2017-10-10T07:05:22.176Z Reads: 166

```
[quote="Okami, post:4, topic:35189"]
if u paint the mount
[/quote]

Even if i like the "prototype-look" i will paint it for sure to prevent it from getting rusty.
I also have to cut some edges...
I've mainly used 6mm thick steel, so it should be sturdy enough. The weakestParts are the four two 
threaded bars ..
```

---
## \#6 Posted by: pat.speed Posted at: 2017-10-10T07:53:00.335Z Reads: 153

```
Sweet build, what gear ratio are you running?
```

---
## \#7 Posted by: florr Posted at: 2017-10-10T08:04:54.144Z Reads: 152

```
Whops, I've forgotten to mention that. I've used 1:2.44 even if i've wanted something between 3-4 (but they're about 5 times  more expensive)
What i like about this build is, that it's relatively easy to replace the gears or the wheels :D
```

---
## \#8 Posted by: pat.speed Posted at: 2017-10-10T08:05:54.930Z Reads: 148

```
Yes it would be and that is pretty much the perfect gearing for esk8. Any higher and you will lose lots of top speed
```

---
## \#9 Posted by: philip91 Posted at: 2017-10-27T16:05:05.336Z Reads: 117

```
So I just ordered the same motor, what are your thoughts after using it? Does it Overheat? And what is your top speed?
```

---
## \#10 Posted by: florr Posted at: 2017-11-02T22:24:54.297Z Reads: 112

```
Sry for the late reply.

Sadly my board broke after about 4km (i'm fixing that soon) - so i don't know much about the motor.
Within that range, i haven't had any overheating issues.
My top speed was about 25km/h
```

---
## \#11 Posted by: GrecoMan Posted at: 2017-11-02T22:30:02.032Z Reads: 110

```
what exactly broke?
```

---
## \#12 Posted by: florr Posted at: 2017-11-02T22:35:04.395Z Reads: 113

```
It was totally my fault. I should have used glue or more/bigger screws.
<a href="https://ibb.co/cJBpLw"><img src="https://preview.ibb.co/kPHULw/Whats_App_Image_2017_10_17_at_18_10_35.jpg" alt="Whats_App_Image_2017_10_17_at_18_10_35" border="0"></a>

PS. It broke because i've tried to pass a curb
```

---
## \#13 Posted by: Bor.inc Posted at: 2017-12-14T21:58:18.737Z Reads: 83

```
How do you like the motor? I have ordered one, is it a good motor?
```

---
## \#14 Posted by: Okami Posted at: 2017-12-14T22:08:27.784Z Reads: 81

```
Cool thing someone recovered this thread.. was already wondering where this unique motor mounting style was used
```

---

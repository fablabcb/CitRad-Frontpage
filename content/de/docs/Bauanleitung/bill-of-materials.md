---
title: Teileliste
description: >
  Welche Teile brauchst du für den Bau der CitRad Sensoreinheit? Wo bekommst du diese und wo ergibt es Sinn, Teile gemeinschaftlich zu bestellen?
date: 2024-01-09
weight: 2
---



## nötiges Werkzeug

- Lötkolben + Lötzinn
- Schraubenzieher
- Seitenschneider
- Abisolierzange
- Messer
- Spitzzange
- Heißluftpistole/Feuerzeug


## Bauteile

- Elektronik
  - [Teensy 4.0](https://www.pjrc.com/store/teensy40.html)
  - [Teensy Audio Board](https://www.pjrc.com/store/teensy3_audio.html)
  - [Innosent IPS-354 Radarmodul](https://www.innosent.de/radarsensoren/ips-354/) ([Handbuch](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/2406/200730_Data%20Sheet_IPS-354_V1.5.pdf))
  - [isolierter DC-DC: ROE-3.305S](https://de.rs-online.com/web/p/dcdc-wandler/1392970)
  - [Akkupack](https://exp-tech.de/products/battery-lipo6600mah?_pos=33&_sid=1be852f75&_ss=r)
  - [USB-C LiPo Charger](https://eckstein-shop.de/AdafruitMicro-LipoChargerforLiPolyBattwithUSBTypeCJack)
  - Micro-SD-Karte nach Wahl
  - [Knopfzellenhalter](https://www.amazon.de/HALJIA-Knopfzellen-Batteriehalter-Ausschalter-Knopfzellen-Halterung/dp/B099HX71JX/ref=sr_1_14?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=I6ZENFBJGDNA&keywords=c2032+battery+holder&qid=1699254568&sprefix=c2032+battery+holder%2Caps%2C89&sr=8-14)
  - Knopfzelle CR2032
  - [Stiftleiste Strip 1x40 Pin](https://eckstein-shop.de/Single-Double-Row-Pin-Male-Header-Stiftleiste-Strip-1x40-Pin-GeradeA-5-Stuecke)
  - 40mm Kabel für Gnd des Radarmoduls
  - 40mm 2-Ader Kabel für Batteriestecker
  - [Batteriestecker JST PH 2Pin 2.0mm](https://eckstein-shop.de/2Pin-JST-PH-20-Kable-Kit-20-Paare)


- Gehäuse
  - [TRU COMPONENTS F3 TC-6649456 Universal-Gehäuse](https://www.conrad.de/de/p/tru-components-f3-tc-6649456-universal-gehaeuse-115-x-90-x-55-abs-hellgrau-1-st-1662364.html)
  - [3D-Druck Halterung](https://community.fablab-cottbus.de/uploads/short-url/1HOEbMkdQxn1l1QFID4sH8OvwRe.stl)
  - [Lasercut Teile](https://community.fablab-cottbus.de/uploads/default/original/2X/5/5f1b514fec6fc872ee79204f1ad61963588dafd5.svg) zur Befestigung.
  - Velcro zur Befestigung des Akkus [180cm](https://www.amazon.de/Klettband-Kabelbinder-Schwarz-Wiederverschlie%C3%9Fbar-Klettverschluss/dp/B0CPLTQWXX/ref=sr_1_39?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=19HZ36R8YGTWB&dib=eyJ2IjoiMSJ9.zfnxfXdxMqAt2BMKak15S3NP-2l6pp5Sw3M6amSeiU5nDnL2BI35ZJ_NRRR-T-y5v3jvoxZzzMvHrxBKWsd-BtsIU_T9unN--GaLoaIFjGVfFsbQnpeqrk4G16SNwbu2i7AAglZ7Z3sk_qxoXZpuIkTi136Rgb6gX-rCMjYR7l0zduayOTpAPWax-oeJLolsrt0oHf6lkCGDt3aH-9L8Ey9O6xGARKGpJkYVm0Zu4ChZuL_3J4Bi_28o3gegeGfW5ZCf9J40mVDYhv066mQsyP552pRPyHMKAe9sjoE3Rag.8v6mmKF8fdiOWVwuZwriRJ59G0zS5hETb26buriVtio&dib_tag=se&keywords=velcro&qid=1730013941&sprefix=velcro%2Caps%2C169&sr=8-39)
  - Befestigungsschrauben
    - 4x M4 5-8mm für Einlegeplatte 
    - 5x M3 5mm für Befestigung der Platine und Seitenteile des Radarmoduls

- Für mehr Diebstahlschutz:
  - 4x [Sicherheitsschrauben M4 20mm Edelstahl](https://www.conrad.de/de/p/toolcraft-888808-senkkopfschraube-m4-20-mm-t-profil-mit-stift-edelstahl-a2-10-st-888808.html)
  - 1x [Hiplok Z LOK](https://www.amazon.de/Hiplok-Multifunktions-Sicherheitsband-Unisex-BLACK-Schlie%C3%9Fumfang/dp/B079P8M5JW/ref=sr_1_6?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=21XX5JDRW7YMJ&dib=eyJ2IjoiMSJ9.-4XGQt9Jd0gLQ4uLShBxvf9z0U4NY4l65tPFVYw6l6t7fXZgVw8vOFMroqwwLD75N7UsokATn_CxioqPYC31IPW64XuX43SBgFuwCPGvQbGktVJ6EXyZsILUm_MgPFL4CvV4IWuESB83kk6EvHwPyjRAsva3u-taJu6-Wwh_6dfAgMO9KA9i5BbE8epuJVVyMCp_KnqBlxWQchhJFYxw0k-QqkQ5-gugDJM8lHwteyCFNple3-r43Yes_Yj6J9LKjoxJV11TSmpvi1_mM_bUzLHlnIB2EMTw7Eqrk2M3fPE.Zl2quaoWBM6ot47Xpnz7J5G3N21nBQB6II6KFKtowiA&dib_tag=se&keywords=Hiplok%2BZ%2BLOK&qid=1730013071&sprefix=hiplok%2Bz%2Blok%2B%2Caps%2C108&sr=8-6&th=1)


- Pfahlbefestigung

   - Lasercut Platte (enthält auch die Unterlegscheiben)
   - 4x M5x10 für die Befestigungsplatte
   - 2x [Velcro Gurt 2cm x 30cm](https://www.amazon.de/ChiliTec-Klettband-Sicheres-Verstauen-Leitungen/dp/B07H7PKW5M/ref=sr_1_9?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=JXGB8D6OZK9Q&dib=eyJ2IjoiMSJ9.S5gVrdnKeDZr7SC4IxM-u0ZPjjsSnxq04rBw6MHmA_7eHcwZKNPOoC-Z93EVQJ35hsQqiIm3CB5kFXSMXmGzqMq8PScr0WdecEoctmtWjCqIfsh5inEukbAtlzNtj1VUF2pAtj9-9XJzDbqEeY_7PCJZeeO3FA0mCEDla0CerNZKUQh35qbqEC5SAgaT6liCuelNOQoG6Fa6MrwHncr7ZFOR3UgDH2h_GWnXxaTDQFH5TzAyqvSfSCFZcNWTpRfjy9rrk_20vf296z4H9gp2psrnBL3Thpydzv3_BcUuC2E.UjdnFJ8URxq9ICWeR1MkZ3TOfijziPI7rewrjIB-BI0&dib_tag=se&keywords=velcro+gurt&qid=1730013320&sprefix=velcro+gurt%2Caps%2C120&sr=8-9)
   - 1x Kabelbinder

## Teileliste nach Anbieter und Warenkörbe zur Bestellung

- Eckstein ([Warenkorb](https://eckstein-shop.de/Projekt?wlid=671dd6ebd2a233.33264534&jtl=w)) (ca. 84 €)
   - [Teensy 4.0](https://eckstein-shop.de/PJRCTeensy42C0DevelopmentBoardCortex-M7600MHzArduinoIDE)
   - [Teensy Audio Shield 1](https://eckstein-shop.de/PJRCAudioAdaptorBoardforTeensy40RevD2C16bit441kHzStereowith35mmOutput)
   - [6600mAh Akkupack (3x 18650)](https://eckstein-shop.de/PKNERGY-Lithium-Ion-Battery-Pack-ICR-18650-37V-6600mAh-LiPo-Li-Ion-with-JST-PH-Connector)
   - [Single Row Pin Male Header Stiftleiste Strip 1x40 Pin Gerade 2,54 mm Abstand](https://eckstein-shop.de/Single-Double-Row-Pin-Male-Header-Stiftleiste-Strip-1x40-Pin-GeradeA-5-Stuecke)
   - [Adafruit USB-C LiPo Charger](https://eckstein-shop.de/AdafruitMicro-LipoChargerforLiPolyBattwithUSBTypeCJack)
   - [Batteriestecker JST PH 2Pin 2.0mm](https://eckstein-shop.de/2Pin-JST-PH-20-Kable-Kit-20-Paare)

- Amazon ([Warenkorb](https://www.amazon.de/hz/wishlist/ls/9DZWF3RX0MH3?ref_=wl_share)) (ca. 50€ )
    - [Stackable Header 6-Pin](https://www.amazon.de/DFRobot-Stackable-Header-Source-BOOOLE/dp/B01B0INCIW/ref=rtpb_d_sccl_2/259-6201765-9188446?pd_rd_w=jCied&content-id=amzn1.sym.f110c583-c94d-4a6a-91be-167cde49faa0&pf_rd_p=f110c583-c94d-4a6a-91be-167cde49faa0&pf_rd_r=89Q4QDRDJNRYP70NCX67&pd_rd_wg=vlWTf&pd_rd_r=0bf15cc2-24ab-4590-96e7-2b7a505a0742&pd_rd_i=B01B0INCIW&psc=1) (kann auch einzeln von uns bestellt werden)
    - [Header 4-Pin](https://www.amazon.de/Stiftleiste-Buchsenleiste-Weiblichen-LeistenStifte-Elektronische/dp/B09NJMBBLX/ref=sr_1_2?dib=eyJ2IjoiMSJ9.shMu9_kjlBX6tzmAqKKdseKx9L78TlF6C65w2o8Ue4MvzhViQsLFN1JbE7ZKlRYMmr1NXgNzkKwdwXHfRwFGXumrN9kBXvZc09yzZQyfFVGMGik6tLCYLP-pYpOBrO3WOHuLNbRxTXpkC9-sb4S69Dxi-Oy6BdD-efAclzPwILORLHX6tfT7RztpVjRgHgJ1OS_Ure6CYrxL4C16_unlGsDerk-p_BwN9H_23WGjf0GRNHz-99m6LkJyzq8D5HyFJgA9lxbBNMXQgzhLPBsMoBB_NEayJGpM4rtzUa3xZww.5nB9Dxl0fO4IVfCUbli4HDkS5AtSRtm5nTdbUJJocgc&dib_tag=se&keywords=header+4-pin&qid=1730091857&sr=8-2)
    - [Knopfzellenhalter mit Kabel](https://www.amazon.de/HALJIA-Knopfzellen-Batteriehalter-Ausschalter-Knopfzellen-Halterung/dp/B099HX71JX/ref=sr_1_14?__mk_de_DE=ÅMÅŽÕÑ&crid=I6ZENFBJGDNA&keywords=c2032+battery+holder&qid=1699254568&sprefix=c2032+battery+holder%2Caps%2C89&sr=8-14)
    - [Velcro Gurt 2cm x 30cm](https://www.amazon.de/ChiliTec-Klettband-Sicheres-Verstauen-Leitungen/dp/B07H7PKW5M/ref=sr_1_9?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=JXGB8D6OZK9Q&dib=eyJ2IjoiMSJ9.S5gVrdnKeDZr7SC4IxM-u0ZPjjsSnxq04rBw6MHmA_7eHcwZKNPOoC-Z93EVQJ35hsQqiIm3CB5kFXSMXmGzqMq8PScr0WdecEoctmtWjCqIfsh5inEukbAtlzNtj1VUF2pAtj9-9XJzDbqEeY_7PCJZeeO3FA0mCEDla0CerNZKUQh35qbqEC5SAgaT6liCuelNOQoG6Fa6MrwHncr7ZFOR3UgDH2h_GWnXxaTDQFH5TzAyqvSfSCFZcNWTpRfjy9rrk_20vf296z4H9gp2psrnBL3Thpydzv3_BcUuC2E.UjdnFJ8URxq9ICWeR1MkZ3TOfijziPI7rewrjIB-BI0&dib_tag=se&keywords=velcro+gurt&qid=1730013320&sprefix=velcro+gurt%2Caps%2C120&sr=8-9) (Gehäusebefestigung für z.B. Straßenschild)
    - [Velcro Klettband Kabelbinder 180cm](https://www.amazon.de/Klettband-Kabelbinder-Schwarz-Wiederverschlie%C3%9Fbar-Klettverschluss/dp/B0CPLTQWXX/ref=sr_1_39?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=19HZ36R8YGTWB&dib=eyJ2IjoiMSJ9.zfnxfXdxMqAt2BMKak15S3NP-2l6pp5Sw3M6amSeiU5nDnL2BI35ZJ_NRRR-T-y5v3jvoxZzzMvHrxBKWsd-BtsIU_T9unN--GaLoaIFjGVfFsbQnpeqrk4G16SNwbu2i7AAglZ7Z3sk_qxoXZpuIkTi136Rgb6gX-rCMjYR7l0zduayOTpAPWax-oeJLolsrt0oHf6lkCGDt3aH-9L8Ey9O6xGARKGpJkYVm0Zu4ChZuL_3J4Bi_28o3gegeGfW5ZCf9J40mVDYhv066mQsyP552pRPyHMKAe9sjoE3Rag.8v6mmKF8fdiOWVwuZwriRJ59G0zS5hETb26buriVtio&dib_tag=se&keywords=velcro&qid=1730013941&sprefix=velcro%2Caps%2C169&sr=8-39) (Akkubefestigung)
    - [Hiplok Z LOK Sicherheitsschloss](https://www.amazon.de/Hiplok-Multifunktions-Sicherheitsband-Unisex-BLACK-Schlie%C3%9Fumfang/dp/B079P8M5JW/ref=sr_1_6?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=21XX5JDRW7YMJ&dib=eyJ2IjoiMSJ9.-4XGQt9Jd0gLQ4uLShBxvf9z0U4NY4l65tPFVYw6l6t7fXZgVw8vOFMroqwwLD75N7UsokATn_CxioqPYC31IPW64XuX43SBgFuwCPGvQbGktVJ6EXyZsILUm_MgPFL4CvV4IWuESB83kk6EvHwPyjRAsva3u-taJu6-Wwh_6dfAgMO9KA9i5BbE8epuJVVyMCp_KnqBlxWQchhJFYxw0k-QqkQ5-gugDJM8lHwteyCFNple3-r43Yes_Yj6J9LKjoxJV11TSmpvi1_mM_bUzLHlnIB2EMTw7Eqrk2M3fPE.Zl2quaoWBM6ot47Xpnz7J5G3N21nBQB6II6KFKtowiA&dib_tag=se&keywords=Hiplok%2BZ%2BLOK&qid=1730013071&sprefix=hiplok%2Bz%2Blok%2B%2Caps%2C108&sr=8-6&th=1) (optional)

- Conrad ([Warenkorb](https://www.conrad.de/de/service/wishlist.html?sharedId=ba5b7472-2fd7-4b78-84e7-a2f183c9bef2)) (ca. 28€)
    - [SD-Karte](https://www.conrad.de/de/p/verbatim-micro-sdhc-32gb-cl-10-adap-microsdhc-karte-32-gb-class-10-inkl-sd-adapter-419772.html)
    - [TRU COMPONENTS F3 TC-6649456 Gehäuse 115x90x55 mm](https://www.conrad.de/de/p/tru-components-f3-tc-6649456-universal-gehaeuse-115-x-90-x-55-abs-hellgrau-1-st-1662364.html)
    - [isolierter DC/DC-Wandler 200 mA RECOM ROE-3.305S](https://www.conrad.de/de/p/recom-roe-3-305s-dc-dc-wandler-print-5-200-ma-1-w-anzahl-ausgaenge-1-x-inhalt-1-st-2330532.html?searchType=SearchRedirect)
    - [Knopfzelle CR2032](https://www.conrad.de/de/p/energizer-knopfzelle-cr-2032-3-v-1-st-240-mah-lithium-cr2032-651088.html)
    - [Sicherheitsschrauben M4 20mm Edelstahl](https://www.conrad.de/de/p/toolcraft-888808-senkkopfschraube-m4-20-mm-t-profil-mit-stift-edelstahl-a2-10-st-888808.html) (optional)

- digikey (47 €)
  - [innosent IPS-354 24GHZ RADAR MODULE](https://www.digikey.de/de/products/detail/innosent-gmbh/80-00000356/10416540)

Einige der Teile oben sind nur als größeres Set erhältlich. Wenn man nicht mehrere Sensoren baut bleibt da natürlich der Großteil liegen. Von daher könnt ihr von uns als Set erhalten:


- 1x stackable Header 6-Pin
- 1x Header 4-Pin
- 1x Velcro Klettband Kabelbinder 180cm für die Batterie
- 2x Velcro Gurt 30cm für die Mastbefestigung
- 1x Knopfzellenhalter
- 1x Batteriestecker JST PH 2Pin 2.0mm
- 4x Sicherheitsschrauben M4 20mm Edelstahl
- 4x M5x10 Schrauben für die Befestigungsplatte
- 4x M4 Schrauben für Einlegeplatte
- 5x M3 für Befestigung der Platine und Seitenteile des Radarmoduls
- nötige Kabel


Damit ihr nicht bei 4x Versandkosten zahlen müsst können wir euch noch das Radarmodul dazu legen:

- 1x innosent IPS-354 24GHZ RADAR MODULE

<figure class="figure">
          <img src="/parts/gehause_ges.png" alt="Gehäuse gesamt" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Gehäuse</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/akku.png" alt="Akku-Pack" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Akku-Pack</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/lasercut_fuesse.png" alt="Lasercut-Füße" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Lasercut-Füße</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/3d_radarhalter.png" alt="3D-Druck-Halterung für Radarmodul" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Radarhalterung</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/radarmodul.jpeg" alt="Radarmodul" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">Radarmodul</figcaption>
        </figure>
        <figure class="figure">
          <img src="/parts/microsd.png" alt="MicroSD-Karte" width="150" class="img-fluid figure-img">
          <figcaption class="figure-caption">MicroSD-Karte</figcaption>
        </figure>
        
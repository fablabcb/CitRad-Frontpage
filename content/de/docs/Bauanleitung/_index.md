---
title: Bauanleitung
description: Wie baut man den CitRad Radarsensor?
categories: []
tags: []
weight: 2
---


## Teile

- Elektronik
  - [Teensy 4.0](https://www.pjrc.com/store/teensy40.html)
  - [Teensy Audio Board](https://www.pjrc.com/store/teensy3_audio.html)
  - [Innosent IPS-354 Radarmodul](https://www.innosent.de/radarsensoren/ips-354/) ([Handbuch](https://mm.digikey.com/Volume0/opasdata/d220001/medias/docus/2406/200730_Data%20Sheet_IPS-354_V1.5.pdf))
  - [isolierter DC-DC: ROE-3.305S](https://de.rs-online.com/web/p/dcdc-wandler/1392970)
  - [Akkupack](https://exp-tech.de/products/battery-lipo6600mah?_pos=33&_sid=1be852f75&_ss=r)
  - [USB-C LiPo Charger](https://eckstein-shop.de/AdafruitMicro-LipoChargerforLiPolyBattwithUSBTypeCJack)
  - SD-Karte nach Wahl
  - [Knopfzellenhalter](https://www.amazon.de/HALJIA-Knopfzellen-Batteriehalter-Ausschalter-Knopfzellen-Halterung/dp/B099HX71JX/ref=sr_1_14?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=I6ZENFBJGDNA&keywords=c2032+battery+holder&qid=1699254568&sprefix=c2032+battery+holder%2Caps%2C89&sr=8-14)
  - Knopfzelle CR2032
  - [Stiftleiste Strip 1x40 Pin](https://eckstein-shop.de/Single-Double-Row-Pin-Male-Header-Stiftleiste-Strip-1x40-Pin-GeradeA-5-Stuecke)
  - 40mm Kabel für Gnd des Radarmoduls
  - 40mm 2-Ader Kabel für Batteriestecker
  - [Batteriestecker JST PH 2Pin 2.0mm](https://eckstein-shop.de/2Pin-JST-PH-20-Kable-Kit-20-Paare)


- Gehäuse
  - [TRU COMPONENTS F3 TC-6649456 Universal-Gehäuse](https://www.conrad.de/de/p/tru-components-f3-tc-6649456-universal-gehaeuse-115-x-90-x-55-abs-hellgrau-1-st-1662364.html)
  - [3D-Druck Halterung](https://community.fablab-cottbus.de/uploads/short-url/1HOEbMkdQxn1l1QFID4sH8OvwRe.stl)
  - [Lasercut Teile](https://community.fablab-cottbus.de/uploads/default/original/2X/0/07901a34dd58c6f2333bfa3191eb76f0abf1efdd.svg) zur Befestigung.
  - Velcro zur Befestigung des Akkus [180cm](https://www.amazon.de/Klettband-Kabelbinder-Schwarz-Wiederverschlie%C3%9Fbar-Klettverschluss/dp/B0CPLTQWXX/ref=sr_1_39?__mk_de_DE=%C3%85M%C3%85%C5%BD%C3%95%C3%91&crid=19HZ36R8YGTWB&dib=eyJ2IjoiMSJ9.zfnxfXdxMqAt2BMKak15S3NP-2l6pp5Sw3M6amSeiU5nDnL2BI35ZJ_NRRR-T-y5v3jvoxZzzMvHrxBKWsd-BtsIU_T9unN--GaLoaIFjGVfFsbQnpeqrk4G16SNwbu2i7AAglZ7Z3sk_qxoXZpuIkTi136Rgb6gX-rCMjYR7l0zduayOTpAPWax-oeJLolsrt0oHf6lkCGDt3aH-9L8Ey9O6xGARKGpJkYVm0Zu4ChZuL_3J4Bi_28o3gegeGfW5ZCf9J40mVDYhv066mQsyP552pRPyHMKAe9sjoE3Rag.8v6mmKF8fdiOWVwuZwriRJ59G0zS5hETb26buriVtio&dib_tag=se&keywords=velcro&qid=1730013941&sprefix=velcro%2Caps%2C169&sr=8-39)
  - Befestigungsschrauben
    - 6x M4 für Einlegeplatte und Seitenteile des Radarmoduls
    - 3x M3 für Befestigung der Platine

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
- 6x M4 Schrauben für Einlegeplatte und Seitenteile des Radarmoduls
- 3x M3 für Befestigung der Platine
- nötige Kabel


Damit ihr nicht bei 4x Versandkosten zahlen müsst können wir euch noch das Radarmodul dazu legen:

- 1x innosent IPS-354 24GHZ RADAR MODULE





## Aufbau

### Platine vorbereiten

1. Teensy Vusb-Verbindung trennen (mit Messer). Danach einmal an USB anstecken und sicherstellen dass der Teensy nicht mehr von USB versorgt wird.
1. Knopfzellenbatterie an Teensy anlöten. Vor dem Anlöten Schrumpfschlauch über beide Kabel (wird später als Zugentlastung an die Stromversorgungskabel geschrumpft).
1. 14-Pin Pinleiste (zuschneiden aus 40-Pin Leiste) mit kurzer Seite in Audio Board einsetzen
1. Teensy auf die langen Stifte aufsetzen (Pins stehen über)
1. Pins auf der Audio Board Seite festlöten
1. Von der Teensy Seite: 5V Pin und GND Pin (rechts und links vom USB) nach vorne biegen.
1. Batteriekabel an die überstehenden Pins von Gnd und 5V des Teensy löten. Dabei das eine Kabel durch den Schrumpfschlauch am Kabel der Knopfzellenbatterie fädeln (Zugentlastung).
1. Danach alle 14 Pins auch von der Teensy-Seite anlöten.
1. Batteriestecker an Batteriekabel löten.
1. Die restlichen überlangen Pins können optional gekürzt werden.
1. DC-DC mit 3.3V und Gnd des Teensy verbinden (siehe Foto)
1. 6-Pin-Stecker mit langen Beinen anlöten:
    1. Pin 1 (Nummerierung wie am Radar-Modul) aus dem Stecker ziehen (wird nicht benötigt).
    1. Pin 5 und 6 umbiegen sodass sie in die line-in Anschlüsse des Audio Boards passen (siehe Foto).
    1. Enable (Pin 2) umbiegen und mit Pin 17 des Teensy verbinden (passt gerade so).
    1. Gnd (Pin 4) und Vcc (Pin 3) mit dem Output des DC-DC verbinden (siehe Foto). Hier muss man ca 4mm mit Lötzinn oder einem kurzen Draht überbrücken.
1. 4-Pin Stecker: GND (Pin 9) über kurzes Kabel mit Gnd am linein oder mic in verbinden.

### Radarmodul zusammen stecken

1. Radarmodul in 3D-Druck Halterung stecken (siehe Foto).
1. Teensy an 3D-Druck Halterung anschrauben (siehe Foto). Dabei die Stecker des Radarmoduls aufstecken.
1. 4-Pin Stecker am Radarmodul einstecken.
1. Lasercut Teile seitlich an das Radarmodul anschrauben.
1. SD-Karte in Audioboard einsetzen.

### Gehäuse vorbereiten

1. Grundplatte in Gehäuse schrauben.
1. Gewinde in Befestigungslöcher (Rückseite) schneiden.
1. Mastplatte mit M5-Schrauben und den Unterlegschrauben (im Lasercut Teil enthalten) an Rückseite anschrauben. 
1. Gummidichtung in Deckel einlegen (was zu lang ist abschneiden).

### Zusammenbau

1. Akku mit Kletterverschluss an Grundplatte befestigen.
1. Knopfzelle in Knopzellenhalter einsetzen.
1. Radarmodul mit Halterung in Schlitze in der Grundplatte stecken.
1. Teensy mit Batterie verbinden.

## Software installieren
1. Sketch drauf laden
2. Uhrzeit einstellen
3. Mit Processing überprüfen ob der Radarsensor richtig funktioniert
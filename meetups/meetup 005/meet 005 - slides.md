---

title: Bastelrunde - #006 Hardware & Software
description: Senden der Daten zum TTN
tags: slide,programming,lorawan
type: slide
  
---
<style>
@import url('https://fonts.googleapis.com/css2?family=Lobster&family=Permanent+Marker&display=swap');
h1, h2 {
	font-family: 'Permanent Marker', cursive !important;
	text-shadow: 0 0 12px #000 !important;
}
</style>

<!-- slide bg="[[vergissberlin_young_person_in_a_garden_with_a_microcontroller_e_4b8f3925-109e-4348-b8c7-eceac7ae8b4e.png]]" data-auto-animate     -->

# Bastelrunde 
<!-- element style="padding-top: 30%; text-shadow: 4px 4px 2px 2px #000;" -->
## #005 Regenfass
<!-- element style="text-shadow: 4px 4px 2px 2px #000" -->

---

## Onbording

1) Was ist LoRaWAN Leipzig
2) Wo wir uns befinden
3) Wo die Toiletten sind
4) Wo gibt es Getränke?

<!--
- [ ] Was ist LoRaWAN Leipzig
	- [ ] Ziele
	- [ ] Wer sind die Leute
- [ ] Wo befinden wir uns (Basislager, Kohlenstraße)
- [ ] Wo sind die Toiletten
- [ ] Wo gibt es Getränke?
-->

--

## Hausregeln 
### Basislager

1) So verlassen wie vorgefunden
2) Getränke gegen Spende in die Box
3) Nicht löten
4) Keine sexistischen Zeichnungen an den Wänden

--

## Hausregeln 
### Glühende Kohlen

- So verlassen wie vorgefunden<!-- element class="fragment" -->

---

## Projektübersicht

1) ✅ Hardware Prototyp
2) Verbindung mit TTN
3) Datenverarbeitung in NodeRED
4) Datenmonitoring und Visualisierung
5) Veröffentlichung

<!--
1. Planung
2. Hardware Prototyp
3. Verbindung mit TTN
4. Datenverarbeitung in NodeRED
5. Datenmonitoring und Visualisierung
	1. Handy Notification
	2. Dashboard
6. Veröffentlichung
-->

---

## Werkzeug

1) Lötkolben, Lötzinn, Flußmittel, Helping Hand
2) Breadboard, Steckkabel
3) Multimeter
4) Notebook, USB Kabel
5) Kabel

---

## Hardware

1) ✅ Sensor
1) ✅ Microcontroller
1) ✅ LoRaWAN Chip
1) ✅ Energieversorgung
1) 🤷‍♂️ OLED Display

--

<grid drag="100 10" drop="0 0" bg="#111"  >
Hardware aktuell - *Boards*
</grid>

<grid drag="20 90" drop="0 10" bg="#222" style="font-size: 1.2rem;"  align="topleft">
<grid drag="100 30" drop="0 0" pad="4px">
![[hardware-board-ttgo-lora32-moo.png]]
</grid>

<grid drag="100 70" drop="0 30" bg="#0000dd33" align="topleft" pad="12px">
**[TTGO LORA32](https://amzn.to/3W2Zi6W)**

**Controller:** ESP32
**Preis:** 30,99 €
</grid>
</grid>


<grid  drag="20 90" drop="20 10" bg="#333" style="font-size: 1.2rem;"  align="topleft">
<grid drag="100 30" drop="0 0" pad="12px">
![[hardware-board-ttgo-lora32-display.png]]
</grid>
<grid drag="100 70" drop="0 30" bg="#0000dd33" align="topleft" pad="12px">
**[LILYGO T-Beam](https://amzn.to/41w2BV1)**

**Controller:** ESP32
**Preis:** 38 €

**Extra Features:**<br>
OLED display
</grid>
</grid>


<grid drag="20 90" drop="40 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px">
<grid drag="100 30" drop="0 0" pad="18px">
![[hardware-board-heltec-esp32lora.png]]
</grid>
<grid drag="100 70" drop="0 30" bg="#0000dd33" align="topleft" pad="12px">
**[Heltec LORA32](https://amzn.to/3o08Vqf)**

**Controller:** ESP32
**Preis:** 29,99 €

**Extra Features:**<br>
OLED display
Batterie Management
</grid>
</grid>

<grid drag="20 90" drop="60 10" bg="#333" style="font-size: 1.2rem;"  align="topleft" pad="24px">
<grid drag="100 30" drop="0 0" pad="12px">
![[hardware-board-esp32.png]]
</grid>
<grid drag="100 70" drop="0 30" bg="#0000dd33" align="topleft" pad="12px">
**[NodeMCU ESP-32](https://amzn.to/3nQV05Y)**

**Controller:** ESP32
**Preis:** 11,49 € + Lora

**Extra Features:**<br>
LoRaWAN not included
</grid>
</grid>

<grid drag="20 90" drop="80 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px">
<grid drag="100 30" drop="0 0" pad="12px">
![[hardware-board-SX1262.png]]
</grid>
<grid drag="100 70" drop="0 30" bg="#0000dd33" align="topleft" pad="12px">
**[SX1262 LoRa](https://amzn.to/3o08Vqf)**

**Controller:** ASR6501
**Preis:** 25,99 €

**Extra Features:**<br>
OLED display
Batterie Management
</grid>
</grid>

--

<grid drag="100 10" drop="0 0" bg="#111"  >
 Hardware aktuell - *Sensoren*
</grid>

<grid drag="20 90" drop="0 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px" >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

**Type:** Ultraschall<br>
**Preis:** 12 €
</grid>

<grid drag="20 90" drop="20 10" bg="#333" style="font-size: 1.2rem;"  align="topleft" pad="24px" >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

**Type:** Ultraschall<br>
**Preis:** 12 €
</grid>

<grid drag="20 90" drop="40 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px">
![[hardware-sensor-removebg-preview.png|200]]
HXXX

**Type:** Ultraschall<br>
**Preis:** 12 €
</grid>

<grid drag="20 90" drop="60 10" bg="#333" style="font-size: 1.2rem;"  align="topleft" pad="24px">
![[hardware-sensor-removebg-preview.png|200]]
HXXX

**Type:** Ultraschall<br>
**Preis:** 12 €
</grid>

<grid drag="20 90" drop="80 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px">
![[hardware-sensor-removebg-preview.png|200]]
HXXX

**Type:** Ultraschall<br>
**Preis:** 12 €
</grid>

---

## Software

1. ✅ Platform.io<!-- element class="fragment" -->
1. ✅ C, C++<!-- element class="fragment" -->
1. ✅ Libraries<!-- element class="fragment" -->
1. TTN Platform<!-- element class="fragment" -->
1. Node-RED<!-- element class="fragment" -->
1. Grafana<!-- element class="fragment" -->
1. GitHub & GitHub Actions<!-- element class="fragment" -->

---


<!-- slide bg="[[vergissberlin_25_year_old_girl_sits_at_a_table_with_a_soldering_e44ef266-6099-429c-9568-ba914be8a7e6.png]]" data-auto-animate     -->

<grid drag="60 30" bg="#000000cc" style="border-radius: 12px;backdrop-filter: blur(10px);" pad="1em 2em 1em 1em">
## Today
👩‍💻🧑🏼‍💻👨🏻‍💻

1. Teams bilden
2. Probleme lösen
3. Ergebnisse teilen

</grid>


---


Let's go!

---

## Offboarding

- 🏁 Was wir heute geschafft haben<!-- element class="fragment" -->
- 🔎 Wo man den Quellcode findet<!-- element class="fragment" -->
- 🙋‍♂️ Fragen, Nöte oder Anregungen?<!-- element class="fragment" -->
- 📆 Wann wir uns das nächste Mal treffen<!-- element class="fragment" -->
- 🫥 Nothing left behind<!-- element class="fragment" -->
	- 🚪 Türen zu
	- 🗑️ Müll mitnehmen
	- 🪑 Stühle ranstellen
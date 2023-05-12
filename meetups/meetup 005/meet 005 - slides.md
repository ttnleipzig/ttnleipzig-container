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
}
</style>

<!-- slide bg="[[vergissberlin_young_person_in_a_garden_with_a_microcontroller_e_4b8f3925-109e-4348-b8c7-eceac7ae8b4e.png]]" data-auto-animate     -->

# Bastelrunde
<!-- element style="padding-top: 30%" -->
## Regenfass

---

## Onbording

- Was ist LoRaWAN Leipzig
- Wo wir uns befinden <!-- element class="fragment" -->
- Wo die Toiletten sind<!-- element class="fragment" -->
- Wo gibt es Getränke?<!-- element class="fragment" -->

<!--
- [ ] Was ist LoRaWAN Leipzig
	- [ ] Ziele
	- [ ] Wer sind die Leute
- [ ] Wo befinden wir uns (Basislager, Kohlenstraße)
- [ ] Wo sind die Toiletten
- [ ] Wo gibt es Getränke?
-->

---

## Projektübersicht

1. ✅ Hardware Prototyp
2. Verbindung mit TTN<!-- element class="fragment" -->
3. Datenverarbeitung in NodeRED<!-- element class="fragment" -->
4. Datenmonitoring und Visualisierung<!-- element class="fragment" -->
5. Veröffentlichung<!-- element class="fragment" -->

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

1. Lötkolben, Lötzinn, Flußmittel, Helping Hand<!-- element class="fragment" -->
2. Breadboard, Steckkabel<!-- element class="fragment" -->
3. Multimeter<!-- element class="fragment" -->
4. Notebook, USB Kabel<!-- element class="fragment" -->
5. Kabel<!-- element class="fragment" -->

---

## Hardware

- ✅ Sensor<!-- element class="fragment" -->
- ✅ Microcontroller<!-- element class="fragment" -->
- ✅ LoRaWAN Chip<!-- element class="fragment" -->
- ✅ Energieversorgung<!-- element class="fragment" -->

--


<grid drag="100 10" drop="0 0" bg="#111"  >
 Hardware aktuell - *Boards*
</grid>

<grid drag="20 90" drop="0 10" bg="#222"  >

![[hardware-controller-removebg-preview.png|200]]

</grid>
<grid drag="80 90" drop="20 10" bg="#333">


| Bezeichnung | Chip        |
| ----------- | ----------- |
| Heltec      | ESP32       |
| Paragraph   | Text        |

</grid>


--

<grid drag="100 10" drop="0 0" bg="#111"  >
 Hardware aktuell - *Sensoren*
</grid>

<grid drag="20 90" drop="0 10" bg="#222"  >
![[hardware-sensor-removebg-preview.png|200]]
<small>
Ultraschall
asdasd
asdasd
asdasd
</small>
</grid>

<grid drag="80 90" drop="20 10" bg="#333">
| Technologie | Bezeichnung |
| ----------- | ----------- |
| Ultraschall | HXXX        |
| Laser       | LXXXX       |
</grid>



--

<grid drag="100 10" drop="0 0" bg="#111"  border="1px #aaa solid"   >
 Hardware aktuell - *Sensoren*
</grid>

<grid drag="20 90" drop="0 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px" border="1px #aaa solid"   >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

1. Ultraschall
2. Preis: 12 €
</grid>

<grid drag="20 90" drop="20 10" bg="#333" style="font-size: 1.2rem;"  align="topleft" pad="24px" border="1px #aaa solid"   >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

Ultraschall
Preis: 12 €
</grid>

<grid drag="20 90" drop="40 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px" border="1px #aaa solid"   >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

Ultraschall
Preis: 12 €
</grid>


<grid drag="20 90" drop="60 10" bg="#333" style="font-size: 1.2rem;"  align="topleft" pad="24px" border="1px #aaa solid"   >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

Ultraschall
Preis: 12 €
</grid>

<grid drag="20 90" drop="80 10" bg="#222" style="font-size: 1.2rem;"  align="topleft" pad="24px" border="1px #aaa solid"   >
![[hardware-sensor-removebg-preview.png|200]]
HXXX

Ultraschall
Preis: 12 €
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

<grid drag="60 30" bg="#000000cc" style="border-radius: 12px" pad="1em 2em 1em 1em">
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

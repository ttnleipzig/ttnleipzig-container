---
title: Bastelrunde - 016 Install Webpage
description: Debugging mit IoT
tags:
  - slide
  - programming
  - lorawan
type: slide
---
<style>
@import url('https://fonts.googleapis.com/css2?family=Lobster&family=Permanent+Marker&display=swap');
h1, h2 {
	font-family: 'Permanent Marker', cursive !important;
	text-shadow: 0 0 12px #000 !important;
}
</style>

<!-- slide bg="[[meetup-016.png]]" data-auto-animate     -->

# Bastelrunde 
<!-- element style="padding-top: 30%; text-shadow: 4px 4px 2px 2px #000;" -->
## #016 Konfigurationsdaten mit dem Browser bearbeiten

<!-- element style="text-shadow: 4px 4px 2px 2px #000" -->

<!--
**Checkliste bevor es losgeht:**

- [ ] Foto gemacht
- [ ] Tweet gesendet
- [ ] Hochkant Video

-->

---

## Onboarding

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

<!-- slide bg="[[vergissberlin_man_on_a_roof_top_with_an_antenna_and_a_soldering_17ba6cf4-1d1b-4eba-b3ee-30b9431dd2c1.png]]" -->

<grid drag="60 30" bg="#ffffff88" style="border-radius: 12px;backdrop-filter: blur(20px);" pad="1em 2em 1em 1em">

<small>sponsored by</small>

![Thinkport](https://thinkport.digital/wp-content/uploads/elementor/thumbs/Logo_horizontral_new-q79kisryfbimg521qvcamhuu9zgajwl52ie1tm6q0s.png)

</grid>

--

## Projektübersicht

1) ✅ Hardware Prototyp
2) ✅ Verbindung mit TTN
3) ✅ Automatisierte Releases auf GitHub
4) 👩‍💻 Veröffentlichung
5) Datenverarbeitung in NodeRED
6) Datenmonitoring und Visualisierung


---
<!-- slide bg="[[vergissberlin_microcontroller_flying_through_clouds_e4ca3e11-4904-4bfb-a259-0a4fbf2dee4e.png]]" -->

<grid drag="60 30" bg="#000000cc" style="border-radius: 12px;backdrop-filter: blur(10px);" pad="1em 2em 1em 1em">

## Today 👩‍💻🧑🏼‍💻👨🏻‍💻

1) Möglichkeiten
1) Werkzeuge und Technologien auswählen
1) Integration bei regenfass
</grid>

--

# Dateisysteme

Verfügbare **Dateisysteme** für **Mikrocontroller**:

1) **FAT (File Allocation Table)**
    <!--
    - FAT16 und FAT32 sind weit verbreitete Dateisysteme, die auf Flash-Speicher eingesetzt werden können.
    - Sie sind einfach zu implementieren und unterstützen Verzeichnisse.
    - Allerdings haben sie einen gewissen Overhead und sind möglicherweise nicht ideal für speicher- oder RAM-beschränkte Anwendungen.
    -->
1) **SPIFFS (SPI Flash File System)**
    <!--    
    - **Ursprüngliches Dateisystem**: SPIFFS war das ursprüngliche Dateisystem für ESP8266 und ESP32.
    - **Geeignet für speicher- und RAM-beschränkte Anwendungen**: SPIFFS eignet sich gut für Anwendungen mit begrenztem Speicherplatz und RAM, die viele kleine Dateien verwenden und statisches und dynamisches Wear-Leveling benötigen.
    - **Minimale Dateisystem-Overhead**: Der Overhead auf dem Flash-Speicher ist minimal.
    - **Keine echte Verzeichnisunterstützung**: SPIFFS unterstützt keine echten Verzeichnisse.
    - **Wird von Espressif nicht mehr empfohlen**: Espressif hat SPIFFS aufgrund seiner mangelnden Robustheit und relativen Langsamkeit nicht weiter empfohlen.
    -->
2) **LittleFS**
    <!--
    - **Neuere Alternative**: LittleFS ist eine neuere Alternative zu SPIFFS.
    - **Höhere Leistung und Verzeichnisunterstützung**: LittleFS konzentriert sich auf höhere Leistung und bietet echte Verzeichnisunterstützung.
    - **Höherer Overhead pro Datei**: LittleFS hat einen höheren Overhead pro Datei (mindestens 4 KB im Vergleich zu SPIFFS’ 256 Byte).
    - **Resilienz bei Stromausfällen**: LittleFS ist widerstandsfähiger gegen Stromausfälle, und das Dateisystem wird nicht beschädigt, wenn der Strom während einer Schreiboperation ausfällt.
    -->
3) **EFSL (Embedded File System Library)**
    <!--
    - EFSL ist ein plattformübergreifendes FAT16/32-Dateisystem, das Partitionen und Superfloppys unterstützt.
    - Es enthält Beispielcode für Mikrocontroller wie AVR, LPC2000 und AT91SAM7.
    -->
4) **YAFFS (Yet Another Flash File System)**
    <!--
    - YAFFS ist ein speziell für NAND-Flash-Speicher entwickeltes Dateisystem.
    - Es bietet hohe Zuverlässigkeit und Wear-Leveling-Funktionen.
    -->
5) **JFFS2**
    <!--
    (Journalling Flash File System 2)
    - JFFS2 ist ein Linux-Dateisystem, das für NOR-Flash-Speicher optimiert ist.
    - Es verwendet ein Journaling-System, um Datenintegrität sicherzustellen.
    -->
6) **UBIFS (Unsorted Block Image File System)**
    <!--
    - UBIFS ist ein weiteres Linux-Dateisystem, das für NAND-Flash-Speicher entwickelt wurde.
    - Es bietet bessere Komprimierung und Wear-Leveling.
    -->
7) **ROMFS (Read-Only Memory File System)**
    <!--
    - ROMFS ist ein schreibgeschütztes Dateisystem, das in den ROM-Bereich des Mikrocontrollers geladen wird.
    - Es eignet sich für statische Daten wie Konfigurationsdateien.
    -->

<!--
Die Wahl des richtigen Dateisystems hängt von deinen spezifischen Anforderungen ab, einschließlich Speicherplatz, Geschwindigkeit und Zuverlässigkeit. [Es ist wichtig, die Vor- und Nachteile jedes Systems zu berücksichtigen und das am besten geeignete für deine Anwendung auszuwählen](https://www.mikrocontroller.net/articles/Kategorie:Speicher_und_Dateisysteme)[1](https://www.mikrocontroller.net/articles/Kategorie:Speicher_und_Dateisysteme)[2](https://www.mikrocontroller.net/articles/MMC-_und_SD-Karten)[3](https://www.mikrocontroller.net/topic/213556).
-->

---
### Beispiel mit LittleFS
```cpp
#include <Arduino.h>
#include <LittleFS.h>

void setup() {
  Serial.begin(115200);

  if (!LittleFS.begin()) {
    Serial.println("An error has occurred while mounting LittleFS");
    return;
  }

  // Erstellt eine Datei und schreibt Daten hinein
  File file = LittleFS.open("/example.txt", "w");
  if (!file) {
    Serial.println("There was an error opening the file for writing");
    return;
  }
  
  if (file.print("Hello World!")) {
    Serial.println("File was written");
  } else {
    Serial.println("File write failed");
  }

  file.close();

  // Liest die Daten aus der Datei
  file = LittleFS.open("/example.txt", "r");
  
  if (!file) {
    Serial.println("There was an error opening the file for reading");
    return;
  }
  
  while (file.available()) {
    Serial.write(file.read());
  }

  file.close();
}

void loop() {
}
```

--
## Reduces example - write

```cpp
#include <Arduino.h>
#include <LittleFS.h>

void setup() {
	Serial.begin(115200);
	LittleFS.begin()
	File file = LittleFS.open("/example.txt", "w");
	file.print("Hello World!");
	file.close();
}

void loop() {
}
```

--
## Off-boarding

1) 🏁 Was wir heute geschafft haben
2) 🔎 Wo man den Quellcode findet
3) 🙋‍♂️ Fragen, Nöte oder Anregungen?
4) 📆 Wann wir uns das nächste Mal treffen
5) 🫥 Nothing left behind
	- 🚪 Türen zu
	- 🗑️ Müll mitnehmen
	- 🪑 Stühle ranstellen

---
## Checkliste nach der Veranstaltung

-  Hardware zusammengesucht und eingepackt
- Nachher Foto
- Folgetermin Termin steht fest
- Hochkant Video - Zusammenfassung, Folgetermin

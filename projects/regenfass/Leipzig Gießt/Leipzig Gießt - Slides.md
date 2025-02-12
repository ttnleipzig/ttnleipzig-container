---
theme: consult
height: 540
margin: 0
maxScale: 4
bg: white
---
<!-- Slide 1 -->
# Was ist LoRa?

+ **LoRa** steht für Long Range.
+ Ist eine drahtlose Übertragungstechnologie.
+ Nutzt das lizenzfreie Sub-GHz-Frequenzband.
+ Ermöglicht große Reichweiten bei geringem Energieverbrauch.
+ Ideal für IoT-Anwendungen, bei denen Geräte batteriebetrieben sind.

![[lora.light.svg]]

---

<!-- Slide 2 -->
# Was ist LoRaWAN?

+ **LoRaWAN** steht für Long Range Wide Area Network.
+ Ein Kommunikationsprotokoll und Systemarchitektur auf Basis von LoRa.
+ Ermöglicht die Verbindung von IoT-Geräten mit dem Internet über Gateways.
+ Unterstützt bidirektionale Kommunikation.

![[lorawan.light.svg]]

note: this is not! Only the speaker might see this text.

---
<!-- Slide 3 -->
# TTN Leipzig User Group

+ Teil des The Things Network (TTN), einer globalen Community für LoRaWAN-Netzwerke.
+ Ziel: Aufbau eines freien und offenen IoT-Datennetzwerkes in Leipzig.
+ Austausch von Wissen und Erfahrungen rund um LoRa/LoRaWAN-Technologien.
+ Regelmäßige Treffen, Workshops und Projekte zur Förderung der Technologie.

--

<!-- slide bg="https://picsum.photos/seed/picsum/800/600" data-background-opacity="0.2" -->

## TTN LoRaWAN Gateways in Städten (03/2025)

```chart
    type: bar
    labels: [Berlin,London,München,Stuttgart,Leipzig,Dresden,Halle ]
    series:
      - title: Städte
        data: [142,129,114,53,31,30,14]
```

--
<iframe src="https://ttnmapper.org/heatmap/" height="100%" width="100%"></iframe>

---

```slide
{
	slide: [[TTN Leipzig]],
	page: 1
}
```

---

<!-- Slide 4 -->
# Projekt Regenfass mit LoRaWAN

![[leipzig-giesst.light.png|]]


---

## Regenfass

```chart
    type: line
    labels: [Jan,Feb,Mrz, Apr, Mai, Jun, Jul, Aug, Sept, Otk,Nov,Dez ]
    series:
      - title: Füllmenge
        data: [142,129,89,77,91,80,60,50,80,100,110,72,12]
```

---


## Ziel des Projekts:
Überwachung des Wasserstands in einem Regenfass mittels LoRaWAN.

--

## Komponenten:
1. Ultraschallsensor zur Messung des Wasserstands.
2. Mikrocontroller mit LoRa-Modul (z.B. Arduino + LoRa Shield).
3. Stromversorgung über Batterie oder Solarzelle.

--
## Vorteile:
- Echtzeitüberwachung des Füllstands aus der Ferne.
- Optimierung der Wassernutzung im Garten oder Landwirtschaft.

--
## Herausforderungen:
- Sicherstellen der Funkabdeckung durch ein geeignetes Gateway in der Nähe.
- Energieeffizientes Design, um Batterielaufzeit zu maximieren.

---

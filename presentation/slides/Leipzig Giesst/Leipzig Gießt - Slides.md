---
theme: consult
height: 540
margin: 0
maxScale: 4
bg: white
---

<!-- slide bg="#111" -->
## Leipzig Gießt & regenfass.eu
### Von der Idee zur smarten Lösung

note: Agenda
- **Einleitung** (Jörg)
	- App Vorstellung
	- [Code for Leipzig](https://codefor.de/leipzig/))
- Was ist LoRa / LoRaWAN?
- Was ist TTN Leipzig?
- regenfass.eu
	- Problem
	- Komponenten
		- Stromversorgung
		- Sensoren
		- Boards
		- Kosten 
		- Bauanleitung 
	- Benutzerfreundlichkeit
	- Integration in die App
	- Demo
	- Konzept Challenge

---
<!-- slide bg="#fff" -->
![[leipzig-giesst-karte.light.svg]]

note: 

**Wir haben ein Problem …**
1. Mit Leipzig gießt haben wir in der Stadt Wasserkanister, die wir immer ausreichend gefüllt haben wollen. Doch wir kennen den aktuellen Wasserstand nicht, weshalb wir immer wieder regelmäßig alle Kanister ansteuern müssen, um den Pegelstand zu messen.
2. Wir können versuchen ihn zu erraten indem wir zählen wir oft aus dem Kanister Wasser abgezogen wurde wurde, und raten wie groß jeweils die Wassermenge war, allerdings ist die Schätzung sehr ungenau.

**Wir haben eine Lösung …**
1. Also bauen wir einen Sensor den man in die Kanister installieren kann, der regelmäßig misst wie der aktuelle Pegelstand ist, und die Daten an Leipzig gießt sendet.
2. Der Plan steht, doch wie kommen wir zu diesem Ziel? Wir vom TTN Leipzig arbeiten nun schon seit zwei Jahren an diesem Problem und möchten euch mitnehmen auf unsere Reise und mit

**Nachbauen, mitmachen …**
1. Wir stecken noch in der Entwicklung, doch schon jetzt suchen wir Städte, denen unsere Lösung helfen könnte um uns Feedback abzuholen, und uns in die richtige Richtung zu lenken.

**Workshop**
1. Was hältst Du von der Idee?
2. Welche neuen Probleme könnten mit der Lösung auftreten und 
3. wie kann man sich ihnen entgegenstellen?
4. Was wären deine Erwartungen?

---

![[leipzig-giesst-hardware-2d.light.svg|580]]

---
### Funktechnologien

![[lora-reichweite.light.svg|500]]

---

# Was ist LoRa?

+ **LoRa** steht für Long Range.
+ Ist eine drahtlose Übertragungstechnologie.
+ Nutzt das lizenzfreie Sub-GHz-Frequenzband.
+ Ermöglicht große Reichweiten bei geringem Energieverbrauch.
+ Ideal für IoT-Anwendungen, bei denen Geräte batteriebetrieben sind.

---
# Was ist LoRaWAN?

+ **LoRaWAN** steht für Long Range Wide Area Network.
+ Ein Kommunikationsprotokoll und Systemarchitektur auf Basis von LoRa.
+ Ermöglicht die Verbindung von IoT-Geräten mit dem Internet über Gateways.
+ Unterstützt bidirektionale Kommunikation.

---
### LoRaWAN in der Praxis
#### Umwelt
+ 🍺 Pegelstandsmessungen in Flüssen
+ 💦 Bodenfeuchte messen

---
### LoRaWAN in der Praxis
### Smart City
+ 🗑️ Füllstandmessung Papierkörbe
+ 🚗 Parkplatz-Belegung
+ 🚴 Verkehrszählung
+ 😗💨 Luftqualität
+ 🔥 Verbrauchsmessung (Heizung)

---
<!-- .slide style="padding: 1em" -->
# TTN Leipzig User Group
<!-- element style="background:#eee;padding: .1em" -->

+ **Ziel:** Aufbau eines freien und offenen IoT-Datennetzwerkes in Leipzig mit dem The Things Network (TTN), einer globalen Community für LoRaWAN-Netzwerke.
+ Austausch von Wissen und Erfahrungen rund um LoRa/LoRaWAN-Technologien.




![[ttnle-team.png|600]]

---

<iframe frameborder=0 src="https://ttnmapper.org/heatmap/" height="100%" width="90%"></iframe>

---
<!-- slide bg="https://picsum.photos/seed/picsum/800/600" data-background-opacity="0.2" -->
## TTN LoRaWAN Gateways in Städten (03/2025)

```chart
type: bar
labels: [Berlin, London, München, Stuttgart, Leipzig, Dresden, Halle]
height: 400
series:
  - title: Städte
	data: [142,129,114,53,31,30,14]
```


---
![[leipzig-giesst-hardware-2d.light.svg|580]]

---
## Vorteile

+ Überwachung des Füllstands aus der Ferne.
+ Automatische Benachrichtigung bei niedrigen Pegelständen.

---
## Herausforderungen

+ Sicherstellen der Funkabdeckung durch ein geeignetes Gateway in der Nähe.
+ Energieeffizientes Design, um Batterielaufzeit zu maximieren.
+ Schutz gegen Korrosion.
+ Schutz gegen Vandalismus.

---
<!-- slide bg="https://img.fotocommunity.com/doppelter-regenbogen-81587c39-53cf-41e0-b08b-0a640d56b9a6.jpg?height=1080"  -->
# 🦄 Demo

---
## Workshop

1. Was hältst Du von der Idee?
2. Welche neuen Probleme könnten mit der Lösung auftreten und 
3. wie kann man sich ihnen entgegenstellen?
4. Was wären deine Erwartungen?

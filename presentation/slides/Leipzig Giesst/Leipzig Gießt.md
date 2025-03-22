

# Titel

---

### Agenda

- **Einleitung** (Jörg)
	- App Vorstellung
	- [Code for Leipzig](https://codefor.de/leipzig/))
	- 
- Was ist LoRa / LoRaWAN?
- Was ist TTN Leipzig?
- regenfass.eu
	- Problem
	- Komponenten
		- Stromversorgung
		- Sensoren
		- Boards
		<!-- Kosten -->
		<!-- Bauanleitung -->
	- Benutzerfreundlichkeit
	- Integration in die App
	- Demo
	- Konzept Challenge


---

### Konzept Challenge

1. Prototypenboard zeigen
2. Gateway zeigen
3. Netzabdeckung und die Reichweite
	1. Sateliten LoRaWAN
	2. Gateways
		1. https://ttnmapper.org/radar/gateway/?gateway=a8404120dc144150&network=NS_TTS_V3://ttn@000013
		2. MPI https://ttnmapper.org/radar/gateway/?gateway=mpi-eva-gw1&network=NS_TTS_V3://ttn@000013
4. Alternative Netze
	1. GSM
	2. LTE
	3. ZigBee
	4. Thread
	5. SigFox (Kommerzielles Netz)
	6. MeshTastic
	7. WLAN (Freifunk)

---
### Konzept Challenge

1. Prototypenboard zeigen
2. Gateway zeigen
3. Netzabdeckung und die Reichweite
	1. Sateliten LoRaWAN
	2. Gateways
4. Alternative Netze
	1. GSM
	2. LTE
	3. ZigBee
	4. Thread
	5. SigFox (Kommerzielles Netz)
	6. MeshTastic
	7. WLAN (Freifunk)

---

## Bauanleitung

- Bauanleitung
	- Anforderungen
- Installation der Software
- Update der Software
- 


---


- Sensoren
	- [Hydrostatischer Druck](https://de.aliexpress.com/w/wholesale-sensor-hydrostatic-.html?spm=a2g0o.detail.search.0)
	- Ultraschall

---

---
## Regenfass

```chart
type: line
height: 400
labels: [Jan,Feb,Mrz, Apr, Mai, Jun, Jul, Aug, Sept, Otk,Nov,Dez ]
series:
  - title: Füllmenge
	data: [0,0,0,77,91,80,60,12,100,70,60,0,0]
```


## Ziel des Projekts

Überwachung des Wasserstands in einem Regenfass mittels LoRaWAN.

---
## Ziel bei *Leipzig gießt*

Effizientes Wassermanagement in den Wasser-Containern

---
## Komponenten

1) Ultraschallsensor zur Messung des Wasserstands.
2) Mikrocontroller mit LoRa-Modul
3) Stromversorgung über Batterie mit Solarzelle.

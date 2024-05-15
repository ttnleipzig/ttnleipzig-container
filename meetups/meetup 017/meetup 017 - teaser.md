
1. Web: Konfiguration über die Weboberfläche
2. Web: Daten codieren und senden
3. Controller: Decoding und Speicherung
4. Controller: Lesen und verwenden

---

## Bastelrunde 017

Über den universellen seriellen Anschluss kann man mit der Serial Web API Daten von einem Browser zu einem Microcontroller übertragen. Diesen Umstand können wir nutzen, um  

1. in einem Webformular Daten einzugeben, 
2. sie zu kodieren, 
3. sie über die API zu versenden,
4. auf dem Microcontroller zu dekodieren,
5. und zu verwenden.

Für das Kodieren und Dekodieren ist es notwendig, das wir uns Regeln definieren, wie diese Daten strukturiert sein sollen. Wir definieren unser eigenes Protokoll. Auf der Seite des Mikrocontrollers dekodieren wir die Daten, speichern sie im lokalen Dateisystem und verwenden sie anschließend im Programmablauf.

**#meetup** **#lora** **#leipzig**

---
### Meetup
In diesem Meetup schauen wir uns speziell die ersten vier Schritte genauer an. 

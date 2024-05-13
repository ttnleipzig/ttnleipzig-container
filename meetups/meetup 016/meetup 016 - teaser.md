
1. Web: Konfiguration über die Weboberfläche
2. Web: Daten codieren und senden
3. Controller: Decoding und Speicherung
4. Controller: Lesen und verwenden

---

Über den universellen seriellen Anschluss kann man mit der Web API  Daten von einem Browser zu einem Microcontroller übertragen. Diesen Umstand können wir nutzen, um  
1. in einem Webformular die Daten einzugeben, 
2. sie zu kodieren 
3. sie über die API zu verwenden
4. auf dem Microcontroller zu decodieren
5. und zu verwenden.

Für das Kodieren und Decodieren ist es notwendig, sich Regeln zu definieren wie diese Daten strukturiert sein sollen. Wir definieren unser eigenes Protokoll. Auf der Seite des Microcontrollers dekodieren wir die Daten, speichern sie im lokalen Dateisystem und verwenden sie anschließend im Programmablauf.

---
### Meetup
In diesem Meetup schauen wir uns speziell die ersten vier Schritte genauer an. 

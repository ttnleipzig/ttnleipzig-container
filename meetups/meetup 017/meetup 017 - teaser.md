
1. Controller: Decoding und Speicherung
2. Controller: Lesen und verwenden

---

## Bastelrunde 017 - Mit dem eigenem Protokoll arbeiten

Wir haben unser eigenes Protokoll definiert. Nun gilt es mit dem Mikrocontroller die codierten Daten über den Serial Port zu empfangen und damit zu arbeiten. Für unsere Konfigurationsdaten heißt dies konkret, dass wir die Daten speichern und im Programmablauf zu verwenden. Im nächsten Schritt werden wir dann vom Mikrocontroller wieder über die serielle Schnittstelle Statusmeldungen an den Browser senden, um dort über den Erfolg, oder Misserfolg der Operation zu informieren. Auch soll es möglich sein, die aktuelle Programmversion abzufragen, die auf dem Mikrocontroller installiert ist.

Wie immer beim #LoRaWAN #Meetup #Leipzig nehmen wir uns die Zeit um tiefer in die Materie einzusteigen, um ein genaues Verständnis von den Vorgängen zu erlangen.

**#meetup** **#lora** **#leipzig**


---

Wenn Du möchtest, dass sich ein Browser und ein Microcontroller unterhalten, dann müssen sie die gleiche Sprache sprechen um sich zu verstehen. Die Web Serial API des Browser ermöglicht Dir generell einen Kommunkationskanal zu öffnen, doch ist damit nicht geregelt wie die Unterhaltung ablaufen kann und soll. Hier musst Du selbst aktiv werden und Dir überlegen wie Du die Daten Strukturierst, damit sie die Gegenstelle entziffern kann.
Für unser Projekt Regenfass haben wir uns ein spezielles Format überlegt, damit wir die Konfigurationdaten die wir im Browser eingegeben haben, im Microcontroller auch speichern und im Programmablauf verwenden können.

Die Kommunikation über die Serielle Schnittstelle ist keine Einbahnstraße. Du kannst auch Daten vom Mikrocontroller an deinen Browser schicken. Inhalte können hier z.B. Statusmeldungen, Softwareversionsnummer, oder auch Sensordaten sein.
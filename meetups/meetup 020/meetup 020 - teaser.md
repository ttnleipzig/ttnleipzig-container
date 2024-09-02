
## #020 Bastelrunde - Ein eigener Web Serial Flasher

Bisher verwendeten wir *ESP Web Tools* zum Flashen unserer Anwendung auf die Microcontroller.. Leider sind wir dabei an Grenzen gestoßen, die die Bedienbarkeit negativ beeinflussten. Zum Beispiel war es notwendig den Browser neu zu starten, wenn man nach dem Flashen gleich Konfigurationen vornehmen wollte. Daher ist es Zeit etwas tiefer in die Materie einzusteigen und weiter unten im Prozess einzusteigen. Wir bauen uns einen eigenen Flasher für die WebSerial API!
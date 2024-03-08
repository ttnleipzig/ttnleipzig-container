## Platforms Teaser

Die Web Serial API eröffnet direkte Kommunikationswege zwischen Webanwendungen und seriellen Geräten. Im kommenden Meetup zeigen wir dir, wie du mit einfachem JavaScript Code eine Verbindung zu Geräten wie einem Arduino herstellen kannst. Dies ermöglicht vielfältige Interaktionen ohne den Umweg über zusätzliche Software. Perfekt für Hobbyprojekte, Bildung oder Prototyping. Wir werden die experimentieren und die Web Serial API selbst verwenden, um mit unserem Mikrocontroller zu kommunizieren.

Hier geht es schon mal zu einer Demo:
[Web Serial Example (ttnleipzig.github.io)](https://ttnleipzig.github.io/experimental-serial-web-api/)

Nächsten Dienstag sprechen wir über die Web Serial API direkt über den Browser, mit unserem Mikrocontroller. Warum? So schaffen wir die Möglichkeit unseren IOT Code auf einfache Art **kon­fi­gu­rier­bar** zu machen. Hier gehts zu einer Demo: https://ttnleipzig.github.io/experimental-serial-web-api/

**#leipzig** **#meetup** **#iot**


## Youtube Short

Kernpunkte der Web Serial API hervorhebt und wie sie für die Kommunikation zwischen Webanwendungen und seriellen Geräten verwendet werden kann. Hier ist ein Beispiel-Skript für einen YouTube Short:

---
## Skript

[Einleitung: 0-5 Sekunden]
Text auf Bildschirm: "Web Serial API in 60 Sekunden!"

[Erklärung der API: 5-20 Sekunden]
Sprecher (Voice-over): "Die Web Serial API ermöglicht es Websites, mit seriellen Geräten zu kommunizieren – direkt im Browser."

[Anwendungsfälle: 20-35 Sekunden]
Sprecher (Voice-over) mit passenden Grafiken oder Clips von Geräten: "Das bedeutet, du kannst auf alles von Arduino-Boards bis hin zu 3D-Druckern zugreifen, ohne eine einzige Zeile Desktop-Software schreiben zu müssen."

[Demo-Szene: 35-50 Sekunden]
Zeigt einen kurzen Clip einer Code-Demo mit Kommentar.
Sprecher (Voice-over): "Ein paar Zeilen JavaScript ermöglichen das Lesen und Schreiben von Daten auf deinem Mikrocontroller"

[Abschluss und Call-to-Action: 50-60 Sekunden]
Bei unserem Meetup implementieren wir die Kommunikation zwischen dem Browser und dem Mikrochip anhand eines Beispielprojektes. Unser Projekt regenfass.

---



**Text für den YouTube Short (für Beschreibung/Untertitel):**

"Entdecke die Möglichkeiten der Web Serial API in nur einer Minute! Lerne, wie du direkt aus dem Browser heraus mit seriellen Geräten wie Arduino oder einem 3D-Drucker interagieren kannst. Keine zusätzliche Software erforderlich – nur reines JavaScript. Abonniere jetzt für mehr Tutorials und Tipps!"

Bitte beachte, dass das tatsächliche Erstellen eines solchen Videos auch Grafiken, Animationen oder Live-Demos beinhalten würde, um den Zuschauer visuell zu engagieren. Zudem müssten alle gezeigten Codebeispiele klar und einfach sein, um innerhalb des kurzen Formats verständlich zu bleiben.

---
## Skript 2

**Beschreibung für YouTube Short:**

"Die Web Serial API eröffnet direkte Kommunikationswege zwischen Webanwendungen und seriellen Geräten. In diesem Short zeigen wir dir, wie du mit einfachem JavaScript Code eine Verbindung zu Geräten wie einem Arduino herstellen kannst. Dies ermöglicht vielfältige Interaktionen ohne den Umweg über zusätzliche Software. Perfekt für Hobbyprojekte, Bildung oder Prototyping. Verpasse keine weiteren Tutorials – abonniere unseren Kanal!"

**Beispiel-Skript für YouTube Short:**

(Start des Videos)
"Hey Macher und Entwickler! In 60 Sekunden zeige ich dir die Kraft der Web Serial API!"

(Bild von einem Arduino und einem 3D-Drucker)
"Mit dieser API kannst du direkt aus deinem Browser heraus mit Geräten wie diesen kommunizieren."

(Einblendung von JavaScript Code)
"Alles was du brauchst, ist ein paar Zeilen JavaScript. Hier ist ein einfacher Befehl zum Öffnen einer seriellen Verbindung."

(Code wird gezeigt)
"`navigator.serial.requestPort().then(...);`"

(Bild einer erfolgreichen Verbindung)
"Sobald die Verbindung steht, kannst du Daten senden und empfangen – in Echtzeit!"

(Aufruf zum Abonnieren)
"Bist du bereit mehr zu lernen? Dann abonniere für detaillierte Tutorials und werde Teil unserer Community!"

(Ende des Videos)

---
# Custom Texte

 Um Konfiguration wie zum Beispiel Zugangsdaten für ein Netzwerk auf ein IoT Device zu bringen, gibt drei wesentliche Möglichkeiten
 1. WiFi Access Point
 2. Konfigration bei Flash mitgeben
 3. Bluetooth oder eine Serielle Schnittstelle

Bei unserem LoRaWAN Meetup schauen wir uns diesmal die Variante mitder Seriellen Schnittstelle an. Dank der Web Serial API ist es möglich, einen Mikrokontroller über eine Webanwendung zu konfigurieren.

### Skript Cridgyyyyyy

 Titel: "Wie man IoT-Geräte über USB konfiguriert!"

[Einblendung: LoRaWAN Meetup Logo]

[Clip: Ein IoT-Gerät wird an einen Computer angeschlossen]

Sprecher:
"Hey IoT-Enthusiasten! Heute zeigen wir euch, wie ihr euer IoT-Device mittels Serieller Schnittstelle und der Web Serial API konfiguriert. Perfekt für unser nächstes LoRaWAN Meetup!"

[Clip: Browserfenster öffnet sich mit einer Webanwendung auf dem Bildschirm]

Sprecher:
"Öffnet eure Webanwendung, die die Web Serial API unterstützt. Keine zusätzliche Software nötig – alles passiert direkt im Browser!"

[Clip: Benutzer klickt auf einen "Verbinden"-Button in der Webanwendung]

Sprecher:
"Klickt auf 'Verbinden' und wählt euer Gerät aus der Liste aus. So einfach ist das!"

[Clip: Daten werden über die Schnittstelle übertragen]

Sprecher:
"Gebt jetzt eure Konfigurationsdaten ein – wie Netzwerkzugangsdaten oder andere Einstellungen."

[Clip: Fortschrittsbalken zeigt den Übertragungsstatus an]

Sprecher:
"Mit einem Klick sendet ihr die Daten direkt an euer IoT-Device. Die Serielle Schnittstelle sorgt für eine sichere und zuverlässige Übertragung."

[Clip: Leuchtende LED am IoT-Gerät signalisiert erfolgreiche Konfiguration]

Sprecher:
"Und voilà! Euer Device ist konfiguriert und einsatzbereit für das Netzwerk."

[Eingeblendetes Textfeld: "Mehr erfahren? Besucht unser LoRaWAN Meetup!"]

Sprecher:
"Ihr wollt mehr lernen und austauschen? Dann kommt zu unserem nächsten LoRaWAN Meetup. Wir freuen uns auf euch!"

[Ende des Clips mit Kontaktinformationen und einem Aufruf zum Abonnieren des Kanals]

Sprecher (Outro):
"Vergesst nicht zu liken, zu teilen und unseren Kanal zu abonnieren für weitere coole IoT-Tipps. Bis zum nächsten Mal!"

### Skript seriös

[Start des Videos, ein kurzes Intro-Clip zeigt das Logo des Kanals]

Moderator (spricht in die Kamera):
"Herzlich willkommen, liebe Tech-Enthusiasten! Heute tauchen wir in die faszinierende Welt der IoT-Geräte ein und zeigen euch, wie man ein Gerät mit Hilfe einer seriellen Schnittstelle konfigurieren kann – unkompliziert direkt über euren Webbrowser!"

[Wechsel zu Bildschirmaufnahmen mit Demonstration]

Moderator (Voiceover):
"Dank moderner Technologien wie der Web Serial API ist es möglich, Mikrocontroller ohne komplizierte Software oder spezielle Hardware zu konfigurieren. Alles, was ihr benötigt, ist ein kompatibler Browser und natürlich euer IoT-Gerät."

[Bilder von einem IoT Device und einem Computerbildschirm]

Moderator (Voiceover):
"Beginnen wir damit, unser Gerät über ein USB-Kabel mit dem Computer zu verbinden. Stellt sicher, dass euer Browser die Web Serial API unterstützt – Google Chrome zum Beispiel ist dafür bestens geeignet."

[Einblendung: "Schritt 1: Verbindung herstellen"]

Moderator (Voiceover):
"Sobald die Verbindung steht, öffnet ihr eine Webanwendung, die für die Kommunikation mit der seriellen Schnittstelle ausgelegt ist. Mit nur wenigen Klicks könnt ihr dann auf das IoT-Gerät zugreifen."

[Einblendung: "Schritt 2: Webanwendung öffnen"]

Moderator (Voiceover):
"In unserer Webanwendung wählt ihr den entsprechenden Port aus und stellt eine sichere Verbindung her. Jetzt seid ihr bereit für die Konfiguration!"

[Einblendung: "Schritt 3: Port auswählen und verbinden"]

Moderator (Voiceover):
"Ob Netzwerkeinstellungen, Zugangsdaten oder andere Parameter – all dies könnt ihr nun direkt über das Interface der Webanwendung anpassen. Die Änderungen werden in Echtzeit auf das IoT-Gerät übertragen."

[Einblendung: "Schritt 4: Konfiguration vornehmen"]

Moderator (Voiceover):
"Und genau so einfach war's! Ihr habt erfolgreich euer IoT Device mittels serieller Schnittstelle konfiguriert. Keine Sorgen mehr um fehlende Treiber oder spezielle Software."

[Zurück zum Moderator]

Moderator:
"Ich hoffe, dieses Tutorial war hilfreich für euch! Wenn ihr mehr solcher Inhalte sehen wollt, vergesst nicht unseren Kanal zu abonnieren und klickt auf die Glocke für Benachrichtigungen über neue Videos."

[Eine Animation zeigt den Abonnieren-Button und die Benachrichtigungsglocke]

Moderator:
"Bis zum nächsten Mal bei unserem LoRaWAN Meetup – bleibt neugierig und experimentierfreudig!"

[Ende des Videos mit Abspann und Verlinkungen zu weiterführenden Inhalten]
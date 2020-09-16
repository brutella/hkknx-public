# hkknx-public
In diesem Repository werden [Releases](https://github.com/brutella/hkknx-public/releases) von `hkknx` veröffentlicht, und über [Issues](https://github.com/brutella/hkknx-public/issues) diskutiert.

- 2020-05-18: Version 1.0 veröffentlicht
- 2020-01-24: Öffentliche Beta hat begonnen.

**Was ist hkknx?**

`hkknx` ist eine HomeKit KNX Brücke um KNX Geräte über HomeKit zu steuern. Dabei wird eine direkte IP Verbindung zu einem KNX IP-Gateway aufgebaut. `knxd` wird nicht benötigt.

`hkknx` ist als Binärdatei für die verschiedenste Platformen und Betriebssystemen (macOS, linux) verfügbar.

**Was ist HomeKit?**

HomeKit ist ein Protokoll entwickelt von Apple und wird in verschiedenen Smart Home Geräten unterstützt.
Privatsphäre und Verschlüsselung sind voll in dem Standard integriert.
Geräte die HomeKit unterstützen können komfortable mit Apple Geräten (iPhone, iPad, Apple Watch, Mac) gesteuert werden.

**Warum möchte ich KNX über HomeKit steuern?**

Die Steuerung von KNX Geräten über HomeKit ist deshalb so interessant, weil HomeKit so gut in das Apple Ecosystem integriert ist.

Hier ein paar Vorteile.

- Die Apple Home App ist auf allen iOS, watchOS und macOS Geräten bereits vorinstalliert. Die Benutzeroberfläche von der App ist einfach und für jedermal verständlich.
- Siri unterstützt HomeKit Befehle, zB Hey Siri, Licht im Schlafzimmer ausschalten. Das heißt man bekommt eine Sprachsteuerung gratis dazu.
- Verschlüsselter Internetzugriff auf die KNX Geräte über eine Steuerzentrale (Apple TV, HomeHub oder iPad).
- Ein iPad kann als KNX Visualisierung an der Wand dienen.
- Mit HomeKit kannst du anwesenheitsgesteuerte Automatisierungen erstellen.

**Was benötige ich um hkknx zu testen?**

Um `hkknx` verwenden zu können, benötigst du

- ein KNX IP-Gateway (KNXnet/IP Tunnelling muss unterstützt werden)
- einen Computer (zB Raspberry Pi), der Zugriff auf deine KNX Installation über das KNX IP-Gateway bekommt
- ein iOS Gerät um die KNX Brücke zu HomeKit hinzufügen zu können

Lade die aktuellste [Releaseversion](https://github.com/brutella/hkknx-public/releases) herunter.
Entpacke die Datei und lese die Anleitung in der INSTALLATION.md Datei durch.

**Ist hkknx kostenlos verfügbar?**

~~Während der Betaphase ist `hkknx` kostenlos verfügbar.
Womöglich wird es nach der Betaphase eine kostenpflichtige Version geben.~~

Die Betaphase ist seit 18. Mai 2020 beendet.

*Hinweis: Beta-Versionen sind 90 Tage ab Veröffentlichung gültig. Danach muss auf die aktuellste Version geupdated werden.*

**Benötigt hkknx eine Internetverbindung?**

Nein. `hkknx` hat eine eingebaute Weboberfläche zum Konfigurieren der KNX Brücke. Die Verbindung zu dem KNX IP-Gateway wird über dein lokales Netzwerk hergestellt.

(Zum Installieren von Updates wird jedoch eine Internetverbindung benötigt.)

**Muss Multicast im Netzwerk erlaubt sein?**

Ja. Damit die HomeKit Brücke eine Verbindung mit HomeKit aufbauen kann, muss Multicast (für [mDNS](https://en.wikipedia.org/wiki/Multicast_DNS)) im Netzwerk erlaubt sein. Verwendet werden dafür die Multicast Adressen `224.0.0.251` (IPv4) und `ff02::fb` (IPv6), sowie Port `5353`.

Multicast wird außerdem noch für die *Automatische Suche* des KNX IP Gateways benötigt. Dafür wird die Multicast Adresse `224.0.23.12` und Port 3671 verwendet.

**Welche Ports müssen offen sein?**

`hkknx` verwendet die Ports 5353 und 3671 für Multicast Anfragen. Falls nicht weiters in den Einstellungen konfiguriert, kommuniziert Brücke mit HomeKit auf einem zufälligen Port. Dieser Port kann aber in den Einstellungen festgelegt werden.

## Releases

Es stehen Packages für macOS, Linux and Raspberry Pi unter [Releases](https://github.com/brutella/hkknx-public/releases) zur Verfügung.

| Platform  | Package |
| ------------- | ------------- |
| Mac 64-bit  | hkknx-x.x.x_darwin_amd64  |
| Linux 64-bit  | hkknx-x.x.x_linux_amd64  |
| Linux 32-bit  | hkknx-x.x.x_linux_386  |
| Raspberry Pi 32-bit   | hkknx-x.x.x_linux_arm  |

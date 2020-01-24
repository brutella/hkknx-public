# hkknx-public
In diesem Repository werden [Releases](https://github.com/brutella/hkknx-public/releases) von `hkknx` veröffentlicht, und über [Issues](https://github.com/brutella/hkknx-public/issues) diskutiert.

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
- Ein "altes" iPad kann als KNX Visualisierung an der Wand dienen.
- Mit HomeKit kannst du anwesenheitsgesteuerte Automatisierungen erstellen.

**Was benötige ich um hkknx zu testen?**

Um `hkknx` verwenden zu können, benötigst du

- ein KNX IP-Gateway
- einen Computer (zB Raspberry Pi), der Zugriff auf deine KNX Installation über das KNX IP-Gateway bekommt
- ein iOS Gerät um die KNX Brücke zu HomeKit hinzufügen zu können

Lade die aktuellste [Releaseversion](https://github.com/brutella/hkknx-public/releases) herunter.
Entpacke die Datei und lese die Anleitung in der INSTALLATION.md Datei durch.

**Was kostet hkknx?**
`hkknx` ist zurzeit noch in der Betaphase und daher gratis verfügbar.
Womöglich wird es nach der Betaphase eine kostenpflichtige Version geben.

## Releases

Es stehen Packages für macOS, Linux and Raspberry Pi unter [Releases](https://github.com/brutella/hkknx-public/releases) zur Verfügung.

| Platform  | Package |
| ------------- | ------------- |
| Mac  | hkknx-x.x.x_darwin_amd64  |
| Linux  | hkknx-x.x.x_linux_amd64  |
| Raspberry Pi  | hkknx-x.x.x_linux_armhf  |

## 0.0.1
2020-01-24

First release

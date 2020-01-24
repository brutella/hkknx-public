# hkknx-public
In diesem (noch nicht öffentlichem) Repository werden **Releases** von `hkknx` veröffentlicht, und über **Issues** diskutiert.

**Was ist hkknx?**

`hkknx` ist eine HomeKit KNX Brücke um KNX Geräte über HomeKit zu steuern. `hkknx` ist als Binärdatei für die verschiedenste Platformen und Betriebssystemen (macOS, linux) verfügbar. Es muss nicht anderes installiert werden – `knxd` wird nicht benötigt.

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
- ein iOS Gerät um die KNX Brücke zu HomeKit hinzufügen zu können.

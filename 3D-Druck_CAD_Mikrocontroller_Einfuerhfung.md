<!--
author:   o0Ikami0o

comment:  Test für C-Code

language: de

narrator: Deutsch Female

mode:     Textbook

import: https://raw.githubusercontent.com/liascript/CodeRunner/master/README.md
        https://github.com/liascript/CodeRunner
        https://github.com/LiaTemplates/AVR8js/main/README.md#10


@run: @LIA.eval(`["main.c"]`, `gcc -Wall main.c -o a.out`, `./a.out`)

-->




# Einblick in 3D-Druck CAD und Mikrocontroller

---
**Allgemeines:**

Beim 3D-Druck handelt es sich um ein additives Fertigungsverfahren, das durch CAD-Kenntnisse (Computer Aided Design) um eine elektronische Komponente erweitert werden kann. Im Folgenden soll aufgezeigt werden, wie den Lernenden ein Einblick in diese Techniken gegeben werden kann. 

![Logo Tinkercad](https://upload.wikimedia.org/wikipedia/commons/4/4c/Logo-tinkercad-wordmark.svg)

[Quelle](https://en.wikipedia.org/wiki/Tinkercad#/media/File:Logo-tinkercad-wordmark.svg)

---

## Kurzinformation für die Lehrkraft

**Titel:** Einblick in 3D-Druck CAD und Controller

**Schulstufe:** Mittelstufe, Oberstufe

**optimale Jahrgagnsstufe:** ab der 8 Klasse

**Themenbereich:** Digital Fabrication, 3D-Druck, Elektronik

---


**Einordnung in Rahmenvorgaben Kerncurriculum Informatik:**


**Sekundabreich I:** Lernfeld "Automatisierte Prozesse" unter technischer Realisierung automatisierter Prozesse
**Sekundarbereich II:**  Lernfeld "Algorithmen und Datenstrukturen" unter Grundlagen der Algorithmik

---

**Material:**

**Erforderliche Materialien:** Endgerate Tabelts (Andriode, IOs) oder PC (Windows, MacOS, Linux) 

**fakultativ für bessere Lernergebnisse:** 3D-Drucker, Klassensatz Arduino Starter Kits

### Lehr- und Lernziel

----

**Lehrziel:** Den Lernenden einen Einblick in den Einsatz von 3D-Druck, CAD und Arduino geben.
Die Relevanz des Themas vermitteln. Die Lernenden können eine Verbindung zwischen den
drei Themen herstellen. Das Interesse der Lernenden an den Themen wecken. Weiterführende
Materialien zur Verfügung stellen, um bei Interesse eine Vertiefung des Themas zu ermöglichen.

----

**Lernziel:** Die Lernenden erhalten einen Einblick in die Themen 3D-Druck, CAD und Arduino, und
können einen Zusammenhang zwischen den drei Themen herstellen.


### Themenüberblick

Im Folgenden wird ein kurzer Überblick über die Themen gegeben

#### 3D-Druck

Mit dem 3D-Druck können Modelle, Prototypen und auch Endprodukte kostengünstig und schnell
hergestellt werden. Beim 3D-Druck handelt es sich um ein Fertigungsverfahren, das auf rech-
nerinternen Datenmodellen basiert. Dies ist auch unter der Bezeichnung Generative Fertigung
bekannt. Auch der Begriff der additiven Fertigung wird mit 3D-Druck in Verbindung gebracht. Beim
3D-Druck werden Bauteile aus festem oder flüssigem Material im Schichtbauverfahren hergestellt.
Grundlage für den 3D-Druck ist eine 3D-CAD-Datei. Dabei muss es sich um ein 3D-Volumenmodell
handeln, in dem die 3. Dimensionen (Höhe, Breite, Tiefe) definiert sind

#### CAD-Computer Aided Design

Für die Erstellung der 3D-Modelle wird ein 3D-Konstruktionsprogramm mit CAD-Funktionalität
verwendet. CAD ist die Abkürzung für Computer Aided Design (computerunterstützte Konstruktion).
Dabei wird empfohlen, parametrisch zu modellieren. Dies hat den Vorteil, dass mit Parametern
und Abhängigkeiten gearbeitet wird. Dadurch können Anpassungen erleichtert werden. 
Beispiele für solche Programme, die teilweise mit Einschränkungen frei verwendet werden
können, sind Fusion360, FreeCAD, Tinkercad. Wobei letzteres eher für den Einstieg gedacht ist
und bei komplexen Projekten an seine Grenzen stößt.

#### Mikrocontroller 

Im Bereich der Mikrocontroller bieten sich für den Bildungsbereich zwei Vertreter an: die Ardunino-
Plattform oder die ESP32-Entwicklungskits. Diese sind bereits auf einer Platine aufgebracht. Somit
muss keine eigene Platine mehr entwickelt oder ein teures Programmiergerät angeschafft werden.
Da beide mit einer UART Schnittstelle ausgestattet sind, können sie bequem über den USB-Port
betrieben werden. Außerdem verfügen sie über zahlreiche Anschlussmöglichkeiten: digitale Pins,
analoge Pins und PWM. Die ESP32-Derivate haben WLAN integriert. Dies macht sie besonders
für den Bereich Smart Home interessant. Als Software zur Programmierung kann der Einsteiger
die Ardunio IDE verwenden. Für Fortgeschrittene bietet sich Platform IO an, eine Erweiterung
zu VSCode. Von blinkenden LEDs bis hin zu intelligenten Robotern kann nahezu jedes Projekt
realisiert werden

#### Zusammenfassung Themenüberblick

Erst die Kombination dieser drei Techniken ermöglicht die Realisierung komplexer Projekte. Um
beim Beispiel des intelligenten Roboters zu bleiben. Dieser kann somit in CAD konstruiert werden.
Mittels 3D-Druck können die notwendigen Bauteile für das Roboter-Chassis hergestellt werden.
Mit dem Arduino oder dem ESP-32 in Kombination mit Aktoren und Sensoren kann dem Roboter
Leben eingehaucht werden. Auch in Industrie 4.0 finden sich diese drei Technologien wieder.

## Ablauf

 **exemplarischer Ablauf:**

In der fiktiven Planung beginnt der Unterricht um 8.00 Uhr und wird in Doppelstunden erteilt.

| Zeit     | Phase    | Inhalt/Methode| Sozialform | Medien |
|----------|----------|----------|----------|----------|
| 8:00 - 8:05 | Einstieg ins Thema   | Präsentation von 3D-gedruckten Modellen, Befragung der Lernenden, welches Thema heute Gegenstand des Unterrichts ist, den Lernenden durch im Raum aufgebaute Materialien (3D-Drucker, Filament) Hinweise geben  | Unterrichtsgespräch | Modelle   |
| 8:05 - 8:35  | Erarbeitung/Sicherung 3D-Drucker | Bearbeitung von Materialien H5P, die auf einem eigenen Arbeitsblatt festgehalten werden. Nachfolgende Erklärung am Modell  | Einzelarbeit/ Partnerarbeit   | H5P, Arbeitsblatt  |
| 8:35 - 9:00  | Erarbeitung/ Sicherung Slicer  | Suche 3D-Modelle Website, Dateien sind im STL-Format in G-Code zu konvertieren. Lernenden sollen erkennen, dass es nicht funktioniert ohne konvertierung (Vorführung), Einführung G-Code und Erklärung Slicer  | Einzelarbeit/ Partnerarbeit  | H5P, Arbeitsblatt  |
| 9:00 - 9:25|  Erarbeitung/ Sicherung CAD| Herleitung über Namensanhänger, dass dieser nicht zum Download zur Verfügung steht, selbst erstellt CAD (kurze Zusammenfassung CAD), Eigene [Schlüsselanhänger](https://www.tinkercad.com/projects/Name-That-Keychain-1) mit Namen anfertigen (o.ä.) Eigene Schlüsselanhänger mit Namen anfertigen (o.ä.) Zeit: 25 Minuten weiter 25 Minuten in folge Stunde | Einzelarbeit/ Partnerarbeit/ Gruppenarbeit  | Tinkercad |
| 9:25 - 9:30 | Abschluss   | Kurze Zusammenfassung (3D-Druckeraufbau, Slicer, Name in CAD), Ausblick Nächste Stunde: 5 Minuten Einarbeitungszeit, 20 Minuten für die Herstellung des Namenanhängers, größere Projekte gerne zu Hause. | Lehrervortrag  |   |

----

Die nächste Doppelstunde in der fiktiven Planung beginnt wieder um 8:00 Uhr.

| Zeit     | Phase    | Inhalt/Methode| Sozialform | Medien |
|----------|----------|----------|----------|----------|
| 8:00 - 8:05 | Einstieg   | Kurzer Rückblick auf die vergangene Stunde, Ausblick auf die Arbeit des Tages | Lehrervortrag |    |
| 8:05 - 8:30  | Erarbeitung/ Sicherung CAD|  Einarbeitung und Fertigstellung des Anhängers    |  Einzelarbeit/ Partnerarbeit/ Gruppenarbeit | Tinkercad |
| 8:30 - 9:00  | Erarbeitung/ Sicherung Slicer  | Tinkercad-Modell exportieren 3D-Druck vorbereiten mitels Slicer **!Hinweis!:** Kontrolle der Druckparameter zwingend erforderlich für den Druckerfolg | Einzelarbeit | Tinkercad, Slicer  |
| 9:00 - 9:25|  Erarbeitung | Vorführung eines interaktiven gestalteten Modells mit Hilfe eines Mikrokontrollers, Präsentation Microcontroller, Liascript, Einblick in die Programmierung,  | Lehrervortrag  | Modell, Liaskript|
| 9:25 - 9:30 | Abschluss   | Kurze Zusammenfassung (CAD, slicen), Ausblick Nächste Stunde: Verteilung des Namensanhängers/ andere Modelle | Lehrervortrag  |   |

----

## Material


**H5P Beschreibung der Bauteile**

<iframe src="https://einstiegh5p.de/h5p/embed/44690" width="615" height="561" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *" title="Beschreibung der Bauteile"></iframe><script src="https://einstiegh5p.de/sites/all/modules/h5p/library/js/h5p-resizer.js" charset="UTF-8"></script>

**H5P-Aufbau 3D-Drucker**

<iframe src="https://einstiegh5p.de/h5p/embed/44689" width="615" height="685" frameborder="0" allowfullscreen="allowfullscreen" allow="geolocation *; microphone *; camera *; midi *; encrypted-media *" title="Bauteile 3D-Drucker"></iframe><script src="https://einstiegh5p.de/sites/all/modules/h5p/library/js/h5p-resizer.js" charset="UTF-8"></script>



**Blinkende LED mit Arduino**

Im folgeden ein klienes Beispiel zu einen blinkenden LED.

**Aufbau**

![Alt text](https://raw.githubusercontent.com/o0Ikami0o/3D-Druck_CAD_Mikrocontroller_Einfuerhfung/main/image.png?token=GHSAT0AAAAAACJDOX23XNILE34XWCELPS2EZJRBD2A)

**Programmierung**

<div>
<wokwi-led color="red" pin="13" port="B"></wokwi-led>
</div>

```cpp Arduino LED
void setup() {
  pinMode(LED_BUILTIN, OUTPUT);
}

void loop() {
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000);
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000);
}
```
@AVR8js.sketch
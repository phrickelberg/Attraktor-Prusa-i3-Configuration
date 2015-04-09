Attraktor Prusa i3 Configuration
================================

Hier findet ihr alle Konfigurationsdaten zum Betrieb des Prusa i3 Einstein Rework im Attraktor. Das ganze funktioniert so:

<h2>1. Installation und Einrichtung</h2>
* [Slic3r](http://slic3r.org) installieren (Mac, Windows, Linux)
* alternativ zu Slic3r könnt ihr auch [Cura](http://software.ultimaker.com) (Mac, Windows, Linux) verwenden
* Optional, nicht unbedingt erforderlich, könnt ihr noch [Repetier](http://www.repetier.com) installieren (Mac, Windows, Linux)
* Die config-bundle.ini hier aus dem Repo-Verzeichnis "Slic3r" downloaden und per "Import Config Bundle" in Slic3r importieren

<h2>2. Slicen..</h2>

<h3>..mit Slic3r</h3>
* Falls erforderlich, unter "Preferences" den "Expert Mode" aktivieren
* Im Plater-Tab für "Print Settings" die Einstellung "E3D 0.4 Standard" auswählen
* Im Plater-Tab für "Filament" die Einstellung "ABS 1.75" oder "PLA 1.75" auswählen (je nachdem, welches Material in den Drucker eingelegt ist)
* Im Plater-Tab für "Printer" die Einstellung "E3Dv6 0.4 Attraktor" auswählen
* Die zu druckende(n) *.STL Datei(en) in den Plater laden
* Auf "Export G-code" klicken und die *.gcode Datei z.B. auf den Desktop abspeichern
* Die *.gcode Datei auf die SD-Karte kopieren

<h3>..mit Cura</h3>
* Beim ersten Start den Drucker einrichten, dazu die Werte aus dem Screenshot "Cura/Machine Settings.png" hier im Repo übernehmen
* Druckprofil "Cura-Settings-Standard.ini" aus dem Repo über "File -> Open Profile" laden
* Die zu druckende(n) *.STL Datei(en) über den "Load" Button laden
* Nachdem Cura fertig ist mit Slicen über "File -> Save G-code" die *.gcode Datei z.B. auf den Desktop abspeichern
* Die *.gcode Datei auf die SD-Karte kopieren

<h2>3. Drucken</h2>
* Drucker am ATX-Netzteil einschalten, der Schalter befindet sich hinten über der Kaltgerätebuchse
* Am Drucker ist ein Display-Controller mit SD-Kartenleser, mit dem Dreh-und-Druckknopf könnt ihr diesen bedienen
* Unter dem Dreh-Druckknopf befindet sich der etwas kleinere Not-Aus-Knopf, diesen bitte bei Bedarf benutzen. Danach muss der Drucker komplett am Netzteil abgeschaltet werden. Dann Netzeil abschalten, warten bis das Display ausgeht, und wieder anschalten. Leider funktioniert der Not-Aus Knopf nicht während der Homing-Prozedur, d.h. hier müsst ihr gleich schnell das Netzteil abschalten.
* Ein Klick auf den Dreh-Druckknopf bringt euch ins Hauptmenü
* Die SD-Karte am Rechner auswerfen und in den Smart-Controller am Drucker stecken
* Das Heizbett vorheizen (Am Smart-Controller der Menüpunkt "Prepare->Preheat ABS/PLA Bed")
* Warten, bis das Heizbett die Betriebstemperatur erreicht hat (auf dem Display gucken), das kann schon mal 20min dauern!
* Während des Aufheizens kann man ein Stück Pappe oder Holz auf das Heizbett legen, um das Aufheizen zu beschleunigen
* Den Extruder vorheizen (Am Smart-Controller der Menüpunkt "Prepare->Preheat ABS/PLA 1")
* Warten, bis der Extruder die Betriebstemperatur erreicht hat (auf dem Display gucken), das dauert nur wenige Minuten!
* Falls schon gedruckt wurde und der Extruder Motor noch "stall" ist (= sich nicht bewegen lässt), im Menü unter "Prepare->Disable Motors" die Motoren abschalten
* Wenn die Motoren ausgeschaltet sind am großen Zahnrad gegen den Uhrzeigersinn drehen bis etwas Kunststoff aus der Düse kommt
* Kunstoff von der Düse entfernen
* Am Smart-Controller unter "Print from SD" die zu druckende *.gcode Datei auswählen
* Der Druckvorgang startet
* Das Auto Bed Leveling wird ausgeführt
* Die erste Druckschicht am besten noch beobachten, danach Druckvorgang gelegentlich überprüfen
* Ist der Drucker fertig, fährt er in eine Ruheposition und schaltet Heizbett, Extruder und Motoren ab
* Um den Druck von der PEI-Platte zu bekommen, muss diese aber auf 110° aufgeheizt sein. Also ggf. nochmal über Prepare -> Preheat ABS -> Preheat ABS Bed aufheizen. Dann kann man den Druck vorsichtig mit einer Teppichmesser-Klinge von Heizbett entfernen.

Slic3r
-------------------------
Drucker und Filamentkonfigurationen für Slic3r sowie gute Druckeinstellungen. Die Konfigurationen sind so angelegt, dass ihr zwischen Slic3r und Cura wechseln könnt, ohne Einstellungen am Drucker zu verändern (z.B. E_STEPS)

Cura
-------------------------
Drucker und Filamentkonfigurationen für Cura sowie gute Druckeinstellungen. Die Konfiguration sind so angelegt, dass ihr zwischen Slic3r und Cura wechseln könnt, ohne Einstellungen am Drucker zu verändern (z.B. E_STEPS)

Repetier
-------------------------
Im Verzeichnis "Repetier" findet ihr Screenshots der richtigen Einstellungen für die Repetier Host Software.

Marlin
-------------------------
Im Verzeichnis "Marlin" findet ihr die Konfigurationsdatei der Marlin Firmware des Druckers.


Quellen
-------------------------
* Slic3r [slic3r.org](http://slic3r.org)
* Cura [ultimaker.com](http://software.ultimaker.com)
* Repetier [repetier.com](http://www.repetier.com)
* Marlin [github.com](https://github.com/ErikZalm/Marlin)

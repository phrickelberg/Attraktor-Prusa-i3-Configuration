Attraktor Prusa i3 Configuration
================================

Hier findet ihr alle Konfigurationsdaten zum Betrieb des Prusa i3 Einstein Rework im Attraktor. Das ganze funktioniert so:

<h2>1. Installation und Einrichtung</h2>
* [Slic3r](http://slic3r.org) installieren (Mac, Windows, Linux)
* alternativ zu Slic3r könnt ihr auch [Cura](http://software.ultimaker.com) (Mac, Windows, Linux) verwenden
* Optional, nicht unbedingt erforderlich, könnt ihr noch [Repetier](http://www.repetier.com) installieren (Mac, Windows, Linux)
* Die config-bundle.ini hier aus dem Repo-Verzeichnis "Slic3r" downloaden und per "Import Config Bundle" in Slic3r importieren

<<<<<<< HEAD
<h2>2. Slicen..</h2>
<h3>..mit Slic3r</h3>
* Im Plater-Tab für "Print Settings" die Einstellung "Attraktor" auswählen
* Im Plater-Tab für "Filament" die Einstellung "Attraktor ABS" oder "Attraktor PLA" auswählen (je nachdem, welches Material in den Drucker eingelegt ist)
* Im Plater-Tab für "Printer" die Einstellung "Attraktor" auswählen
=======
<h2>2. Slicen</h2>
* Im Plater-Tab für "Print Settings" die Einstellung "E3D 0.4 Standard" auswählen
* Im Plater-Tab für "Filament" die Einstellung "ABS 1.75" oder "PLA 1.75" auswählen (je nachdem, welches Material in den Drucker eingelegt ist)
* Im Plater-Tab für "Printer" die Einstellung "E3Dv6 0.4" auswählen
>>>>>>> FETCH_HEAD
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
* Die SD-Karte auswerfen und in den Smart-Controller am Drucker stecken
* Den Drucker vorheizen (Am Smart-Controller der Menüpunkt "Prepare->Preheat ABS/PLA")
* Warten, bis der Drucker die Betriebstemperatur erreicht hat (auf dem Display gucken)
* Falls schon gedruckt wurde und der Extruder Motor noch "stall" ist, im Menü unter "Prepare->Disable Motors" die Motoren abschalten
* Wenn der Drucker ausgeschaltet ist am großen Zahnrad im Uhrzeigersinn drehen bis etwas Kunststoff aus der Düse kommt
* Kunstoff von der Düse entfernen
* Am Smart-Controller unter "Print from SD" die zu druckende *.gcode Datei auswählen
* Der Druckvorgang startet
* Während der Drucker den Skirt druckt, kann an den Wellenverbindern der Z-Achse noch die Höhe leicht nachjustiert werden, bis die Kunstoffbahnen guten Bodenkontakt haben (immer gleich viele "Ticks" am rechten und am linken Motor!!!)
* Die erste Druckschicht am besten noch beobachten, danach Druckvorgang gelegentlich überprüfen

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
* Repetier [repetier.com](http://www.repetier.com)
* Marlin [github.com](https://github.com/ErikZalm/Marlin)

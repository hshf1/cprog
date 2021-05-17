# Aufgabe 12

## Teil 1

In einem Lager eines Automobilherstellers werden Fahrzeuge zwischengelagert.
Ein Lagerplatz wird beschrieben durch eine Struktur ```PLATZ_T```, die folgende Komponenten enthält:

- nr:  Seriennummer des KFZ, positive ganze achtstellige Zahl
- x:   x-Koordinate des Platzes, positive ganze Zahl zwischen 1 und 10
- y:   y-Koordinate des Platzes, positive ganze Zahl zwischen 1 und 10
- typ: ist wiederum eine Struktur vom Datentyp ```TYP_T```. In dieser Struktur ist:
  - Fahrzeug: Als Zeichenkette char* mit Fahrzeugtyp ("Kombi","Limousine","Cabrio")
  - KW:       Die Motorstärke als KW-Ganzzahl hinterlegt

Deklarieren Sie über ```typedef``` den Datentypen ```TYP_T```
Deklarieren Sie die Datenstruktur für ```PLATZ_T``` und definieren Sie ein Feld mit Namen ```lager``` mit 20 Einträgen von Typ ```PLATZ_T```.
Diese 20 Plätze sollen durch Änderung beliebig erweitert werden.
Initialisieren Sie in Ihrem Hauptprogramm die ersten 5 Einträge des Feldes ```lager``` mit beliebigen Werten (Fest oder Einlesen von der Tastatur).
Geben Sie in einer Schleife die Seriennummer und den Typ der ersten 5 Einträge am Bildschirm aus.


## Teil 2

Erstellen Sie nun ein Programm zur **dynamischen Lagerverwaltung'', mit dem Sie an beliebige Stellen Fahrzeuge einlagern und auslagern könne.
Gehen Sie hierzu folgendermaßen vor:

- Erstellen Sie ein neues _Hauptprogramm_. Initialisieren Sie alle Einträge Ihres Feldes ```lager``` mit folgenden _default_-Werten:
  -  nr = 0
  -  x und y = 0
  -  typ.Fahrzeug = "--"
  -  typ.KW = 0
  - (Mit diesen Werten werden freie Lagerplätze gekennzeichnet)
- Schreiben Sie eine Funktion ```ausgabe```, die den kompletten Lagerbestand ausgibt mit Seriennummer, Position und Fahrzeugtyp.
- Schreiben Sie eine Funktion ```einlagern```, die an der ersten freien Stelle Ihres Feldes ```lager``` die übergebenen Werte schreibt. Überprüfen Sie in Ihrer Funktion, ob der vorgegebene Lagerplatz frei oder bereits vergeben ist.
  - Erstellen Sie vor der Programmierung ein Struktogramm
- Schreiben Sie eine Funktion ```auslagern```, die ein Fahrzeug mit der angegebenen Seriennummer aus dem Feld entfernt, indem die Werte der Feldstruktur auf die ```default```-Werte zurückgesetzt werden.
- Schreiben Sie eine Funktion ```inventur```, die ermittelt, wie viele Fahrzeuge insgesamt und wie viele Kombis, Limousinen und Cabrios im Lager sind.

# Aufgabe 13

## Teil 1

Erstellen Sie ein Programm zur Erzeugung einer CSV-Datei in welcher 4 Wertereihen
(Winkel in Grad, Winkel in Bogenmaß, Sinuswert, Cosinuswert) abgespeichert werden.

Hinweis: Eine CSV Datei ist eine Textdatei mit Dateiendung CSV. In der ersten Dateizeile
werden die Überschriften (der Spalte) getrennt durch Semikolon geschrieben. Jede
Folgezeile enthält die Werte getrennt durch Semikolon.

Über eine Menüfunktion soll auswählbar sein, ob Sie eine CSV-Datei erstellen oder lesen
oder das Programm verlassen möchten.

- Erstellen Sie eine Unterfunktion ```int menue(void)``` in der Sie drei Menüeinträge
anbieten:
  - schreiben, lesen, abbrechen.
  - Vor Ausgabe der Menüpunkte löschen Sie den Bildschirm mit ```system("cls")```; (aus der stdlib.h)
- Über den Rückgabewert wählen Sie mittels ```switch() case```  dann die Funktionen
```void schreibeCSV(void)``` oder ```void leseCSV(void)``` aus.
- In der Funktion ```schreibeCSV``` fragen Sie zuerst die Schrittweite (Winkel in Grad) ab.
Dann öffnen Sie eine Textdatei (beliebiger Name mit Endung .csv) und schreiben die
Überschriften in die Datei. Die Überschriften werden in einer Zeile separiert mit ;
(Semikolon) geschrieben. Danach schreiben Sie in einer Schleife mit der eingegebenen
Schrittweite beginnend ab Winkel 0 bis 360° die o.g. 4 Werte je Zeile separiert mit ;
(Semikolon).

## Teil 2

- Lesen Sie in der Funktion ```leseCSV```  die Datei wieder ein zuerst die Überschrift (```char
Array[50]```) nutzen sie dafür ```fgets()``` und dann die Messwerte in ein
```Messwertarray[1000][4]``` (```scanf(%f;%f;…)```) Geben Sie die Werte ohne Semikolon
mit Tab und Feldweite 7 bei 3 Nachkommastellen auf dem Bildschirm aus. Lese Sie max.
100 Werte oder bis Sie EOF erhalten.
- Schreiben Sie eine Funktion
  - ```void ChangeString(char*Zeichenkette, char Suchzeichen, char Ersatzzeichen)```. Dieser Funktion wird ein String übergeben und alle Zeichen die
Suchzeichen entsprechen, werden durch Ersatzzeichen ersetzt.
- Übergeben Sie der Funktion ```ChangeString``` die eingelesene Überschrift und ersetzten Sie
';' durch '\t‚. Geben Sie die so erzeugte neue Überschrift anstelle der alten aus.
- Um die CSV Datei in Excel automatisch öffnen zu können, benötigt Excel (in der
Spracheinstellung Deutschland) als Dezimaltrenner das Komma anstatt den Punkt. Drucken
Sie die Messwerte zuerst in einen String mittels ```sprintf```. Dann ersetzten Sie im String alle
Punkte durch Kommata. Drucken Sie dann den String in die Datei.
- Beim Laden laden Sie zuerst die Messwerte in ein String ein, dann ersetzten sie alle
Kommata durch Punkte und lesen dann final die Messwerte aus dem String mittels sscanf
ein.

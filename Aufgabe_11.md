# Aufgabe 11

Ihr Programm soll analysieren, welche die ersten 5 Worte eines Satzes (max. 50 Zeichen inkl. Leerzeichen) sind.
Lösen Sie dazu die folgenden Teilaufgaben:

- Lesen Sie den Satz als Zeichenkette ein und legen Sie ihn in einer passenden Datenstruktur ab
- Legen Sie ein char*-Feld mit 5 Elementen mit dem Namen ````wortSpeicher```` an. Für jedes Feldelement reservieren Sie mit dem Befehl ```calloc``` Speicher für mindestens 20 Zeichen.
- Ermitteln Sie die ersten 5 Worte innerhalb der eingegebenen Zeichenkette und kopieren Sie jedes einzelne Wort in den Wortspeicher. 
  - Hinweis zur erlaubten Eingabe eines Satzes: Worte sind durch das Leerzeichen getrennt, der Satz endet immer mit einem "."
- Geben Sie jedes Wort des Wortspeichers auf dem Bildschirm aus, falls der Satz weniger als 5 Wörter hat.


## Info - calloc
<details>
  <summary>Klicken zum Öffnen</summary>
  
  calloc reserviert Speicherplatz in Ihrem Rechner, setzt den Inhalt, den calloc reserviert auf 0 und gibt einen Zeiger auf die erste Stelle des Speichers zurück. malloc reserviert Speicher und gibt einen Pointer auf die erste Stelle des Speichers zurück, ohne den Speicher vorher auf 0 zu setzten.
  
  Verwendung von calloc:
 - Vor dem Befehl sollte der Datentyp des Pointers stehen [(int*),(float*),...]
 - In dem Befehl stehen dann die Anzahl der Elemente und die Größe
    - calloc(5,4) -> Es werden fünf Adresse für den Datentyp int reserviert
    - calloc(5, sizeof(int)) -> Gleich zum anderen Beispiel 
  
  https://www.tutorialspoint.com/c_standard_library/c_function_calloc.htm
  
  </details>

# Zusatz 
<details>
  <summary>Klicken zum Öffnen</summary>
    
Erstellen Sie für Ihre Lösung ein Struktogramm.

</details>

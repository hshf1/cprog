# Aufgabe 9

Erstellen und testen Sie ein Programm, das für eine beliebige Ganzzahl die nächsthöhere gerade Zahl ausgibt. Falls die Zahl bereits gerade ist, ist die Zahl selbst auszugeben. 
Die Zahl ist durch den Benutzer einzugeben.

## Teil 1

  
  Erstellen Sie hierzu folgende Unterprogramme
  
  >void eingeben (int*)
  >
_erhält einen Zeiger auf eine Zahl und ermöglicht die Eingabe dieser Zahl durch die Tastatur._

>void korrigieren (int*)
>
_erhält einen Zeiger auf die vorher eingegeben Zahl und korrigiert diese, falls sie ungerade ist._

>void ausgeben (int*)
>
_erhält einen Zeiger auf die vorher eingegebene und korrigierte Zahl und gibt diese mit Wert und Adresse am Bildschirm aus._

Testen Sie Ihr Programm mit unterschiedlichen Testfällen.

### Zusatz
<details>
<summary>Click to expand</summary>
  
  Erstellen Sie das Struktogramm für Ihr Hauptprogramm und für die Unterfunktionen
  //kleiner Test für GitDesktop
  </details>

  
  ## Teil 2

  
  Erweitern Sie Ihr Programm um eine weitere Funktion, die überprüft, ob die eingegebene Zahl mindestens 5-stellig ist und diese bei Bedarf korrigiert.
  
  ````korrigieren2```` soll nach der Funktion aus Teil 1 aufgerufen werden.
  Füllen Sie dazu die fehlenden Stellen **rechts** neben der Zahl mit 0 auf.
  
  ``` void korrigieren2 (int*) :``` erhält einen Zeiger auf eine vorher eingegeben Zahl und erweitert diese bei Bedarf um 5 Stellen.
  Wandeln Sie die Zahl in einen Text ```sprintf()```.
  Ermitteln Sie mit ```strlen()``` die Anzahl der Stellen.
  Erweitern Sie mit ```strcat()``` den Text und wandeln Sie den String wieder in eine Zahl zurück(Je Zeichen über ASCII Tabelle oder per ````sscanf()````).
  
  Ändern Sie die Eingaberoutine so ab, dass der Anwender darauf hingewiesen wird, dass er keine _0_ eingeben darf.
  
  Testen Sie Ihre neue Funktion mit unterschiedlichen Tesfällen
  (z.B. -10001, -9999, -1, 1, 9999, 10001)
  
  ### Zusatz
<details>
<summary>Click to expand</summary>
  
  Erstellen Sie das Struktogramm für die Unterfunktionen ````korrigieren2````.
  </details>

  
   ## Teil 3

  
  Erstellen Sie eine Schleife, die die Eingaben, Ausgabe und die Korrekturen solange widerholt, bis die Zahl _0_ eingegeben wird. Weisen Sie den Anwender auf dieses Abbruchkriterium hin.
  Das Programm wird nach Eingabe dieser Zahlbeendet.
  
  ### Zusatz
<details>
<summary>Click to expand</summary>
  
  Erstellen Sie das Struktogramm Ihres so modifizierten Programms.
  </details>
 

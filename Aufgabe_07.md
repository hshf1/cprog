# Aufgabe 7


Sie suchen für Ihr Projekt einen Widerstand. Sie haben den Baukasten der E12 Reihe mit den Widerständen von 1 bis 10.000.
Leider ist kein Widerstand dabei, der nah genug an ihrem Wunschwert liegt. Sie möchten dem durch 2 parallel geschaltete Widerstände aus der E12 Reihe möglichst nahe kommen.  Entwickeln Sie ein Programm, das alle Kombinationen automatisch erstellt und das beste Widerstandspaar für Sie ermittelt und ausgibt.
Ihr Programm soll die folgenden Punkte erfüllen:  
  
  - [ ] Berechnen Sie die E12 Reihe bis 10.000 Ohm und geben Sie diese aus
  - [ ] Erstellen Sie eine Funktion zur Berechnung von Parallelwiderständen
    - [ ] Testen Sie Ihre Unterfunktion mit zwei Werten  
  - [ ] Berechnen Sie jede mögliche Kombination von zwei parallel geschalteten Widerständen der E12-Reihe
  - [ ] Speichern Sie die Kombination mit der kleinsten Differenz zum Wunschwiderstand
  - [ ] Geben Sie die gefundene Kombination von Widerständen aus
  - [ ] Ermitteln Sie die Abweichung in Ohm und Prozent und geben Sie diese aus
  
  
# Info E12
 
 Die E12-Reihe ist eine Widerstandsreihe, welche eine logarithmische Verteilung aufweist.
 Sie hat pro Dekade 12 Widerstandswerte, die sich von Dekade zu Dekade lediglich um den Faktor 10 unterscheiden.
 Wie sich die E12-Reihe berechnen lässt kann unter dem Wikipedia-Link nachgelesen werden
 
 Wiki:
 https://de.wikipedia.org/wiki/E-Reihe
 

  
## Tip - E12 Reihe

<details>
<summary>Click to expand</summary>

Die E12 Reihe sind Widerstände, die 12 Widerstände pro Dekade erhalten !
Geben Sie die E12-Reihe von 1 bis 10.000 an

Es kann die Funktion pow() mit 10 hoch x/12 verwendet werden.
pow() befindet sich in der math.h Bibliothek

 </details>
  
  ## Tip - Parallelschaltung
  
  <details>
  <summary>Click to expand</summary>
  
  Die Parallelschaltung kann durch 
  
  >R1*R2/(R1+R2)
  >
 
   realisiert werden.
  
  </details>

  
 ## Tip - Wiederstände berechnen
  
  <details>
  <summary>Click to expand</summary>

 Um alle Widerstandskombinationen zu brechnen kann eine doppelte for-Schleife verwendet werden 
  
  Beispiel:
  
  > int i=0;
  > int k=0;
  > int iZaehler1=0;aehler2=0;
  > 
  > // Doppelte for-Schleife mit den Schleifenvariablen i und k
  > 
  > for(i=0;i<4;i++){
  > 
  >   for(k=0;k<4;k++){
  >   
  >     iZaehler1++;
  >     
  >   }
  >   
  >   iZaehler2+=2;
  >   
  > }
  > 
  > 
Die erste For-Schleife ist die äußere Schleife mit Schleifenvariable i. In dieser ist eine zweite Schleife mit der Schleifenvariable k enthalten.
Zuerst wird die innere "k"-Schleife 4 mal durchlaufen, in diesem Beispiel wird iZaehler1 dabei jedes mal um 1 erhöht.
Danach wird iZaehler2 um 2 erhöht. Anschließend ist ist die "i"-Schleife zu Ende und i wird um 1 erhöht, solange i kleiner 4 ist. Anschließend die "i"-Schleife erneut durchlaufen.
Dies wird widerholt, bis i=4 ist und die Bedingung i<4 nicht mehr erfüllt wird. Die äußere Schleife wird verlassen. 

</details>
  



## Tip - Widerstände speichern


<details>
 <summary>Click to expand</summary>


Erweiter dein Programm so, dass die Widerstandswerte gespeichert werden, wenn sie am dichtesten an dem gewünschten Wert sind.


 - [x] E12 Reihe
 - [x] Parallelschaltung
 - [x] Widerstände finden
 - [x] Widerstände speicher


  
  ### Tip 4
  
  <details>
 <summary>Click to expand</summary>
  
   Berechne die Differenz zwischen dem letzten und aktuellen Widerstand im Vergleich zum gewünschten Widerstand, speichere den besseren.
   Speicher den Zähler und übergib ihn am Ende wieder der passenden Unterfunktion, um den ermittelten Widerstand zu bestimmen.
   Überprüfe, ob die Differenz negativ ist.
    
  
   </details>

  </details>

## Zusatz

<details>
 <summary>Click to expand</summary>
  
  Bitte erst dann weiter machen, wenn alles zuvor funktioniert!

### Gewinnspiel
<details>
 <summary>Click to expand</summary>
 
 Sie dürfen nun 3 Widerstände für Ihren gesuchten Widerstand benutzen und **beliebig** anordnen.
 
 Schrieben Sie ihr Programm so um, dass die gegebene E12 Reihe den gesucht Widerstand aus allen möglichen Kombinationen die beste Kombination berechnet.
 Die Widerstandswerte und die verwendete Kombination sind am Ende auf dem Bildschirm auszugeben.

 Testen Sie Ihr Programm mit einem Widerstand von 3542,58 Ohm, welcher wieder über die Tastatur eingegeben werden soll.
 Wenn Sie glauben Sie haben den besten Widerstand gefunden, dann tragen Sie sich bitte in die Liste in dem folgenden Dokument ein.
 
 https://docs.google.com/document/d/1sco9P2rn9MxPSt3fn9-zedgIXZ3zUD99GXpPp0ODjQs/edit
 
 </details>
  </details>



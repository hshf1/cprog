# Aufgabe 7


Sie suchen für Ihr Projekt einen Widerstand. Sie haben den Baukasten der E12 Reihe mit den Widerständen von 1 bis 10.000 Ohm.
Leider ist kein Widerstand dabei, der nah genug an ihrem Wunschwert liegt. Sie möchten diesem durch 2 parallel geschaltete Widerstände aus der E12 Reihe möglichst nahekommen.  Entwickeln Sie ein Programm, das alle Kombinationen automatisch erstellt und das beste Widerstandspaar für Sie ermittelt und ausgibt.
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
 Wie sich die E12-Reihe berechnen lässt, kann unter dem Wikipedia-Link nachgelesen werden.
 
 Wiki:
 https://de.wikipedia.org/wiki/E-Reihe
 

  
## Tipp - E12 Reihe

<details>
<summary>Klicken zum Öffnen</summary>

Die E12 Reihe sind Widerstände, die 12 Widerstände pro Dekade enthalten!
Geben Sie die E12-Reihe von 1 bis 10.000 an.

Es kann die Funktion pow() mit 10 hoch x/12 verwendet werden.
pow() befindet sich in der math.h Bibliothek

 </details>
  
  ## Tipp - Parallelschaltung
  
  <details>
  <summary>Klicken zum Öffnen</summary>
  
  Die Parallelschaltung kann durch 
  
  >R1*R2/(R1+R2)
  >
 
   realisiert werden.
  
  </details>

  
 ## Tipp - Wiederstände berechnen
  
  <details>
  <summary>Klicken zum Öffnen</summary>

 Um alle Widerstandskombinationen zu berechnen, kann eine doppelte for-Schleife verwendet werden 
  
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
Zuerst wird die innere "k"-Schleife 4 Mal durchlaufen, in diesem Beispiel wird iZaehler1 dabei jedes Mal um 1 erhöht.
Danach wird iZaehler2 um 2 erhöht. Anschließend ist die "i"-Schleife zu Ende und i wird um 1 erhöht, solange i kleiner 4 ist. Anschließend die "i"-Schleife erneut durchlaufen.
Dies wird wiederholt, bis i=4 ist und die Bedingung i<4 nicht mehr erfüllt wird. Die äußere Schleife wird verlassen. 

</details>
  



## Tipp - Widerstände speichern


<details>
 <summary>Klicken zum Öffnen</summary>
  
   Berechnen Sie die Differenz zwischen dem letzten und aktuellen Widerstand im Vergleich zum gewünschten Widerstand, speichern Sie den besseren.
   Ist der passendste Widerstand gefunden, kann der Zähler gespeichert und als Rückgabewert übergeben werden.
   Sie können auch den Wert des Widerstandes übergeben und nicht die Potenz. Das kann variieren, je nachdem, wie Sie die Schleife aufgebaut haben.
   Überprüfen Sie auch, ob die Differenz negativ ist. (20 Ohm kleiner als der gesuchte Widerstand ist besser als 50 Ohm größer!)

  </details>

## Zusatz

<details>
 <summary>Klicken zum Öffnen</summary>
  
  Bitte erst dann weiter machen, wenn alles zuvor funktioniert!

### Gewinnspiel(Sose2021)
<details>
 <summary>Klicken zum Öffnen</summary>
 
 Sie dürfen nun 3 Widerstände für Ihren gesuchten Widerstand benutzen und **beliebig** anordnen.
 
 Schrieben Sie ihr Programm so um, dass die gegebene E12 Reihe den gesucht Widerstand aus allen möglichen Kombinationen die beste Kombination berechnet.
 Die Widerstandswerte und die verwendete Kombination sind am Ende auf dem Bildschirm auszugeben.

 Testen Sie Ihr Programm mit einem Widerstand von 3542,58 Ohm, welcher wieder über die Tastatur eingegeben werden soll.
 Wenn Sie glauben Sie haben den besten Widerstand gefunden, dann tragen Sie sich bitte in die Liste in dem folgenden Dokument ein.
 
 https://docs.google.com/document/d/1sco9P2rn9MxPSt3fn9-zedgIXZ3zUD99GXpPp0ODjQs/edit
 
 </details>
  </details>



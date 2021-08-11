
# Aufgabe 0

Herzlich Wilkommen zu Ihrer ersten Programmieraufgabe in C !

Ihr erstes Programm soll die folgenden Daten auf dem Bildschirm ausgeben.
- [ ] Ihren Namen, Studiengang und E-Mail
- [ ] Summe von 2 Zahlen ausgeben
- [ ] Kapital berechnen, 180€ zu 2%
- [ ] Die 24 durch Bit-Operatoren vierteln

Diese Ausgaben sollen alle in einer main() Funktion stehen und nacheinander auf dem Bildschirm erscheinen. 
  Alle Werte und Daten sollen im Code stehen.


### Tipp - Wie schreibe ich ein Programm
<details>
<summary> Klicken zum öffnen</summary>

Jedes Programm enthält neben der Hauptfunktion die benötigten Bibliotheken.
Diese werden ganz zu Beginn mit Hilfe des ```include``` Befehls angegeben.
  
Danach folgt die ```main()``` Methode.
In dieser sollen die oben genannten Aufgaben bearbeitet werden.
</details>

### Tipp - Ausgabe auf dem Bildschirm mit ```printf()```  
<details>
<summary> Klicken zum öffnen</summary>
  
Mit dem ```printf``` Befehl können Zahlen, Zeichen und Zeichenketten (z.B. Wörter) auf dem Bildschirm ausgegeben werden.
Im einfachsten Fall sieht ```printf``` wie folgt aus:
 ```C
  printf("<Text>");
```
  Alles was zwischen den Anführungszeichen steht wird von ```printf```auf dem Bildschirm ausgegeben.
  Die "<>" werden demnach mit ausgegeben und sind nicht relevant für den Syntax!
</details> 


### Tipp - Rechnen
<details>
<summary>Klicken zum öffnen</summary>

In C können die bekannten Rechenoperatoren wie gewohnt angewandt werden.
  Auch hier gilt Punkt vor Strich, sonst Klammer setzten!
  
  Achten Sie dabei auf den richtigen Datentypen !
  
  Legen Sie für jeden Wert eine passende Variable an. 
</details>

### Tipp - Kapital
<details>
<summary>Klicken zum öffnen</summary>
  Sie haben ein Kapital von 180€, das jährlich mit 2% verzinst wird.
  Berechnen sie den Gewinn nach einem Jahr und geben sie diesen auf dem Bildschirm aus.
</details>

### Tipp - Bit-Operatoren
<details>
<summary>Klicken zum öffnen</summary>
  Legen Sie einen Integer mit dem Werte 24 an.
  Dieser Integer soll durch Bit-Operatoren geviertelt werden.
  Geben Sie beide Zahlen auf dem Bildschirm aus.
  
  #### Hilfe
<details>
<summary>Klicken zum öffnen</summary>

Überlegen sie sich, wie die 24 und das Ergebniss 24/4 in Binär aussieht.  
  Was passiert, wenn eine Zahl um ein Bit nach rechts verschoben wird?

</details>
</details>

  ### Tipp - Ordung/Zeilenverschub
<details>
<summary>Klicken zum öffnen</summary>

Damit die Ausgaben nicht alle in der selben Zeile stehen, kann ein Zeilenverschub mit "\n" erzeugt werden.
Der Zeilenverschub wird mit in ```printf()``` geschrieben. Dieser beinhaltet dann neben dem Text der ausgegeben werden soll noch das "\n".
  Das Zeichen kann vor oder nach dem Text stehen. Wichtig ist, dass es wie der Text zwichen den Anführungszeichen steht.
 ```C
  printf("<Text>\n"); //Zeilenverschub nach der Ausgabe
  //oder
  printf("\n<Text>"); // Zeilenverschub vor der Ausgabe
  //oder
  printf("<Text>");
  printf("\n"); // Zeilenverschub nach der Ausgabe, sonst reihenfolge tauschen!
```
</details>
  

### *Herzlichen Gl\x9Ackwunsch Sie haben gerade ihr erstes Programm in C geschrieben !*

  
## Zusatz - Kapital
<details>
<summary>Klicken zum öffnen</summary>
  
  

Erzeugen sie durch die Wahl entsprechender Datentypen einen Rechenfehler. 

</details>


© 2021 GitHub, Inc.

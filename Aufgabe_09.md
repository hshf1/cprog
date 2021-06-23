# Aufgabe 9

Erstellen und testen Sie ein Programm, das für eine beliebige Ganzzahl die nächsthöhere gerade Zahl ausgibt. Falls die Zahl bereits gerade ist, ist die Zahl selbst auszugeben. 
Die Zahl ist durch den Benutzer einzugeben.

## Teil 1

  
  Erstellen Sie hierzu folgende Unterprogramme
  
  >void eingeben (int*)
  >
_Erhält einen Zeiger auf eine Zahl und ermöglicht die Eingabe dieser Zahl durch die Tastatur._

>void korrigieren (int*)
>
_Erhält einen Zeiger auf die vorher eingegeben Zahl und korrigiert diese, falls sie ungerade ist._

>void ausgeben (int*)
>
_Erhält einen Zeiger auf die vorher eingegebene und korrigierte Zahl und gibt diese mit Wert und Adresse am Bildschirm aus._

Testen Sie Ihr Programm mit unterschiedlichen Testfällen.

## scanf()
<details>
  <summary> klicke zum öffnen </summary>
  
  ```scanf``` liest von der Tastatur ein und vergleicht mit der angegebenen Formatanweisung.
  Bei dem bereits bekannten verfahren weisen sie mit dem "&" dem eingelesenen Werte eine Adresse zu in welche diese gespeichert werden soll.
  ```
  int a=0;
  scanf("%d",&a);
  ````
  
  Wenn mit pointern gearbeitet wird, dann wird bereites eine Adresse übergeben und das "&" wird weggelassen.
  ``` 
  void einlesen(*ptr)
  {
    printf("Bitte geben sie eine Zahle ein:\n");
    scanf("%f",ptr);
  }
  ```
  
  </details>

## Beispiel Pointer
<details>
<summary>Click to expand</summary>
  
  

  In dem folgenden Beispiel wird ein Pointer an ein Unterprogramm übergeben und in diesem Unterprogramm wird der eingelesen Wert direkt an die in der main deklarierten Variable gespeichert.
  ![Screenshot (41)](https://user-images.githubusercontent.com/79829648/121770494-e477e780-cb69-11eb-82ef-566f3bb7d404.png)

An der Ausgabe kann das nachvefolgt werden.
  
  ## Ausführlich
  <details>
<summary>Click to expand</summary>
  Sie werden einen Programmcode sehen, welcher ähnlich dem zu dieser Aufgabe ist.
  Der Code, den Sie auf den Bildern sehen, bearbeitet die folgenden Punkte:
  
  - [ ] Buchstabe einlesen
  - [ ] Buchstabe verändern
  - [ ] Buchstabe ausgeben

Im ersten Punkt mit "Buchstabe einlesen", ist noch eine Fehlerabfrage eingebaut, welche vom Verständnis etwas schwierigerer ist. In den Kommentaren steht dazu aber genug.

# Main
![Screenshot (31)](https://user-images.githubusercontent.com/79829648/117532858-e9d19780-afe9-11eb-8998-6357607d014e.png)

# Buchstaben einlesen
[Screenshot (49)](https://user-images.githubusercontent.com/79829648/123069864-8376cc00-d413-11eb-8e05-0ca7d66f4684.png)


# Buchstaben verändern
![Screenshot (33)](https://user-images.githubusercontent.com/79829648/117532872-f7871d00-afe9-11eb-9e77-71b95c358ac3.png)

# Buchstaben ausgeben
![Screenshot (34)](https://user-images.githubusercontent.com/79829648/117532875-fa820d80-afe9-11eb-85b4-f26a4f26048d.png)


  
  </details>
  </details>

## Zusatz
<details>
<summary>Click to expand</summary>
  
  Erstellen Sie das Struktogramm für Ihr Hauptprogramm und für die Unterfunktionen
  </details>

  
  ## Teil 2

  
  Erweitern Sie Ihr Programm um eine weiter Funktion, die überprüft, ob die eingegebene Zahl mindestens 5-stellig ist und diese bei Bedarf korrigiert.
  
  _korrigieren2_ soll nach der Funktion aus Teil 1 aufgerufen werden.
  Füllen Sie dazu die fehlenden Stellen **rechts** neben der Zahl mit 0 auf.

# Aufgabe 14 - Einfach verkettete Listen

Internetkommunikation erfolgt über zentrale Router als Punkt zu Punkt Verbindung. Sendet ein User eine Anfrage an eine Webseite, wird das TCP/IP Telegramm von seinem Rechner an seinen Provider gesendet, der sendet es weiter an einen Internetknoten und der sendet es weiter an den nächsten Knoten, bis es an den Hoster der Webseite zugestellt wird. Der Weg von der Quelle bis zum Ziel ist nicht immer derselbe, sondern wird dynamisch bestimmt.


## Teil 1

Diese Kommunikation soll in einer verkettetetn Liste nachvollzogen werden:

- Erstellen Sie mit ```typedef``` einen neuen Datentypen ```IPHub```, der die Struktur ```struct IPHub_s``` abbildet.
- Erstellen Sie nun die Struktur ```struct IPHub_s``` mit dem Inhalt:
    - int KnotenNr
    - int Kollision
    - IPHub NextHub
- Erstellen Sie  in der Main ein Array ```Routing``` vom Datentyp ```IPHup```, welches 6 Felder aufweist. Der 0-te Index ist der Quellhub und der 6. Index ist der Zielhub. Initialisieren Sie das Feld. Denken Sie sich eigene _KnotenNr_ aus. Die Variable Kollision ist zuerst immer 0. Initialisieren Sie eine mögliche Route über alle Hubs von der Quelle bis zum Ziel (d.h. verbinden Sie die Strukturelemente ```NextHub```).

- Erstellen Sie eine Unterfunktion ```void RouteAusgeben(IPHub *Start)``` um die Route der Pakete auszugeben. Übergeben Sie der Unterfunktion die Adresse der Quelle. Geben Sie die ```KnotenNr``` Und Kollisionen aus, solange bis das Ziel Erreicht wurde (NextHub==NULL)

- Erstellen Sie eine Unterfunktion ```void SetzeKollision(IPHub *Start)```. Geben Sie die Knotennummer über die Tastatur ein, bei der das Strukturelement ```Kollision``` auf 1 oder 0 gesetzt werden kann. Prüfen Sie, ob die ```KnotenNr``` existiert. Wenn diese existiert, dann setzen Sie das Strukturelement ```Kollision``` dieses und aller Folgeknoten auf 1 oder 0 (gemäß Eingabe). Geben Sie die Route neu aus.

## Teil 2

Nutzen Sie nun anstatt des Arrays eine dynamische Routingverwaltung.

- Fragen Sie über die Tastatur ab, wie viele Knoten angelegt werden sollen.
- Legen Sie die Konten über ```malloc```an und verknüprfen sie diese mit einander.
- Geben Sie die Knoten nacheinander aus.
- Fragen Sie ab, welcher Knoten eine Kollision hat und setzen Sie das Bit Kollision in allen Folgeknoten auf 1 oder 0.

## Unterschied Array und malloc
<details>
    <summary>klicken zum öffnen</summary>   

## Verkettetet Liste im Array
 ![Verkettete Liste Array](https://user-images.githubusercontent.com/79829648/123070303-ecf6da80-d413-11eb-83fc-92e783d46cdb.png)

## Verkettetet Liste mit malloc    
![Verkettete Liste malloc](https://user-images.githubusercontent.com/79829648/123070311-ef593480-d413-11eb-9194-1b11ac60f5de.png)

  </details>

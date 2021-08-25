
# Aufgabe 14 - Einfach verkettete Listen

Internetkommunikation erfolgt über zentrale Router als Punkt zu Punkt Verbindung. Sendet ein User eine Anfrage an eine Webseite, wird das TCP/IP Telegramm von seinem Rechner an seinen Provider gesendet, der sendet es weiter an einen Internetknoten und der sendet es weiter an den nächsten Knoten, bis es an den Hoster der Webseite zugestellt wird. Der Weg von der Quelle bis zum Ziel ist nicht immer derselbe, sondern wird dynamisch bestimmt.


## Teil 1

Diese Kommunikation soll in einer verketteten Liste nachvollzogen werden:

- Erstellen Sie mit ```typedef``` einen neuen Datentyp ```IPHub```, der die Struktur ```struct IPHub_s``` abbildet.
- Erstellen Sie nun die Struktur ```struct IPHub_s``` mit dem Inhalt:
    - int KnotenNr
    - int Kollision
    - IPHub NextHub
- Erstellen Sie in der Main ein Array ```Routing``` vom Datentyp ```IPHup```, welches 6 Felder aufweist. Der 0-te Index ist der Quellhub und der 6. Index ist der Zielhub. Initialisieren Sie das Feld. Denken Sie sich eigene _KnotenNr_ aus. Die Variable Kollision ist zuerst immer 0. Initialisieren Sie eine mögliche Route über alle Hubs von der Quelle bis zum Ziel (d.h. verbinden Sie die Strukturelemente ```NextHub```).

- Erstellen Sie eine Unterfunktion ```void RouteAusgeben(IPHub *Start)``` um die Route der Pakete auszugeben. Übergeben Sie der Unterfunktion die Adresse der Quelle. Geben Sie die ```KnotenNr``` und Kollisionen aus, solange bis das Ziel erreicht wurde (NextHub==NULL)

- Erstellen Sie eine Unterfunktion ```void SetzeKollision(IPHub *Start)```. Geben Sie die Knotennummer über die Tastatur ein, bei der das Strukturelement ```Kollision``` auf 1 oder 0 gesetzt werden kann. Prüfen Sie, ob die ```KnotenNr``` existiert. Wenn diese existiert, dann setzen Sie das Strukturelement ```Kollision``` dieses und aller Folgeknoten auf 1 oder 0 (gemäß Eingabe). Geben Sie die Route neu aus.

## Teil 2

Nutzen Sie nun anstatt des Arrays eine dynamische Routingverwaltung.

- Fragen Sie über die Tastatur ab, wie viele Knoten angelegt werden sollen.
- Legen Sie die Knoten über ```malloc```an und verknüpfen Sie diese mit einander.
- Geben Sie die Knoten nacheinander aus.
- Fragen Sie ab, welcher Knoten eine Kollision hat und setzen Sie das Bit Kollision in allen Folgeknoten auf 1 oder 0.

## Unterschied Array und malloc
<details>
    <summary>klicken zum Öffnen</summary>   

## Verkettete Liste im Array
![Verkettete Liste Array](https://user-images.githubusercontent.com/79829648/129008005-7d9453a9-bbb6-4264-a29e-406273545332.png)

## Verkettete Liste mit malloc   
![Verkettete Liste malloc](https://user-images.githubusercontent.com/79829648/129008068-352088d7-16e5-4d4e-a9da-85d00f0be5a4.png)

  </details>

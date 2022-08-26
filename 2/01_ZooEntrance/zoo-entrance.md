# Zoo Entrance

## Beschreibung

Zur Verwaltung der Eintrittskasse eines Zoos sollen Ticketklassen erstellt werden. Der Zoodirektor beschreibt die Zusammenhänge folgendermaßen:

> Jedes Ticket besitzt einen Preis. Es werden Tickets für Kinder, Erwachsene und Gruppen angeboten. Kinder zahlen keine Eintritt, Erwachsene zahlen 14,70 Euro und Gruppen zahlen 50 Euro Eintritt. Bei jedem Gruppenticket soll die Anzahl der Personen gespeichert werden. Pro Tag können maximal 100 Tickets ausgegeben werden.

Die Klasse `Entrance`soll das Tagesgeschehen des Zooeingangs repräsentieren. In der Klasse werden die ausgegebenen Tickets verwaltet. Außerdem bietet sie Funktionen zur Berechnung des Tagesumsatzes und der Besucherzahl.

## Aufgabenstellung

Setzen Sie das abgebildete Klassendiagramm anhand der obigen Beschreibung in einer Java Applikation um:

![img](./pics/class-diagram.png)

## Test

Implementieren Sie in der `main`-Methode einen Testfall mit folgenden Zoobesuchern:

- eine Gruppe mit 6 Personen
- zwei Erwachsene mit drei Kindern

Die erwarteten Ergebnisse sind daher:

- Besucherzahl: 11
- Umsatz: 79,40 Euro

## Zusatzaufgaben

### Fehlerbehandlung

Falls `addTicket()` das Argument `null` übergeben wird, soll die Methode eine `NullPointerException` werfen.

Falls ein Ticket nicht hinzugefügt werden kann, weil die maximale Ticketanzahl bereits ausgegeben wurde, soll `addTicket()` eine `SoldOutException` werfen.

### Ausgabeformatierung

Formatieren Sie die Ausgabe des Tagesumsatzes wie im folgenden Screenshot:

![img](./pics/console.png)
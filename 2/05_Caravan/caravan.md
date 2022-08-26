# Übung Karawane

Entwickeln Sie die folgenden Klassen zur Umsetzung einer *E-Karawane*. Implementieren Sie anschließend Unit-Tests für die beschriebenen Methoden.

## Klasse `Camel`

Ein Kamel besitzt folgende Felder:

- `int maxPace`: Geschwindigkeit des Kamels im unbeladenen Zustand
- `int load`: Anzahl der Ballen, die das Kamel im Moment trägt
- `Camel next`: Nächstes Kamel in der Karawane

Die Klasse soll nur über folgenden Konstruktor verfügen:

- `Camel(int maxPace)`: Initialisiert `load` mit `0` und `next` mit `null`.

Implementieren Sie für alle Felder `Getter` und `Setter`. Außerdem soll die Klasse über folgende Methode verfügen:

- `int getPace()`: Liefert die tatsächliche Geschwindigkeit des Kamels. Mit jedem Ballen Ladung nimmt die Geschwindigkeit um 1 km/h ab. Die minimale Geschwindigkeit beträgt 0 km/h.

## Klasse `Caravan`

Eine Karawane nur ein Feld:

- `Camel first`: Erstes Kamel der Karawane (`null` bedeutet, dass die Karawane noch keine Kamele besitzt)

Implementieren Sie in der Klasse `Caravan` folgende Methoden:

- `int getPace()`: Liefert die aktuelle Reisegeschwindigkeit der Karawane, die vom langsamsten Kamel bestimmt wird.
- `void addCamel(Camel camel)`: Fügt das übergebene Kamel am Anfang der Karawane ein.
- `void removeCamel(Camel camel)`: Entfernt das übergebene Kamel aus der Karawane.
- `void addLoad(int load)`: Verteilt die übergebene Anzahl an Ballen so auf die Kamele, dass die Reisegeschwindigkeit der Karawane möglichst hoch bleibt.
- `void unload()`: Entlädt alle Kamele der Karawane.

## Klasse `CaravanTest`

Implementieren Sie mehrere Testfälle und rufen Sie diese in der `main`-Methode auf.
# BigInt

Entwickeln Sie eine Anwendung, mit der beliebig große natürlich Zahlen addiert, multipliziert und potenziert werden können. 

## Klasse BigInt

Ein Objekt der Klasse `BigInt` repräsentiert eine beliebig große natürliche Zahl.

### Felder

- `private String number`: damit die Zahl beliebig groß sein kann, wird sie als `String` abgespeichert.
- `public final static BigInt ZERO`: Zahl `0` als `BigInt`-Objekt
- `public final static BigInt ONE`: Zahl `1` als `BigInt`-Objekt

### Konstruktoren

- `BigInt(int number)`
- `BigInt(String number)`

Prüfen Sie im zweiten Konstruktor, ob tatsächlich eine natürliche Zahl übergeben wurde. Falls nicht soll der Konstruktor eine `InvalidArgumentException` werfen.

### Methoden

Bei den folgenden Methoden wird das Ergebnis immer als **neues** `BigInt`-Objekt zurückgegeben (`this` nicht verändern!!!).

- `BigInt add(BigInt other)`: addiert die übergebene Zahl und gibt die Summe zurück
- `BigInt subtract(BigInt other)`: subtrahiert die übergebene Zahl und gibt die Differenz zurück
- `BigInt multiply(BigInt other)`: multipliziert die übergebene Zahl und gibt das Produkt zurück
- `BigInt pow(PositiveBigInt exponent)`: potenziert mit dem übergebenen Exponenten und gibt die Potenz zurück
  - `PositiveBigInt` ist eine Kindklasse von `BigInt`, in deren Konstruktor sichergestellt wird, dass die Zahl positiv ist (wenn nein => `IllegalArgumentException`).

### Interfaces

Implementieren Sie das Interface `Comparable<BigInt>`.

## Klasse `BigIntTest`

Entwickeln Sie in der `main`-Methode ein Testprogramm, in dem Sie alle Rechenoperationen mit kleinen **und** großen Zahlen überprüfen.










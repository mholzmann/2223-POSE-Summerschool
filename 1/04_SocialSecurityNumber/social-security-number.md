# Social Security Number

Eine Sozialversicherungsnummer soll auf Gültigkeit überprüft werden.  

**SVNr-Aufbau:** 123xTTMMJJ

- Die ersten drei Stellen sind eine fortlaufende Nummer.
- Die Ziffer an der 4. Stelle ist die Prüfziffer und
- die letzten 6 Ziffern sind das Geburtsdatum.  

**Überprüfung auf Gültigkeit:** Die Einerziffer der Ziffernsumme (alle Ziffern außer die an der 4. Stelle werden berücksichtigt) muss die Prüfziffer ergeben.  

**Beispiel:** SVNr = 1238010191

- 8 ist die Prüfziffer (vierte Ziffer)  
- Ziffernsumme: (1+2+3+0+1+0+1+9+1)=18 => Einerziffer ist 8 
- Also ist hier die Prüfziffer gleich der Einerziffer, daher ist diese Nummer gültig!  

**Entwickeln Sie folgende Methoden:**  

- `public static int digitsCount(long number)`
  - gibt die Ziffernanzahl der übergebenen Zahl zurück
- `public static int digitsSum(long number)`
  - gibt die Ziffernsumme der übergebenen Zahl zurück
  - soll auch für Zahlen funktionieren, die weniger / mehr als 10 Ziffern besitzen
- `public static int fourthDigit(long number)`
  - gibt die vierte Ziffern einer Zahl zurück
  - falls die Zahl keine vierte Ziffer besitzt, wird `-1` zurückgegeben
- `public static boolean checkSocialSecurityNumber(long number)`
  - überprüft die übergebene Sozialversicherungsnummer (positive Zahl, genau 10 Stellen lang, Prüfziffer ok)
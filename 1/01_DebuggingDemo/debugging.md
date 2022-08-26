# Debugging

**Debuggen** Sie die folgende `main`-Methode, um herauszufinden, welche Werte die Variable `x` annimmt. Schreibe Sie **alle** Werte in der richtigen Reihenfolge auf und dokumentieren Sie die Debugging-Schritte mithilfe von Screenshots.

```java
public static void main(String[] args) {
    int x = 100;
    int v;
    for (int i = 5; i < 7; i++) {
        v = i * i;
        while (v > 10) {
            v = v - i / 2;
            if (v % i == 0) {
                x = v / 2 * 3;
            }
        }
    }
    System.out.println(x);
}
```

**Achtung:** Es ist nicht erlaubt, die Werte von `x` einfach auf der Konsole auszugeben.

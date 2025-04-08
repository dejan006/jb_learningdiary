# Objektorientierte Programmierung (OOP)

## Einführung

Wenn in einem Programm alle Funktionen und Variablen in einer einzigen Datei ohne Struktur untergebracht sind, kann dies schnell zu Chaos führen. Die Übersichtlichkeit leidet, der Code wird schwer wartbar und Fehler schleichen sich leichter ein. Hier kommt die **objektorientierte Programmierung (OOP)** ins Spiel.

OOP hilft uns dabei, Programme in logisch getrennte **Objekte** zu strukturieren. Jedes Objekt ist eine Kombination aus:

- **Attributen** (Variablen, die den Zustand beschreiben)
- **Methoden** (Funktionen, die das Verhalten definieren)

So entsteht übersichtlicher, wiederverwendbarer und wartbarer Code.

---

## Was ist ein Objekt?

Ein Objekt ist eine Art "Mini-Programm" in sich. Es enthält sowohl die Daten als auch die Funktionen, die mit diesen Daten arbeiten.

### Beispiel: Ein Auto als Objekt

Stellen wir uns ein Auto als Objekt vor. Ein Auto hat bestimmte Eigenschaften (**Attribute**) und bestimmte Fähigkeiten (**Methoden**):

- **Attribute**: `model`, `color`
- **Methoden**: `startCar()`, `turnOffCar()`

---

## Beispiel in Code

Hier ein einfaches Beispiel in Java (funktioniert sehr ähnlich in anderen OOP-Sprachen wie C++, Python, etc.):

### Klasse `Car`

```java
public class Car {
    String model;
    String color;

    // Konstruktor
    public Car(String model, String color) {
        this.model = model;
        this.color = color;
    }

    // Methode zum Starten des Autos
    public void startCar() {
        System.out.println(model + " startet.");
    }

    // Methode zum Ausschalten des Autos
    public void turnOffCar() {
        System.out.println(model + " wird ausgeschaltet.");
    }
}

public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("VW Golf", "Rot");
        myCar.startCar();
        myCar.turnOffCar();
    }
}
```
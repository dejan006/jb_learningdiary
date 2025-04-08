# Object-Oriented Programming (OOP)

## Introduction

When all functions and variables are placed in a single file without any structure, things can quickly become chaotic. Code becomes difficult to manage, hard to maintain, and prone to errors. This is where **object-oriented programming (OOP)** comes in.

OOP helps us structure programs into logically separated **objects**. Each object is a combination of:

- **Attributes** (variables that describe the state)
- **Methods** (functions that define behavior)

This results in cleaner, reusable, and maintainable code.

---

## What is an Object?

An object is like a "mini-program" in itself. It contains both data and the functions that operate on that data.

### Example: A Car as an Object

Let’s take a car as an example of an object. A car has certain properties (**attributes**) and certain capabilities (**methods**):

- **Attributes**: `model`, `color`
- **Methods**: `startCar()`, `turnOffCar()`

---

## Code Example

Here’s a simple example in Java (the concept is very similar in other OOP languages like C++, Python, etc.):

### Class `Car`

```java
public class Car {
    String model;
    String color;

    // Constructor
    public Car(String model, String color) {
        this.model = model;
        this.color = color;
    }

    // Method to start the car
    public void startCar() {
        System.out.println(model + " is starting.");
    }

    // Method to turn off the car
    public void turnOffCar() {
        System.out.println(model + " is turning off.");
    }
}
```

### Class `Main`
```java
public class Main {
    public static void main(String[] args) {
        Car myCar = new Car("VW Golf", "Rot");
        myCar.startCar();
        myCar.turnOffCar();
    }
}
```
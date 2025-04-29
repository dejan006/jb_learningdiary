# Table-Driven Tests in Go (Einfach erklärt)

## Idee

- Statt viele einzelne Tests zu schreiben, legt man eine **Tabelle mit Testfällen** an.
- Dann geht eine **Schleife** durch diese Tabelle und prüft alles automatisch.
- Ergebnis: **Weniger Code**, **übersichtlicher**, **leichter zu erweitern**.

---

## Einzelne Tests (klassisch)

```go
if Sum(1, 2) != 3 {
    t.Error("Expected 3")
}
if Sum(2, 2) != 4 {
    t.Error("Expected 4")
}
if Sum(5, 5) != 10 {
    t.Error("Expected 10")
}
```

- Jeder Test ist separat geschrieben.
- Viel wiederholter Code.

---

## Table-Driven Tests (besser)

```go
var tests = []struct {
    a, b int
    want int
}{
    {1, 2, 3},
    {2, 2, 4},
    {5, 5, 10},
}
for _, tt := range tests {
    got := Sum(tt.a, tt.b)
    if got != tt.want {
        t.Errorf("Sum(%d, %d) = %d; want %d", tt.a, tt.b, got, tt.want)
    }
}
```

- Alle Testfälle sind in einer **Liste** gespeichert.
- Eine **Schleife** prüft automatisch jeden Fall.
- Neue Tests einfach hinzufügen.

---

## Vorteile

- Einfach neue Tests ergänzen
- Weniger Fehler
- Bessere Übersicht
- Kürzerer Code

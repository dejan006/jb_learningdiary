# Kubernetes Objekte – Einfach erklärt
## Was sind Kubernetes Objekte?

In Kubernetes gibt es **Objekte**, die zeigen, **wie ein Cluster aussehen soll**. Sie speichern Infos darüber, **was laufen soll**, **wie es laufen soll** und **wie viele Ressourcen** verwendet werden dürfen.

Beispiele für Infos im Objekt:
- Welche App soll laufen?
- Wie viele Kopien (Replicas) soll es geben?
- Welche Regeln gelten (z.B. Neustarten bei Fehler)?

So ein Objekt ist wie ein **Wunschzettel** – Kubernetes nennt das den **"desired state"** (gewünschter Zustand). Kubernetes kümmert sich dann darum, dass alles genau so umgesetzt wird. Wenn etwas schiefläuft (z.B. ein Container fällt aus), wird es automatisch repariert.

## Wie arbeitet Kubernetes damit?

Jedes Objekt hat zwei wichtige Teile:
- `spec`: was möchte man (der Wunschzustand)
- `status`: was gerade wirklich los ist

Kubernetes gleicht diese beiden ständig ab und bringt das System in den gewünschten Zustand zurück.

## Wie erstellt man ein Objekt?
Du kannst ein Objekt mit der Kommandozeile **`kubectl`** erstellen, z.B.:

```bash
kubectl apply -f test.yaml

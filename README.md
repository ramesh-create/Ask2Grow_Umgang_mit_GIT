# Ask2Grow – Umfragen App

Eine interaktive Umfrage-App für Teams und Abteilungen: Fragen erstellen, live beantworten, auswerten und vergleichen – inklusive Punkte-System, Anonym-Modus und Feedback.

Dieses Repository enthält die **Requirements-Quelle** (`Anforderung.md`) sowie einen **lauffähigen Prototyp** (`prototyp.html`).

---

## Features

- Fragen **erstellen** und **beantworten**
- **Live-Ergebnisse** &amp; **Auswertung** der Antworten
- Lösungstypen: **Mehrfachauswahl** und **Ja/Nein**
- **Anonym-Modus**
- **Punkte** für das Beantworten von Fragen
- **Fragen vergleichen**
- Teilen per **Code** (QR-Code-Platzhalter vorhanden)
- Erfassen von Zusatzdaten (z. B. **Alter**)
- **Feedback** zu den Fragen

## Rollen

| Rolle         | Beschreibung                                                       |
| ------------- | ------------------------------------------------------------------ |
| **Host**      | Erstellt und verwaltet Fragen, sieht Live-Ergebnisse, wertet aus.  |
| **Teilnehmer**| Beantwortet Fragen, sammelt Punkte und gibt Feedback.              |
| **Abteilungen**| Antwortet als eigene Abteilung (z. B. Marketing).                 |

## Design-Vorgabe

Die Benutzeroberfläche beschränkt sich auf **maximal drei Farben**: Indigo, Grün und Dunkelgrau (Weiß/Hellgrau als Neutrale).

---

## Prototyp nutzen

Der Prototyp ist eine **eigenständige HTML-Datei ohne Abhängigkeiten** und benötigt kein Build-Tooling.

1. Datei `prototyp.html` in einem Browser öffnen.
2. Rolle wählen: **Host**, **Teilnehmer** oder **Abteilung**.
3. Als Teilnehmer mit dem Code **`ASK2024`** beitreten.
4. Mit einem zweiten Browser-Tab lässt sich eine Antwort simulieren – im Host-Dashboard unter *Live-Ergebnisse* direkt sichtbar.

> Hinweis: Die Daten werden lokal im Browser gespeichert (`localStorage`). Der QR-Code ist als Platzhalter vorgesehen und kann über eine QR-Library ergänzt werden.

---

## Repository-Struktur

```
Anforderung.md     # Single Source of Truth – der Produktvertrag (deutsch)
prototyp.html      # Lauffähiger, eigenständiger Prototyp
AGENTS.md          # Arbeitsanleitung für Agenten / Contributors
.gitignore
```

## Status

- **Requirements:** initial erfasst (`Anforderung.md`)
- **Prototyp:** funktionsfähig
- **Produktion/App-Implementierung:** ausstehend

---

## Entwicklung

Das Projekt hat derzeit **kein Build-Tooling** (keine `package.json`, kein Test-/Lint-Setup). Für weitere Implementierungsschritte wird ein geeignetes Setup eingeführt; `AGENTS.md` beschreibt die aktuellen Konventionen.

### Voraussetzungen

- Nur Git für die Versionskontrolle (kein Laufzeit-Setup für den Prototyp nötig).
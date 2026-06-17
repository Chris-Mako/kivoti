# Kivoti - Projektstruktur

## Ziel

Die Projektstruktur soll übersichtlich, wartbar und erweiterbar sein.

Funktionen werden nach Features organisiert, damit zusammengehöriger Code an einem Ort liegt.

---

## Geplante Struktur

```text
lib/
│
├── core/
│
├── shared/
│
├── features/
│
└── main.dart
```

---

## main.dart

Startpunkt der Flutter-App.

Von hier aus wird die gesamte Anwendung gestartet.

---

## core

Enthält appweite Funktionen und Konfigurationen.

Beispiele:

```text
core/
├── database/
├── network/
├── constants/
└── theme/
```

### database

SQLite-Datenbank und Datenbankkonfiguration.

### network

Netzwerkkommunikation und API-Zugriffe.

### constants

Globale Konstanten der Anwendung.

### theme

Farben, Schriftarten und App-Design.

---

## shared

Gemeinsam genutzte Komponenten.

Beispiele:

```text
shared/
├── widgets/
├── models/
└── utils/
```

### widgets

Wiederverwendbare UI-Komponenten.

### models

Gemeinsam genutzte Datenmodelle.

### utils

Hilfsfunktionen.

---

## features

Enthält die eigentlichen Funktionen der App.

Jedes Feature besitzt seinen eigenen Bereich.

```text
features/
├── food/
├── diary/
├── weight/
├── water/
├── profile/
├── statistics/
├── scanner/
└── speech/
```

---

### food

Lebensmittelverwaltung und Lebensmittelsuche.

### diary

Kalorientagebuch und Mahlzeiten.

### weight

Gewichtsverlauf und Gewichtseinträge.

### water

Wassertracking.

### profile

Benutzerprofil und Zieleinstellungen.

### statistics

Auswertungen, Diagramme und Verläufe.

### scanner

Barcode-Scanner für Lebensmittel.

### speech

Sprachbasierte Lebensmittelerfassung.

---

## Vorteile dieser Struktur

* Klare Trennung der Verantwortlichkeiten
* Leicht erweiterbar
* Features sind unabhängig voneinander organisiert
* Gute Übersichtlichkeit auch bei wachsendem Projektumfang
* Geeignet für Offline-First und spätere Cloud-Erweiterungen

```
```

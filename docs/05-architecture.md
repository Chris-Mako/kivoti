# Kivoti - Architektur

## Ziel

Die Architektur von Kivoti soll einfach verständlich, erweiterbar und wartbar sein.

Die App soll zunächst offline mit SQLite funktionieren und später ohne große Umbauten um Cloud-Funktionen erweitert werden können.

---

## Architekturziele

* Einfache Wartbarkeit
* Klare Verantwortlichkeiten
* Offline First
* Erweiterbarkeit
* Trennung von Benutzeroberfläche und Datenzugriff

---

## Architekturübersicht

UI (Screens)

↓

Repositories

↓

Data Sources

↓

SQLite / Open Food Facts API

---

## UI Layer

Der UI Layer enthält alle Screens und Widgets.

Beispiele:

* DashboardScreen
* FoodSearchScreen
* DiaryScreen
* WeightScreen

Aufgabe:

* Daten anzeigen
* Benutzereingaben entgegennehmen
* Aktionen auslösen

Der UI Layer soll keine SQL-Abfragen und keine API-Aufrufe enthalten.

---

## Repository Layer

Repositories bilden die zentrale Schnittstelle zwischen UI und Datenquellen.

Beispiele:

* FoodRepository
* DiaryRepository
* WeightRepository
* WaterRepository

Aufgabe:

* Daten bereitstellen
* Daten speichern
* Datenquellen koordinieren

Die UI kommuniziert ausschließlich mit Repositories.

---

## Data Sources

Data Sources kümmern sich um den tatsächlichen Datenzugriff.

Beispiele:

* SQLite Database
* Open Food Facts API

Aufgabe:

* Daten lesen
* Daten schreiben
* Externe Systeme ansprechen

---

## Datenfluss

Beispiel: Lebensmittel suchen

FoodSearchScreen

↓

FoodRepository

↓

Open Food Facts API

↓

FoodRepository

↓

FoodSearchScreen

↓

Anzeige für den Nutzer

---

## Vorteile

* UI bleibt übersichtlich
* Datenquellen können ausgetauscht werden
* SQLite und API können parallel genutzt werden
* Funktionen lassen sich leichter testen

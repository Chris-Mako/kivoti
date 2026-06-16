# Kivoti - MVP 1.0

## Ziel

Kivoti soll Nutzern ermöglichen, ihre tägliche Ernährung einfach und schnell zu dokumentieren und ihre Kalorien- und Makroziele zu verfolgen.

## Funktionen

### Onboarding

Der Nutzer gibt folgende Informationen an:

* Geschlecht
* Alter
* Größe
* Aktuelles Gewicht
* Zielgewicht
* Aktivitätslevel
* Ziel (Abnehmen, Halten, Zunehmen)

Kivoti berechnet daraus ein tägliches Kalorienziel.

---

### Dashboard

Anzeige von:

* Tageskalorien
* Kalorienziel
* Makronährstoffen

  * Eiweiß
  * Kohlenhydrate
  * Fett
  * Zucker
* Wasserverbrauch

---

### Mahlzeiten

Folgende Mahlzeiten stehen zur Verfügung:

* Frühstück
* Mittagessen
* Abendessen

Lebensmittel können einer Mahlzeit hinzugefügt werden.

---

### Lebensmittel

Nutzer können:

* Lebensmittel über Open Food Facts suchen
* Eigene Lebensmittel anlegen
* Lebensmittel nach Gramm erfassen
* Lebensmittel über Portionen erfassen

Lebensmittel enthalten:

* Name
* Kalorien pro 100g
* Eiweiß pro 100g
* Kohlenhydrate pro 100g
* Fett pro 100g
* Zucker pro 100g
* Portionsname (optional)
* Portionsgewicht (optional)
* Barcode (optional)

---

### Wassertracking

Der Nutzer kann seine tägliche Wasseraufnahme erfassen.

---

### Verlauf

* Kalenderansicht
* Vergangene Tage anzeigen
* Wochenübersicht
* Gewichtshistorie

---

## Technische Anforderungen

* Flutter
* Dart
* SQLite
* Open Food Facts API
* Offline First
* Android

---

## Nicht Bestandteil von MVP 1.0

* Benutzerkonten
* Cloud-Synchronisation
* Spracheingabe
* Barcode-Scanner
* KI-Funktionen
* Smartwatch-Anbindung
* Rezepte
* Fasten-Tracking
* Premium-Modell

---
name: risikoregister
description: Erstellt aus einem Projekt-Factsheet ein vollständiges Risikoregister mit Eintrittswahrscheinlichkeit, Schadenshöhe, Erwartungswert, Frühindikatoren und Maßnahmen, priorisiert nach Erwartungswert. Nutzen bei Projektstart, vor einem Stage Gate, bei einer Risikorevision oder zur Vorbereitung des Lenkungsausschusses.
---

# Risikoregister aus dem Projekt-Factsheet

## Auftrag

Aus dem Projekt-Factsheet entsteht ein belastbares Risikoregister. Es soll im
Lenkungsausschuss bestehen, also konkret sein, nachvollziehbar hergeleitet und frei von
Floskeln.

Grundlage ist ausschließlich das Factsheet. Fehlt eine Angabe, arbeite mit einer
ausdrücklich gekennzeichneten Annahme oder einer Spannweite (etwa 10 bis 20 Prozent) und
schreibe in einem Halbsatz dazu, woraus du sie ableitest. Erfinde keine Fakten.

## Voraussetzung

Liegt kein Factsheet im Chat, fordere es in genau einem Satz an und liefere zusätzlich
die leere Tabellenvorlage mit denselben Spalten. Kläre dabei mit, falls nicht aus dem
Material ersichtlich:

- Währung und Bezugsgröße der Schadensschätzung (Gesamtprojekt, Jahr, Release)
- Ob Folgekosten (Vertragsstrafen, Nacharbeit, Betriebsausfall, Reputationsschaden)
  einbezogen werden sollen
- Ob bereits ein Risikoregister existiert, das fortgeschrieben wird

## Schritt 1: Rahmenparameter extrahieren

Ziehe aus dem Factsheet heraus und halte sie vor der Tabelle in wenigen Zeilen fest:

Ziele und Scope, Timeline und Meilensteine, Budgetrahmen, Lieferanten und Partner,
Abhängigkeiten, Technologie und Architektur, Datenarten (personenbezogen?), Länder und
Rechtsräume, Betriebs- und Rollout-Modell, Governance und Stakeholder.

Was im Factsheet fehlt, wird hier bereits als Lücke benannt. Eine fehlende Angabe ist
oft selbst ein Risiko.

## Schritt 2: Risiken ableiten

Arbeite mindestens diese Kategorien durch:

Termin und Planung, Kosten, Scope und Anforderungen, Qualität, Technik und Integration,
Security und Datenschutz, Recht und Compliance, Lieferanten und Verfügbarkeit, Betrieb,
Change und Adoption, Stakeholder und Kommunikation.

Ergänze bei KI-Anteilen im Projekt: Datenqualität und Trainingsgrundlage, Abhängigkeit
von einem Modellanbieter, Modell- oder Preisänderungen beim Anbieter, Nachvollziehbarkeit
der Ergebnisse, Einordnung nach der KI-Verordnung.

Jedes Risiko muss sich an einer konkreten Stelle des Factsheets festmachen lassen.

## Schritt 3: Bewerten

Je Risiko:

- Eintrittswahrscheinlichkeit in Prozent (0 bis 100)
- Schaden in Euro, direkte Kosten plus plausible Folgekosten
- Risikowert = Wahrscheinlichkeit mal Schaden

Nutze runde Größenordnungen statt Scheingenauigkeit. 250.000 Euro ist eine Schätzung,
247.500 Euro täuscht eine Präzision vor, die es nicht gibt.

## Schritt 4: Dringlichkeit

Bewerte zusätzlich, wann gehandelt werden muss, abgeleitet aus Timeline und
Abhängigkeiten im Factsheet:

- **Sofort mitigieren:** Auslöser liegt vor dem nächsten Meilenstein oder die
  Gegenmaßnahme braucht Vorlauf
- **Aktiv beobachten:** Frühindikator definiert, Maßnahme vorbereitet
- **Auf Wiedervorlage:** relevant erst in einer späteren Phase, Termin nennen

## Schritt 5: Priorisieren und ausgeben

Sortiere absteigend nach Risikowert, bei Gleichstand nach Eintrittswahrscheinlichkeit.

Gib eine einzige Markdown-Tabelle mit diesen Spalten aus:

| ID | Risiko | Ursache / Trigger | Betroffene Ziele | Eintritt (%) | Schaden (€) | Risikowert (€) | Dringlichkeit | Frühindikatoren | Präventive Maßnahmen | Reaktive Maßnahmen | Owner (Rolle) | Annahmen |

- **Risiko:** ein Satz, Ursache und Wirkung erkennbar
- **Betroffene Ziele:** Zeit, Kosten, Qualität, Scope, Compliance (Mehrfachnennung
  möglich)
- **Frühindikatoren:** ein bis drei, messbar. "Stimmung im Team" ist keiner,
  "Anzahl offener Schnittstellentickets über 20" schon
- **Präventive Maßnahmen:** ein bis drei
- **Reaktive Maßnahmen:** ein bis zwei, der Notfallplan
- **Owner:** Rolle, wenn im Factsheet kein Name steht
- **Annahmen:** kurz, nur wo etwas nicht im Factsheet stand

## Schritt 6: Gegenprüfung

Nach der Tabelle in wenigen Zeilen:

1. Welche der Kategorien aus Schritt 2 haben kein Risiko ergeben, und warum nicht? Eine
   leere Kategorie ist entweder eine gute Nachricht oder eine Lücke im Factsheet.
2. Welche drei Angaben würden die Bewertung am stärksten verändern, wenn sie nachgereicht
   werden?
3. Summe der Risikowerte, gestellt neben den Budgetrahmen aus dem Factsheet.

## Hinweise zum Einsatz

- Die Zahlen sind Schätzungen auf Basis eines Dokuments, keine Bewertung im Sinne des
  Risikomanagements nach ISO 31000 und keine versicherungsmathematische Größe. Sie
  strukturieren das Gespräch, sie ersetzen es nicht.
- Das Register gehört ins Team und in den Lenkungsausschuss, nicht in die Schublade der
  Projektleitung. Ein Risiko ohne benannten Owner ist kein Risiko, sondern eine Notiz.
- Enthält das Factsheet Kunden-, Personal- oder Vertragsdaten, prüfe vorher, welches
  Werkzeug diese Daten verarbeiten darf.
- Risiken zu Personen und Leistungen von Einzelnen gehören nicht in ein Register, das
  breit verteilt wird.

## Leere Vorlage

| ID | Risiko | Ursache / Trigger | Betroffene Ziele | Eintritt (%) | Schaden (€) | Risikowert (€) | Dringlichkeit | Frühindikatoren | Präventive Maßnahmen | Reaktive Maßnahmen | Owner (Rolle) | Annahmen |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R01 | | | | | | | | | | | | |

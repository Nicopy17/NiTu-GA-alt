# User Journey: Franz erstellt einen Monatsbericht

**Persona:** Franz Weber, 44, Geschäftsführer (siehe [Persona Canvas](../analysis/persona.md))
**Szenario:** Es ist der 3. Werktag nach Monatsende. Die Buchhaltung hat die Oktober-Zahlen als Excel-Datei geschickt.
Franz braucht bis zur Gesellschafterrunde am Nachmittag den aktualisierten Finanzbericht.
**Ziel:** Bericht in ≤ 10 Minuten statt 3–4 Stunden, jede Zahl mit Quelle, Daten bleiben im Unternehmen.

## Heute (ohne NiTu-GA)

| Phase | Was Franz tut | Gefühl | Schmerzpunkt |
|---|---|---|---|
| Auslöser | Excel-Datei der Buchhaltung kommt per Mail | 😐 genervt, „schon wieder“ | Weiß, dass jetzt Stunden Copy-Paste kommen |
| Vorbereiten | Kopiert die .pptx vom Vormonat | 😐 | Dateichaos, welche Version war die letzte? |
| Übertragen | Tippt Zahlen aus Excel/ERP in Folien und Tabellen | 😟 | Stumpfe Arbeit, Angst vor Tippfehlern |
| Diagramme | Baut Diagramme neu und fügt sie ein | 😠 | Layout verrutscht, gefällt ihm danach nicht |
| Prüfen | Vergleicht Zahlen stichprobenartig | 😟 unsicher | Keine Sicherheit, dass alles stimmt |
| Abschluss | Verschickt den Bericht nach 3–4 Stunden | 😮‍💨 erschöpft | Keine Zeit mehr für die eigentliche Auswertung |

## Morgen (mit NiTu-GA)

| # | Phase | Was Franz tut | Berührungspunkt | Was das System tut | Gedanken & Gefühl | Chance / Bezug |
|---|---|---|---|---|---|---|
| 1 | Auslöser | Bekommt die Oktober-Excel von der Buchhaltung | E-Mail | – | „Okay, das geht ja inzwischen schnell.“ 🙂 | Business Case |
| 2 | Vorlage wählen | Öffnet NiTu-GA am Büro-PC und wählt seine gespeicherte Vorlage „Monatsbericht Finanzen“ | Browser, Vorlagenliste | Zeigt gespeicherte Vorlagen mit Vorschau | „Mein Layout ist noch da.“ 🙂 | Functional Overview 1, Bedürfnis „vorhandene Layouts“ |
| 3 | Datenquelle anfügen | Zieht die Excel-Datei ins Fenster | Upload | Liest die Datei, erkennt Blätter und Spalten, meldet unklare Zuordnungen | „Hoffentlich erkennt es die neue Spalte.“ 😐 | Functional Overview 2, Risiko #5 |
| 4 | Zuordnung bestätigen | Bestätigt eine Rückfrage: „Ist ‚Umsatz netto‘ dasselbe wie ‚Nettoumsatz‘?“ | Chat | Merkt sich die Zuordnung für nächsten Monat | „Gut, dass es fragt statt rät.“ 🙂 | Q1 Korrektheit |
| 5 | Auftrag geben | Schreibt: „Baue mir den Finanzbericht für Oktober.“ | Chat | Aktualisiert Zahlen, Tabellen und Diagramme, Layout bleibt gleich, Fließtext nur aus Quelldaten | „Bin gespannt.“ 😐 | Functional Overview 3 und 4 |
| 6 | Prüfen | Fährt über eine Zahl und sieht Datei, Blatt und Zelle | Berichtsvorschau | Zeigt Quellenangabe je Zahl, markiert nicht gefundene Werte | „Ich kann jede Zahl nachprüfen.“ 😊 Vertrauen wächst | Q1, Bedürfnis „Zahl mit Quelle“, Risiko #4 |
| 7 | Korrigieren | Bittet: „Formuliere den Kommentar zum Umsatz kürzer.“ | Chat | Passt nur den Text an, Zahlen bleiben unverändert | „Geht schnell.“ 🙂 | Bedienbarkeit Q3 |
| 8 | Freigabe | Schickt den Entwurf an die Buchhaltung zur Prüfung, diese gibt frei | Freigabe-Funktion | Hält Freigabe fest | „Vier-Augen-Prinzip ist erfüllt.“ 🙂 | Org. Constraint „vor Freigabe prüfen“ |
| 9 | Export | Exportiert den Bericht als bearbeitbares HTML | Export | Erzeugt HTML, öffnet in Browser/Office | „Nach 10 Minuten fertig.“ 😊 | Functional Overview 5, Tech. Constraint HTML |
| 10 | Nachwirkung | Nutzt die gewonnene Zeit für die Auswertung und das Gesellschaftergespräch | – | Löscht Rohdaten nach Auftragsende | „So soll es sein.“ 😊 | Persona-Ziel, Q2 Datenschutz |

## Gefühlskurve

```
Gefühl   😊 |                        ●───────────●───●
         🙂 |  ●───●           ●───●       ●
         😐 |          ●───●
            +--------------------------------------------
              1   2   3   4   5   6   7   8   9   10   Phase
```

## Erkenntnisse

- **Kritischster Moment:** Phase 3–5 (Datenquelle und Auftrag). Erkennt das System die Excel-Struktur falsch oder
  erfindet Zahlen, verliert Franz sofort das Vertrauen. Daraus folgen Epic E2 und E3.
- **Vertrauensanker:** Quellenangabe je Zahl (Phase 6) ist das, was Franz vom Misstrauen gegenüber KI-Tools wegbringt.
- **Keine neuen Tools lernen:** Maximal drei Schritte bis zum Bericht, Bedienung per Chat in Alltagssprache.
- **Abdeckung:** Alle fünf Funktionen aus dem Functional Overview kommen vor (Phasen 2, 3, 5, 9).

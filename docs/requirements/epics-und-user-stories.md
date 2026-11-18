# Epics und User Stories

Abgeleitet aus dem [Functional Overview](../analysis/aic.md#2-functional-overview) und der [User Journey](user-journey.md).
Jedes Epic und jede Story ist ein eigenes GitHub-Issue, die Stories hängen als Sub-Issues am Epic.
Die Akzeptanzkriterien stehen vollständig in den Issues (Format Gegeben / Wenn / Dann).

## Übersicht

| Epic | Functional Overview | User Stories |
|---|---|---|
| [E1 Vorlagen verwalten (#13)](https://github.com/Nicopy17/NiTu-GA/issues/13) | 1 Vorlage auswählen & speichern | US 1.1, US 1.2 |
| [E2 Datenquellen anbinden (#14)](https://github.com/Nicopy17/NiTu-GA/issues/14) | 2 Datenquelle anfügen | US 2.1, US 2.2, US 2.3 |
| [E3 Bericht per Chat erstellen (#15)](https://github.com/Nicopy17/NiTu-GA/issues/15) | 3 Auftrag per Chat, 4 Zahlen aktualisiert / Layout bleibt | US 3.1 bis US 3.4 |
| [E4 Prüfen, freigeben und exportieren (#16)](https://github.com/Nicopy17/NiTu-GA/issues/16) | 5 Export als bearbeitbares HTML | US 4.1, US 4.2, US 4.3 |

## E1 Vorlagen verwalten

| ID | Issue | User Story | Wichtigste Akzeptanzkriterien |
|---|---|---|---|
| US 1.1 | [#17](https://github.com/Nicopy17/NiTu-GA/issues/17) | Als Geschäftsführer möchte ich meinen bisherigen Monatsbericht als Vorlage hochladen und speichern, um jeden Monat mit meinem gewohnten Layout weiterzuarbeiten. | .pptx/.html wird gespeichert und erscheint in der Liste; erkannte Platzhalter werden angezeigt; Vorschau entspricht dem Original |
| US 1.2 | [#18](https://github.com/Nicopy17/NiTu-GA/issues/18) | Als Geschäftsführer möchte ich eine gespeicherte Vorlage mit Vorschau auswählen, um sicher den richtigen Bericht zu aktualisieren. | Liste mit Name, letzter Nutzung, Vorschau; ein Klick führt zu „Datenquelle anfügen“; umbenennen und löschen |

## E2 Datenquellen anbinden

| ID | Issue | User Story | Wichtigste Akzeptanzkriterien |
|---|---|---|---|
| US 2.1 | [#19](https://github.com/Nicopy17/NiTu-GA/issues/19) | Als Geschäftsführer möchte ich die Excel-Datei per Drag-and-drop anfügen, um die Zahlen nicht mehr von Hand übertragen zu müssen. | Blätter und Spalten werden erkannt; Zuordnung Platzhalter zu Zelle sichtbar; verständliche Fehlermeldung bei defekter Datei |
| US 2.2 | [#20](https://github.com/Nicopy17/NiTu-GA/issues/20) | Als Geschäftsführer möchte ich, dass das System bei geänderten Spaltennamen nachfragt und sich die Antwort merkt, um mich auch bei wechselnden Excel-Strukturen auf die Zahlen verlassen zu können. | Rückfrage statt Raten; ohne Bestätigung kein unsicherer Wert im Bericht; bestätigte Zuordnung gilt im Folgemonat |
| US 2.3 | [#21](https://github.com/Nicopy17/NiTu-GA/issues/21) | Als Geschäftsführer möchte ich den CSV-Export aus dem ERP anfügen, um Zahlen direkt aus der Quelle zu nutzen. | Semikolon und Komma als Trennzeichen; deutsche Zahlenformate; Excel und CSV kombinierbar |

## E3 Bericht per Chat erstellen

| ID | Issue | User Story | Wichtigste Akzeptanzkriterien |
|---|---|---|---|
| US 3.1 | [#22](https://github.com/Nicopy17/NiTu-GA/issues/22) | Als Geschäftsführer möchte ich per Chat „Baue mir den Finanzbericht für Oktober“ schreiben, um in wenigen Minuten einen aktuellen Bericht im gewohnten Layout zu bekommen. | Alle Zahlen, Tabellen, Diagramme aktualisiert; Layout unverändert; Entwurf in ≤ 2 min; Gesamtablauf ≤ 10 min |
| US 3.2 | [#23](https://github.com/Nicopy17/NiTu-GA/issues/23) | Als Geschäftsführer möchte ich zu jeder Zahl die Quelle sehen, um dem Bericht zu vertrauen. | Datei, Blatt, Zelle je Zahl; 100 % der Zahlen mit Quelle; berechnete Werte zeigen Formel |
| US 3.3 | [#24](https://github.com/Nicopy17/NiTu-GA/issues/24) | Als Geschäftsführer möchte ich, dass fehlende Werte markiert statt erfunden werden, um sicher zu sein, dass keine falschen Zahlen im Bericht stehen. | Markierung „Wert nicht in der Quelle gefunden“; 0 erfundene Zahlen im Fließtext; Hinweis vor Export |
| US 3.4 | [#25](https://github.com/Nicopy17/NiTu-GA/issues/25) | Als Geschäftsführer möchte ich Texte per Chat anpassen lassen, um den Bericht schnell an meine Aussage anzupassen. | Nur betroffener Abschnitt ändert sich; Zahlen und Layout bleiben; rückgängig machen möglich |

## E4 Prüfen, freigeben und exportieren

| ID | Issue | User Story | Wichtigste Akzeptanzkriterien |
|---|---|---|---|
| US 4.1 | [#26](https://github.com/Nicopy17/NiTu-GA/issues/26) | Als Geschäftsführer möchte ich den Entwurf zur Prüfung und Freigabe schicken, um das Vier-Augen-Prinzip einzuhalten. | Prüfer sieht Quellen; Freigabe oder Zurückweisung mit Kommentar; „Entwurf“-Kennzeichnung; Freigabe wird protokolliert |
| US 4.2 | [#27](https://github.com/Nicopy17/NiTu-GA/issues/27) | Als Geschäftsführer möchte ich den Bericht als bearbeitbares HTML exportieren, um ihn in meiner gewohnten Umgebung weiterzuverwenden. | HTML entspricht der Vorschau; Texte und Zahlen bearbeitbar; öffnet ohne Zusatzsoftware |
| US 4.3 | [#28](https://github.com/Nicopy17/NiTu-GA/issues/28) | Als Geschäftsführer möchte ich, dass Rohdaten nach Auftragsende gelöscht und nie zum Training genutzt werden, um die DSGVO einzuhalten. | Löschung nach 24 h; gespeicherte Daten einsehbar und sofort löschbar; 0 Übertragungen nach außen |

## Abdeckung

| Quelle | Abgedeckt durch |
|---|---|
| Functional Overview 1–5 | E1 bis E4 (siehe Übersicht) |
| Quality Goal Q1 Korrektheit & Nachvollziehbarkeit | US 2.2, US 3.2, US 3.3 |
| Quality Goal Q2 Datenschutz | US 2.1, US 4.3 |
| Quality Goal Q3 Bedienbarkeit | US 1.2, US 3.1, US 3.4 |
| Risiko #4 Halluzination | US 3.3 |
| Risiko #5 Wechselnde Excel-Strukturen | US 2.2 |
| Risiko „lange Laufzeit“ | US 3.1 |
| Org. Constraint „vor Freigabe prüfen“ | US 4.1 |
| Tech. Constraint HTML | US 4.2 |

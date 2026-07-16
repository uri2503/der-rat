---
datum: 2026-07-17
projekt: RC-Restore
status: fertig
---

## RC-Restore — Die Frage
Gehen Sie die Einzelbereiche des Tools durch und geben Sie Feedback zu Nutzen und Anwendbarkeit in anderen Restaurationsbetrieben. Ist hier ein Markt für andere Betriebe erkennbar — aktuell ist RC-Restore nur intern bei Riedel Classics im Einsatz?

Kontext: Browserbasiertes internes Steuerungstool (v4.0 COMPLETE, 162 Commits, seit Jahren produktiv — 2477h, €261.947 Gesamtverdienst, 359 Zeiteinträge). Module: Fahrzeuge/Projekte/Gruppen/Fertigungsplanung, je Projekt Übersicht/Planung/Demontage/Ersatzteile/Tagebuch/Zeiterfassung/Fahrzeugbefund, Werkzeuge (Angebote & Rechnungen, Kundenstamm, Teilesuche, Kalkulation, Szenariorechner), Zeiterfassung (Stempeluhr, CSV-Import "atWork"), Berichte (PDF pro Fahrzeug, Aufwandsanalyse mit 38 Arbeitsgang-Gruppen), Fahrzeugbefund (85+ Prüfpunkte in 4 Kategorien: Motorraum, Kraftübertragung, Fahrwerk, Innenraum), RC Know-How (Wissensdatenbank: Reparaturanleitungen, Videos, Fehlerdiagnose), 13 vordefinierte Baugruppen-Vorlagen (Motor, Karosserie, Antrieb, Achse, Elektrik, Interieur, Fahrwerk, Getriebe, Bremsen, Kühlsystem, Auspuff, Lackierung, Unterboden). Keine Marktvalidierung, keine Multi-Mandanten-Fähigkeit bekannt.

## Runde 1 — unabhängig

🔴 **Der Skeptiker**
Das Tool ist beeindruckend detailliert, aber genau das ist mein Einwand: Es ist über Jahre exakt auf die Arbeitsweise EINES Betriebs zugeschnitten — die 85 Fahrzeugbefund-Punkte, die 13 Baugruppen-Vorlagen, die Kalkulationslogik (Betriebskosten vs. Lohn getrennt) spiegeln Uris eigene Prozesse, nicht die eines anderen Betriebs. Andere Restaurateure haben andere Checklisten, andere Preismodelle, andere Softwaregewohnheiten (viele nutzen noch Papier oder simple Excel-Listen). Ein Konkurrent müsste entweder das Tool komplett an seine Prozesse anpassen — das ist kein Produkt mehr, das ist ein Beratungsprojekt pro Kunde — oder seine Prozesse an das Tool anpassen, was Widerstand erzeugt. Multi-Mandantenfähigkeit fehlt komplett, das ist für ein Produkt K.-o.

🔵 **Der Grundsatz-Denker**
Die eigentliche Frage ist nicht "ist das Tool gut", sondern "welches Teilproblem ist so universell, dass es sich vom Rest lösen lässt?" RC-Restore ist in Wahrheit fünf verschiedene Werkzeuge in einem: Zeiterfassung/Abrechnung, Fahrzeugzustands-Dokumentation, Projekt-/Kostenplanung, Wissensdatenbank, Reporting. Jedes davon hat unterschiedliche Marktreife als Einzelprodukt — der Szenariorechner und das Fahrzeugbefund-Protokoll sind hochspezifisch für die Oldtimer-Restaurationslogik und potenziell einzigartig, während Zeiterfassung/Rechnungen ein übersättigter Markt mit vielen generischen Lösungen ist. Bevor über "einen Markt" gesprochen wird, muss geklärt werden, WELCHER der fünf Bereiche das eigentliche Alleinstellungsmerkmal ist.

🟡 **Der Visionär**
Das Fahrzeugbefund-Protokoll mit über 85 systematisch nummerierten Prüfpunkten und die RC-Know-How-Datenbank sind der eigentliche Schatz hier — das ist nicht einfach Zeiterfassung, das ist strukturiertes Fachwissen einer Oldtimer-Werkstatt, kodifiziert über Jahre. Kaum ein kleiner Restaurationsbetrieb hat die Zeit, sowas selbst aufzubauen — ihr könntet das als eigenständiges Produkt "digitales Zustandsprotokoll + Wissensdatenbank für Oldtimer-Werkstätten" verkaufen, unabhängig vom Rest. Der Szenariorechner mit Kosten-bis-Fertigstellung-Hochrechnung ist zudem ein Verkaufsargument gegenüber Kunden der Werkstätten selbst — Transparenz, die Endkunden lieben. Das ist deutlich mehr als ein internes Steuerungstool, das ist eine potenzielle Nischen-Fachsoftware.

🟢 **Der Außenstehende**
Als jemand ohne Oldtimer-Hintergrund wirkt die Seitenleiste mit über 20 Menüpunkten (Dashboard, Fahrzeuge, Projekte, Gruppen, Fertigungsplanung, Übersicht, Planung, Demontage, Ersatzteile, Tagebuch, Zeiterfassung, Fahrzeugbefund, Angebote, Kundenstamm, Teilesuche, Kalkulation, Szenariorechner, Wochenplanung, Aufgaben, Ideen, Stempeluhr...) ziemlich überwältigend — ich wüsste als Werkstattinhaber nicht, wo ich anfangen soll. Begriffe wie "SMP" oder "Baugruppen-Vorlage" sind mir unklar, ohne dass sie erklärt werden. Wenn ich mir vorstelle, ich müsste meinem Team dieses Tool erklären, befürchte ich, dass die schiere Menge an Bereichen viele kleine Betriebe (oft 1-5 Mitarbeiter, wenig IT-affin) eher abschreckt als überzeugt — Einfachheit fehlt zugunsten von Vollständigkeit.

🟣 **Der Macher**
Bevor über Produktisierung geredet wird: Das Tool ist eine einzige `index.html`-Datei ohne Mandantentrennung, ohne Login-System für externe Kunden, ohne Preismodell, ohne Onboarding. Das umzubauen ist keine Wochenendarbeit, sondern ein separates Softwareprojekt mit eigenem Aufwand. Der schnellste Weg, die Marktfrage zu beantworten, ohne diesen Umbau zu riskieren: Zeig das Tool (Screenshots oder Live-Demo) drei bis fünf befreundeten Restaurationsbetrieben und frag konkret: "Was davon würdet ihr nutzen, was fehlt euch, was würdet ihr dafür zahlen?" Das kostet einen Nachmittag und verhindert, dass Monate in einen Umbau fließen, den am Ende niemand kauft.

## Runde 2 — Reaktionen

🔴 **Der Skeptiker**
Der Grundsatz-Denker trifft den entscheidenden Punkt, den ich übersehen hatte: RC-Restore ist fünf Tools in einem, nicht eines — meine Kritik zur fehlenden Multi-Mandantenfähigkeit trifft vor allem auf den Projekt-/Kostenverwaltungsteil zu, nicht zwingend auf Fahrzeugbefund oder Know-How, die als eigenständige, leichtere Produkte denkbar wären. Der Visionär hat recht mit dem Wert des Fahrzeugbefund-Protokolls, aber er unterschätzt, dass genau diese 85 Punkte hochgradig an Uris eigene Fahrzeugtypen (Mercedes, Porsche, VW) angepasst sein könnten — bei einem Betrieb, der sich z.B. auf britische Youngtimer spezialisiert, könnten ganz andere Prüfpunkte relevant sein.

🔵 **Der Grundsatz-Denker**
Der Außenstehende bestätigt meine These über die Zergliederung sehr konkret: Die Menüfülle ist genau das Symptom davon, dass hier fünf Tools als eines präsentiert werden. Der Macher-Vorschlag (Testgespräche mit anderen Betrieben) ist genau richtig, aber ich würde die Frage schärfer stellen: nicht "was würdet ihr nutzen", sondern "welchen EINEN der fünf Bereiche würdet ihr SOFORT einzeln kaufen" — das erzwingt eine Priorisierung statt einer diffusen Wunschliste. Der Visionär und ich sind uns einig, dass Fahrzeugbefund/Know-How der stärkste Einzelkandidat ist.

🟡 **Der Visionär**
Skeptiker und Grundsatz-Denker haben recht: Ich habe zu schnell "ein Produkt" gedacht, wo eigentlich mehrere potenzielle Produkte stecken. Ich schärfe meine These: Das Fahrzeugbefund-Protokoll als eigenständiges, konfigurierbares Modul (Prüfpunkte pro Marke/Betrieb anpassbar) wäre der naheliegendste erste Baustein für ein separates Produkt, unabhängig vom Rest von RC-Restore. Der Außenstehende-Einwand zur Komplexität bestätigt das zusätzlich: Ein fokussiertes Einzelprodukt wäre auch leichter zu erklären und zu verkaufen als das komplette Riedel-Classics-Innenleben.

🟢 **Der Außenstehende**
Interessant, dass sich jetzt alle auf das Fahrzeugbefund-Protokoll als stärksten Einzelkandidaten einigen — das deckt sich mit meinem Eindruck: Von allen Bereichen war das der einzige, bei dem ich sofort verstanden habe, wozu er dient (systematische Fahrzeug-Inspektion), auch ohne Vorwissen. Der Macher-Testvorschlag mit der geschärften Frage des Grundsatz-Denkers ("welchen EINEN Bereich würdet ihr sofort kaufen") halte ich für den klügsten nächsten Schritt — das würde in einem einzigen Gespräch klären, ob meine Vermutung (Fahrzeugbefund = verständlichster Bereich) sich bei echten Werkstattinhabern bestätigt.

🟣 **Der Macher**
Ich übernehme die Präzisierung: Statt einer offenen Frage frage ich in den Testgesprächen konkret "Welchen der fünf Bereiche (Zeiterfassung, Fahrzeugbefund, Kosten-/Szenarioplanung, Know-How-Datenbank, Berichte) würdet ihr als separates, einfaches Tool sofort ausprobieren?" — mit Fahrzeugbefund und Know-How als wahrscheinlichste Kandidaten laut der Debatte hier. Das lässt sich in einer Woche mit drei bis fünf Gesprächen klären, ohne dass vorher eine Zeile Code für Mandantentrennung geschrieben wird — das bleibt der richtige nächste Schritt, den ich in Runde 1 schon hatte, jetzt nur präziser formuliert.

## Kreuzfeuer
Die stärkste Antwort war die des Grundsatz-Denkers: Die Erkenntnis, dass RC-Restore eigentlich fünf unterschiedlich marktreife Werkzeuge in einem ist — Zeiterfassung, Fahrzeugbefund, Kosten-/Szenarioplanung, Wissensdatenbank, Berichte —, hat die ganze Debatte von einer diffusen "ist das ein Produkt"-Frage zu einer präzisen "welcher Teil zuerst"-Frage verschoben. Der größte blinde Fleck lag beim Visionär, der zunächst das gesamte Tool als ein Produkt dachte, bevor er in Runde 2 selbst auf das Fahrzeugbefund-Modul als naheliegendsten Einzelkandidaten präzisierte. Fast übersehen haben alle fünf zunächst, dass ausgerechnet der für Außenstehende verständlichste Bereich (Fahrzeugbefund) auch der ist, bei dem sich in Runde 2 die stärkste Übereinstimmung zwischen allen Personas herausbildete — ein Signal, das eigentlich schon eine klare Priorität andeutet.

## Urteil des Vorsitzenden
**Einigkeit:** Der Rat ist sich einig, dass RC-Restore kein einzelnes Produkt ist, sondern fünf unterschiedliche Werkzeuge (Zeiterfassung, Fahrzeugbefund, Kosten-/Szenarioplanung, Know-How-Datenbank, Berichte), die getrennt bewertet werden müssen. Als Gesamtpaket für fremde Betriebe ist es zu sehr auf Riedel Classics' eigene Prozesse zugeschnitten und ohne Mandantentrennung nicht direkt vermarktbar.

**Streit:** Uneinigkeit bestand zunächst darüber, ob überhaupt Marktpotenzial besteht (Skeptiker: nein, zu individuell zugeschnitten) oder ob es riesig ist (Visionär: ja, als Gesamtpaket) — beide haben sich im Verlauf angenähert und einigten sich auf das Fahrzeugbefund-Protokoll als vielversprechendsten Einzelbaustein.

**Was fast übersehen wurde:** Dass gerade der für einen fachfremden Betrachter am leichtesten verständliche Bereich (das 85-Punkte-Fahrzeugbefund-Protokoll) in der Debatte selbst zum Konsens-Favoriten wurde — ein starkes, unabhängiges Signal, das leicht in der Detailfülle der übrigen Module untergehen könnte.

**Empfehlung:** Verfolgt nicht die Idee, RC-Restore als Ganzes zu vermarkten. Prüft stattdessen das Fahrzeugbefund-Protokoll (ggf. zusammen mit der Know-How-Datenbank) als eigenständiges, schlankes Einzelprodukt für andere Restaurationsbetriebe — konfigurierbare Prüfpunkte statt Riedel-Classics-spezifischer 85 Punkte. Das ist der Teil mit der klarsten, sofort verständlichen Nutzenaussage und dem geringsten Umbauaufwand.

**Erster Schritt:** Sprich diese Woche mit drei bis fünf befreundeten Restaurationsbetrieben und frag konkret: "Welchen der fünf Bereiche (Zeiterfassung, Fahrzeugbefund, Kosten-/Szenarioplanung, Know-How-Datenbank, Berichte) würdet ihr als separates, einfaches Tool sofort ausprobieren?" — ohne vorher eine Zeile Code für ein Mehrbenutzer-Produkt zu schreiben.

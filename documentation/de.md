<!-- ELUCENIA technical documentation · canadian-c-spine-rule · de · no clinical/professional/rights approval -->

# Canadian C-Spine Rule

[Bedingungen, Quellen und Berechtigungen](https://elucenia.org/de/werkzeuge/canadian-c-spine-rule)

## Verwendung

Verwenden Sie das Werkzeug im Portal oder öffnen Sie index.html über einen lokalen HTTP-Server. Wählen Sie die Sprache, füllen Sie die Felder aus und berechnen Sie das Ergebnis.

## Eingaben und Einheiten

### Ausschlusskriterium: Alter \< 16 Jahre, Glasgow \< 15, abnorme Vitalzeichen, Trauma vor mehr als 48 h, penetrierendes Trauma, akute Lähmung, bekannte Wirbelsäulenerkrankung/frühere Halswirbelsäulenoperation, erneute Beurteilung derselben Verletzung oder Schwangerschaft

`excl`

### Hohes Risiko: Alter ≥ 65 Jahre

`idade65`

### Hohes Risiko: gefährlicher Mechanismus (Sturz ≥ 0,9 m oder 5 Stufen, axiale Belastung des Kopfes, Hochgeschwindigkeitskollision, Überschlag oder Herausschleudern, motorisiertes Freizeitfahrzeug, Fahrradkollision)

`mecanismo`

### Hohes Risiko: Parästhesien der Extremitäten

`parestesia`

### Niedriges Risiko: einfacher Auffahrunfall (kein Stoßen in den Gegenverkehr, kein Aufprall durch Bus/großen Lkw, kein Überschlag oder Hochgeschwindigkeitsaufprall)

`colisao`

### Niedriges Risiko: sitzend in der Notaufnahme

`sentado`

### Niedriges Risiko: irgendwann nach dem Trauma gehfähig

`deambulou`

### Niedriges Risiko: verzögerter Beginn von Nackenschmerzen

`tardia`

### Niedriges Risiko: kein Druckschmerz in der zervikalen Mittellinie

`semdor`

### Aktive Rotation des Halses um 45° nach rechts und links möglich?

`rot`

optional

- `0` — Nein
- `1` — Ja
- `na` — Noch nicht geprüft

### Stumpfes Trauma vor ≤ 48 h; Alter ≥ 16 Jahre, Glasgow 15, normale Vitalzeichen und Einschluss durch Nackenschmerz oder Verletzung oberhalb der Schlüsselbeine + fehlende Gehfähigkeit + gefährlichen Mechanismus bestätigt?

`contexto`

- `0` — Nein
- `1` — Ja

## Fassung der Methode

Stiell 2001; Canadian C-Spine Rule

## Dokumentierte Formel

Abfolge: Ausschlüsse → Hochrisikofaktoren → Vorliegen eines Niedrigrisikofaktors → bereits klinisch beurteilte aktive Rotation.

## Grenzen und Population

Gibt keine Anleitung zu Halsbewegungen. Nicht beurteilte Rotation führt zu einem unvollständigen Ergebnis. Ein fehlendes Kriterium bedeutet nicht, dass keine Verletzung vorliegt.

## Referenzen

- [Stiell et al. · Canadian C-Spine Rule · vollständiger Artikel und Kriterien von 2001](https://jamanetwork.com/journals/jama/fullarticle/194296)

- [Stiell IG et al. The Canadian C-Spine Rule for radiography in alert and stable trauma patients. JAMA, 2001.](https://doi.org/10.1001/jama.286.15.1841)

- [Stiell IG et al. The Canadian C-Spine Rule versus the NEXUS low-risk criteria in patients with trauma. N Engl J Med, 2003.](https://doi.org/10.1056/NEJMoa031375)

## Technische Tests reproduzieren

Führen Sie node test.cjs im Stammverzeichnis dieses Repositorys aus, um die dokumentierten synthetischen Fälle zu wiederholen. Ursprüngliche Eingaben, erwartete Ergebnisse und Toleranzen bleiben erhalten. Technische Tests stellen keine klinische Validierung dar.

```sh
node test.cjs
```

tool.json enthält Quellen, Ausgabe und Umfang der Überprüfung. examples.json bewahrt die synthetischen Eingaben und erwarteten Ergebnisse; results.json dokumentiert die tatsächlich erhaltenen Ergebnisse.

[Eintrag und Referenzen](../tool.json) · [JavaScript-Code](../calculator.js) · [Referenzfälle](../examples.json) · [results.json](../results.json)

## Überprüfung und Nutzungsbedingungen

Eine unabhängige klinische Prüfung wurde nicht durchgeführt.

Diese Benutzeroberfläche ist eine selbst erstellte Übersetzung und keine offizielle oder zertifizierte Ausgabe. Eine unabhängige klinische Überprüfung, eine professionelle sprachliche Prüfung und eine Klärung der Rechte an den Instrumenten wurden nicht durchgeführt.

Ergebnis der Formel oder Klassifikation. Interpretation, Vorgehen und Anwendbarkeit hängen von der fachlichen Beurteilung und der ausgewählten Quelle ab.

## Lizenz und Urheberangaben

Apache-2.0 gilt nur für den ELUCENIA-Code. Die Rechte an Instrumenten, Veröffentlichungen, Übersetzungen und Daten verbleiben bei den jeweiligen Rechteinhabern. Bewahren Sie LICENSE und NOTICE auf.

ELUCENIA · Felipe Guedes · Copyright © 2026

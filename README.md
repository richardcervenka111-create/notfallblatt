# Notfallblatt

Ein Blatt für den Kühlschrank, das dem Rettungsdienst die wichtigsten Antworten gibt:
Medikamente, Allergien, Diagnosen, wer anzurufen ist, wo die Patientenverfügung liegt.
Wird im Browser ausgefüllt und gedruckt. **Nichts wird gesendet, nichts liegt auf einem Server.**

Live: **https://richardcervenka111-create.github.io/notfallblatt/**

## Für wen

Menschen mit Dauermedikation, nach einer Operation, im Alter, mit Demenz; und die
Angehörigen, Spitex-Teams, Hausarztpraxen und Apotheken, die das Blatt mit ihnen ausfüllen.

## Was es macht

- Formular in **DE / FR / IT / EN** (Schweizer Schreibweise, ohne ß), Vorschau live als A4.
- Rote Markierungen für das, was Rettungsdienste zuerst wissen wollen: Blutverdünner,
  Medikamentenallergien, Schrittmacher, Diabetes, Zugang zur Wohnung.
- Medikamententabelle mit Einnahmezeit, Kontakte, Ärztin/Arzt, Apotheke, Spitex,
  Dokumente (Patientenverfügung, Vorsorgeauftrag, Organspende) und wo sie liegen.
- **Drucken / PDF** über den Browser (auch am Handy: Teilen → Drucken). Das Datum steht oben rechts.
- «Auf diesem Gerät merken» ist ein Schalter: standardmässig aus. Eingeschaltet, bleibt der
  Entwurf im lokalen Speicher des Browsers; «Alles löschen» entfernt ihn (zweifach tippen).
- Ohne Eingaben zeigt die Vorschau ein Beispiel («Rosa Muster») mit Wasserzeichen BEISPIEL.

## Drucksachen (`print/`)

- `flyer-A4-de-fr.pdf`: A4, Deutsch vorne, Französisch hinten, für Apotheken, Spitex, Praxen, Angehörige.
- `qr-notfallblatt.svg` / `.png`: QR-Code auf die Live-Adresse (Fehlerkorrektur H).
- `flyer.html`: Quelle des Flyers.

## Datenschutz, technisch

Eine einzige Datei ohne Skripte von Dritten. Die Seite enthält keinen `fetch`, kein
`XMLHttpRequest`, keinen `sendBeacon`; der Deploy-Workflow bricht ab, wenn eines davon
auftaucht. Einzige externe Ressource: eine Schrift von Google Fonts (Atkinson Hyperlegible,
mit System-Fallback). Wer auch das nicht will, entfernt die zwei `<link>`-Zeilen.

## Anpassen für eine andere Stadt oder Sprache

Alle Texte stehen im Objekt `I18N` in `index.html`. Notrufnummer 144 steht in `s_sub`.
Lizenz CC0: nehmen, ändern, weitergeben, ohne Nennung.

## Verwandt

[Bärn hilft](https://github.com/richardcervenka111-create/baern-hilft): Reanimationstakt,
Notrufnummern, nächster Defibrillator, Trinkwasser, WC in Bern.

# Palabra a Palabra

Flashcard-app om Spaanse woorden te leren, met herhaalschema, uitspraak en inspreken. Het is een statische website zonder server of database. De voortgang staat in de browser van elke telefoon.

## Bestanden

| Bestand | Wat |
|---|---|
| `index.html` | De app |
| `woorden.csv` | De woordenlijst (bewerkbaar in Excel) |
| `icon.png`, `icon-512.png`, `apple-touch-icon.png` | App-icoon (1024, 512 en 180 px), illustratie door Studio Me |
| `mascot.jpg` | Illustratie op het eindscherm van een ronde |
| `manifest.webmanifest` | Naam en icoon voor "Zet op beginscherm" |

## Online zetten met GitHub Pages (eenmalig, ±10 minuten)

1. Log in op github.com en klik op **New repository**.
2. Naam: `palabra`. Zet hem op **Public**: GitHub Pages is alleen gratis voor openbare repositories. Klik op **Create repository**.
3. Klik op **uploading an existing file** en sleep alle bestanden uit deze map erin. Klik op **Commit changes**.
4. Ga naar **Settings → Pages**. Kies bij *Source* **Deploy from a branch**, en daarna branch **main** en map **/ (root)**. Klik op **Save**.
5. Na 1 à 2 minuten staat de app op `https://<gebruikersnaam>.github.io/palabra/`.

## Op de iPhone zetten

Open de link in **Safari** en kies **Deel → Zet op beginscherm**. Gebruik daarna steeds dat icoon: de voortgang wordt per browser bewaard.

## Woorden bijwerken

- Open `woorden.csv` in Excel. De kolommen zijn: `spaans`, `engels`, `onderwerp`, `voorbeeld`, `voorbeeld_nl` en `tip`. Alleen de eerste twee zijn verplicht. Heet de tweede kolom `nederlands`, dan toont de app NL in plaats van EN.
- Sla op als **CSV UTF-8**. Gewone CSV verminkt de accenten (á, ñ, ¿).
- Upload het bestand opnieuw in de repository (**Add file → Upload files**). Binnen een minuut staat de nieuwe lijst online.
- Let op: de voortgang hangt aan het Spaanse woord. Pas je de Spaanse spelling aan, dan begint dat woord opnieuw.

## App-icoon vervangen

Lever één tekening aan als **vierkante PNG van 1024 × 1024 px**:

- **Achtergrond:** volledig gevuld, niet transparant (iOS maakt transparantie zwart).
- **Hoeken:** recht. iOS rondt ze zelf af.
- **Compositie:** het belangrijkste binnen het middelste deel, met ±10% ruimte aan de randen.
- **Eenvoud:** grote, eenvoudige vormen. Het icoon wordt op de telefoon maar ±60 px groot.

Maak daarvan `icon.png` (1024), `icon-512.png` (512) en `apple-touch-icon.png` (180) en vervang de bestanden. Een icoon dat al op het beginscherm staat, ververst pas als je het verwijdert en opnieuw toevoegt.

## Inspreken

Inspreken gebruikt de ingebouwde spraakherkenning van de browser (Spaans, es-ES) en staat onder **Instellingen → Woorden inspreken**.

- **Wat het doet:** het controleert of het herkende woord klopt. Het beoordeelt niet hoe goed je uitspraak is.
- **iPhone:** Dicteren moet aanstaan (Instellingen → Algemeen → Toetsenbord → Dicteer).
- **Werkt het niet vanaf het beginscherm-icoon?** Gebruik dan dezelfde link in Safari.

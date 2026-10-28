# SVG Icon Guide — Face Prompt Builder (Teil 5, neue Frisur-Kacheln)

Icons für das neue Feld **Hairstyle / „Frisur"** — 20 Kacheln (2026-Trend-Schnitte). Die Kategorie rendert bereits als Kachel-Grid, alle 20 Kacheln sind aktuell **ohne Icon** (nur Label). Sobald eine Kachel gezeichnet ist, einfügen: die anderen dürfen leer bleiben, bis sie dran sind. Gleiche Optik wie Teil 1–4 (viewBox 32, `stroke-width 1.2`).

## SVG Characteristics

Jedes Icon ist ein standalone SVG im **Line-Art-Stil** (nur Striche, keine Flächen):

| Attribut | Wert | Bedeutung |
|---|---|---|
| `xmlns` | `http://www.w3.org/2000/svg` | nötig für standalone Dateien |
| `viewBox` | `0 0 32 32` | 32×32 Zeichenfläche |
| `fill` | `none` | keine Fläche füllen — nur Konturen |
| `stroke` | `currentColor` | Farbe aus CSS erben (standalone = schwarz) |
| `stroke-width` | `1.2` | Strichstärke (Detail-Striche: `1.1`–`1.3`) |
| `stroke-linecap` | `round` | abgerundete Strichenden |
| `stroke-linejoin` | `round` | abgerundete Ecken |

### Template

```svg
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 32 32" fill="none" stroke="currentColor" stroke-width="1.2" stroke-linecap="round" stroke-linejoin="round">
  <!-- hier zeichnen -->
  <path d="M4 16 Q16 6 28 16 Q16 26 4 16 Z"/>
</svg>
```

### Zeichen-Regeln

- **Randabstand**: Form zwischen ca. `2` und `30` zeichnen — sonst schneidet der Strich (1.2 px) am Rand ab.
- **Basis-Motiv fast immer derselbe Kopf**: Kreis/Oval (Kopf) + Haar-Form drumherum — 32 px ist klein, dicke Formen, wenige Details.
- **Kopf-Position** als Referenz: Kopfoval ca. `cx 16, cy 17, rx 7.5, ry 9` (wie die bestehenden hairLength-Icons) — Haarform immer relativ dazu zeichnen.
- **Schnittlänge erkennen lassen**: die Unterlinie des Haars (Kinn / Ohr / Schulter / Kragen) ist die wichtigste Information — sauber eine Linie.
- **Locken/Wellen**: 2–3 Bögen (`Q`-Kurvendellen) reichen, nicht über 4.
- **Asymmetrie**: bei Asymmetrischer Schnitt eine Seite deutlich kürzer zeichnen — das ist die Aussage, kein Zeichenfehler.
- **Stirnhaar (Curtain bangs)**: zwei auseinanderfallende Strähnen über der Stirn (V-Form) — nicht eine gerade Linie (das wäre Blunt bangs).
- **Dateiname**: `hairstyle_` + Label-Slug (siehe Tabelle unten).
- **Prüfen**: Datei im Browser öffnen — schwarz auf transparent muss sichtbar sein.

## Labels (20)

### 1. Hair (20)

#### hairstyle (20) — „Frisur / Hairstyle“

| # | English Label | Dateiname | Motiv |
|---|---|---|---|
| 1 | Pixie cut | `hairstyle_pixie_cut.svg` | Kurz gescheitelt: Haar endet über den Ohren, schräger Abschnitt zur Seite, etwas Volumen oben |
| 2 | Bixie | `hairstyle_bixie.svg` | Zwischen Pixie und Bob: kurz an den Seiten, hinten bis zum Kinn, federig nach oben geöffnet |
| 3 | French bob | `hairstyle_french_bob.svg` | Kinn-langer Bob mit gerader, dichter Stirnhaar-Linie (gerade Fringe) + glatte Seiten |
| 4 | Blunt bob | `hairstyle_blunt_bob.svg` | Kinn- bis Ohrlanger Bob, perfectly gerade Unterlinie (keine Wellen), keine Fringe |
| 5 | Micro bob | `hairstyle_micro_bob.svg` | Sehr kurz: Haar endet deutlich unter den Ohren / am Hinterkopf, rund um den Kopf, glatt |
| 6 | Wavy bob | `hairstyle_wavy_bob.svg` | Kinnlanger Bob mit 2–3 Wellenbögen an der Unterlinie |
| 7 | Collarbone lob | `hairstyle_collarbone_lob.svg` | Langer Bob bis zur Schulter/Keyhole: gerade bis leicht abgerundete Unterlinie, Länge bis „Schulter“-Höhe (tiefer als Blunt bob) |
| 8 | Wolf cut | `hairstyle_wolf_cut.svg` | Stark gestuft: spitz zulaufende, zerzauste Spitzen (oben länger, an den Seiten keilförmig abgenommen) |
| 9 | Shag cut | `hairstyle_shag_cut.svg` | Mehrere sichtbare Ebenen (3–4 gestufte Bögen) + kurze Fringe oben |
| 10 | Butterfly cut | `hairstyle_butterfly_cut.svg` | Gesichterahmende lange Strähnen, die wie Flügel nach außen fallen (V-Form am Kinn), innen kurz gestuft |
| 11 | Layered cut | `hairstyle_layered_cut.svg` | Langes Haar mit 3–4 parallelen Stuf-Linien (Ebenen) entlang der Länge |
| 12 | Asymmetrical cut | `hairstyle_asymmetrical_cut.svg` | Eine Seite deutlich kürzer/schärfer geschnitten als die andere (Schrägschnitt) |
| 13 | Feathered cut | `hairstyle_feathered_cut.svg` | Federn-artig nach innen gekämmte feine Strähnen (2–3 Bögen, die sich zum Gesicht biegen) |
| 14 | Hime cut | `hairstyle_hime_cut.svg` | Japanisch: gerade, scharf geschnittene Fringe + zwei gerade Gesichtssträhnen am Kinn + langer, glatter Rest |
| 15 | Curtain bangs | `hairstyle_curtain_bangs.svg` | Mittelscheitel: zwei Strähnen fallen in einem V auseinander und rahmen die Stirn/ Augen |
| 16 | Beach waves | `hairstyle_beach_waves.svg` | Langes, locker welliges Haar: weiche, unregelmäßige Wellenbögen, Mittel- oder Seitenscheitel |
| 17 | Loose curls | `hairstyle_loose_curls.svg` | Lockeres Locken-Volumen: 4–5 kleine Rundungen (C-Form) um den Kopf |
| 18 | Messy bun | `hairstyle_messy_bun.svg` | Oberer/unterer Dutt als unordentlicher Knoten (2–3 kreisförmige Bögen) + 2–3 lose Strähnen am Hals |
| 19 | High ponytail | `hairstyle_high_ponytail.svg` | Hoher Pferdeschwanz: Strähnen laufen zur oberen Mittellinie zusammen, Schweif fällt nach unten |
| 20 | Half-up half-down | `hairstyle_half_up_half_down.svg` | Oberes Haar festgebunden (kleiner Knoten/Bow oben), unteres Haar offen und lang |

## Zusammenfassung

| Kategorie | Icons |
|---|---|
| hairstyle | 20 |
| **Gesamt** | **20** |

Dateiordner: `/mnt/2TB_SAM_850/LM Studio python/face_prompt_builder_icons_teil5/`

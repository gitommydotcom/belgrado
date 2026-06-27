# Belgrado & Adriatico — Manuale di stile

Guida per ricreare il design del sito in stampa (fotolibro delle vacanze).
Tutti i valori sono presi 1:1 dal CSS del sito. I **CMYK sono indicativi**:
fai sempre un soft‑proof con il profilo della tua tipografia/carta.

> **Anima del progetto.** Un “dossier di viaggio” editoriale e caldo: carta color
> crema, verde pino come colore guida, accenti ambra e terracotta, titoli in
> grazie e tutto il resto in un grottesco pulito. Metafore di viaggio (biglietto,
> cartelli, pallini-timeline). Molto respiro, bordi sottili, ombre leggere.

---

## 1. Palette colori

### Colori base / neutri
| Ruolo | Nome | HEX | RGB | CMYK ~ |
|---|---|---|---|---|
| Sfondo pagina (crema) | paper | `#F4F0E6` | 244, 240, 230 | 0 · 2 · 6 · 4 |
| Superficie secondaria | paper‑2 | `#FBF8F1` | 251, 248, 241 | 0 · 1 · 4 · 2 |
| Superficie / card | card | `#FFFFFF` | 255, 255, 255 | 0 · 0 · 0 · 0 |
| Testo principale | ink | `#16241F` | 22, 36, 31 | 39 · 0 · 14 · 86 |
| Testo secondario | ink‑soft | `#4A5953` | 74, 89, 83 | 17 · 0 · 7 · 65 |
| Linee / bordi | line | `#E2DACB` | 226, 218, 203 | 0 · 4 · 10 · 11 |

### Colori guida e accenti
| Ruolo | Nome | HEX | RGB | CMYK ~ |
|---|---|---|---|---|
| Verde pino (primario) | pine | `#0E4A43` | 14, 74, 67 | 81 · 0 · 9 · 71 |
| Verde salvia (accento) | pine‑2 | `#2C7A6F` | 44, 122, 111 | 64 · 0 · 9 · 52 |
| Verde chiaro (wash) | teal‑wash | `#E4EFEA` | 228, 239, 234 | 5 · 0 · 2 · 6 |
| Ambra | amber | `#D8913A` | 216, 145, 58 | 0 · 33 · 73 · 15 |
| Ambra chiara (wash) | amber‑wash | `#F6EAD3` | 246, 234, 211 | 0 · 5 · 14 · 4 |
| Terracotta | clay | `#BC4F36` | 188, 79, 54 | 0 · 58 · 71 · 26 |
| Terracotta chiara (wash) | clay‑wash | `#F4E2D8` | 244, 226, 216 | 0 · 7 · 11 · 4 |
| Verde mare (gradiente) | sea‑2 | `#1E8C82` | 30, 140, 130 | 79 · 0 · 7 · 45 |

### Colori su fondo scuro (testo/etichette negli header)
- Testo chiaro su pino: `#EAF2EF` · su ambra/terracotta: `#FBF3E6`
- Etichette tenui su pino: `#9FC4BC` · su mare: `#A6D0C8` · su valigia: `#F6E2C8`

### Gradienti degli header
- **Gargano (mare):** lineare 150° → `#0E4A43` 0% · `#15756B` 58% · `#1E8C82` 100%
  con “sole” radiale ambra `rgba(216,145,58,.95)` in alto a destra.
- **Valigia (caldo):** lineare 150° → `#D8913A` 0% · `#C9722F` 55% · `#B7472F` 100%.

### Regole d’uso del colore
- **Fondo = crema (`paper`)**, mai bianco pieno per le pagine; il bianco è solo per le card.
- Verde **pino** = colore guida (titoli forti, pill, marker “da vedere”).
- Ogni accento ha la sua **versione “wash”** (chiarissima) usata come sfondo di etichette/badge, con il colore pieno come testo.
- Ambra = energia/sole (bullet, prezzi). Terracotta = compleanno/avvisi/“barca”.

---

## 2. Tipografia

Due famiglie, entrambe gratuite (Google Fonts, licenza SIL Open Font License 1.1, ok anche per uso commerciale e stampa).

- **Display / titoli / numeri:** **Instrument Serif** — pesi 400 (regular) e *400 italic*. È una grazia editoriale dal contrasto alto; usala grande.
- **Testo / UI / didascalie:** **Inter** — pesi 400, 500, 600, 700.

Base: **16 px**, interlinea **1.65**, colore `ink`. Antialiasing attivo.

### Scala tipografica
| Elemento | Font | Dimensione (px) | Peso | Stile | Colore | Tracking | Interlinea |
|---|---|---|---|---|---|---|---|
| Titolone copertina | Instrument Serif | 40 → 74 (responsive) | 400 | regular/italic | ink (em in pine‑2) | – | 1.1 |
| Titolo header Gargano/Valigia | Instrument Serif | 42 → 66 | 400 | regular | testo chiaro | – | .95 |
| Titolo sezione `h2` | Instrument Serif | 28 → 40 | 400 | regular | ink | – | 1.1 |
| Numero sezione | Instrument Serif | 30 | 400 | regular | pine‑2 | – | 1 |
| Sottotitolo (subhead) | Instrument Serif | 24 | 400 | regular | ink | – | – |
| Titolo card/giornata | Instrument Serif | 24–26 | 400 | regular | ink | – | 1.05 |
| Codici biglietto (FCO/BEG) | Instrument Serif | 54 (40 mobile) | 400 | regular | testo chiaro | .01em | .9 |
| Occhiello (eyebrow) | Inter | 12 | 600 | maiuscolo | pine‑2 | .16em | – |
| Etichetta blocco | Inter | 11 | 700 | maiuscolo | pine‑2 | .10em | – |
| Corpo / paragrafo | Inter | 14–16 | 400 | – | ink / ink‑soft | – | 1.55–1.65 |
| Testo card | Inter | 13.5 | 400 | – | ink‑soft | – | 1.55 |
| Titolo card | Inter | 15.5 | 600 | – | ink | – | – |
| Voce navigazione / pulsante | Inter | 13–14 | 500–600 | – | ink‑soft / chiaro | – | – |
| Tag / badge | Inter | 9.5–10 | 700 | maiuscolo | colore accento | .04–.06em | – |
| Kicker (sopra titolo) | Instrument Serif | 15 | 400 | *italic* | ink‑soft | – | – |

Regola pratica: **se è un titolo o un numero → Instrument Serif; tutto il resto → Inter.** Gli occhielli e i tag sono sempre **maiuscoletto Inter con tracking ampio**.

---

## 3. Griglia, margini, spaziature

- **Larghezza colonna di testo:** max **920 px**, margini laterali **20 px** (su carta: gabbia centrata con margini generosi, vedi §8).
- **Ritmo delle sezioni:** padding verticale **40 px**, separate da una **linea 1 px `line`** in alto.
- **Raggi di arrotondamento:** pill/etichette `999px` · card `12–16px` · header/biglietto `20px` · modale `18px` · pulsanti `7–12px`.
- **Ombra standard:** `0 1px 2px rgba(22,36,31,.04)` + `0 8px 24px rgba(22,36,31,.06)` (molto morbida, mai dura).
- **Spazio tra card in griglia:** 14 px. Griglie a riempimento automatico, colonna minima ~220–260 px.

---

## 4. Iconografia

Stile **a tratto (line icons)**: viewBox 24×24, `stroke = colore corrente`, spessore **2 px** (1.5 px per le filigrane), estremità e giunzioni **arrotondate**, nessun riempimento. È lo stile di **Lucide / Feather** — usa quelle per ricreare tutto.

Icone usate (con equivalente Lucide):
- Viaggio/sezioni: aereo *(plane)*, palma/pino *(palm/trees)*, valigia *(luggage/briefcase)*, auto *(car)*.
- Giorno per giorno: orologio *(clock)*, stella-scintilla *(sparkle/star)*, alba *(sunrise)*, sole *(sun)*, luna *(moon)*.
- Azioni: spunta *(check)*, matita *(pencil)*, cestino *(trash)*, più *(plus)*.
- Consigli: scudo, taxi, banca, monete, caffè, posata, nota musicale, goccia, presa, smartphone, bus, chiesa, fumetto, luna, onde, barca, pesce, sole, ombrellone, “P” parcheggio.

---

## 5. Componenti (ricette)

### Pill / etichetta (tag)
Fondo = *wash* dell’accento, testo = accento pieno. `font 10px/700 maiuscolo`, tracking `.06em`, padding `2×7px`, raggio `6px`.
Semantica colori:
- **Critico** → clay‑wash / clay · **Importante** → amber‑wash / `#9A6519` · **Utile** → teal‑wash / pine
- **Tag tema** giorno‑per‑giorno: Storia/Relax/Natura → teal‑wash/pine · Mare → `#DCEAF0`/`#1C5E78` · Cibo/Shopping → amber‑wash/`#9A6519` · Notte/Avventura → clay‑wash/clay
- **Etichette valigia:** Valigia BG → teal‑wash/pine · Mare·auto → amber‑wash/`#9A6519` · A mano → clay‑wash/clay

### Pill data (giornata)
Fondo **pino**, testo `#EAF2EF`, `11px/700 maiuscolo` tracking `.08em`, padding `4×11px`, raggio `999px`. (Compleanno → fondo terracotta.)

### Pulsante a pillola (navigazione)
Bordo `1px line`, fondo `paper‑2`, testo `ink‑soft`. **Attivo:** fondo pino, testo chiaro. Raggio `999px`, padding `10×14px`.

### Card
Fondo bianco, bordo `1px line`, raggio `14px`, padding `16×18px`. Hover: solleva di 2 px + ombra. Titolo Inter 15.5/600; eventuale prezzo in pine‑2 13/600; testo 13.5 ink‑soft.

### Riga checklist
Card bianca, bordo line, raggio 14. Casella **24×24**, raggio 7, bordo `2px #C9CFC9`; **spuntata** = fondo pino + ✓ chiara, testo barrato e attenuato (opacità .55).

### Card “giornata” (il cuore)
Card bianca. In alto: **pill data** + (eventuale badge Oggi/Compleanno) + titolo in grazie 26.
- **In programma**: etichetta blocco + lista con **pallino ambra 6px** a sinistra, orari in grassetto.
- **Idee per voi**: etichetta blocco con contatore; voci raggruppate per **Mattina/Pomeriggio/Sera** (icona alba/sole/luna ambra). Ogni idea è una mini‑card su `paper‑2`, bordo line, raggio 12, con tag‑tema a destra.

### Header “biglietto” (Belgrado)
Card **pino** piena, raggio 20. Layout a biglietto aereo: due codici grandi in grazie (54px) con città sotto in maiuscoletto `#9FC4BC`, freccia tratteggiata al centro. **Perforazione**: linea tratteggiata `rgba(234,242,239,.32)` con due tacche circolari (Ø 26px) color crema ai lati. In basso una riga di dati (etichetta tenue + valore chiaro).

### Header “board” (Gargano) e “valigia”
Card a **gradiente** (vedi §1), raggio 20. Struttura: occhiello + grande titolo in grazie + frase introduttiva + **3 “fatti”** in chip semitrasparenti (`rgba(255,255,255,.10–.13)`, bordo `rgba(255,255,255,.18)`, icona + valore in grassetto + sottotesto). Decori: “sole” radiale ambra e onde per il Gargano; filigrana valigia per la valigia.

### Accordion (consigli)
Card bianca, bordo line, raggio 13. Riga: icona pine‑2 + titolo 15/600 + chevron che ruota all’apertura. Testo aperto: 14 ink‑soft, rientrato sotto l’icona.

### Tabella (frasario)
Card bianca, righe separate da `1px line`. Colonne: italiano (ink) · serbo (pine, 500) · pronuncia (*italic* ink‑soft).

### Mappa (se la stampi)
Tiles OpenStreetMap (attribuzione obbligatoria: “© OpenStreetMap contributors”). Marker = **cerchi pieni** Ø~18px, bordo bianco 2px:
- Casa base → terracotta `#BC4F36` · Da vedere → pino `#0E4A43` · Mangiare → ambra `#D8913A` · In barca → salvia `#2C7A6F`.

---

## 6. Indicazioni per la stampa / fotolibro

**Carta.** Interno **uncoated** (opaco) avorio/crema per richiamare `#F4F0E6` — evita carta bianca brillante, “spegnerebbe” la palette. Grammatura interni ~150–170 g.

**Colore.** Lavora i testi in **nero ricco verde** partendo da `ink #16241F`; il verde pino è il colore guida di tutto il libro. Converti gli HEX con il profilo della tua carta (i CMYK in §1 sono un punto di partenza) e **soft‑proof**: i verdi profondi e l’ambra virano facilmente in stampa.

**Margini & abbondanza.** Gabbia con margini generosi (consigliati 15–20 mm), **bleed 3–5 mm** su foto e fondi colore a vivo. Mantieni il “respiro” del sito: meglio meno elementi e più aria.

**Gerarchia da replicare.**
- Titoli grandi in **Instrument Serif**; corpo, occhielli, didascalie e tag in **Inter**.
- Didascalie foto: Inter 9–10 pt, `ink‑soft`. Occhielli di sezione: Inter maiuscoletto, tracking ampio, pine‑2.
- Bullet/elenchi cronologici: **pallino ambra**. Numeri di sezione in grazie, pine‑2.

**Elementi ricorrenti riutilizzabili (danno coerenza al libro):**
- Il **“biglietto” pino** come copertina o come divisore di capitolo (Belgrado vs Gargano vs Casa).
- Le **pill data** per marcare le giornate nelle pagine diario.
- Le **card bianche** con bordo sottile `#E2DACB` su fondo crema per box, mappe, menù, frasi.
- Header a **gradiente mare/ambra** come aperture di sezione a tutta pagina.

**Trattamento foto.** Luce naturale, ora dorata, toni caldi; riduci i blu freddi. Per i divisori puoi usare **duotone pino+ambra** o un velo crema in sovrimpressione per fondere le foto con lo sfondo. Mantieni qualche pagina “bianca crema” solo testo: il vuoto fa parte dello stile.

---

## 7. Risorse

- **Instrument Serif** — Google Fonts · SIL OFL 1.1 · https://fonts.google.com/specimen/Instrument+Serif
- **Inter** — Google Fonts · SIL OFL 1.1 · https://fonts.google.com/specimen/Inter
- **Icone** — Lucide (stile a tratto, 2px, arrotondato) · https://lucide.dev
- **Mappe** — © OpenStreetMap contributors (attribuzione obbligatoria se usi le mappe).

---

*Estratto dal CSS del sito “Belgrado & Adriatico · 13–19 luglio 2026”. I valori HEX/RGB sono esatti; i CMYK sono indicativi e vanno adattati in fase di soft‑proof.*

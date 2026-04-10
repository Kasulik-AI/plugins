---
name: ülevaade
description: "Iganädalane AI töökeskkonna ülevaade — mis läks hästi, mida parandada, järgmise nädala fookus, alakasutatud skillide tuvastamine, memory uuendamine. Kasuta kui kasutaja kirjutab '/ülevaade' või mainib: weekly review, nädala kokkuvõte, check in, kuidas mul läheb, weekly reflection, ülevaade."
---

# /ülevaade — Iganädalane Kokkuvõte

Struktureeritud 15-minutiline refleksioon, mis parandab su AI töökeskkonda aja jooksul.

## Enne Alustamist

1. Loe CLAUDE.md ärikonteksti ja praeguse setup'i kohta
2. Loe MEMORY.md ja hiljutised memory-failid — mis on õpitud
3. Kontrolli millised Kasulik pluginad on installeeritud

---

## Ülevaate Voog

### Samm 1: Võidud (2 min)

Küsi: "Mis läks sel nädalal AI-ga hästi? Kas oli ülesandeid kus see säästis reaalselt aega või andis suurepärase tulemuse?"

Kuula:
- Konkreetsed skillid mis töötasid hästi → kinnista need memory'sse
- Töövood mis klõpsusid → märgi muster üles
- Enesekindluse kasv → tunnusta seda

Salvesta võidud memory'sse kui need sisaldavad taaskasutatavaid teadmisi.

### Samm 2: Raskused (3 min)

Küsi: "Kus jäi AI sel nädalal alla? Kas oli frustratsioone või ülesandeid kus väljund polnud kasulik?"

Diagnoos:
- Kas probleem oli promptimises? → Õpeta lahendust
- Kas kasutati vale skilli? → Soovita paremat
- Kas puudus kontekst? → Soovita CLAUDE.md uuendamist
- Kas see oli AI reaalne piiratus? → Tunnista ausalt ja paku alternatiive

### Samm 3: Avastamine (3 min)

Nende rolli ja tegevuste põhjal soovita 1-2 skilli, mida nad pole proovinud:

"Sinu sel nädalal tehtud töö põhjal võiksid need kasulikud olla:
- **[skilli nimi]**: [üks lause miks see sobib nende olukorraga]
- Kas tahad et näitan kuidas see töötab kiire näitega?"

Soovita AINULT installeeritud pluginate skille.

### Samm 4: Töökeskkonna Tervis (3 min)

Kontrolli ja soovita parandusi:

- **CLAUDE.md**: Kas on veel ajakohane? Kas lisada uut konteksti?
- **Memory**: Kas on uusi teadmisi, mida tasub salvestada? Kas on aegunud memory'sid?
- **Töövood**: Kas on korduvaid ülesandeid, mis peaksid saama töövoo retseptiks?
- **Kohandatud skill**: Kui neil pole, kas on aeg see luua?

### Samm 5: Järgmine Nädal (2 min)

Küsi: "Mis on su suurim prioriteet järgmisel nädalal? Las soovitan kuidas AI saab aidata."

Kaardista nende vastus konkreetsete skillidega ja paku miniplaani.

### Samm 6: Uuendamine

Vestluse põhjal:
1. Uuenda asjakohaseid memory-faile
2. Soovita CLAUDE.md muudatusi kui vaja (näita diff, lase kasutajal kinnitada)
3. Salvesta kõik avastatud uued töövoomustrid

---

## Väljundformaat

Lõpeta lühikese kokkuvõttega:

```
## Nädala Ülevaade — {kuupäev}

**Võidud**: {1-2 bullet kokkuvõte}
**Parandatud**: {mida parandati või õpiti}
**Proovi järgmisel nädalal**: {1-2 skilli soovitust koos põhjendusega}
**Töökeskkonna uuendused**: {mida muudeti CLAUDE.md-s või memory's}
```

## Ajastamine

Seda ülevaadet saab seadistada ajastatud ülesandena. Soovita:
"Kas tahad et seadistan selle iganädalase check-in'ina? Saan selle panna jooksma igal reedel su tööpäeva lõpus."

Kui scheduled-tasks MCP on saadaval, kasuta seda korduva ülesande loomiseks.

## Põhimõtted

- **Tähista enne kritiseerimist** — alusta alati võitudega
- **Üks parandus korraga** — ära ülekoormata 5 soovitusega
- **Konkreetne, mitte abstraktne** — "Proovi /tekst oma Acme turunduspostituseks" mitte "uuri rohkem skille"
- **Kasutaja dikteerib tempot** — mõned nädalad on kergemad, see on ok
- **Ehita harjumust** — järjepidevus loeb rohkem kui sügavus

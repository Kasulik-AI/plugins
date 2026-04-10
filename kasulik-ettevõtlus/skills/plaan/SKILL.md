---
name: plaan
description: "Loo strateegilisi plaane — konkurentsianalüüs, SWOT, tegevuskava, hooajaplaan Kasuta kui kasutaja kirjutab '/plaan' või mainib seotud teemasid."
---

# /plaan — Strateegilised Plaanid

Loo struktureeritud strateegilisi plaane oma ettevõtte arendamiseks.

## Plaani tüübid

- **Strateegiline plaan** — aasta eesmärgid, SMART kriteeriumid, KPI-d
- **Tegevuskava** — konkreetsed sammud koos tähtaegade ja vastutajatega
- **Konkurentsianalüüs** — turupositsioon, eristuvus, võimalused
- **SWOT analüüs** — tugevused, nõrkused, võimalused, ohud
- **Hooajaplaan** — kõrg-, vahe- ja madalhooaja strateegiad
- **Arengusuunad** — uued teenused, turud, partnerid

## Kuidas see töötab

1. Küsin, millist plaani vajad
2. Kogun konteksti (CLAUDE.md + lisaküsimused)
3. Loon struktureeritud plaani koos prioriteetidega
4. Pakun mõõdikuid edu jälgimiseks

## Mida ma sinult vajan

- Plaani tüüp ja ajaperiood
- Kontekst: mis on praegune seis, kuhu tahad jõuda
- Piirangud: eelarve, meeskond, aeg

## Näited

```
/plaan strateegiline plaan 2026. aastaks
/plaan konkurentsianalüüs meie piirkonna majutusettevõtted
/plaan tegevuskava sügishooaja turunduseks
/plaan SWOT analüüs
```

---

## Strateegilise Plaani Raamistik

### Konkurentsianalüüsi Mall

```markdown
## Konkurentsianalüüs: [Turg/Segment]

### Konkurendid
| Konkurent | Tugevused | Nõrkused | Positsioneerimine | Hinnatase |
|-----------|-----------|----------|-------------------|-----------|

### Võrdlusmaatriks
| Omadus | Meie | Konkurent A | Konkurent B |
|--------|------|-------------|-------------|
| [Omadus 1] | ✅/❌ | ✅/❌ | ✅/❌ |

### Strateegilised Järeldused
- **Meie eristuvus:** [Mida teeme teisiti/paremini]
- **Ohud:** [Kus konkurendid on tugevamad]
- **Võimalused:** [Mida keegi veel ei tee]
- **Soovitused:** [Konkreetsed tegevused]
```

### SWOT Analüüsi Mall

```markdown
## SWOT: [Ettevõte/Projekt]

| Tugevused (S) | Nõrkused (W) |
|---------------|-------------|
| [Sisemised positiivsed] | [Sisemised negatiivsed] |

| Võimalused (O) | Ohud (T) |
|----------------|----------|
| [Välised positiivsed] | [Välised negatiivsed] |

### Strateegia maatriks
- **SO (kasuta tugevusi + võimalusi):** [Tegevus]
- **WO (ületa nõrkusi võimalustega):** [Tegevus]
- **ST (kasuta tugevusi ohtude vastu):** [Tegevus]
- **WT (minimeeri nõrkusi ja ohte):** [Tegevus]
```

### Tegevuskava Mall

```markdown
## Tegevuskava: [Eesmärk]

### Prioriteet 1: [Nimi]
- **Mida:** [Tegevus]
- **Kes:** [Vastutaja]
- **Millal:** [Tähtaeg]
- **Edukriteerium:** [Kuidas teame et õnnestus]
- **Ressursid:** [Mida vaja]

### Mõõdikud
| KPI | Algväärtus | Sihtväärtus | Tähtaeg |
|-----|-----------|-------------|---------|
```

### Põhimõtted

- **Konkreetne > üldine** — "Kasvatame broneeringuid 20% Q3-ks" mitte "kasvatame äri"
- **Vähem prioriteete** — max 3-5 peamist fookust. Kõik on prioriteet = mitte midagi pole
- **Mõõdetav** — iga eesmärk peab olema numbriliselt jälgitav
- **Ajakohane** — seotud konkreetse perioodiga, mitte "kunagi"
- **Realistlik** — arvesta reaalsete ressurssidega (meeskond, eelarve, aeg)

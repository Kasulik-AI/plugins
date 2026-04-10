---
name: kontekst
description: "Seadista oma ettevõtte turunduskontekst — sihtrühm, positsioneerimine, konkurendid ja brändi hääl Kasuta kui kasutaja kirjutab '/kontekst' või mainib seotud teemasid."
---

# /kontekst — Turunduse Alustala

Seadista oma ettevõtte turunduskontekst, et kõik turundus- ja müügiskillid töötaksid sinu äri kontekstis.

## Kuidas see töötab

1. **Kogun infot** — küsin su ettevõtte kohta ja uurin veebilehte
2. **Analüüsin** — tuvestan sihtrühma, positsioneerimise ja brändi hääle
3. **Salvestan** — loon turunduskonteksti faili, mida teised skillid kasutavad

## Mida ma sinult vajan

- Ettevõtte nimi ja veebileht (kui on)
- Mida pakud ja kellele
- Mis sind konkurentidest eristab

Ülejäänu uurin ise välja su veebilehelt ja küsin täpsustusi.

## Väljund

Loon `.claude/product-marketing-context.md` faili, mis sisaldab:
- **Positsioneerimine** — mida pakud, kellele, miks just sina
- **Sihtrühm** — ideaalkliendi profiilid ja nende vajadused
- **Konkurendid** — peamised konkurendid ja sinu eristuvus
- **Brändi hääl** — toon, stiil, sõnavara
- **Väärtuspakkumine** — selge sõnastus kliendikasust

→ Seejärel kasutavad /tekst, /meilid ja teised skillid seda konteksti automaatselt.

---

## Turunduskonteksti Mall

Loodav `.claude/product-marketing-context.md` fail järgib seda struktuuri:

```markdown
# [Ettevõtte nimi] — Turunduskontekst

## Positsioneerimine
**Mida:** [Mis toode/teenus]
**Kellele:** [Kelle jaoks]
**Miks just meie:** [1-2 lauset mis eristab]

## Ideaalklient (ICP)

### Segment 1: [Nimi]
- **Kes:** [Demograafia, roll, suurus]
- **Probleem:** [Mida nad lahendada üritavad]
- **Motivaator:** [Mis neid liigutab]
- **Takistus:** [Mis hoiab tagasi]
- **Keel:** [Sõnad mida nad kasutavad oma probleemi kirjeldamiseks]

### Segment 2: [Nimi]
[Sama struktuur]

## Konkurendid

| Konkurent | Tugevus | Nõrkus | Kuidas eristume |
|-----------|---------|--------|-----------------|

## Brändi Hääl

### Toon
[2-3 omadussõna, nt "professionaalne aga sõbralik, praktiline"]

### Keele reeglid
- **Kasutame:** [sõnad ja väljendid]
- **Ei kasuta:** [väldi neid]
- **Näide heast toonist:** "[näide]"
- **Näide halvast toonist:** "[näide]"

## Väärtuspakkumine

### Ühe lausega
[Selge lause mis vastab: mida sa teed, kellele, ja miks see oluline on]

### Peamised kasud
1. [Kasu 1] — [Miks see kliendile oluline]
2. [Kasu 2] — [Miks see kliendile oluline]
3. [Kasu 3] — [Miks see kliendile oluline]

### Tõestuspunktid
- [Numbriline tõestus, nt "500+ klienti"]
- [Sotsiaalne tõestus, nt "TripAdvisor 4.8/5"]
- [Autoriteeditõestus, nt "10 aastat kogemust"]
```

### Protsess

1. **Küsi alust** — ettevõtte nimi, veebileht, tegevusala
2. **Uuri veebilehte** — kasuta WebSearch/WebFetch et ammutada kontekst
3. **Täpsusta intervjuuga** — küsi mida veebilehelt ei leidnud
4. **Genereeri ja valideeri** — näita kasutajale enne salvestamist
5. **Salvesta** — kirjuta `.claude/product-marketing-context.md`

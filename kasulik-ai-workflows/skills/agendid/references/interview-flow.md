# Intervjuu voog — AI Assistendi Loomine

## Üldpõhimõtted

- Kasuta AskUserQuestion tööriista IGA küsimuse jaoks
- Üks teema korraga — ära küsi kõike korraga
- Paku multiple-choice valikuid + "Muu" vabatekst
- Kohanda järgmist küsimust eelmise vastuse põhjal
- Kui kasutaja jätab midagi vastamata, märgi see "täiendamist vajab" ja liigu edasi

## Küsimus 1: Ettevõte ja väärtuspakkumine

**Küsimus**: Räägi oma ettevõttest — mis on nimi, mida te teete, ja mis teid eristab?

**Valikud (ettevõtte tüüp):**
- Teenindusettevõte (konsultatsioonid, koolitused, teenused)
- Toode (füüsiline toode, tootmine)
- SaaS / tarkvara
- E-kaubandus
- Turism ja majutus
- Vabakutse / freelance
- Muu (kirjelda)

**Edasine loogika:**
- Turism → aktiveeri turismispetsiifilised küsimused (hooajalisus, teenused, booking)
- SaaS → aktiveeri tehniline terminoloogia küsimused
- E-kaubandus → aktiveeri tootekataloogi küsimused

## Küsimus 2: Teenused ja tooted

**Küsimus**: Nimeta oma peamised teenused või tooted. Mis on hinnavahemik ja mis on kõige populaarsem?

**Valikud (teenuste arv):**
- 1-3 põhiteenust
- 4-10 teenust/toodet
- 10+ ulatuslik kataloog
- Muu (kirjelda)

**Edasine loogika:**
- 1-3 → küsi detailsemalt iga teenuse kohta
- 10+ → küsi kategooriaid ja top-3 teenust

## Küsimus 3: Sihtrühm

**Küsimus**: Kes on sinu ideaalne klient? Kus nad asuvad?

**Valikud (kliendi tüüp):**
- B2B (ettevõtted)
- B2C (eraisikud)
- Mõlemad
- Muu

**Valikud (geograafia):**
- Kohalik (linn/maakond)
- Üle-Eestiline
- Baltimaad
- Euroopa
- Rahvusvaheline

**Edasine loogika:**
- B2B → küsi ettevõtte suuruse ja valdkonna kohta
- Turism → küsi päritoluriikide ja hooajaliste erinevuste kohta

## Küsimus 4: Brändi hääletoon

**Küsimus**: Milline on sinu brändi toon? Mis sõnu või väljendeid tuleks VÄLTIDA?

**Valikud (toon):**
- Professionaalne ja ekspertne
- Sõbralik ja ligipääsetav
- Lõbus ja energiline
- Inspireeriv ja motiveeriv
- Luksuslik ja eksklusiivne
- Maalähedane ja aus
- Muu (kirjelda)

**Lisaküsimus**: Kas sul on näidet tekstist, mis kõlab "nagu sina"?
(Vaba teksti väli — veebilehe link, postituse näide, jne)

## Küsimus 5: Meeskond ja terminoloogia

**Küsimus**: Kes on võtmeisikud, keda AI peaks tundma? Kas teil on sisetermineid või lühendeid?

**Valikud (meeskonna suurus):**
- Üksi / solopreneur
- 2-5 inimest
- 6-20 inimest
- 20+ inimest
- Muu

**Edasine loogika:**
- Üksi → jäta meeskonna rollid vahele, fokuseeri terminoloogiale
- 6+ → küsi osakondade ja võtmeisikute kohta

## Küsimus 6: AI töövood

**Küsimus**: Milliste ülesannetega peaks AI sind peamiselt aitama? Mis võtab praegu kõige rohkem aega?

**Valikud (vali mitu):**
- Turunduse sisu loomine (sotsiaalmeedia, blogi, uudiskirjad)
- Müügitekstid ja pakkumised
- Klienditeeninduse vastused
- Strateegia ja planeerimine
- Aruandlus ja analüüs
- E-kirjad ja kommunikatsioon
- Dokumentatsioon ja protsessid
- Muu (kirjelda)

## Küsimus 7: Platvorm

**Küsimus**: Millisel platvormil sa peamiselt AI-d kasutad? Milliste eksportide jaoks vajad väljundit?

**Valikud (platvorm):**
- Cowork (Claude desktop app)
- Claude Code (terminal)
- ChatGPT
- Claude.ai (veebiversioon)
- Mitu platvormi

**Valikud (eksport):**
- Ainult Cowork/Claude Code (Project Instructions + CLAUDE.md + memory/)
- + ChatGPT GPT eksport
- + Claude.ai Projects eksport
- Kõik kolm

## Küsimus 8: Lisakontekst

**Küsimus**: Mis on veel oluline, mida ma ei küsinud? Kas on midagi spetsiifilist, mida AI peaks kindlasti teadma?

**Valikud:**
- Kõik oluline on juba öeldud
- Jah, lisan veel infot (vaba tekst)

## Pärast intervjuud

Koosta kokkuvõte ja esita kinnitamiseks:

```
## Kokkuvõte sinu AI assistendi jaoks

**Ettevõte**: [nimi] — [1-lauseline kirjeldus]
**Tüüp**: [ettevõtte tüüp]
**Teenused**: [top teenused]
**Sihtrühm**: [segmendid]
**Toon**: [hääletoon]
**Meeskond**: [võtmeisikud]
**AI ülesanded**: [valitud valdkonnad]
**Platvorm**: [valitud platvormid]
**Eksportid**: [valitud formaadid]

**Valitud ekspertrollid**: [nimekiri]

Kas see on korrektne? Kas on midagi, mida muuta?
```

# Memory/ Kausta Struktuur ja Mallid

## Kausta struktuur

```
memory/
├── glossary.md                    # Terminoloogia sõnastik
├── context/
│   ├── company.md                 # Ettevõtte täiskirjeldus
│   ├── brand-voice.md             # Brändi hääl + näidistekstid
│   ├── target-audience.md         # Sihtgrupi detailne profiil
│   └── services.md                # Teenuste/toodete täiskirjeldus
├── people/                        # Meeskonnaliikmete profiilid
│   ├── [nimi-1].md
│   └── [nimi-2].md
└── projects/                      # Aktiivsed projektid
    ├── [projekt-1].md
    └── [projekt-2].md
```

## glossary.md mall

```markdown
# Terminoloogia sõnastik

## Ettevõttesisesed terminid

| Termin | Tähendus | Kontekst |
|--------|----------|----------|
| [TERMIN] | [SELGITUS] | [Kus/millal kasutatakse] |

## Valdkonna terminid

| Termin | Tähendus | Kontekst |
|--------|----------|----------|
| [TERMIN] | [SELGITUS] | [Kus/millal kasutatakse] |

## Lühendid

| Lühend | Täistähendus |
|--------|-------------|
| [LÜHEND] | [SELGITUS] |
```

## context/company.md mall

```markdown
# [ETTEVÕTTE NIMI] — Ettevõtte kirjeldus

## Ülevaade
[2-3 lõiku ettevõttest: ajalugu, missioon, visioon]

## Väärtuspakkumine
[Mida pakute, miks see on väärtuslik, mis eristab]

## Ärimudel
[Kuidas raha teenite: tuluvood, hinnastamine, kliendisegmendid]

## Peamised numbrid
- Asutatud: [AASTA]
- Meeskond: [SUURUS]
- Teenindusala: [GEOGRAAFIA]
- Aastakäive: [KUI TEADA]

## Väärtused
[Ettevõtte põhiväärtused]
```

## context/brand-voice.md mall

```markdown
# Brändi hääl ja kommunikatsioon

## Hääletoon
[DETAILNE KIRJELDUS: milline bränd kõlab, kuidas räägib]

## Keelereeglid
- Pöördumisviis: [sina/teie]
- Keel: [eesti/inglise/mõlemad]
- Stiil: [formaalne/mitteformaalne]

## Hea teksti näited
[3-5 NÄIDET tekstidest, mis kõlavad "nagu meie"]

## Väldi
[NIMEKIRI: sõnad, väljendid, toonid, mida mitte kasutada]

## Kanalipõhised erinevused
- Veebileht: [toon]
- Sotsiaalmeedia: [toon]
- E-kirjad: [toon]
- Ametlikud dokumendid: [toon]
```

## context/target-audience.md mall

```markdown
# Sihtrühma profiil

## Segment 1: [NIMI]
- **Kirjeldus**: [Kes nad on]
- **Demograafia**: [Vanus, sugu, sissetulek, asukoht]
- **Vajadused**: [Mida otsivad]
- **Valupunktid**: [Mis probleem neil on]
- **Otsustuskriteeriumid**: [Mille põhjal valivad]
- **Kanalid**: [Kust nad infot saavad]
- **Osakaal**: [~% käibest/klientidest]

## Segment 2: [NIMI]
[Sama struktuur]
```

## context/services.md mall

```markdown
# Teenused ja tooted

## [TEENUS 1]
- **Kirjeldus**: [Detailne kirjeldus]
- **Hind**: [Hind/vahemik]
- **Kestus**: [Kui asjakohane]
- **Sihtrühm**: [Kellele sobib]
- **Eripärad**: [Mis teeb eriliseks]
- **Hooajalisus**: [Kui asjakohane]

## [TEENUS 2]
[Sama struktuur]
```

## people/[nimi].md mall

```markdown
# [NIMI]

- **Roll**: [Ametinimetus]
- **Vastutusala**: [Mille eest vastutab]
- **Kontakt**: [E-post, telefon — kui jagatud]
- **Märkused**: [Mis on oluline teada]
```

## projects/[projekt].md mall

```markdown
# [PROJEKTI NIMI]

- **Staatus**: [Käimas / Plaanis / Lõpetatud]
- **Periood**: [Algus — lõpp]
- **Eesmärk**: [Mida saavutatakse]
- **Vastutaja**: [Kes juhib]
- **Märkused**: [Oluline kontekst]
```

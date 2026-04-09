---
description: "Loo personaalne AI assistent — intervjuu, skaneerimine, kihistatud väljund"
argument-hint: "<ettevõtte URL või nimi>"
---

# /agendid — AI Assistendi Loomine

Loo oma ettevõttele personaalne AI assistent, mis tunneb sinu äri, brändi ja meeskonda.

## Mida see loob

- **Project Instructions** — AI käitumisreeglid ja ekspertrollid
- **CLAUDE.md** — Operatiivmälu (teenused, terminid, meeskond)
- **memory/ kaust** — Süvateadmised (täiskirjeldused, brändi hääl, sihtgrupid)
- **ChatGPT eksport** — Ühe-faili juhis GPT loomiseks
- **Claude Projects eksport** — Juhis Claude.ai projektidele

## Kuidas see töötab

1. **Allikate tuvastamine** — Kas on URL, faile, MCP ühendusi?
2. **Intervjuu** — 5-8 küsimust sinu ettevõtte kohta (valikutega)
3. **Automaatne skaneerimine** — Veebisait, dokumendid, Slack jne
4. **Analüüs** — Kokkuvõte kinnitamiseks
5. **Genereerimine** — Kõik failid korraga
6. **Esitlemine** — Lingid, juhised, järgmised sammud

## Mida ma sinult vajan

- Ettevõtte veebisait (URL) — kui on
- Paar minutit küsimustele vastamiseks
- Kinnitust enne lõplikku genereerimist

## Näited

```
/agendid https://minuettevote.ee
/agendid Minu Hotell OÜ
/agendid
```

Ilma argumendita alustab kohe intervjuuga.

## Olemasoleva uuendamine

Kui sinu workspace'is on juba CLAUDE.md ja memory/ kaust, pakun nende uuendamist
(mitte üle kirjutamist). Nii saad lisada uusi teenuseid, meeskonnaliikmeid või projekte.

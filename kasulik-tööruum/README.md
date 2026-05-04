# kasulik-tööruum

AI töökeskkonna seadistamine, coaching, AI assistentide loomine ja töövood VKE-dele. Kasulik AI SMB Skills Collection'i alusplugin.

## Quick Start

Käivita `/alusta` — see tuvastab praeguse oleku ja kohandub vastavalt:
- **Uus tööruum?** → Juhendatud seadistamine 5–10 minutiga
- **Põhiseadistus tehtud?** → Süvendamise ja kohandamise pakkumine
- **Juba seadistatud?** → Coaching-režiim koos skillide soovitustega

## Käsud

| Käsk | Kirjeldus |
|------|-----------|
| `/alusta` | Tark alguspunkt — seadistamine, parendamine või coaching töökeskkonna oleku põhjal |
| `/agendid` | AI assistendi loomine — intervjuu, automaatne skaneerimine, kihistatud väljund |
| `/ai-coach` | Õige skilli leidmine, töövoogude soovitused, parem promptimine |
| `/töövood` | 15 eelseadistatud mitmeskillset töövoogu levinud äriülesannete jaoks |
| `/ülevaade` | Iganädalane 15-minutiline ülevaade AI kasutuse parendamiseks |
| `/tabel` | Exceli ja CSV failide analüüs |
| `/wordpress` | WordPress MCP integreerimise juhend |

## Skillid

### alusta
Adaptiivne sisseelamine: tuvastab töökeskkonna oleku ja juhendab edasi — uue seadistamine, olemasoleva süvendamine või coaching.

### agendid
AI assistendi loomine ja treenimine: 6-faasiline töövoog (intervjuu → automaatne skaneerimine → süntees → genereerimine → esitlus), mis loob kihistatud AI tööruumi — Project Instructions + CLAUDE.md + memory/ kaust + ChatGPT GPT eksport + Claude Projects eksport.

### ai-coach
Pidev coaching: leiab õige skilli iga ülesande jaoks, õpetab töövoo retsepte, parandab promptimist ja ehitab strateegilist AI enesekindlust.

### töövood
15 eelseadistatud mitmeskillset töövoogu levinud äriülesannete jaoks (turundus, müük, operatsioonid, strateegia, andmeanalüüs).

### ülevaade
Struktureeritud iganädalane ülevaade: tähistab võite, diagnoosib raskusi, soovitab uusi skillide proovimisi ja hoiab töökeskkonna konteksti värske.

### tabel
Exceli ja CSV failide analüüs Claude'iga — laadi üles, küsi, visualiseeri, ekspordi.

### wordpress
WordPress veebilehe ühendamine Claude'iga — samm-sammuline juhend MCP ühenduseks, sisu haldamiseks, SEO optimeerimiseks.

## Töötab kõige paremini koos

See plugin on disainitud töötama koos teiste Kasulik AI pluginatega:
- **kasulik-turundus** — 8 turundusskilli (kontekst, tekst, meilid, SEO, reklaam, kampaania, hind, käivitus)
- **kasulik-müük** — 5 müügiskilli (kõnekokkuvõte, klient, ettevalmistus, pöördumine, prospekt)
- **kasulik-strateegia** — 5 strateegiaskilli (plaan, aruanne, protsess, kasv, konkurent)
- **kasulik-turism** — 9 turismiettevõttele suunatud skilli

`/ai-coach` skill teab kõikide pluginate skillidest ja soovitab õiget igaks ülesandeks.

*Ehitatud [Kasulik AI](https://kasulik.ai) poolt — praktiline AI koolitus ettevõtetele.*

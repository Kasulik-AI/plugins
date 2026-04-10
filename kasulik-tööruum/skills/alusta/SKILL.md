---
name: alusta
description: "Start here — set up your AI workspace or get coaching to improve it. Kasuta kui kasutaja kirjutab '/alusta' või mainib: set up workspace, new project, configure Claude, alusta, seadista, uus projekt, tööruumi seadistamine."
---

# /alusta — AI Töökeskkonna Seadistamine

See käsk kohandub vastavalt sinu praegusele seisule: uus kasutaja saab täieliku setup'i,
olemasolev kasutaja saab täiustamisvõimalused.

## Samm 0: Olemasoleva Tuvastamine (KRIITILINE)

**ENNE midagi loomist kontrolli ALATI:**

1. `CLAUDE.md` — kas eksisteerib juurkaustas?
2. `.auto-memory/MEMORY.md` — kas eksisteerib?
3. `memory/` kaust — kas eksisteerib?
4. `.claude/settings.json` — kas on juba konfigureeritud?

**Kui MIDAGI eksisteerib → ÄRA LOO UUESTI.**
→ Näita kasutajale mis juba olemas on
→ Paku ainult: täiendamine, uuendamine, ülevaade
→ Küsi kinnitust ENNE igasugust muutmist

**Kui mitte midagi ei eksisteeri → Täielik seadistamine (allpool)**

## Marsruutimine

| Seis | Tegevus |
|------|---------|
| 🆕 CLAUDE.md puudub | → Täielik seadistamine (Quick Setup) |
| 🔧 CLAUDE.md olemas, aga baasne | → Täiustamisrežiim |
| 🚀 CLAUDE.md + memory + skill olemas | → Suuna /ai-coach skillile |

---

## Täielik Seadistamine (Quick Setup — 5-10 min)

### Samm 1: Põhiintervjuu

Küsi ÜKS küsimus korraga. Kasuta valikvastuseid kus võimalik.

1. "Mis on su ettevõtte/projekti nimi?"
2. "Mida su ettevõte teeb? (ühe lausega)"
3. "Kas sul on veebileht, mida saan uurida?" → Kui jah, kasuta WebSearch/WebFetch:
   - Mida ettevõte teeb
   - Sihtrühma signaalid
   - Tooted/teenused
   - Tooni ja keele mustrid
4. "Mis on su roll?" (asutaja, turundusjuht, tegevjuht, müük jne)
5. "Milleks sa peamiselt AI-d kasutad?" (valikvastused: turundus/sisu, müük, protsessid, strateegia, kõik)

### Samm 2: Genereeri CLAUDE.md

Kasuta malli [references/claude-md-template.md](references/claude-md-template.md).

Kirjuta `CLAUDE.md` projekti juurkausta. Sisalda:
- Ärikontekst (nimi, tegevus, sihtrühm)
- Kasutaja roll ja peamised kasutusjuhud
- Tooni/hääle juhised veebilehe uuringu põhjal
- Installeeritud Kasulik pluginad ja nende põhiskillid
- Kiirviide: "X jaoks proovi Y skilli"

### Samm 3: Loo Memory-failid

Loo `.auto-memory/` kaust:

**MEMORY.md** (indeks):
```markdown
- [Ärikontekst](user_business.md) — {ettevõte} ülevaade, sihtrühm, positsioneerimine
- [Kasutajaprofiil](user_profile.md) — {nimi}, {roll}, peamised AI kasutusjuhud
```

**user_business.md**:
```markdown
---
name: Ärikontekst
description: {ettevõte} — {ühe lausega mida teevad}
type: user
---
{Intervjuust ja veebilehe uuringust saadud detailid}
```

**user_profile.md**:
```markdown
---
name: Kasutajaprofiil
description: {nimi}, {roll} — kasutab AI-d {peamised kasutusjuhud}
type: user
---
{Roll, kogemustase, eesmärgid}
```

### Samm 4: Paku Süvaseadistamist

Pärast quick setup'i valmimist küsi:

"Sinu tööruum on valmis! Kas tahad minna sügavamale?
1. **Loo kohandatud skill** — su ettevõtte spetsiifilised töövood (10-15 min)
2. **Seadista töövoo retseptid** — igapäevaste ülesannete automatiseerimine (5 min)
3. **Praegu piisab** — saad alati /alusta uuesti käivitada"

---

## Süvaseadistamine: Kohandatud Skill

Kui kasutaja valib valiku 1:

1. Laiendatud intervjuu töövoogude kohta:
   - "Kirjelda tüüpilist töönädalat — mis ülesanded korduvad?"
   - "Millist sisu lood kõige sagedamini?"
   - "Milliseid otsuseid teed regulaarselt, kus AI saaks aidata?"
   - "Kas on terminoloogiat, malle või protsesse, mis on su äri jaoks unikaalsed?"

2. Loo kohandatud skill `skills/{ettevõtte-nimi}-töövood/SKILL.md`:
   - Ettevõttespetsiifiline terminoloogia ja kontekst
   - Levinumad ülesandemallid (e-kirja formaadid, aruannete struktuurid jne)
   - Otsustusraamistikud nende valdkonnale
   - Viited product-marketing-context'ile kui see eksisteerib

3. Nimeta skill `{ettevõtte-nimi}-töövood` (nt `acme-töövood`)

## Süvaseadistamine: Töövoo Retseptid

Kui kasutaja valib valiku 2:

Loe [ai-coach skill'i viited](../ai-coach/references/workflow-recipes.md) ja esita 3-5 kõige relevantsemad retseptid kasutaja rolli ja kasutusjuhtude põhjal. Salvesta valitud retseptid memory'sse.

---

## Täiustamisrežiim (CLAUDE.md juba olemas)

Näita mis juba olemas on ja paku valikuid:

1. **Süvenda konteksti** — uuenda CLAUDE.md täiendava äridetailiga
2. **Loo kohandatud skill** — ehita su äri spetsiifilised töövood
3. **Õpi töövoo retsepte** — avasta multi-skill töövood igapäevasteks ülesanneteks
4. **Saa coaching'ut** — promptimise ja itereerimise nipid → suuna /ai-coach

---

## Põhimõtted

- **Üks küsimus korraga** — ära dumbi vormi
- **Uuri enne küsimist** — kui annavad URL-i, ammuta sealt mida saad enne lisaküsimusi
- **Näita progressi** — kasuta TodoWrite et setup-sammud oleksid jälgitavad
- **Mõistlikud vaikeväärtused** — kui kasutaja jätab küsimuse vahele, kasuta uuringu põhjal vaikeväärtusi
- **Lõpeta alati järgmise sammuga** — "Proovi küsida mult [konkreetne ülesanne nende rollile]"
- **Eesti äridele:** küsi kas eelistavad eesti- või ingliskeelset väljundit

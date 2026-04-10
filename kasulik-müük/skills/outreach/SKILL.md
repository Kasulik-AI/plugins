---
name: outreach
description: "Uuri prospekti ja koosta personaalne pöördumine — e-kiri, LinkedIn sõnum, järelkontakt. Kasuta kui kasutaja mainib: outreach, pöördumine, kirjuta kiri, cold email, külm kiri, LinkedIn sõnum, müügikiri, kontakti pöördumine, draft outreach, reach out, write cold email, personaalne kiri, müügipöördumine, prospektile kirjutamine, esimene kontakt."
---

# Personaalne müügipöördumine (Outreach)

## Töövoog

```
┌─────────────────────────────────────────────┐
│ SAMM 1: UURING (Research)                   │
│ • Prospekti äritausta uurimine              │
│ • LinkedIn, ettevõtte veebisait, Crunchbase│
│ • Otsing "XX äri + XXX teemad"              │
│ • Samatööliste/partnerlite asukohtade leidmine │
│ • CRM andmed (kui saadaval)                 │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│ SAMM 2: KIRJUTAMINE (Message Drafting)      │
│ • Kontekstiga AIDA mudel (Attention,        │
│   Interest, Desire, Action)                 │
│ • Vaakumi-valitud mallid (Soojad/külmad)   │
│ • Personaalse detaili kasutamine            │
│ • 3-5 lauseline struktuur e-kirjadele       │
│ • LinkedIn sõnumid 2-3 lausega (lühemad)   │
└──────────────────┬──────────────────────────┘
                   │
┌──────────────────▼──────────────────────────┐
│ SAMM 3: SAATMINE (Delivery)                 │
│ • E-posti saatmise ühendamine (Gmail, etc.)│
│ • LinkedIn sõnumi kopeerimise täpsus        │
│ • Järelkontaktide ajastamine                │
│ • Vastuste jälgimine ja logimine            │
└─────────────────────────────────────────────┘
```

## Sisendid

Kasutaja peab andma:

- **Prospekti nimi ja/või ettevõte** (nt: "Jaan Tamm, TechCorp OÜ")
- **Pöördumise tüüp**: 
  - `cold` — esimene kontakt (täiesti uus)
  - `warm` — ühine sidemees või tuttav teema
  - `re-engagement` — varasem kontakt, mille soovitakse taasalustada
  - `post-event` — pärast konverentsi/webinari
- **Teie rolli/ettevõtte teave** (nt: "Müügidirektor, kasulik.ai")
- **Pakutava väärtuse tuumik** (nt: "müügipipe arvutamine, B2B pöördumiste automatiseerimine")
- **Soovitud väljund**: 
  - `email` — kogu e-kiri
  - `subject` — ainult teemarida
  - `linkedin` — LinkedIn sõnum
  - `followup` — järelkontakt
  - `all` — kõik versioonid

## Kasutamise näited

**Näide 1: Külm e-kiri (cold email)**
```
Kasutaja: "Kirjuta külm kiri TechCorp OÜ müügidirektorile Jaan Tammele. 
Meie teen B2B müügide automatiseerimist. Lisaks tema LinkedIn profiil näitab, 
et ta otsib müügiteamide juhtimise lahendusi."

Väljund: Täielik e-kiri koos teemaridaga
```

**Näide 2: LinkedIn sõnum (warm)**
```
Kasutaja: "Tee LinkedIn sõnum Kertu Käosele (Brand_Co müügijuht). 
Me jagame ühise tuttava – Mart, kes töötas Brand_Co-s. 
Müügipipe analüüsist räägiksin."

Väljund: 2-3 lauseline LinkedIn DM
```

**Näide 3: Järelkontakt (follow-up)**
```
Kasutaja: "Tee järelkontakt e-kiri. Esimene e-kiri saadeti eile. 
Ei ole veel vastust. Sobiks mingid uued argumendid mainitamiseks?"

Väljund: Mitte-agressiivne järelkontakt
```

## Väljundi mall

Väljund on alati struktuuritud järgmiselt:

```yaml
type: [email | linkedin | subject | followup]
persona: "[Prospekti roll ja ettevõte]"
tone: "[professional | casual | urgent | curious]"
content: |
  [Tegelik sõnum]
tips:
  - Nõuanne 1
  - Nõuanne 2
next_step: "[Mida teha, kui saatmine on tehtud]"
```

## Mallid erinevate stsenaariumide jaoks

### 1. KÜLM E-KIRI (Cold Email)

**Struktuur**: Tähelepanu → Ühine punkt → Väärtus → Tegevuspalve → Allkiri

```
Teemarida: [Äkitsus + personaalne detailid]

Tere [Nimi],

[TÄHELEPANU: Kiire, intrigeeriv lause, miks sa oled seal otsustaja]
Näide: "Nägin, et Brand_Co ei ole veel [teema] digitaliseerinud."

[HUVI: Miks see oluline on]
Näide: "Paljud sarnased ettevõtted annavad praegu ~30% müügivõimalusi käest..."

[SOOV: Konkreetne lahendus, mitte üldiselt]
Näide: "Aitame teil [konkreetne tulemus] 60 päevaga [tõendatud meetod abil]."

[TEGEVUS: 1-2 selge sammu]
- "Kas oleksite avatud 15 min rääkimiseks neljapäeval?"
- "Saadetud link —uurige [millised väärtused] ja öelge, mis teie jaoks kehtib."

Tervitused,
[Teie nimi + ühendusinfo]
```

**Anti-mustriad**:
- Ärge kirjutage "Lihtsalt tahtsin jõuda..." (näitab, et te ei uurinud)
- Ärge kasutage üldisi fraase ("Teie ettevõte on suurepärane")
- Ärge kirjutage liiga pikka esimest lauset

---

### 2. SOOJEM E-KIRI (Warm Email – ühine sidemees)

```
Teemarida: [Ühise tuttava nimi] soovitas teil räägida [teema]

Tere [Nimi],

[ÜHINE SIDEMEES]
"[Ühine tuttav] andis teie kontakti ja mainis, et vaatate praegu [teema]."

[LÜHIKE KONTEKST – Miks räägib ühine tuttav?]
"[Tuttav] teab, et aitame [tüüp ettevõtteid] [konkreetne tulemus]."

[PERSONAALNE DETAILIDE LISAMINE]
"Nägin teie [LinkedIn / veebileht], et te olete hiljuti [tähtis sündmus]. 
Selle taustal teadsime, et [ühendus teemaga]."

[VÄÄRTUS]
"Võiksime teid abistaada [konkreetne tulemus] – [meetod või ajaline raam]."

[TEGEVUS]
"Kas oleksite avatud 15 min telefonikõnele [päev]?"

Tervitused,
[Teie nimi]
```

---

### 3. LINKEDIN SÕNUM (Warm – lühike ja sisukas)

```
Tere [Nimi], 

[Ühine tuttav] andis sulle soovituse. 👋 Vaatame, kuidas B2B müügikanaleid optimeeritakse – tundus, et see on su fokusala.

15 min kõnele?

—[Teie nimi]
```

---

### 4. JÄRELKONTAKT (Follow-up – 3-5 päeva pärast)

```
Teemarida: Re: [Algne teemarida]

Tere [Nimi],

Teadsin, et inimesed on kiirused. 😊 Lihtsalt tahtsin veelkord öelda: 
meil on 3-5 ettevõtet teie suuruses, kes näivad olevat [teema] osas takerdunud.

Kui teil on 2 minutit, saadetud on link [ressursile] – võib aidata.

Edu,
[Teie nimi]
```

---

### 5. PÄRAST ÜRITUST (Post-Event – konverents, webinar)

```
Teemarida: Tore sinuga rääkida [ürituse nimi]

Tere [Nimi],

Meeldis, kuidas sa rääkisid [spetsiifiline punkt] konverentsi paneelis. 
Teie ärinägemus [millal] sobib tegelikkuga, mida me teeme.

Kui sa oled avatud, saatsime artikli [teemast] – kas seda arvustad?

Chat soon,
[Teie nimi]
```

---

## Stilistilised reeglid

1. **Personaalse detaili nõue**
   - Iga pöördumine peab sisaldama vähemalt ühte faktiliselt kontrollitud detaili prospektist
   - LinkedIn URL, linastatud artikel, uudis, ettevõtte teade

2. **Pikkuse reegel**
   - E-kirid: 3-5 lõiku, 150-250 sõna
   - LinkedIn sõnumid: 2-3 lõiku, 30-60 sõna
   - Järelkontaktid: 2 lõiku, väga sisukas

3. **Grammatika ja toon**
   - Eesti keel: professionaalne, kuid mitte jäik
   - Ärge tõlkige otse ingliskeelsete failide järgi
   - Kasutage "käed vabad" asemel "käed lahti" (üheselt mõistetav)

4. **Anti-mustrid**
   - Ärge kasutage AI-lõhnade fraase ("Mul on arusaam, et...") 
   - Ärge näidake uurimisega seotud probleeme ("Leidsin, et...")
   - Ärge esitage küsimusi, millele te vastate
   - Ärge kirjutage loo nagu suur müügiesitlus

---

## Integratsioonid (välised rakendused)

Sel skillil on integratsioonid järgmistega:

1. **E-posti saatmine**: Gmail, Outlook, Mailchimp
2. **LinkedIn**: LinkedIn API (sõnumite vaatamine/saatmine)
3. **CRM andmed**: HubSpot, Pipedrive
4. **Andmerikastamine**: RocketReach, Apollo.io, Hunter.io
5. **Analüütika**: Lemlist, Outreach.io

---

## Vaadaku ka

- `linkedin-profile-analysis` — detailne profiiliga tutvumine
- `prospect-research` — süvaanalüüs ettevõtte kohta
- `sales-follow-up-sequence` — jäljekaarte automatiseerimine


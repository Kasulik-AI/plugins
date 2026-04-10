---
name: protsess
description: "Dokumenteeri või optimeeri äriprotsess — SOP, RACI maatriks, kitsaskohtade analüüs Kasuta kui kasutaja kirjutab '/protsess' või mainib seotud teemasid."
---

# /protsess — Protsesside Dokumenteerimine ja Optimeerimine

Dokumenteeri olemasolev äriprotsess või tuvasta ja paranda kitsaskohti.

## Kuidas see töötab

Küsin kõigepealt: **kas soovid protsessi dokumenteerida või parandada?**

### Dokumenteerimine
1. Kirjelda mulle protsess oma sõnadega
2. Loon struktureeritud SOP (standardne tööprotseduur)
3. Lisan RACI maatriksi (kes vastutab, kes teeb, kellega konsulteeritakse)
4. Lisan erijuhtumid ja erandid

### Optimeerimine
1. Kirjelda praegune protsess ja mis on probleem
2. Analüüsin kitsaskohti ja raiskamist
3. Pakun konkreetseid parandusettepanekuid
4. Loon uue optimeeritud protsessi

## Mida ma sinult vajan

- Protsessi nimi (nt "broneeringu käsitlemine", "hommikusöögi ettevalmistus")
- Kes on kaasatud
- Mis on praegune probleem (kui optimeerid)

## Näited

```
/protsess broneeringu käsitlemine algusest lõpuni
/protsess hommikusöögi ettevalmistus — liiga palju aega kulub
/protsess uue töötaja sisseelamine
```

---

## Protsessidokumendi Raamistik

### Väljundi Formaat

```markdown
## Protsessidokument: [Protsessi Nimi]
**Omanik:** [Isik/Tiim] | **Uuendatud:** [Kuupäev] | **Ülevaatuse sagedus:** [Kvartaalselt]

### Eesmärk
[Miks see protsess eksisteerib ja mida saavutab]

### Ulatus
[Mis on kaasatud ja mis välistatud]

### RACI Maatriks
| Samm | Responsible (teeb) | Accountable (vastutab) | Consulted (konsulteeritakse) | Informed (teavitatakse) |
|------|--------------------|------------------------|------------------------------|-------------------------|

### Detailsed Sammud

#### Samm 1: [Nimi]
- **Kes**: [Roll]
- **Millal**: [Trigger või ajastus]
- **Kuidas**: [Detailsed juhised]
- **Väljund**: [Mida see samm toodab]

### Erandid ja Erijuhtumid
| Stsenaarium | Kuidas Käituda |
|-------------|----------------|

### Mõõdikud
| Mõõdik | Sihtmärk | Kuidas Mõõta |
|--------|----------|-------------|
```

### Optimeerimise Raamistik

Kui kasutaja soovib protsessi parandada:

1. **Kaardista praegune seis** (AS-IS)
   - Mis sammud toimuvad praegu?
   - Kui kaua iga samm aega võtab?
   - Kus tekivad viivitused ja ootamine?

2. **Tuvasta kitsaskohad**
   - Kus kuhjub töö?
   - Kus toimub üleandmine tiimide vahel?
   - Kus on käsitöö mida saaks automatiseerida?
   - Kus puudub info ja tuleb tagasi minna küsima?

3. **Disaini uus protsess** (TO-BE)
   - Eemalda mittevajalikud sammud
   - Automatiseeri korduvtegevused
   - Vähenda üleandmisi
   - Lisa kontrolli- ja kinnituspunktid

4. **Mõõda paranemist**
   - Aeg: kui palju kiirem?
   - Kvaliteet: kui palju vähem vigu?
   - Rahulolu: kas meeskond/klient rahul?

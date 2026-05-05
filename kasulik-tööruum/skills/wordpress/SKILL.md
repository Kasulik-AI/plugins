---
name: wordpress
description: "Ühenda oma WordPress veebileht Claude'iga — samm-sammuline juhend MCP ühenduseks, sisu haldamiseks, SEO optimeerimiseks. Kasuta kui kasutaja mainib: wordpress, veebileht, koduleht, WP, blog, MCP adapter, sisu haldamine CMS, wordpress ühendamine, postituste haldamine, lehtede muutmine, kodulehe tekst, wordpress plugin."
---

# WordPress'i ühendamine Claude'iga

Sa oled WordPress'i ja CMS-integratsioonide ekspert. Võta lisaks kolm toetavat ekspertrolli (MCP konfigureerimise ekspert, WordPress'i turvalisuse ekspert, sisuhaldusstrateegia ekspert), millesse kehastu täielikult, et anda kasutajale parim juhend.

Kui kasutaja mainib WordPress'i ühendamist või seadistamist, juhi teda läbi alljärgneva juhendi sammhaaval.

---

## Mis sind ootab

- ⏱ **Aeg**: ~10–15 minutit
- 🛠 **Tehniline tase**: madal — kopeerimine ja kleepimine, mitte koodi kirjutamine
- 📋 **Mida vaja**: WordPress'i admin sisselogimisinfo + Claude Desktop arvutis (Mac või Windows)

---

## Eeldused

Sul peab olema:

1. **WordPress veebileht.** Kui logid sisse aadressil `sinu-sait.ee/wp-admin` (mitte `wordpress.com/login`), siis on see õige tüüp.
2. **Administraatori ligipääs** WordPress'ile.
3. **Claude Desktop rakendus** Mac'is või Windows'is (lae alla: [claude.ai/download](https://claude.ai/download)).

> **Pole kindel, kus su WordPress on?**
> - Logid sisse aadressil `wordpress.com/login` kaudu? → see juhend ei sobi (vt märkust lõpus)
> - Logid sisse aadressil `sinu-sait.ee/wp-admin` kaudu? → see juhend sobib ✓

---

## Samm 1A: Installi MCP Adapter plugin WordPress'is

1. Ava oma WordPress admin: `https://sinu-sait.ee/wp-admin`
2. Mine **Pluginad → Lisa uus** (Plugins → Add New)
3. Otsi: **MCP Adapter**
4. Installi ja aktiveeri plugin nimega **MCP Adapter** (autor: WordPress)

---

## Samm 1B: Loo Application Password

Application Password on eraldi parool ühenduseks — turvalisem kui peamise parooli kasutamine.

1. WordPress admin'is mine **Kasutajad → Sinu profiil** (Users → Your Profile)
2. Keri lehe alaosani, kuni leiad sektsiooni **"Application Passwords"** (Rakenduste paroolid)
3. Sisesta uue parooli nimi: `Claude AI`
4. Kliki nupule **"Add New Application Password"** (Lisa uus rakenduse parool)
5. **Kopeeri parool kohe** — see on 4×4 tähemärki (näiteks `abcd EFGH ijkl MNOP`) ja seda näidatakse ainult ühe korra!

> 💡 Soovitus: salvesta parool ajutiselt mõnda märkmesse, kuni järgmised sammud on tehtud.

---

## Samm 2: Ava Claude Desktop seadete fail

1. Ava Claude Desktop rakendus
2. **Mac**: `Claude → Settings...` (või kasuta `⌘,`)
3. **Windows**: kliki `Settings`
4. Vasakus menüüs **alaosas** (sektsioon "Desktop app") → kliki **Developer**
5. Sektsioonis "Local MCP servers" kliki nuppu **Edit Config**

See avab `claude_desktop_config.json` faili sinu vaikimisi tekstiredaktoris.

### Mis rakendusega see avaneb?

| Su arvuti | Vaikimisi avaneb | Soovitatud parem valik |
|-----------|-------------------|------------------------|
| **Mac** | TextEdit (sisseehitatud, töötab) | **VS Code** (tasuta, kuvab JSON-vigu, värvib teksti) — [code.visualstudio.com](https://code.visualstudio.com) |
| **Windows** | Notepad (sisseehitatud, töötab) | **VS Code** (tasuta, samad eelised) — [code.visualstudio.com](https://code.visualstudio.com) |

> ⚠️ **Mac TextEdit hoiatus**: Kui kasutad TextEdit'i, **enne salvestamist** veendu kahes asjas:
> 1. **Format → Make Plain Text** (`⌘⇧T`) — muidu salvestab .rtf failina
> 2. **Edit → Substitutions → Smart Quotes** välja lülitatud — muidu asendab `"` → `"` ja JSON läheb katki
>
> VS Code'is need probleemid puuduvad — see on usaldusväärsem valik.

---

## Samm 3: Lisa WordPress'i info konfiguratsioonile

Kui fail on tühi (näeb välja nagu `{}`), asenda kogu sisu alljärgneva tekstiga. Kui failis on juba muu sisu, lisa `wordpress` plokk olemasoleva `mcpServers` sektsiooni alla.

```json
{
  "mcpServers": {
    "wordpress": {
      "command": "npx",
      "args": ["-y", "@automattic/mcp-wordpress-remote@latest"],
      "env": {
        "WP_API_URL": "https://sinu-sait.ee",
        "WP_API_USERNAME": "sinu-kasutajanimi",
        "WP_API_PASSWORD": "xxxx xxxx xxxx xxxx"
      }
    }
  }
}
```

**Kolm asja, mida pead muutma:**

- 🌐 `WP_API_URL` → sinu veebilehe aadress (näiteks `https://minu-hotell.ee`)
- 👤 `WP_API_USERNAME` → su WordPress'i kasutajanimi (sama, millega `wp-admin`-i sisse logid)
- 🔑 `WP_API_PASSWORD` → sammus 1B saadud Application Password (16 tähemärki, tühikud võivad jääda)

---

## Samm 4: Salvesta ja taaskäivita Claude

1. Salvesta fail: `⌘S` Macis, `Ctrl+S` Windowsis
2. **Lõpeta Claude Desktop täielikult** (mitte ainult akna sulgemine):
   - **Mac**: `⌘Q` või menüüst `Claude → Quit Claude`
   - **Windows**: paremklikk Claude'i ikoonil tegumiribal (paremas alanurgas) → `Quit`
3. Ava Claude Desktop uuesti

---

## Samm 5: Testi ühendust

Kui Claude on uuesti avatud, proovi mõnda alljärgnevat näidisprompti. Claude peaks vastama, et tal on nüüd ligipääs sinu WordPress'ile.

---

## Mida saad teha pärast ühendamist

Kolm konkreetset prompti, mida saad kohe katsetada — kopeeri ja kleebi Claude'i:

**1. Vaata oma postitusi**

```
Näita mu 5 viimast avaldatud blogipostitust
```

Annab kiire ülevaate sellest, mis sul WordPress'is olemas on.

**2. Saa SEO soovitusi**

```
Vaata blogipostitust pealkirjaga "[postituse pealkiri]" ja paku 3 SEO parendust
```

Asenda `[postituse pealkiri]` mõne sinu päris postituse pealkirjaga. Claude analüüsib teksti ja annab konkreetsed soovitused.

**3. Uuenda kodulehte**

```
Uuenda avalehe pealkirja: muuda "[vana tekst]" → "[uus tekst]"
```

Asenda nurksulgudes olevad tekstid päris sõnastusega. Claude muudab ja salvestab kohe.

---

## Turvalisuse märkus

🔒 Claude saab teha kõike, mida sina admin-kontona teha saaksid — lugeda, luua, muuta ja kustutada postitusi ning lehti. Ühendus käib **Application Password**'i kaudu, mille saad igal ajal tühistada (sammus 1B näidatud kohas → klõpsa "Revoke" parooli kõrval). **Sinu peamine WordPress'i parool ei lähe kunagi Claude'ile.**

---

## Märkus Cowork kasutajatele

See juhend on Claude Desktop'i jaoks. Cowork'is on olemas eraldi WordPress Connector, kuid see töötab ainult **wordpress.com**-il majutatud saitidel — enamik Eesti VKE-de WordPress'e on kohalikus hostingus, seetõttu on õige kasutada käesolevat juhendit.

---

## Vajad abi?

Kui jääd hätta, kirjuta: [kristo@kasulik.ai](mailto:kristo@kasulik.ai) või vaata [kasulik.ai](https://kasulik.ai)

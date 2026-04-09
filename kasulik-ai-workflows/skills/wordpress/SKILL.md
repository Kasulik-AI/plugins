---
name: wordpress
description: "Ühenda oma WordPress veebileht Claude'iga — samm-sammuline juhend Kasuta kui kasutaja kirjutab '/wordpress' või mainib seotud teemasid."
---

# /wordpress — WordPress Ühendamine Claude'iga

Samm-sammuline juhend oma WordPress veebilehe ühendamiseks Claude'iga, et saaksid otse Claude'ist sisu hallata.

## Eeldused

- WordPress veebileht (ise majutatud, wordpress.org, mitte wordpress.com tasuta)
- Administraatori ligipääs WordPress'ile
- Claude Desktop või Cowork rakendus arvutis

## Samm 1: Installi MCP Adapter plugin

1. Ava oma WordPress admin: `https://sinu-sait.ee/wp-admin`
2. Mine **Pluginad → Lisa uus**
3. Otsi: **"MCP Adapter"**
4. Installi ja aktiveeri plugin nimega **MCP Adapter** (autor: WordPress)

## Samm 2: Loo rakenduse parool

1. Mine **Kasutajad → Sinu profiil** (või Users → Your Profile)
2. Keri alla kuni leiad **"Rakenduse paroolid"** (Application Passwords)
3. Sisesta nimi: `Claude AI`
4. Kliki **"Lisa uus rakenduse parool"**
5. **Kopeeri parool kohe** — seda näidatakse ainult üks kord!

## Samm 3: Seadista Claude'is

Lisa see oma Claude konfiguratsiooni (Claude Desktop: Settings → MCP Servers):

```json
{
  "mcpServers": {
    "wordpress": {
      "command": "npx",
      "args": ["-y", "@anthropic/mcp-wordpress"],
      "env": {
        "WORDPRESS_URL": "https://sinu-sait.ee",
        "WORDPRESS_USERNAME": "sinu-kasutajanimi",
        "WORDPRESS_PASSWORD": "xxxx-xxxx-xxxx-xxxx"
      }
    }
  }
}
```

Asenda:
- `https://sinu-sait.ee` → sinu veebilehe aadress
- `sinu-kasutajanimi` → su WordPress kasutajanimi
- `xxxx-xxxx-xxxx-xxxx` → sammus 2 loodud rakenduse parool

## Samm 4: Testi ühendust

Taaskäivita Claude ja proovi:
- "Näita mu WordPress postitusi"
- "Loo uus blogipostitus teemal..."
- "Uuenda avalehe teksti"

## Mida saad teha pärast ühendamist

- **Postituste haldamine** — loo, muuda, kustuta blogipostitusi
- **Lehtede muutmine** — uuenda kodulehe tekste otse Claude'ist
- **SEO optimeerimine** — lase Claude'il analüüsida ja parandada tekste
- **Sisukalender** — planeeri ja ajasta postitusi

## Veaotsing

**"Ühendus ebaõnnestus":**
- Kontrolli, et URL on õige (koos https://)
- Kontrolli kasutajanime ja parooli
- Veendu, et MCP Adapter plugin on aktiivne

**"Ligipääs keelatud":**
- Su WordPress kasutajal peab olema administraatori roll
- Kontrolli, et rakenduse paroolid on lubatud (mõned turvapluginad blokeerivad neid)

**"npx käsku ei leita":**
- Installi Node.js: https://nodejs.org (LTS versioon)

# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Download

I link seguenti puntano sempre ai pacchetti dell'ultima versione (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Tutti i download passano attraverso `releases/latest/download/`, quindi ottieni sempre il pacchetto più recente senza dover aggiornare questo indirizzo.

## Localizzazione

Invitiamo tutti a contribuire alla localizzazione di questo progetto — sia aggiungendo una nuova lingua sia migliorando una traduzione esistente. Ogni aiuto è benvenuto.

Tutte le stringhe traducibili si trovano nella directory `res/`. Ogni lingua ha la propria cartella denominata in base al suo locale:

- `res/values/` — stringhe predefinite/di base (cinese semplificato), usate come fonte di riferimento
- `res/values-en/` — inglese
- `res/values-ja/` — giapponese
- `res/values-ko/` — coreano
- `res/values-ru/` — russo
- `res/values-de/` — tedesco
- `res/values-fr/` — francese
- `res/values-es/` — spagnolo
- `res/values-pt/` — portoghese
- `res/values-it/` — italiano
- `res/values-tr/` — turco
- `res/values-ar/` — arabo
- `res/values-th/` — thailandese
- `res/values-vi/` — vietnamita
- `res/values-in/` — indonesiano
- `res/values-ms/` — malese
- `res/values-zh-rTW/` — cinese tradizionale

Ogni cartella contiene un file `strings.xml`. L'attributo `name` di ogni voce `<string>` è la chiave e **non deve essere modificato** — traduci solo il testo tra i tag.

### Come tradurre

1. Fai il fork di questo repository e clonalo in locale.
2. Apri la directory `res/` e trova la cartella della lingua su cui vuoi lavorare.
   - Per **migliorare una lingua esistente**, modifica direttamente il suo `strings.xml`.
   - Per **aggiungere una nuova lingua**, copia `res/values-en/strings.xml` in una nuova cartella chiamata `values-<locale>` (ad esempio `values-nl` per l'olandese) e traduci il suo contenuto.
3. Traduci il valore di ogni voce `<string>`. Usa sempre `res/values/strings.xml` come riferimento per il significato originale.
4. Mantieni i segnaposto (come `%1$s`, `%d`) e i tag di formattazione (come `<b>`, `\n`) esattamente come sono — non tradurli né rimuoverli mai.
5. Rimuovi le voci con `translatable="false"` o lasciale intatte; non devono essere tradotte.
6. Verifica le tue modifiche, poi apri una Pull Request descrivendo quale lingua hai aggiornato.

Esempio:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Grazie per aiutarci a rendere okmore disponibile per più persone in tutto il mondo!

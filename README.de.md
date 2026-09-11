# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Download

Die folgenden Links verweisen immer auf die Pakete der neuesten Version (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Alle Downloads erfolgen über `releases/latest/download/`, sodass Sie immer das neueste Paket erhalten, ohne diese Adresse aktualisieren zu müssen.

## Lokalisierung

Wir laden alle ein, zur Lokalisierung dieses Projekts beizutragen — sei es durch das Hinzufügen einer neuen Sprache oder die Verbesserung einer bestehenden Übersetzung. Jede Hilfe ist willkommen.

Alle übersetzbaren Zeichenketten befinden sich im Verzeichnis `res/`. Jede Sprache hat einen eigenen Ordner, der nach ihrem Locale benannt ist:

- `res/values/` — Standard-/Basiszeichenketten (vereinfachtes Chinesisch), dienen als Ausgangsquelle
- `res/values-en/` — Englisch
- `res/values-ja/` — Japanisch
- `res/values-ko/` — Koreanisch
- `res/values-ru/` — Russisch
- `res/values-de/` — Deutsch
- `res/values-fr/` — Französisch
- `res/values-es/` — Spanisch
- `res/values-pt/` — Portugiesisch
- `res/values-it/` — Italienisch
- `res/values-tr/` — Türkisch
- `res/values-ar/` — Arabisch
- `res/values-th/` — Thailändisch
- `res/values-vi/` — Vietnamesisch
- `res/values-in/` — Indonesisch
- `res/values-ms/` — Malaiisch
- `res/values-zh-rTW/` — Traditionelles Chinesisch

Jeder Ordner enthält eine Datei `strings.xml`. Das Attribut `name` jedes `<string>`-Eintrags ist der Schlüssel und **darf nicht geändert werden** — übersetzen Sie nur den Text zwischen den Tags.

### Wie man übersetzt

1. Forken Sie dieses Repository und klonen Sie es lokal.
2. Öffnen Sie das Verzeichnis `res/` und suchen Sie den Sprachordner, an dem Sie arbeiten möchten.
   - Um eine **bestehende Sprache zu verbessern**, bearbeiten Sie deren `strings.xml` direkt.
   - Um eine **neue Sprache hinzuzufügen**, kopieren Sie `res/values-en/strings.xml` in einen neuen Ordner namens `values-<locale>` (zum Beispiel `values-nl` für Niederländisch) und übersetzen Sie dessen Inhalt.
3. Übersetzen Sie den Wert jedes `<string>`-Eintrags. Verwenden Sie stets `res/values/strings.xml` als Referenz für die ursprüngliche Bedeutung.
4. Behalten Sie Platzhalter (wie `%1$s`, `%d`) und Formatierungs-Tags (wie `<b>`, `\n`) exakt bei — übersetzen oder entfernen Sie sie niemals.
5. Entfernen Sie `translatable="false"`-Einträge oder lassen Sie sie unverändert; sie dürfen nicht übersetzt werden.
6. Testen Sie Ihre Änderungen und öffnen Sie einen Pull Request, in dem Sie beschreiben, welche Sprache Sie aktualisiert haben.

Beispiel:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Vielen Dank, dass Sie helfen, okmore für mehr Menschen weltweit verfügbar zu machen!

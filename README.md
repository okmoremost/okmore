# okmore

[简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Download

The links below always point to the latest release packages (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> All downloads go through `releases/latest/download/`, so you always get the latest package without updating this address.

## Localization

We welcome everyone to contribute to the localization of this project — whether adding a brand-new language or improving an existing translation. Every bit of help is appreciated.

All translatable strings live in the `res/` directory. Each language has its own folder named after its locale:

- `res/values/` — default/base strings (Simplified Chinese), used as the source of truth
- `res/values-en/` — English
- `res/values-ja/` — Japanese
- `res/values-ko/` — Korean
- `res/values-ru/` — Russian
- `res/values-de/` — German
- `res/values-fr/` — French
- `res/values-es/` — Spanish
- `res/values-pt/` — Portuguese
- `res/values-it/` — Italian
- `res/values-tr/` — Turkish
- `res/values-ar/` — Arabic
- `res/values-th/` — Thai
- `res/values-vi/` — Vietnamese
- `res/values-in/` — Indonesian
- `res/values-ms/` — Malay
- `res/values-zh-rTW/` — Traditional Chinese

Each folder contains a `strings.xml` file. The `name` attribute of every `<string>` entry is the key and **must not be changed** — only translate the text between the tags.

### How to translate

1. Fork this repository and clone it locally.
2. Open the `res/` directory and find the language folder you want to work on.
   - To **improve an existing language**, edit its `strings.xml` directly.
   - To **add a new language**, copy `res/values-en/strings.xml` into a new folder named `values-<locale>` (for example `values-nl` for Dutch), then translate its contents.
3. Translate the value of each `<string>` entry. Always use `res/values/strings.xml` as the reference for the original meaning.
4. Keep placeholders (such as `%1$s`, `%d`) and formatting tags (such as `<b>`, `\n`) exactly as they are — never translate or remove them.
5. Remove the `translatable="false"` entries or leave them untouched; they should not be translated.
6. Test your changes, then open a Pull Request describing which language you updated.

Example:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Thanks for helping make okmore available to more people around the world!

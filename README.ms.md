# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Muat Turun

Pautan di bawah sentiasa menunjuk kepada pakej versi terkini (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Semua muat turun melalui `releases/latest/download/`, jadi anda sentiasa mendapat pakej terkini tanpa perlu mengemas kini alamat ini.

## Penyetempatan

Kami mengalu-alukan semua orang untuk menyumbang kepada penyetempatan projek ini — sama ada menambah bahasa baharu atau menambah baik terjemahan sedia ada. Segala bantuan amat dihargai.

Semua rentetan yang boleh diterjemah terletak dalam direktori `res/`. Setiap bahasa mempunyai folder tersendiri yang dinamakan mengikut lokalnya:

- `res/values/` — rentetan lalai/asas (Cina Ringkas), digunakan sebagai sumber rujukan
- `res/values-en/` — Inggeris
- `res/values-ja/` — Jepun
- `res/values-ko/` — Korea
- `res/values-ru/` — Rusia
- `res/values-de/` — Jerman
- `res/values-fr/` — Perancis
- `res/values-es/` — Sepanyol
- `res/values-pt/` — Portugis
- `res/values-it/` — Itali
- `res/values-tr/` — Turki
- `res/values-ar/` — Arab
- `res/values-th/` — Thai
- `res/values-vi/` — Vietnam
- `res/values-in/` — Indonesia
- `res/values-ms/` — Melayu
- `res/values-zh-rTW/` — Cina Tradisional

Setiap folder mengandungi fail `strings.xml`. Atribut `name` bagi setiap entri `<string>` ialah kunci dan **tidak boleh diubah** — terjemah hanya teks di antara tag.

### Cara menterjemah

1. Fork repositori ini dan klon ke komputer tempatan anda.
2. Buka direktori `res/` dan cari folder bahasa yang ingin anda kerjakan.
   - Untuk **menambah baik bahasa sedia ada**, edit fail `strings.xml`-nya secara terus.
   - Untuk **menambah bahasa baharu**, salin `res/values-en/strings.xml` ke folder baharu bernama `values-<locale>` (contohnya `values-nl` untuk bahasa Belanda), kemudian terjemah kandungannya.
3. Terjemah nilai setiap entri `<string>`. Sentiasa gunakan `res/values/strings.xml` sebagai rujukan maksud asal.
4. Kekalkan placeholder (seperti `%1$s`, `%d`) dan tag pemformatan (seperti `<b>`, `\n`) tepat seperti asalnya — jangan sekali-kali menterjemah atau menghapusnya.
5. Buang entri dengan `translatable="false"` atau biarkan sebagaimana adanya; entri tersebut tidak boleh diterjemah.
6. Uji perubahan anda, kemudian buka Pull Request dengan menerangkan bahasa yang anda kemas kini.

Contoh:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Terima kasih kerana membantu menjadikan okmore boleh diakses oleh lebih ramai orang di seluruh dunia!

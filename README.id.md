# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Unduh

Tautan di bawah ini selalu mengarah ke paket versi terbaru (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Semua unduhan melewati `releases/latest/download/`, sehingga Anda selalu mendapatkan paket terbaru tanpa perlu memperbarui alamat ini.

## Lokalisasi

Kami mengundang semua orang untuk berkontribusi pada lokalisasi proyek ini — baik menambahkan bahasa baru maupun meningkatkan terjemahan yang ada. Segala bantuan sangat kami hargai.

Semua string yang dapat diterjemahkan berada di direktori `res/`. Setiap bahasa memiliki folder sendiri yang dinamai sesuai locale-nya:

- `res/values/` — string default/dasar (Tionghoa Sederhana), digunakan sebagai sumber acuan
- `res/values-en/` — Inggris
- `res/values-ja/` — Jepang
- `res/values-ko/` — Korea
- `res/values-ru/` — Rusia
- `res/values-de/` — Jerman
- `res/values-fr/` — Prancis
- `res/values-es/` — Spanyol
- `res/values-pt/` — Portugis
- `res/values-it/` — Italia
- `res/values-tr/` — Turki
- `res/values-ar/` — Arab
- `res/values-th/` — Thai
- `res/values-vi/` — Vietnam
- `res/values-in/` — Indonesia
- `res/values-ms/` — Melayu
- `res/values-zh-rTW/` — Tionghoa Tradisional

Setiap folder berisi file `strings.xml`. Atribut `name` pada setiap entri `<string>` adalah kunci dan **tidak boleh diubah** — terjemahkan hanya teks di antara tag.

### Cara menerjemahkan

1. Fork repositori ini dan clone ke komputer lokal Anda.
2. Buka direktori `res/` dan temukan folder bahasa yang ingin Anda kerjakan.
   - Untuk **meningkatkan bahasa yang sudah ada**, edit file `strings.xml`-nya secara langsung.
   - Untuk **menambahkan bahasa baru**, salin `res/values-en/strings.xml` ke folder baru bernama `values-<locale>` (misalnya `values-nl` untuk bahasa Belanda), lalu terjemahkan isinya.
3. Terjemahkan nilai setiap entri `<string>`. Selalu gunakan `res/values/strings.xml` sebagai acuan makna asli.
4. Pertahankan placeholder (seperti `%1$s`, `%d`) dan tag pemformatan (seperti `<b>`, `\n`) persis seperti aslinya — jangan pernah menerjemahkan atau menghapusnya.
5. Hapus entri dengan `translatable="false"` atau biarkan apa adanya; entri tersebut tidak boleh diterjemahkan.
6. Uji perubahan Anda, lalu buka Pull Request dengan menjelaskan bahasa mana yang Anda perbarui.

Contoh:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Terima kasih telah membantu membuat okmore dapat diakses oleh lebih banyak orang di seluruh dunia!

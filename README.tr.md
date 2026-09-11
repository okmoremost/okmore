# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## İndirme

Aşağıdaki bağlantılar her zaman en son sürüm paketlerine (GitHub Release) yönlendirir:

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Tüm indirmeler `releases/latest/download/` üzerinden geçer, böylece bu adresi güncellemeden her zaman en son paketi elde edersiniz.

## Yerelleştirme

Bu projenin yerelleştirilmesine herkesi katkıda bulunmaya davet ediyoruz — ister yeni bir dil ekleyin, ister mevcut bir çeviriyi iyileştirin. Her türlü katkı memnuniyetle karşılanır.

Çevrilebilir tüm dizeler `res/` dizininde bulunur. Her dilin kendi yerel ayarına göre adlandırılmış bir klasörü vardır:

- `res/values/` — varsayılan/temel dizeler (Basitleştirilmiş Çince), kaynak olarak kullanılır
- `res/values-en/` — İngilizce
- `res/values-ja/` — Japonca
- `res/values-ko/` — Korece
- `res/values-ru/` — Rusça
- `res/values-de/` — Almanca
- `res/values-fr/` — Fransızca
- `res/values-es/` — İspanyolca
- `res/values-pt/` — Portekizce
- `res/values-it/` — İtalyanca
- `res/values-tr/` — Türkçe
- `res/values-ar/` — Arapça
- `res/values-th/` — Tayca
- `res/values-vi/` — Vietnamca
- `res/values-in/` — Endonezce
- `res/values-ms/` — Malayca
- `res/values-zh-rTW/` — Geleneksel Çince

Her klasörde bir `strings.xml` dosyası bulunur. Her `<string>` girdisinin `name` özniteliği anahtardır ve **değiştirilmemelidir** — yalnızca etiketler arasındaki metni çevirin.

### Nasıl çevrilir

1. Bu depoyu çatallayın (fork) ve yerel olarak klonlayın.
2. `res/` dizinini açın ve üzerinde çalışmak istediğiniz dil klasörünü bulun.
   - **Mevcut bir dili iyileştirmek** için doğrudan onun `strings.xml` dosyasını düzenleyin.
   - **Yeni bir dil eklemek** için `res/values-en/strings.xml` dosyasını `values-<locale>` adlı yeni bir klasöre kopyalayın (örneğin Hollandaca için `values-nl`), ardından içeriğini çevirin.
3. Her `<string>` girdisinin değerini çevirin. Özgün anlam için her zaman `res/values/strings.xml` dosyasını referans olarak kullanın.
4. Yer tutucuları (örneğin `%1$s`, `%d`) ve biçimlendirme etiketlerini (örneğin `<b>`, `\n`) olduğu gibi koruyun — bunları asla çevirmeyin veya silmeyin.
5. `translatable="false"` girdilerini kaldırın ya da olduğu gibi bırakın; bunlar çevrilmemelidir.
6. Değişikliklerinizi test edin, ardından hangi dili güncellediğinizi açıklayan bir Pull Request açın.

Örnek:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

okmore'u dünyanın dört bir yanındaki daha fazla kişi için erişilebilir kılmaya yardımcı olduğunuz için teşekkürler!

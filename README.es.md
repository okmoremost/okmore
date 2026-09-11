# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Descarga

Los siguientes enlaces siempre apuntan a los paquetes de la última versión (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Todas las descargas pasan por `releases/latest/download/`, así que siempre obtienes el paquete más reciente sin actualizar esta dirección.

## Localización

Damos la bienvenida a todos para contribuir a la localización de este proyecto, ya sea añadiendo un nuevo idioma o mejorando una traducción existente. Toda ayuda es bienvenida.

Todas las cadenas traducibles se encuentran en el directorio `res/`. Cada idioma tiene su propia carpeta nombrada según su locale:

- `res/values/` — cadenas predeterminadas/base (chino simplificado), usadas como fuente de referencia
- `res/values-en/` — inglés
- `res/values-ja/` — japonés
- `res/values-ko/` — coreano
- `res/values-ru/` — ruso
- `res/values-de/` — alemán
- `res/values-fr/` — francés
- `res/values-es/` — español
- `res/values-pt/` — portugués
- `res/values-it/` — italiano
- `res/values-tr/` — turco
- `res/values-ar/` — árabe
- `res/values-th/` — tailandés
- `res/values-vi/` — vietnamita
- `res/values-in/` — indonesio
- `res/values-ms/` — malayo
- `res/values-zh-rTW/` — chino tradicional

Cada carpeta contiene un archivo `strings.xml`. El atributo `name` de cada entrada `<string>` es la clave y **no debe modificarse**; solo traduce el texto entre las etiquetas.

### Cómo traducir

1. Haz un fork de este repositorio y clónalo localmente.
2. Abre el directorio `res/` y busca la carpeta del idioma en el que quieras trabajar.
   - Para **mejorar un idioma existente**, edita directamente su `strings.xml`.
   - Para **añadir un nuevo idioma**, copia `res/values-en/strings.xml` en una nueva carpeta llamada `values-<locale>` (por ejemplo `values-nl` para neerlandés) y traduce su contenido.
3. Traduce el valor de cada entrada `<string>`. Usa siempre `res/values/strings.xml` como referencia del significado original.
4. Mantén los marcadores de posición (como `%1$s`, `%d`) y las etiquetas de formato (como `<b>`, `\n`) exactamente como están; nunca los traduzcas ni los elimines.
5. Elimina las entradas `translatable="false"` o déjalas intactas; no deben traducirse.
6. Prueba tus cambios y abre un Pull Request describiendo qué idioma has actualizado.

Ejemplo:

```xml
<!-- res/values/strings.xml (origen) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

¡Gracias por ayudar a que okmore esté disponible para más personas en todo el mundo!

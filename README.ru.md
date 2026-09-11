# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Загрузка

Приведённые ниже ссылки всегда указывают на пакеты последней версии (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Все загрузки проходят через `releases/latest/download/`, поэтому вы всегда получаете последний пакет без необходимости обновлять этот адрес.

## Локализация

Мы приглашаем всех принять участие в локализации этого проекта — как в добавлении нового языка, так и в улучшении существующего перевода. Мы благодарны за любую помощь.

Все переводимые строки находятся в каталоге `res/`. Для каждого языка есть своя папка, названная по его локали:

- `res/values/` — строки по умолчанию/базовые (упрощённый китайский), используются как источник
- `res/values-en/` — английский
- `res/values-ja/` — японский
- `res/values-ko/` — корейский
- `res/values-ru/` — русский
- `res/values-de/` — немецкий
- `res/values-fr/` — французский
- `res/values-es/` — испанский
- `res/values-pt/` — португальский
- `res/values-it/` — итальянский
- `res/values-tr/` — турецкий
- `res/values-ar/` — арабский
- `res/values-th/` — тайский
- `res/values-vi/` — вьетнамский
- `res/values-in/` — индонезийский
- `res/values-ms/` — малайский
- `res/values-zh-rTW/` — традиционный китайский

Каждая папка содержит файл `strings.xml`. Атрибут `name` каждого элемента `<string>` — это ключ, и его **нельзя изменять**; переводите только текст между тегами.

### Как переводить

1. Сделайте форк этого репозитория и клонируйте его локально.
2. Откройте каталог `res/` и найдите папку нужного вам языка.
   - Чтобы **улучшить существующий язык**, отредактируйте его `strings.xml` напрямую.
   - Чтобы **добавить новый язык**, скопируйте `res/values-en/strings.xml` в новую папку с именем `values-<locale>` (например, `values-nl` для нидерландского) и переведите её содержимое.
3. Переведите значение каждого элемента `<string>`. Всегда используйте `res/values/strings.xml` как источник исходного значения.
4. Сохраняйте плейсхолдеры (например, `%1$s`, `%d`) и теги форматирования (например, `<b>`, `\n`) в точности как есть — никогда не переводите и не удаляйте их.
5. Удалите элементы с `translatable="false"` или оставьте их без изменений; их не следует переводить.
6. Протестируйте изменения и создайте Pull Request с описанием того, какой язык вы обновили.

Пример:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Спасибо за помощь в том, чтобы сделать okmore доступным для всё большего числа людей по всему миру!

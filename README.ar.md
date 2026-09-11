# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## التنزيل

تشير الروابط أدناه دائمًا إلى حزم الإصدار الأخير (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> تمر جميع التنزيلات عبر `releases/latest/download/`، لذا ستحصل دائمًا على أحدث حزمة دون الحاجة إلى تحديث هذا العنوان.

## الترجمة (التعريب)

ندعو الجميع للمساهمة في تعريب هذا المشروع — سواء بإضافة لغة جديدة أو تحسين ترجمة موجودة. نرحّب بكل مساعدة.

توجد جميع النصوص القابلة للترجمة في الدليل `res/`. لكل لغة مجلد خاص بها مُسمّى وفقًا للغة الخاصة بها:

- `res/values/` — النصوص الافتراضية/الأساسية (الصينية المبسطة)، تُستخدم كمصدر مرجعي
- `res/values-en/` — الإنجليزية
- `res/values-ja/` — اليابانية
- `res/values-ko/` — الكورية
- `res/values-ru/` — الروسية
- `res/values-de/` — الألمانية
- `res/values-fr/` — الفرنسية
- `res/values-es/` — الإسبانية
- `res/values-pt/` — البرتغالية
- `res/values-it/` — الإيطالية
- `res/values-tr/` — التركية
- `res/values-ar/` — العربية
- `res/values-th/` — التايلاندية
- `res/values-vi/` — الفيتنامية
- `res/values-in/` — الإندونيسية
- `res/values-ms/` — الملايوية
- `res/values-zh-rTW/` — الصينية التقليدية

يحتوي كل مجلد على ملف `strings.xml`. سمة `name` لكل عنصر `<string>` هي المفتاح و**يجب عدم تغييرها** — قم بترجمة النص الموجود بين الوسمين فقط.

### كيفية الترجمة

1. قم بعمل Fork لهذا المستودع ثم استنسخه محليًا.
2. افتح الدليل `res/` وابحث عن مجلد اللغة التي تريد العمل عليها.
   - لـ**تحسين لغة موجودة**، عدّل ملف `strings.xml` الخاص بها مباشرةً.
   - لـ**إضافة لغة جديدة**، انسخ `res/values-en/strings.xml` إلى مجلد جديد باسم `values-<locale>` (مثلًا `values-nl` للهولندية)، ثم ترجم محتواه.
3. ترجم قيمة كل عنصر `<string>`. استخدم دائمًا `res/values/strings.xml` كمرجع للمعنى الأصلي.
4. احتفظ بالعناصر النائبة (مثل `%1$s` و`%d`) ووسوم التنسيق (مثل `<b>` و`\n`) كما هي تمامًا — لا تترجمها أو تحذفها أبدًا.
5. احذف العناصر ذات `translatable="false"` أو اتركها دون تغيير؛ إذ لا ينبغي ترجمتها.
6. اختبر تغييراتك، ثم افتح Pull Request مع وصف اللغة التي حدّثتها.

مثال:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

شكرًا لمساعدتك في جعل okmore متاحًا لمزيد من الناس حول العالم!

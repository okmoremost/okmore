# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## 下載

以下連結永遠指向最新版本的安裝包（GitHub Release）：

- **中/英**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **全語言**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> 所有下載都經過 `releases/latest/download/`，因此你總是能取得最新套件，無需更新此地址。

## 本地化

我們歡迎所有人參與本專案的本地化工作——無論是新增一門語言，還是改進現有翻譯。每一份幫助都值得感謝。

所有可翻譯的字串都位於 `res/` 目錄。每種語言都有以地區代碼命名的專屬資料夾：

- `res/values/` — 預設/基礎字串（簡體中文），作為原始來源
- `res/values-en/` — 英文
- `res/values-ja/` — 日文
- `res/values-ko/` — 韓文
- `res/values-ru/` — 俄文
- `res/values-de/` — 德文
- `res/values-fr/` — 法文
- `res/values-es/` — 西班牙文
- `res/values-pt/` — 葡萄牙文
- `res/values-it/` — 義大利文
- `res/values-tr/` — 土耳其文
- `res/values-ar/` — 阿拉伯文
- `res/values-th/` — 泰文
- `res/values-vi/` — 越南文
- `res/values-in/` — 印尼文
- `res/values-ms/` — 馬來文
- `res/values-zh-rTW/` — 繁體中文

每個資料夾都包含一個 `strings.xml` 檔案。每個 `<string>` 項目的 `name` 屬性是鍵名，**不可修改**——只需翻譯標籤之間的文字。

### 如何翻譯

1. Fork 此儲存庫並複製到本機。
2. 開啟 `res/` 目錄，找到你想處理的語言資料夾。
   - 若要**改進現有語言**，直接編輯其 `strings.xml`。
   - 若要**新增語言**，將 `res/values-en/strings.xml` 複製到命名為 `values-<locale>` 的新資料夾（例如荷蘭文為 `values-nl`），然後翻譯其內容。
3. 翻譯每個 `<string>` 項目的值。請務必以 `res/values/strings.xml` 作為原始含義的參考。
4. 保留佔位符（例如 `%1$s`、`%d`）與格式標籤（例如 `<b>`、`\n`）原樣不變——絕不翻譯或刪除它們。
5. 移除或保留 `translatable="false"` 的項目不動；它們不應被翻譯。
6. 測試你的變更，然後提交 Pull Request，說明你更新了哪種語言。

範例：

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

感謝你幫助 okmore 觸及全世界更多的人！

# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## ダウンロード

以下のリンクは常に最新リリースのパッケージ（GitHub Release）を指します：

- **中/英**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **全言語**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> すべてのダウンロードは `releases/latest/download/` を経由するため、このアドレスを更新しなくても常に最新のパッケージを取得できます。

## ローカライズ

本プロジェクトのローカライズにぜひご協力ください。新しい言語の追加でも、既存の翻訳の改善でも歓迎します。皆さまのご協力に感謝します。

翻訳可能な文字列はすべて `res/` ディレクトリにあります。各言語にはロケールに基づく専用フォルダがあります：

- `res/values/` — デフォルト/基準の文字列（簡体字中国語）、参照元として使用
- `res/values-en/` — 英語
- `res/values-ja/` — 日本語
- `res/values-ko/` — 韓国語
- `res/values-ru/` — ロシア語
- `res/values-de/` — ドイツ語
- `res/values-fr/` — フランス語
- `res/values-es/` — スペイン語
- `res/values-pt/` — ポルトガル語
- `res/values-it/` — イタリア語
- `res/values-tr/` — トルコ語
- `res/values-ar/` — アラビア語
- `res/values-th/` — タイ語
- `res/values-vi/` — ベトナム語
- `res/values-in/` — インドネシア語
- `res/values-ms/` — マレー語
- `res/values-zh-rTW/` — 繁体字中国語

各フォルダには `strings.xml` ファイルが含まれています。各 `<string>` 要素の `name` 属性はキーであり、**変更してはいけません**。タグ間のテキストのみを翻訳してください。

### 翻訳方法

1. このリポジトリを Fork してローカルにクローンします。
2. `res/` ディレクトリを開き、作業したい言語のフォルダを探します。
   - **既存の言語を改善する**場合は、その `strings.xml` を直接編集します。
   - **新しい言語を追加する**場合は、`res/values-en/strings.xml` を `values-<locale>` という名前の新しいフォルダ（例：オランダ語なら `values-nl`）にコピーし、その内容を翻訳します。
3. 各 `<string>` 要素の値を翻訳します。元の意味の参照として、必ず `res/values/strings.xml` を使用してください。
4. プレースホルダー（`%1$s`、`%d` など）と書式タグ（`<b>`、`\n` など）はそのままの形で保持してください。決して翻訳したり削除したりしないでください。
5. `translatable="false"` の要素は削除するか、そのままにしておいてください。翻訳する必要はありません。
6. 変更をテストしたら、どの言語を更新したかを記載して Pull Request を作成します。

例：

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

okmore を世界中のより多くの人に届けるためのご協力に感謝します！

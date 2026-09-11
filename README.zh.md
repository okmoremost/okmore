# okmore

[English](README.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## 下载

以下链接始终指向最新版本的发布包（GitHub Release）：

- **中/英精简版**：[okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **多语言完整版**：[okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> 所有下载均走 `releases/latest/download/`，发布新版本后无需更新本地址即可获取最新安装包。

## 本地化

欢迎大家参与本项目的本地化翻译工作——无论是新增一门语言，还是改进已有翻译，都欢迎贡献力量。

所有可翻译的字符串都位于 `res/` 目录。每种语言都有以地区代码命名的独立文件夹：

- `res/values/` — 默认/基础字符串（简体中文），作为原始来源
- `res/values-en/` — 英文
- `res/values-ja/` — 日文
- `res/values-ko/` — 韩文
- `res/values-ru/` — 俄文
- `res/values-de/` — 德文
- `res/values-fr/` — 法文
- `res/values-es/` — 西班牙文
- `res/values-pt/` — 葡萄牙文
- `res/values-it/` — 意大利文
- `res/values-tr/` — 土耳其文
- `res/values-ar/` — 阿拉伯文
- `res/values-th/` — 泰文
- `res/values-vi/` — 越南文
- `res/values-in/` — 印尼文
- `res/values-ms/` — 马来文
- `res/values-zh-rTW/` — 繁体中文

每个文件夹都包含一个 `strings.xml` 文件。每个 `<string>` 条目的 `name` 属性是键名，**不可修改**——只需翻译标签之间的文本。

### 如何翻译

1. Fork 本仓库并克隆到本地。
2. 打开 `res/` 目录，找到你想处理的语言文件夹。
   - 若要**改进已有语言**，直接编辑其 `strings.xml`。
   - 若要**新增语言**，将 `res/values-en/strings.xml` 复制到命名为 `values-<locale>` 的新文件夹（例如荷兰文为 `values-nl`），然后翻译其内容。
3. 翻译每个 `<string>` 条目的值。请务必以 `res/values/strings.xml` 作为原始含义的参考。
4. 保留占位符（例如 `%1$s`、`%d`）与格式标签（例如 `<b>`、`\n`）原样不变——绝不要翻译或删除它们。
5. 删除或保留 `translatable="false"` 的条目不动作；它们不应被翻译。
6. 测试你的修改，然后提交 Pull Request，说明你更新了哪种语言。

示例：

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

感谢你帮助 okmore 触达全世界更多的人！

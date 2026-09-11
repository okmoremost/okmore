# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## 다운로드

아래 링크는 항상 최신 릴리스 패키지(GitHub Release)를 가리킵니다:

- **중/영**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **전체 언어**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> 모든 다운로드는 `releases/latest/download/`를 거치므로, 이 주소를 업데이트하지 않아도 항상 최신 패키지를 받을 수 있습니다.

## 현지화

이 프로젝트의 현지화에 많은 참여를 환영합니다. 새로운 언어를 추가하거나 기존 번역을 개선하는 것 모두 환영합니다. 모든 도움에 감사드립니다.

번역 가능한 모든 문자열은 `res/` 디렉터리에 있습니다. 각 언어는 로케일 기반의 고유한 폴더를 가집니다:

- `res/values/` — 기본/기준 문자열(중국어 간체), 원본 기준으로 사용
- `res/values-en/` — 영어
- `res/values-ja/` — 일본어
- `res/values-ko/` — 한국어
- `res/values-ru/` — 러시아어
- `res/values-de/` — 독일어
- `res/values-fr/` — 프랑스어
- `res/values-es/` — 스페인어
- `res/values-pt/` — 포르투갈어
- `res/values-it/` — 이탈리아어
- `res/values-tr/` — 터키어
- `res/values-ar/` — 아랍어
- `res/values-th/` — 태국어
- `res/values-vi/` — 베트남어
- `res/values-in/` — 인도네시아어
- `res/values-ms/` — 말레이어
- `res/values-zh-rTW/` — 중국어 번체

각 폴더에는 `strings.xml` 파일이 있습니다. 각 `<string>` 항목의 `name` 속성은 키이며 **변경해서는 안 됩니다**. 태그 사이의 텍스트만 번역하세요.

### 번역 방법

1. 이 저장소를 Fork하고 로컬에 클론합니다.
2. `res/` 디렉터리를 열고 작업하려는 언어 폴더를 찾습니다.
   - **기존 언어를 개선**하려면 해당 `strings.xml`을 직접 편집합니다.
   - **새 언어를 추가**하려면 `res/values-en/strings.xml`을 `values-<locale>`라는 새 폴더(예: 네덜란드어는 `values-nl`)에 복사한 후 내용을 번역합니다.
3. 각 `<string>` 항목의 값을 번역합니다. 원래 의미의 기준으로 항상 `res/values/strings.xml`을 사용하세요.
4. 자리 표시자(예: `%1$s`, `%d`)와 서식 태그(예: `<b>`, `\n`)는 그대로 유지하세요. 절대 번역하거나 삭제하지 마세요.
5. `translatable="false"` 항목은 제거하거나 그대로 두세요. 번역해서는 안 됩니다.
6. 변경 사항을 테스트한 후 어떤 언어를 업데이트했는지 설명하여 Pull Request를 생성합니다.

예시:

```xml
<!-- res/values/strings.xml (source) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

okmore를 전 세계 더 많은 사람들이 사용할 수 있도록 도와주셔서 감사합니다!

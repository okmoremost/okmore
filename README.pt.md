# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Download

Os links abaixo sempre apontam para os pacotes de versão mais recentes (GitHub Release):

- **Zh/En**: [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language**: [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Todos os downloads passam por `releases/latest/download/`, então você sempre obtém o pacote mais recente sem atualizar este endereço.

## Localização

Convidamos todos a contribuir com a localização deste projeto — seja adicionando um novo idioma ou melhorando uma tradução existente. Toda ajuda é bem-vinda.

Todas as strings traduzíveis ficam no diretório `res/`. Cada idioma tem sua própria pasta nomeada com base em seu locale:

- `res/values/` — strings padrão/base (chinês simplificado), usadas como fonte de referência
- `res/values-en/` — inglês
- `res/values-ja/` — japonês
- `res/values-ko/` — coreano
- `res/values-ru/` — russo
- `res/values-de/` — alemão
- `res/values-fr/` — francês
- `res/values-es/` — espanhol
- `res/values-pt/` — português
- `res/values-it/` — italiano
- `res/values-tr/` — turco
- `res/values-ar/` — árabe
- `res/values-th/` — tailandês
- `res/values-vi/` — vietnamita
- `res/values-in/` — indonésio
- `res/values-ms/` — malaio
- `res/values-zh-rTW/` — chinês tradicional

Cada pasta contém um arquivo `strings.xml`. O atributo `name` de cada entrada `<string>` é a chave e **não deve ser alterado** — traduza apenas o texto entre as tags.

### Como traduzir

1. Faça um fork deste repositório e clone-o localmente.
2. Abra o diretório `res/` e encontre a pasta do idioma com o qual deseja trabalhar.
   - Para **melhorar um idioma existente**, edite seu `strings.xml` diretamente.
   - Para **adicionar um novo idioma**, copie `res/values-en/strings.xml` para uma nova pasta chamada `values-<locale>` (por exemplo `values-nl` para holandês) e traduza seu conteúdo.
3. Traduza o valor de cada entrada `<string>`. Sempre use `res/values/strings.xml` como referência do significado original.
4. Mantenha os placeholders (como `%1$s`, `%d`) e as tags de formatação (como `<b>`, `\n`) exatamente como estão — nunca os traduza nem os remova.
5. Remova as entradas `translatable="false"` ou deixe-as intactas; elas não devem ser traduzidas.
6. Teste suas alterações e abra um Pull Request descrevendo qual idioma você atualizou.

Exemplo:

```xml
<!-- res/values/strings.xml (fonte) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Obrigado por ajudar a tornar o okmore acessível a mais pessoas ao redor do mundo!

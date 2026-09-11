# okmore

[English](README.md) | [简体中文](README.zh.md) | [繁體中文](README.zh-Hant.md) | [Português](README.pt.md) | [Español](README.es.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | [Русский](README.ru.md) | [Deutsch](README.de.md) | [Français](README.fr.md) | [Italiano](README.it.md) | [Türkçe](README.tr.md) | [العربية](README.ar.md) | [ไทย](README.th.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) | [Bahasa Melayu](README.ms.md)

## Téléchargement

Les liens ci-dessous pointent toujours vers les paquets de la dernière version (GitHub Release) :

- **Zh/En** : [okmore_lite.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_lite.apk)
- **All Language** : [okmore_full.apk](https://github.com/okmoremost/okmore/releases/latest/download/okmore_full.apk)

> Tous les téléchargements passent par `releases/latest/download/`, vous obtenez donc toujours le paquet le plus récent sans avoir à mettre à jour cette adresse.

## Localisation

Nous invitons tout le monde à contribuer à la localisation de ce projet — que ce soit en ajoutant une nouvelle langue ou en améliorant une traduction existante. Toute aide est la bienvenue.

Toutes les chaînes traduisibles se trouvent dans le répertoire `res/`. Chaque langue possède son propre dossier nommé d'après sa locale :

- `res/values/` — chaînes par défaut/de base (chinois simplifié), utilisées comme source de référence
- `res/values-en/` — anglais
- `res/values-ja/` — japonais
- `res/values-ko/` — coréen
- `res/values-ru/` — russe
- `res/values-de/` — allemand
- `res/values-fr/` — français
- `res/values-es/` — espagnol
- `res/values-pt/` — portugais
- `res/values-it/` — italien
- `res/values-tr/` — turc
- `res/values-ar/` — arabe
- `res/values-th/` — thaï
- `res/values-vi/` — vietnamien
- `res/values-in/` — indonésien
- `res/values-ms/` — malais
- `res/values-zh-rTW/` — chinois traditionnel

Chaque dossier contient un fichier `strings.xml`. L'attribut `name` de chaque entrée `<string>` est la clé et **ne doit pas être modifié** — traduisez uniquement le texte entre les balises.

### Comment traduire

1. Forkez ce dépôt et clonez-le localement.
2. Ouvrez le répertoire `res/` et trouvez le dossier de la langue sur laquelle vous souhaitez travailler.
   - Pour **améliorer une langue existante**, modifiez directement son `strings.xml`.
   - Pour **ajouter une nouvelle langue**, copiez `res/values-en/strings.xml` dans un nouveau dossier nommé `values-<locale>` (par exemple `values-nl` pour le néerlandais), puis traduisez son contenu.
3. Traduisez la valeur de chaque entrée `<string>`. Utilisez toujours `res/values/strings.xml` comme référence pour le sens d'origine.
4. Conservez les espaces réservés (comme `%1$s`, `%d`) et les balises de formatage (comme `<b>`, `\n`) exactement tels quels — ne les traduisez jamais et ne les supprimez jamais.
5. Supprimez les entrées `translatable="false"` ou laissez-les intactes ; elles ne doivent pas être traduites.
6. Testez vos modifications, puis ouvrez une Pull Request en décrivant la langue que vous avez mise à jour.

Exemple :

```xml
<!-- res/values/strings.xml (origen) -->
<string name="web_browsing_settings">网页浏览设置</string>

<!-- res/values-en/strings.xml (translation) -->
<string name="app_name">Browsing Settings</string>
```

Merci d'aider à rendre okmore accessible à davantage de personnes dans le monde !

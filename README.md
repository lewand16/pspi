##  [Technologie internetowe](ug.geojson), 2015/16

Projekty do wykonania:

1. Wprawki z notacji Markdown lub Asciidoctor (na rozgrzewkę 😅)
1. Moje notatki z … – zamiast wielokropka wpisać z czego
1. Prezentacja lub blog.


## Lista obecności

Linki do projektów na zaliczenie wpisujemy w jednym wierszu według wzoru:

    1. [Nazwisko, Imię](link do strony na github.io lub firebaseapp.com), [Moje notatki z …](link do repo z notatkami).

Nasze projekty:

1. [Włodek Bzyl](https://bayesian.firebaseapp.com), [Projekty](https://github.com/h5c3j/project-template).
1. MJ Andrzejewski
2. [Ewa Barczak](https://github.com/ewagrzywka)
1. AA Bemke
1. K Idziak
1. D Lachowicz
1. [Michał Lewandowski](https://github.com/lewand16)
1. SL Majewska
1. JG Mankiewicz
1. EM Ostrowska-Janczak
1. MH Pieper
1. M Puciato
1. J Rajewicz
1. J Rajewicz
1. D Stoltmann
1. AM Szostak
1. M Sawicka
1. D Uss
1. J Wałek
1. A Wróblewska
1. R Wróblewski
1. A Zieliński


### Linki

1. Sigma:
  - [Konfiguracja](https://inf.ug.edu.pl/konfiguracja). U dołu strony
    jest informacja dla studentów – loginy, adresy majlowe, stron domowych.
  - Michael Hartl.
    [Learn Enough Command Line to Be Dangerous](http://www.learnenough.com/command-line-tutorial)
  - [Bash](http://wbzyl.inf.ug.edu.pl/sp/unix-commands)
1. Git:
  - Michael Hartl.
    [Learn Enough Git to Be Dangerous](http://www.learnenough.com/git-tutorial)
  - [ProGit Book, v2](http://git-scm.com/book/en/v2)
  - [Using pull requests (on GitHub)](https://help.github.com/articles/using-pull-requests/)
  - [Konfiguracja](http://wbzyl.inf.ug.edu.pl/sp/git)
1. Edytory:
  - Michael Hartl.
    [Learn Enough Text Editor to Be Dangerous](http://www.learnenough.com/text-editor-tutorial)
1. Markdown na GitHub:
  - [Syntax](http://daringfireball.net/projects/markdown/syntax)
  - [GitHub Flavored Markdown](http://guides.github.com/overviews/mastering-markdown/)
1. [Asciidoctor](http://asciidoctor.org)
  - [AsciiDoc User’s Guide](http://asciidoctor.org/docs/asciidoc-writers-guide/)
  - [AsciiDoc](http://www.methods.co.nz/asciidoc/) – home page
1. [GeoJSON Format Specification](http://geojson.org/geojson-spec.html):
  - [GeoJSON.io](http://geojson.io) – simply edit GeoJSON map data
  - [Mapping geoJSON files on GitHub](https://help.github.com/articles/mapping-geojson-files-on-github)
1. Prezentacje:
  - [Reveal.js](http://lab.hakim.se/reveal-js/) oraz [Slides](http://slid.es/)

[Firebase](https://www.firebase.com) – build extraordinary apps.
A powerful platform for your mobile or web application:

* [Hosting](https://www.firebase.com/docs/hosting/)
  Deploy your web app in seconds with our production-grade static
  asset hosting. From acquiring the SSL cert to serving your content on our
  global CDN, we do it all for you.

1. Sign in and log in.
1. Utwórz nową Appkę.
1. Na konsoli Bash wykonaj:

Następnie wykonaj:

```bash
mkdir public
asciidoctor -o public/index.html hello_world.adoc
firebase init
```

Przykładowy plik _hello_world.adoc_ użyty w poleceniu powyżej
jest w katalogu [asciidoctor](asciidoctor).
Zamiast niego użyj własnego pliku w formacie AsciiDoctor.


### Użyteczne narzędzia

- [Atom](https://atom.io) – a hackable text editor for the 21st Century:
  - [Atom Flight Manual](https://atom.io/docs/latest/) – the latest version
  - packages: [language-asciidoc](https://atom.io/packages/language-asciidoc),
    [asciidoc-preview](https://atom.io/packages/asciidoc-preview)
  - themes: seti-syntax, seti-ui, monokai, monokai-inverted
  - [keyboard shortcuts](https://github.com/nwinkler/atom-keyboard-shortcuts)
- [Secure Shell](http://en.wikipedia.org/wiki/Secure_Shell)
  (klucz publiczny, klucz prywatny; generowanie kluczy)
- [GitHub Desktop](http://windows.github.com/)


### Zrób to sam

- [JS Bin](http://jsbin.com/) – collaborative JavaScript Debugging
- [CodePen](http://codepen.io/) – front end developer playground & code editor in the browser
- [Adobe Kuler](https://kuler.adobe.com/create/color-wheel/) – color wheel and schemes
- [Reply.it](http://repl.it/languages/JavaScript)
- Atom: zmieniamy wielkość fontu w widoku „tree”, wklejając w pliku
  *~/.atom/styles.less* ten kod:

```less
@tree-view-font-size: 14px;
@tree-view-line-height: 28px;

.tree-view {
  font-size: @tree-view-font-size;

  .list-group li:not(.list-nested-item),
  .list-tree li:not(.list-nested-item),
  .list-group li.list-nested-item > .list-item,
  .list-tree li.list-nested-item > .list-item {
    line-height: @tree-view-line-height;
  }
  .list-group .selected::before,
  .list-tree .selected::before {
    height: @tree-view-line-height;
  }
}
```
Przedefinowujemy w pliku *keymap.json* (Settings>Keybindings)
skrót do Command Palette:

```yaml
'.platform-linux':
  'cmd-shift-p': 'command-palette:toggle'
```

Do pliku *~/.atom/snippets.cson* dopisujemy dwa snippety:

```yaml
'.source.asciidoc':
  'Relative link':
    'prefix': 'link'
    'body': 'link:$1[$2]'
  'Code block with title and syntax highlighting':
    'prefix': 'ch'
    'body': '[source,$1]\n----\n$0\n----'
```

## Rozkład zajęć

1\. Git:

- Zakładamy konto na serwerze GitHub
- Tworzymy pierwsze repozytorium na GitHub
- [GitHub Guides](https://guides.github.com/)
- [Got 15 minutes and want to learn Git?](http://try.github.io/levels/1/challenges/1)

2\. HTML & CSS

- [HTML 5 Outliner](https://gsnedders.html5.org/outliner/);
  [Chrome extension](https://chrome.google.com/webstore/detail/html5-outliner/afoibpobokebhgfnknfndkgemglggomo)
- [Thinkful HTML](https://github.com/mjhea0/thinkful-html) –
  wprowadzenie do HTML i CSS
  - [Web Design/HTML Challenges](http://en.wikiversity.org/wiki/Web_Design/HTML_Challenges)
- [Learn CSS Layout](http://learnlayout.com/)

3\. HTML5

- [HTML5 element list](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML/HTML5/HTML5_element_list) –
  [MDN](https://developer.mozilla.org/pl/) (Mozilla Developer Network)
- [HTML5 Element Index](http://html5doctor.com/element-index/)
- [HTML4 Element Index](http://www.w3.org/TR/html4/index/elements.html)
- [To close or not to close](http://www.colorglare.com/2014/02/03/to-close-or-not-to-close.html)
- Tommi Kaikkonen:
  * [Interactive Guide to Blog Typography](http://www.kaikkonendesign.fi/typography/)
  * [Why Websites Are White](http://www.kaikkonendesign.fi/why-websites-are-white/)
- [Materialize](http://materializecss.com) –
  a modern responsive front-end framework based on
  [material design](http://www.google.com/design/spec/material-design/introduction.html);
  zob. też [Make Material Design Websites with the Materialize CSS Framework](https://scotch.io/tutorials/make-material-design-websites-with-the-materialize-css-framework)

4\. CSS3

- [Bootstrap](http://getbootstrap.com)
  - [Less](http://lesscss.org) (LessCSS czy Less.js)
- [Foundation](http://foundation.zurb.com)
- [Milligram](http://milligram.github.io/) – a minimalist CSS framework
- [Cascading Style Sheets](http://www.w3.org/Style/CSS/)
- [Getting started with CSS](https://developer.mozilla.org/en-US/docs/Web/Guide/CSS/Getting_started)
- [CSS Diner](http://flukeout.github.io/) – where we feast on CSS Selectors!

5\. JavaScript

- Marijn Haverbeke. [Eloquent JavaScript](http://eloquentjavascript.net/) –
  A Modern Introduction to Programming
- Kyle Simpson. [You Don’t Know JS](https://github.com/getify/You-Dont-Know-JS)

Rozszerzenia dla przeglądarki Firefox:

  - [Firebug](https://addons.mozilla.org/en-US/firefox/addon/firebug/)
  - [Firebug Command Line API](https://getfirebug.com/wiki/index.php/Command_Line_API)

[Node.js](http://nodejs.org/):
```console
alias n="env NODE_NO_READLINE=1 rlwrap node"
```

Dokumentacja:

- [MDN & JavaScript](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
  - [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
- John Resig.
  [Secrets of the JavaScript Ninja](http://ejohn.org/apps/learn/) – funkcje w JavaScript

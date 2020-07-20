[![kawa.css](src/img/kawacss-logo.svg)](https://kawacss.rriver.dev)

# kawa.css
クラスレス（class-less）で使えるデモページ作成用の簡易CSSフレームワーク。

※まだ最新版のMac Chrome、Firefox、Safariでしか確認できてません！

## シンプルなスタイルです
ブラウザのデフォルトを極力生かしてスタイルしたシンプルなフレームワークです。文章が読みやすいように、見出しや文字サイズ、行間を設定しています。

## デモページ
スタイルはデモページでご確認ください。

- [デモページ](https://kawacss.rriver.dev/)

## ファイル構成
- ソースファイルはすべてsrcディレクトリに入ってます。
- スタイルはSassを使って書いています。
- HTML要素にあてているベースのスタイルは[src/sass/foundation/_base.scss](src/sass/foundation/_base.scss)に書いてあります。
- ウィンドウ幅に合わせて文字サイズをフレキシブルに変更するレスポンシブ・タイプのMixin（[_mixin-fluid-type.scss](src/sass/global/_mixin-fluid-type.scss)）を使っています。
- Sassは[@useを使った新しいモジュールシステム](https://parashuto.com/rriver/development/sass-module-system-from-import-to-use)で記述しています。

### srcディレクトリの構成

```
├── css
│   └── style.css
├── sass
│   ├── foundation
│   │   └── _base.scss
│   ├── global
│   │   ├── _index.scss
│   │   ├── _mixin-fluid-type.scss
│   │   └── _variables.scss
│   └── style.scss
├── elements.html
├── elements-en.html
├── flexible-typesize.html
└── index.html
```

## サンプルページ
### 日本語
- [ページ構成要素一覧](src/elements.html)
- [フレキシブルなタイプサイズの検証](src/flexible-typesize.html)

### English
- [A List of HTML Element Styles](src/elements-en.html)

## フォントサイズ・チャート
### 日本語
|| h1 | h2 | h3 | h4 | p |
|--|:--:|:--:|:--:|:--:|:--:|
| Max | 2.625rem<br>(42px) | 2rem<br>(32px) | 1.625rem<br>(26px) | 1.125rem<br>(18px) | 1.0625rem<br>(17px) |
| Min | 2rem<br>(32px) | 1.764705882rem<br>(28.235294112px) | 1.433823529rem<br>(22.941176464px) | 0.992647059rem<br>(15.882352944px) | 0.9375rem<br>(15px) |

### English
英語版はh4要素だけサイズが異なります。

|| h4 |
|--|:--:|
| Max | 1.25rem<br>(20px) |
| Min | 1.102941176rem<br>(17.647058816px) |

## section要素
コンテンツ・ブロックをsection要素で囲むことで最大幅680pxで中央寄せのカラムになります。幅は[src/sass/global/_variables.scss](src/sass/global/_variables.scss)の$width-max-contentで変更可能。

## ToDo
- ブラウザテスト（すみません、まだMac Chrome、Firefox、Safariでしか見てません！）
- グローバルナビゲーション（header）の追加
- ローカルナビーゲーション（aside）の追加
- レスポンシブ対応
- 抜けている要素のスタイルの追加
  - summary/details
  - image with a caption
  - table caption
  - focus style
  - pre > code block
- フォーム要素のスタイルの追加
- 英語版の追加
- Themeableにする（クラスあり？Sassで？）
- Dark Modeの追加（いる？）
# [![kawa.css](img/kawacss-logo.svg)](https://kawacss.rriver.dev)

クラスレス（class-less）で使えるデモページ作成用の簡易CSSフレームワーク。
ブラウザのデフォルトを極力生かしてスタイルしたシンプルなフレームワークです。文章が読みやすいように、見出しや文字サイズ、行間を設定しています。

※まだ最新版のMac Chrome、Firefox、Safariでしか確認できてません！

## デモページ
スタイルはデモページでご確認ください。

- [デモページ](https://kawacss.rriver.dev/)

## 使い方
kawa.cssを使いたいページの`<head>`で以下のCSSを読み込んでください。

```
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/rriver/kawa.css@0.1.1-alpha/css/kawa.min.css">
```

[デモページの要素一覧](https://kawacss.rriver.dev/elements.html)のスタイルを参考に、セマンティックなHTMLでページを構成してください。

## section要素
コンテンツ・ブロックをsection要素で囲むことで最大幅680pxで中央寄せのカラムになります。幅は[_variables.scss](sass/global/_variables.scss)の$width-max-contentで変更可能。

## レスポンシブ・フォントサイズ
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

## ToDo
- 「使い方」ページの追加
- Githubリポジトリへのリンク追加
- ブラウザテスト（すみません、まだMac Chrome、Firefox、Safariでしか見てません！）
- レスポンシブ対応
- 抜けている要素のスタイルの追加
  - image with a caption
  - table caption
  - focus style
- フォーム要素のスタイルの追加
- 各要素のソースコードを追加
- Githubリポジトリのディレクトリ構成の整理
- 英語版の追加
- Themeableにする（クラスあり？Sassで？）
- Dark Modeの追加（いる？）
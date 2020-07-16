# kawa.css
クラスレス（class-less）で使えるデモページ作成用の簡易CSSフレームワーク。

## シンプルなスタイルです
こんな感じのすごくシンプルなスタイルですが、日本語が読みやすいように、見出しや文字サイズ、行間などを細かく設定しています。

<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">スタイルを読み込めばブラウザのデフォルトスタイルをもう少し読みやすく調整してくれるノークラス（no-class）またはクラスレス（classless）のスタイルコレクションを作ってみてる<br><br>添付の動画はサンプルページをスクロースしているものをキャプチャしたもの <a href="https://t.co/QrVkeub2uO">pic.twitter.com/QrVkeub2uO</a></p>&mdash; RYO@Rriver (@rriver) <a href="https://twitter.com/rriver/status/1283312011447635968?ref_src=twsrc%5Etfw">July 15, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

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
├── flexible-typesize.html
└── index.html
```

## サンプルページ
### 日本語
- [ページ構成要素一覧](src/elements.html)
- [フレキシブルなタイプサイズの検証](src/flexible-typesize.html)

## フォントサイズ・チャート
|| h1 | h2 | h3 | h4 | p |
|--|:--:|:--:|:--:|:--:|:--:|
| Min | 2rem<br>(32px) | 1.764705882rem<br>(28.235294112px) | 1.433823529rem<br>(22.941176464px) | 0.992647059rem<br>(15.882352944px) | 0.9375rem<br>(15px) |
| Max | 2.625rem<br>(42px) | 2rem<br>(32px) | 1.625rem<br>(26px) | 1.125rem<br>(18px) | 1.0625rem<br>(17px) |

## ToDo
- レスポンシブ対応
- 抜けている要素のスタイルの追加
- フォーム要素のスタイルの追加
- 英語版の追加
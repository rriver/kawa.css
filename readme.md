# kawa.css
クラスレス（class-less）で使えるデモページ作成用の簡易CSSフレームワーク。

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
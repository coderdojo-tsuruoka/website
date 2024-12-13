[hugo]: https://gohugo.jo
[go]: https://go.devb
[hugo-universal-theme]: https://github.com/devcows/hugo-universal-theme
[DojoPaaS]: https://github.com/coderdojo-japan/dojopaas

<img src="http://images.coderdojo-tsuruoka.com/CoderDojoLogo.png" alt="CoderDojo Tsuruoka">

CoderDojo Tsuruoka Webサイト(ホームページ)

---- 

## 概要

CoderDojo Tsuruokaの公開用Webページ。
どんな活動をしているかなどをお知らせする。


## 利用している技術

| Technology | Version | Note |
| ---------- | ------- | ---- |
| [Hugo] | 0.138.0 | [Go]を利用した静的サイトジェネレーター |
| [Go] | 1.20 or later | Hugoのバックエンド / Dependency: Hugo |
| Git | - | ページリソースの共有ツール / Dependency: Hugo |
| Dart Sass | - | Dartで書かれたSassコンパイルツール / Dependency: Hugo |
| [hugo-universal-theme] | 1.4.1 | Hugoで利用しているテーマ |
| [DojoPaaS] | - | Webサイト公開クラウド(Ubuntu) |
| nginx | - | Webサイト公開Webサーバ |

## よく使うコマンド

| Command | Process | Note |
| ---------- | ------- | ---- |
| `hugo new <filepath>` | 新しい記事を作る | `<filepath>`の基準は`content`フォルダ |
| `hugo server` | プレビュー用仮想サーバの起動 | オプション`-D`をつけると、ドラフト状態のものも表示される |
| `hugo` | 公開用のファイル生成 | `public`フォルダにファイルを出力する |
| `hugo version` | Hugoのバージョン表示 ||

[公式サイトのコマンドページ](https://gohugo.io/commands/)

## フォルダ構造

```
.
├── archetypes                  コンテンツ(個別ページ)のテンプレート
├── content                     コンテンツ(個別ページ)の管理フォルダ
│   └── coderdojo                   定期イベント関連
│       └── secret                      参加者限定ページ(git submoduleとして取得/private)
├── data                        ウィジェット用のデータ管理フォルダ
│   ├── carousel                    トップページの上部カルーセル表示
│   ├── features                    提供サービス表示
│   ├── testimonials                参加者の声
│   └── clients                     ご支援いただいている企業・団体
├── layouts                     レイアウト管理フォルダ
│   ├── _default                    デフォルト
│   ├── partials                    テーマを上書きするレイアウト
│   └── shortcodes                  ショートコード(カスタムウィジェット)
├── public                      公開ページの出力先(Git管理外)
├── static                      CSSや画像などの静的ファイル管理フォルダ
└── themes                      Webサイトのテーマ(git submoduleとして取得)
```

## 環境構築方法

Wikiページの[Installation](https://github.com/coderdojo-tsuruoka/website/wiki/Installation)参照


## 変更ルール

Wikiページの[DevRule](https://github.com/coderdojo-tsuruoka/website/wiki/DevRule)参照

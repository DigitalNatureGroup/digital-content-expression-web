# digital-content-expression-web

このレポジトリは、ディジタルコンテンツ表現演習の制作展のWebページを公開するためのレポジトリです。

## ディレクトリ構造

- `/`
  - 当該年のホームページを格納する
- `/20XX`
  - 20XX年のホームページを格納する
  - 2023年度はReactを採用したため、ビルドされたファイルのみを `/2023` に配置しました（[リポジトリ](https://github.com/inaniwaudon/digicon2023-web)）
- `CNAME`
  - カスタムドメインの設定に使用されている
- `404.html`
  - SPAのリダイレクトに使用されている
- `.gitignore`

## 開発

```bash
yarn
# localhost:8080 に開発サーバを立ち上げる
yarn run start
```

## URL

このレポジトリはGitHub Pagesによってホスティングされています。

GitHub PagesのURLに対してカスタムドメインを適用しています。

参考: [https://docs.github.com/ja/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages](https://docs.github.com/ja/pages/configuring-a-custom-domain-for-your-github-pages-site/about-custom-domains-and-github-pages)


## 各年Web担当者の操作 (WIP)

1. 自分の年度のディレクトリを作成する
2. 自分の年度のディレクトリにウェブサイトのデータをアップロードする
3. トップページに自分の年度のディレクトリへのリンクを追加する
4. (optional) トップページ(各年度へのリンクを収めたページ)のデザインを変更する
   - 作り方は前年度のトップページを参考に
5. 来年度に引き継ぐ

- 作業時の注意点としてトップディレクトリの以下のファイルを削除しないように
  - `CNAME`: カスタムドメインの設定に使用されている
  - `404.html`: SPAのリダイレクトに使用されている
  - `.gitignore`

### `404.html`の動作に関して
404ページではreactやVueなどのRouterを使ったSPAなサイト向けにパスのルーティングをクエリ文字列で解決しています。

設定方法や各年度のサイトでの実装方法は参考サイトを参考にしてください。

参考: [https://maku.blog/p/9u8it5f/](https://maku.blog/p/9u8it5f/)

### 担当者

| 年度 | 名前     | 学籍番号  | 連絡先                  | Twitter |
| ---- | -------- | --------- | ----------------------- | -------- |
| 2021 | 浪川洪作 | 201911425 | cigarbox.nami@gmail.com | @73_ch |
| 2022 | 香取賢佑 | 202010246 | kenkenissocool@gmail.com | @kenkenissocool |
| 2023 | 和田優斗 | 202111710 | <me@yokohama.dev> | @kyoto_inaniwa |

なお、本レポジトリの仕組み等については2021年度担当者浪川に連絡のこと

当レポジトリはDNGオーガニゼーション内にあるため、研究室外の担当者が操作する場合などは先生の確認などを取ること、基本的にはDNGの人間がアップロード等の操作をすることが望ましい

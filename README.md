# 知っているようで知らない OGP の書き方

こちらは OGP についての勉強会資料です。

動作確認用のコードになります。
詳しい解説はブログに記載しする予定です。

## OGP とは？

[公式サイト](https://ogp.me/#metadata)

## 基本設定

#### サイトタイトル

```html
<meta property="og:title" content="（サイトタイトル）" />
```

- サイトのタイトルを指定
- og:title に`<title>`タグと別の言葉を設定すると、そちらが優先して表示される。
- 文字数は 20 文字以内が適切。

#### ページの URL

```html
<meta property="og:url" content="（ページのURL）" />
```

- WEB ページの URL を指定
- URL は相対パスではなく絶対パスで記述

#### ページの種類

```html
<meta property="og:type" content="（ページの種類）" />
```

- website: Web サイト TOP ページ
- blog: ブログ TOP ページ
- article: 記事ページ等のページ
- product: 製品紹介ページ
- #### ページの説明

```html
<meta property="og:description" content="（ページの説明）" />
```

- ６０〜８０文字の概要説明を設定

- #### OGP 画像

```html
<meta property="og:image" content="（ogp画像のURL）" />
```

- シェア時に表示する画像を指定
- こちらも絶対パスで指定
- 基本サイズは幅 1200px 高さ 630px
- 表示確認は[OGP シュミレーター](http://ogimage.tsmallfield.com/)が便利

## Twitter での OGP 設定

[Twitter 公式サイト](https://developer.twitter.com/ja/docs/tweets/optimize-with-cards/guides/getting-started)

### カードの種類

```html
<meta name="twitter:card" content="カードの種類" />
```

- summary：通常の表示
- summary_large_image：大きめのカードで表示される
- app：アプリ配布用の表示カード。アプリの名前や紹介文、アプリアイコンに加えて、評価や価格などの表示もされる。
- player：ビデオやオーディオなどのメディアを表示できるカード

## Facebook での OGP 設定

### トラフィックの分析

```html
<meta name="fb:app_id" content="FacebookアプリID" />
```

- Facebook インサイトを使ってトラフィックの分析を行うことができる。
- [Facebook for Developers](https://developers.facebook.com/?no_redirect=1)の登録が必要

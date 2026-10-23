---
title: 'Goodbye gatsby. Hello astro'
description: 'gatsbyからastroに乗り換え'
pubDate: '2026/10/23'
---

## 構成を  gatsby から Astro に変更
- [gatsby](https://github.com/gatsbyjs/gatsby "gatsby")
- [astro](https://github.com/withastro/astro "astro")

このサイトのGitHub Pagesを、GatsbyからAstroに乗り換えました。  
移行して感じたメリットは次のとおりです。  

### 1. ビルドが速く、動作が軽い
Astroは、必要な部分以外はJavaScriptを出力せず、基本的に静的なHTMLだけを生成します。そのため、ページの読み込みが軽くなり、ビルドも短時間で終わります。GatsbyのようにReactのランタイムが全ページに乗ることがありません。

### 2. 依存関係がシンプルで、メンテナンスしやすい
Gatsbyは、GraphQLやプラグイン群、Reactのバージョンの組み合わせに悩まされがちでした。Astroは構成が単純なので、依存パッケージの更新で壊れにくく、長く運用しやすいと感じています。

### 3. Markdownとの相性が良い
記事はMarkdown(MDX)でそのまま書け、Content Collectionsでフロントマターの型チェックもできます。GatsbyのようにGraphQLでデータを取得する手間がなく、記事の管理が直感的になりました。

### 4. 好きなUIフレームワークを使える
React、Vue、Svelteなどを必要な部分だけに導入できます。普段は静的HTMLで軽く保ちつつ、インタラクティブな部品だけ後から足すことも可能です。

### 5. GitHub Pagesと相性が良い
静的ファイルとして出力されるので、GitHub Actionsによるデプロイ設定が簡単です。公式のデプロイ手順も整っていて、迷わず公開できました。

## まとめ
「軽い、速い、壊れにくい」という点が、乗り換えの決め手でした。  
個人ブログや技術メモのような静的サイトには、Astroがちょうど良い選択だと思います。  
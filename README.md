# NUEE 宇宙電磁環境工学 宇宙情報処理研究グループ 三好研究室 ウェブサイト

## フレームワーク

本ウェブサイトは以下の技術スタックで構築されています。

- 静的ウェブサイトジェネレータ [Hugo](https://github.com/gohugoio/hugo)
- テーマ [PaperMod](https://github.com/adityatelange/hugo-PaperMod)
- デプロイ: GitHub Pages (GitHub Actions)

## ローカルでのプレビュー方法

事前準備: Hugoをインストールしておく必要があります。公式サイトの[インストールガイド](https://gohugo.io/installation/)を参照してください。

```shell
# ① ローカルサーバーの起動
hugo server

# ② ブラウザで http://localhost:1313/ にアクセスしてプレビュー
```

## 記事の編集方法

- 基本的には `content/`以下のマークダウンファイルを編集して済ませる
- 画像や動画などそのまま公開したいファイルは `static/`以下に置く
- 各記事のYAMLヘッダには、タイトル、日付、タグをつける (次項参照)

## 記事作成上のルール: YAMLヘッダをつける

`content/posts/` 以下のマークダウンファイルには、以下のようなYAMLヘッダをつけることが推奨されます。

```yaml
---
title: "American Geophysical Union (AGU) 2025 Fall meeting"
date: 2025-12-15
tags: ["events"]
---
```

- `title`: 記事のタイトル
- `date`: 記事の日付 (YYYY-MM-DD形式)
- `tags`: 記事のタグ (カンマ区切りで複数指定可能)
  - `"events"`: イベント関連の記事

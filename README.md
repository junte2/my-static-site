# my-static-site

GitHub Pages で公開するテキスト日記サイトです。

## 概要

シンプルな HTML / CSS / JavaScript のみで構成された静的サイトです。
日々の記録・気づき・読書メモなどをテキスト形式で掲載しています。

## ファイル構成

```
.
├── index.html        # メインページ（日記一覧 & 記事詳細モーダル）
├── style.css         # スタイルシート
├── diary/
│   ├── index.json    # 日記ファイルの一覧（yyyymmdd 形式の配列）
│   ├── 20260305.md   # 日記ファイル（yyyymmdd.md 形式）
│   └── ...
└── README.md
```

## 日記の追加方法

1. `diary/yyyymmdd.md` を作成し、以下の形式で記述します。

   ```markdown
   # タイトル

   本文（マークダウン記法）
   ```

2. `diary/index.json` の配列の先頭に `"yyyymmdd"` を追加します。

   ```json
   ["20260306", "20260305", ...]
   ```

## 公開方法

GitHub のリポジトリ設定 → **Pages** から、ブランチを `main`、フォルダを `/ (root)` に指定するだけで公開できます。

## ライセンス

MIT

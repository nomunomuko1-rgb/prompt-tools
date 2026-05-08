# prompt-tools

はてなブログ用コピペボックス ジェネレーター（単一HTMLツール）。

**URL:** `https://nomunomuko1-rgb.github.io/prompt-tools/generator.html`

---

## ファイル構成

```
prompt-tools/
├── generator.html   ← はてなブログ用コピペボックス ジェネレーター
└── README.md        ← このファイル
```

---

## 使い方

1. `generator.html` をブラウザで開く（PCでもスマホでも可）
2. 絵文字・ラベル名・お題本文を入力
3. 「生成してプレビュー」→ 「HTMLをコピー」
4. はてなブログのHTML編集モードに貼り付け

**出力HTMLに内蔵されているもの:**
- コピペボックスのCSS（紫グラデーションテーマ）
- コピーボタンのJavaScript
- ラベル＋textareaにお題本文

**保存機能:** 作成したお題はブラウザのlocalStorageに自動保存される（ブラウザを閉じても残る）。左カラムの一覧からクリックで再読み込み・再編集可能。

---

## 🚨 お題配布サイトは別リポジトリ

このリポジトリは **ジェネレーター専用**。
AI用お題（プロンプト）の配布サイト本体は以下のリポジトリにある:

- **リポジトリ:** `nomunomuko1-rgb/nomunomuko1-rgb.github.io`
- **URL:** `https://nomunomuko1-rgb.github.io/`

お題HTMLの追加・編集が必要な場合はそちらを操作すること。

---

## デプロイ

```bash
git add .
git commit -m "..."
git push origin main
```

プッシュ後、自動的にGitHub Pagesに反映される。

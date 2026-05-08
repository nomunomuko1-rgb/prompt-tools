# prompt-tools

AI用お題（プロンプト）の配布サイト＋はてなブログ用コピペボックスジェネレーター。

**デプロイ先:** `https://nomunomuko1-rgb.github.io/prompt-tools/`

---

## ファイル構成

```
prompt-tools/
├── index.html              ← お題一覧サイト（GitHub Pagesのトップ）
├── generator.html          ← はてなブログ用コピペボックス ジェネレーター
├── *.html                  ← 各お題ページ（AI用プロンプト本文＋コピーUI）
├── images/                 ← 画像アセット
└── README.md               ← このファイル
```

---

## 2つのツール

### 1. お題配布サイト (`index.html` + 各 `*.html`)

GitHub Pagesでホストされる静的サイト。カテゴリ別にお題カードが並び、各ページに飛ぶとプロンプト本文をコピーできる。

**新しいお題を追加する手順:**
1. お題用のHTMLファイルを作成（既存の `*.html` をテンプレートに）
2. `index.html` の該当カテゴリにカードを追加
3. コミット＆プッシュ → 自動デプロイ

### 2. はてなブログ用ジェネレーター (`generator.html`)

ブラウザで開くだけで使える単一HTMLツール。はてなブログのHTML編集モードに貼り付けるコピペボックスを生成する。

**使い方:**
1. `generator.html` をブラウザで開く
2. 絵文字・ラベル名・お題本文を入力
3. 「生成してプレビュー」→ 「HTMLをコピー」
4. はてなブログのHTML編集に貼り付け

**出力されるHTMLには以下が内蔵されている:**
- コピペボックスのCSS（紫グラデーションテーマ）
- コピーボタンのJavaScript
- ラベル＋textareaにお題本文

**保存機能:** localStorageに保存される（ブラウザを閉じても残る）。

---

## デプロイ

リポジトリ: `nomunomuko1-rgb/prompt-tools`
GitHub Pages: `main` ブランチ → 自動デプロイ

```bash
git add .
git commit -m "..."
git push origin main
```

---

## 外部依存

- お題配布サイト: 一部のお題は外部リンク（`nomunomuko1.web.fc2.com`）を参照
- はてなブログ用ジェネレーター: 完全自己完結、外部依存なし

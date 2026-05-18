# 買い物メモ PWA

## Vercelへのデプロイ手順

### 方法1：ドラッグ＆ドロップ（最も簡単）

1. [vercel.com](https://vercel.com) にアクセスしてアカウント作成（無料・GitHubログイン可）
2. ダッシュボードの **"Add New → Project"** をクリック
3. **"Or deploy from your local files"** のリンクから、この `shopping-memo` フォルダをまるごとドラッグ＆ドロップ
4. そのまま **Deploy** をクリック
5. 数秒で `https://xxxxx.vercel.app` のURLが発行されます

### 方法2：Vercel CLI

```bash
npm i -g vercel
cd shopping-memo
vercel --prod
```

---

## iPhoneでホーム画面に追加する手順

1. SafariでデプロイされたURLを開く
2. 画面下の **共有ボタン（□↑）** をタップ
3. **「ホーム画面に追加」** をタップ
4. 名前はそのままで **「追加」** をタップ

これでアプリとして使えます。オフラインでも動作します。

---

## 機能

- **いつも買うもの**：買い物完了後もリストに残る
- **今回だけ買うもの**：リセット時に削除される
- タップでチェック／チェック解除
- 「買い物完了・リセット」で一括リセット
- ダークモード対応
- オフライン対応（Service Worker）
- データはブラウザのlocalStorageに保存（サーバー不要）

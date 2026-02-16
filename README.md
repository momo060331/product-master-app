# 商品マスター登録アプリ

在庫管理アプリと連携する商品マスター登録専用アプリです。

## 📦 機能

- 📷 バーコードスキャン（通常・連続）
- ✍️ 手動登録
- ✏️ 商品編集・削除
- 🔍 検索機能
- 📊 CSV入出力
- 🔄 Firebase同期（在庫管理アプリと連携）
- 📱 PWA対応（オフラインでも動作）

## 🚀 GitHub Pagesでのデプロイ方法

### 1. GitHubリポジトリを作成

```bash
# リポジトリを作成（GitHubのWebサイトで）
# 例: product-master-app
```

### 2. ファイルをアップロード

以下のファイルをリポジトリのルートにアップロード：

```
product-master-app/
├── product-master.html  （メインファイル）
├── manifest.json         （PWA設定）
├── service-worker.js     （オフライン対応）
├── icon-192.png          （アイコン192x192）
├── icon-512.png          （アイコン512x512）
└── README.md             （このファイル）
```

### 3. GitHub Pagesを有効化

1. リポジトリの **Settings** → **Pages**
2. **Source** を **Deploy from a branch** に設定
3. **Branch** を **main** / **root** に設定
4. **Save** をクリック

### 4. アクセス

数分後、以下のURLでアクセス可能：
```
https://[ユーザー名].github.io/product-master-app/product-master.html
```

## 📱 スマホにインストール

### iOS (Safari)
1. 上記URLにアクセス
2. 共有ボタン → 「ホーム画面に追加」

### Android (Chrome)
1. 上記URLにアクセス
2. メニュー → 「ホーム画面に追加」

## 🔗 在庫管理アプリとの連携

1. 在庫管理アプリと同じブラウザで開く
2. 自動で同じユーザーIDが使用される
3. 商品マスターで登録した商品が在庫管理アプリで利用可能

## 📝 CSV形式

```csv
JANコード,商品名,大カテゴリ,中カテゴリ,小カテゴリ,保管場所,基準価格,メモ
4901234567890,醤油,食品,調味料,醤油,キッチン棚A,298,1Lボトル
```

## 🛠️ 技術スタック

- HTML5/CSS3/JavaScript
- Firebase Firestore（データベース）
- html5-qrcode（バーコードスキャン）
- PWA（Progressive Web App）

## 📄 ライセンス

MIT License

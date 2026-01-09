# 📚 資料検索AI Pro v4

Google Drive + Gemini File Search API を使った資料検索AIアプリケーション

## 機能

- ✅ Google Drive 共有ドライブからファイル取得
- ✅ 正確な拡張子表示（MIMEタイプ + ファイル名から判定）
- ✅ 拡張子別ファイル集計・フィルタリング
- ✅ ダウンロード前プレビュー機能
- ✅ 個別PCへのダウンロード
- ✅ Gemini AI によるRAG検索

## セットアップ

### 1. Gemini API キー取得

[Google AI Studio](https://aistudio.google.com/app/apikey) でAPIキーを取得

### 2. Google Cloud OAuth 設定

1. [Google Cloud Console](https://console.cloud.google.com/) でプロジェクト作成
2. OAuth 2.0 クライアントIDを作成
3. 承認済みJavaScriptオリジンに GitHub Pages URL を追加
   - `https://<username>.github.io`

### 3. クライアントID設定

`index.html` 内の `GOOGLE_CLIENT_ID` を自分のクライアントIDに変更

```javascript
const GOOGLE_CLIENT_ID = 'your-client-id.apps.googleusercontent.com';
```

## 使い方

1. https://<username>.github.io/<repo-name>/ にアクセス
2. Gemini API キーを入力
3. Google Drive に接続
4. 共有ドライブを選択
5. ファイルを選択してAI分析開始

## 対応ファイル形式

| カテゴリ | 形式 |
|---------|------|
| ドキュメント | PDF, DOC, DOCX |
| スプレッドシート | XLS, XLSX, CSV |
| プレゼンテーション | PPT, PPTX |
| テキスト | TXT, MD, JSON, HTML |
| アーカイブ | ZIP |
| 画像 | JPG, PNG, GIF, WebP |

## ライセンス

MIT License

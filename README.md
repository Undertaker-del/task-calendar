# タスクカレンダー

松尾研課題・大学課題・テスト・インターン等の予定を管理する自作カレンダー（依存ゼロの単一HTML / PWA）。

## 公開URL
- 本番（Vercel・常設）: https://task-calendar-calendar6.vercel.app/
- 予備（GitHub Pages）: https://undertaker-del.github.io/task-calendar/

`main` への push で Vercel が自動デプロイします。

## 特徴
- 月表示 / リスト表示、カテゴリ色分け、締切カウントダウン
- ライト・ダーク切替
- **PWA**: スマホの「ホーム画面に追加」でアプリ化（Dockに配置可）
- **GitHub Gist同期**: PC⇄スマホでデータを同期（トークンは各端末のブラウザ内のみ保存）
- JSONバックアップ / Googleカレンダー用 `.ics` 書き出し

## 使い方（スマホ）
1. 公開URLを Safari / Chrome で開く
2. 共有 →「ホーム画面に追加」
3. アプリ内「⋯ → 同期」で GitHubトークン（Gist権限）を登録

## 保存とデータ
- 予定データは各端末の localStorage に保存され、Gist経由で同期されます。
- 同期用トークンはリポジトリには含まれません（各端末で入力）。

## ローカルで開く
`index.html` をブラウザで開くだけで動作します（同期・PWA機能はHTTPS公開時のみ有効）。

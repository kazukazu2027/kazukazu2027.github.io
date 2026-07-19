# kazukazu2027.github.io

個人開発 iOS アプリ群のプライバシーポリシー・利用規約の公開用リポジトリ（GitHub Pages）。

- 公開 URL: https://kazukazu2027.github.io/
- 各アプリの規約はサブディレクトリ配下に置く: `https://kazukazu2027.github.io/{アプリ名}/privacy-policy.html`（利用規約は `terms-of-service.html`）

## 構成

- `index.html` — 全アプリの規約一覧ページ
- `{アプリ名}/privacy-policy.html` / `{アプリ名}/terms-of-service.html` — 各アプリの規約
- `.nojekyll` — Jekyll 処理の無効化（ファイルをそのまま配信）

正本は各アプリリポジトリの `docs/` にあり、ここは公開用のコピー置き場。

## アプリを追加・更新する手順

1. アプリリポジトリの `docs/privacy-policy.html` と `docs/terms-of-service.html` を、このリポジトリの `{アプリ名}/` にコピーする
   - ディレクトリ名は **アプリ内から参照している URL のパスに合わせる**こと（例: `https://kazukazu2027.github.io/worklog-app/...` なら `worklog-app/`）
2. 新規アプリの場合は `index.html` の一覧に行を追加する
3. コミットして push（push で自動的に再デプロイされる）

## 初回公開の手順

```sh
cd ~/kazukazu2027.github.io
gh repo create kazukazu2027/kazukazu2027.github.io --public --source=. --push
```

その後 GitHub の Settings > Pages で以下を確認する。

- Source: `Deploy from a branch`
- Branch: `main` / `/ (root)`

`kazukazu2027.github.io` という名前のリポジトリは Pages が自動で有効になるはずだが、反映まで数分かかることがある。デプロイ状況はリポジトリの Actions タブ（pages-build-deployment）で確認できる。

## 連絡先

- 開発者: kazukazu2027
- Email: kazu2000027@gmail.com

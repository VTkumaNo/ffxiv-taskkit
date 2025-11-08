# FINAL FANTASY XIV Task Tool Kit (GitHub Pages Starter)

このフォルダをそのまま GitHub リポジトリにアップロードすれば、GitHub Pages で公開できます。

## 手順（Web UI）
1. GitHub で新規リポジトリ作成（Public）
2. このフォルダの **全部のファイル** をアップロード（`index.html` がホームになります）
3. リポジトリの **Settings → Pages** を開き、
   - **Source:** `Deploy from a branch`
   - **Branch:** `main`（または `master`） / **Folder:** `/root`
4. 数十秒で公開 URL が発行されます（例: `https://<username>.github.io/<repo>/`）

## 手順（CLI）
```bash
git init
git add .
git commit -m "publish"
git branch -M main
git remote add origin https://github.com/<username>/<repo>.git
git push -u origin main
```
その後、Settings → Pages で公開設定を同様に行ってください。

## 補足
- `.nojekyll` は Jekyll のビルドをオフにするためのファイルです（ルート直下のファイルをそのまま配信したい場合に便利）。
- 保存データは **localStorage** に保持されます。公開 URL が変わると別ドメイン扱いになるため、ブラウザの保存データも別になります。
- スマホでホーム画面に追加すると、アプリっぽく起動できます。
  - Android: Chrome → 右上メニュー → **Add to Home screen**
  - iPhone: Safari → 共有 → **ホーム画面に追加**
- 変更を反映するには、`index.html` を置き換えて再コミット＆PushするだけでOKです。

Generated: 2025-11-08T15:44:56.594264

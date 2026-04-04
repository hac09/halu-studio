# halu-studio（GitHub Pages）

Halu Studio のプライバシーポリシー・サポート用サイトです。GitHub Pages で公開します。

- 公開例: [https://hac09.github.io/halu-studio/](https://hac09.github.io/halu-studio/)
- TravelLogger の例: [プライバシー](https://hac09.github.io/halu-studio/TravelLogger/) / [サポート](https://hac09.github.io/halu-studio/TravelLogger/support)

## 公開手順（概要）

1. このリポジトリを GitHub に push する（通常は `main` ブランチ）。
2. リポジトリの **Settings → Pages** でソースを指定する。
   - **Deploy from a branch** の場合: `main` + `/ (root)` など、Jekyll がビルドされる設定に合わせる。
   - **GitHub Actions** で Jekyll を使う場合は、公式の Pages 用ワークフローを利用してもよい。
3. 数分待つと `https://<ユーザー名>.github.io/halu-studio/` 配下に反映される。

※ リポジトリ名が `halu-studio` で、ユーザー／組織サイトでない **Project サイト** のときの URL は上記のとおり `.../halu-studio/` になります。

## 新しいアプリ用ページを足すとき

1. `アプリ名/` フォルダを作成する。
2. `index.html` … プライバシーポリシー（先頭に `layout: default` の YAML）。
3. `support.html` … サポートページ（同様に YAML）。
4. 公開済みアプリだけ、ルートの `index.md` のアプリ一覧にカードを追加する（未公開のときはページだけ置いて一覧から外すことも可）。
5. 一覧に載せる場合は `assets/images/` に `アプリ名-icon.png` などを置き、`index.md` の `img` パスを合わせる。

既存の `TravelLogger/` や `divvy/` をコピーして文言を差し替えると早いです。

## ローカルで確認（任意）

Ruby + Bundler 環境で Jekyll を実行するか、GitHub 上でプレビュー用ブランチを用意して確認してください。

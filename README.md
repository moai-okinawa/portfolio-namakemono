# 自己紹介サイト

ニックネーム・やっていること・作ったものを紹介する1ページのサイトです。
名前・プロフィール・活動は本人提供の内容です。掲載作品はダミーデータです。

## 表示方法

`index.html` をブラウザで開いてください。インストールやビルドは不要です。

## 編集方法

`index.html` の文章とイラストを編集してください。スタイルとSVG画像もこのファイルに含まれています。

- ニックネーム：ナマケモノ🦥
- 自己紹介：人間ですが、ナマケモノで活動中
- 活動：沖縄で猫と海とAIでなんかやってます
- 作品：喫茶店サイト、タスク管理ツール案、ポストカード
- PC・スマートフォン対応

## GitHub Pagesへの公開

`main` へのpushで `.github/workflows/deploy-pages.yml` が実行され、GitHub Pagesへ自動公開されます。Actionsの「Deploy to GitHub Pages」から手動実行もできます。

公開URL: https://moai-okinawa.github.io/portfolio-namakemono/

初回はリポジトリの **Settings → Pages → Build and deployment → Source** を **GitHub Actions** に設定します。

現在は外部ファイルを必要としないHTMLのため、`index.html` だけを公開対象にしています。画像・CSSなどを別ファイルにした場合は、ワークフローの `Prepare static site` でそれらも `_site` へコピーしてください。

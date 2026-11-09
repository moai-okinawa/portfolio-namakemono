# ナマケモノ🦥 ポートフォリオ Ver.1

沖縄 × 海 × 猫 × AI × ナマケモノの個人ポートフォリオ

公開URL: https://moai-okinawa.github.io/portfolio-namakemono/

## 掲載内容

- 自己紹介とAIを使った制作・学びの記録
- 海ドキ｜UMIDOKI?♥ — 一般公開中
- しまイマ。 — 一般公開中 / https://miwa-apps.github.io/shima-ima/
- MŌCHI!｜モ〜チッ — 開発中・ローカル版
- 羽海の気持ち推定機 — MUSE内で制作・ログ保存版
- AIキャラクター「ロイ」とInstagramへのリンク
- note記事とThreadsのリンクは追加待ち
- アプリ統合は将来の構想として記載

## 構成と編集

HTMLとCSSだけの1ページ構成で、インストールやビルドは不要です
`index.html` をブラウザで開いてプレビューできます

- `index.html` — 本文、作品カード、CSS
- `assets/` — アバター・海の背景写真・作品画像
- `assets/IMAGE-CREDITS.md` — 画像の出典と利用条件
- `.github/workflows/deploy-pages.yml` — mainへのpushによるGitHub Pages自動公開

海の背景写真はCC0素材をWebPへ最適化し、外部画像に依存せず配信しています
既存のアバターはそのまま使用しています
4作品の画像枠はPC300px・スマホ240pxで統一し、縦横比を保って全体を表示します

## 画像の差し替え

`assets/` に画像を追加し、該当カードのimgタグのsrc・alt・width・heightを変更します
width・heightは画像の実寸を指定してください
顧客情報・個人情報・業務データを含む画像は掲載しないでください

## リンクや記事の追加

未提供のURLは推測せず、確認できたものを追加します
外部リンクには `target="_blank" rel="noopener noreferrer"` を設定しています
限定公開・開発中の作品には閲覧リンクを設置していません

## Ver.1の確認

- PC1280px・スマホ390px／320pxのレイアウトを確認
- ページ内リンク、外部リンク設定、全画像の参照を確認
- 個人連絡先・認証情報・端末固有の絶対パスがないことを確認
- 提供された画面は紹介用で、MŌCHI!は未入力の操作確認用画面
- 海況判定と猫の気持ちの推定に関する注意書きを維持

# ナマケモノ🦥 ポートフォリオ

沖縄 × 海 × 猫 × AI × ナマケモノの個人ポートフォリオ
HTMLとCSSだけの1ページ構成で、インストールやビルドは不要です

## ローカルでのプレビュー

`index.html` をブラウザで開くと表示できます

HTTPで確認する場合は、このフォルダで以下を実行します

```sh
python3 -m http.server 4173 --bind 127.0.0.1
```

ブラウザで `http://127.0.0.1:4173/` を開きます
終了はターミナルで Ctrl+C

## 編集する場所

- `index.html` — 本文、作品カード、CSS
- `assets/namakemono.jpeg` — 既存のプロフィール画像
- `.github/workflows/deploy-pages.yml` — 既存の公開設定を維持

作品は `umidoki` → `shimaima` → `mochi` → `umi` の順です
カード内の `SCREENSHOT:` コメントを検索すると画像欄を見つけられます

## スクリーンショットの追加

1. 公開してよい画像を `assets/` に追加
2. 対象カードの `<div class="media-slot">…</div>` を次のような画像タグへ差し替え

```html
<img src="assets/umidoki.webp"
     alt="海ドキの海況比較画面"
     width="1200" height="800" loading="lazy">
```

ファイル名とaltは各画像に合わせて変更し、widthとheightは実寸を指定します
画像は縦横比を保って全体を表示します
スクリーンショットは未提供のため、仮画像や架空のアプリ画面は使用していません
ロイのサムネイルも同じ方法で追加できます
ブラウザUIは可能なら画像提供時に除き、個人情報や業務データが写っていないか確認します

## note記事の追加

`NOTE ARTICLE:` コメントのある準備中カードを、以下の形式に置き換えます
URLが未提供の間はリンクを付けません

```html
<article class="note-placeholder">
  <h3>実際の記事タイトル</h3>
  <p>記事の短い説明</p>
  <a href="提供された記事URL" target="_blank" rel="noopener noreferrer">noteで読む ↗</a>
</article>
```

note・ThreadsはURL確認待ちです
Instagramはロイの作品アカウント、GitHubはこのサイトのリポジトリへリンクします
限定公開のしまイマや、開発中のMŌCHI!に公開リンクは設けません

## 公開について

既存設定では `main` へのpushでGitHub Pagesが更新されます
改修は `codex/namakemono-portfolio-renewal` ブランチで行います
miwaの最終確認と承認までは、mainへのマージ・push・本番公開を行いません

公開URL: https://moai-okinawa.github.io/portfolio-namakemono/

## 今回の確認結果

- PC 1280px / スマホ 390px・320pxでレイアウト確認
- PCは作品2列、スマホは1列で横はみ出しなし
- 既存のナマケモノ画像は元ファイルと同一、読み込みと縦横比を確認
- 4作品の表示順、ページ内リンク先、外部リンクの安全属性を確認
- 海ドキ・Instagram・GitHubのリンク先はHTTP 200で応答
- 画面内の句点なし
- スクリーンショット4点、ロイのサムネイル、note記事・ThreadsのURLは追加待ち
- 公開ワークフローは変更なし

実機のスマートフォンでの最終確認はmiwaが行います

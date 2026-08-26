# zenn-content

Zenn の記事を管理するリポジトリです。GitHub 連携で `articles/*.md` が自動で公開されます。

## 公開までの手順

1. Zenn にログイン（GitHub アカウント推奨）
2. https://zenn.dev/dashboard/deploys で、このリポジトリを連携
3. 記事の frontmatter を `published: true` に変更
4. push すると Zenn 側に反映される

`published: false` の間は下書き扱いで、公開されません。

## 画像・GIF

`/images` に配置し、記事からは `/images/xxx.png` で参照します。
- **画像（png）** … 最終レポート `report.docx` の埋め込み画像
- **GIF** … 発表資料 `C3TB2504_webcom_final.pptx` の埋め込み動画から切り出し（ffmpeg、8fps、パレット最適化）

pptxには内容のある画像がほぼ入っていないため、静止画はレポート側から取っています。
Zennは動画ファイルを配信できないため、長い操作デモを載せる場合はYouTubeにアップロードして
`@[youtube](動画ID)` で埋め込みます。

## ローカルプレビュー

```bash
npm install
npx zenn preview
```

## 記事

| slug | タイトル | 状態 |
|---|---|---|
| `glossalyze-vocab-learning-app` | 英語教材のPDFや写真から単語・熟語を自動抽出する学習アプリを作った | 下書き |

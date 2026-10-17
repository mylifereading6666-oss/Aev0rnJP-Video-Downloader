# Aev0rnJP Video Downloader

スマートフォン・PCのブラウザで使える、無料の動画URL確認ツールです。GitHub Pagesでの公開を想定しています。

## 公開サイト

GitHub Pagesを有効化すると、通常は次のURLで公開されます。

https://mylifereading6666-oss.github.io/Aev0rnJP-Video-Downloader/

## 現在の機能

- スマートフォン・PC向けのレスポンシブUI、ダークテーマ
- HTTP/HTTPS URLの形式チェック
- 直接動画ファイルURLらしい形式（MP4、WebM、MOVなど）の簡易判定
- 動画URLを別タブで開く、URLをコピー
- 利用上の注意とプライバシー説明
- GitHub ActionsによるGitHub Pages自動デプロイ設定

## 重要な制限

このバージョンは、動画ページから動画ファイルを抽出したり、YouTube・SNS・配信サービスの保護を回避したりするダウンローダーではありません。直接動画ファイルのURLを開く機能を提供します。実際に保存できるかは配信元の設定、CORS、ブラウザ、端末に依存します。動画ファイルURLでも、別タブで再生されるだけの場合があります。

映画・ドラマ、YouTube Shorts、SNSなどは、サービスの公式ダウンロード機能や権利者が許可した方法を利用してください。著作権・利用規約・DRMなどの制限を守り、保存する権利のあるコンテンツだけを扱ってください。

## 無料公開の設定

1. GitHubリポジトリの **Settings → Pages** を開く。
2. **Build and deployment → Source** を **GitHub Actions** に設定する。
3. **Actions** タブで「Deploy website to GitHub Pages」の実行結果を確認する。
4. 成功後、上記の公開URLを開く。

以後、mainブランチへの変更はGitHub Actionsで自動公開されます。GitHub Pagesは静的サイト用のため、サーバー側で動画を取得・変換する処理は実行できません。

## プライバシー

入力されたURLを外部サーバーへ送信・保存する処理は実装していません。「動画URLを開く」を押した場合、そのURLの配信元へアクセスします。

# Meilisearch-Japanese-Build
[![Publish binaries to GitHub release](https://github.com/AmaseCocoa/Meilisearch-Japanese/actions/workflows/publish.yml/badge.svg)](https://github.com/AmaseCocoa/Meilisearch-Japanese/actions/workflows/publish.yml)

日本語の精度を向上させるために中国語のトークン化を無効にしたMeilisearchビルド。

MeilisearchのビルドにはオリジナルのActionsを一部改変して利用しています。
## これは何？
非Docker向けのhttps://github.com/meilisearch/meilisearch/pull/3882 の非公式ビルド。リリースを検知したら自動的にビルドされます。

これはビルド時にフラグを追加しているだけなのでローカルでビルドすることもできます。

Actionsが動いていない時はご報告下さい。

### 参考
https://github.com/meilisearch/meilisearch/issues/4561#issuecomment-2058594295
## FAQ
### ソースコードは？
オリジナルのMeiliSearchから変更されていないため公開していません。

ビルドアクションのコードは[check.yml (リリース確認、作成自動化用)](https://github.com/AmaseCocoa/Meilisearch-ForceJP/blob/main/.github/workflows/check.yml)と[publish.yml (ビルドしたものをReleasesにバイナリをアップロードする用、本家のアクションベース)](https://github.com/AmaseCocoa/Meilisearch-ForceJP/blob/main/.github/workflows/publish.yml)です。
### 何が違うの？
日本語検索の精度を向上させるために中国語のトークン化が無効になっています。

また、v1.11.0~v1.11.3のビルドでは設定のミスでmini-dashboardが無効化されています

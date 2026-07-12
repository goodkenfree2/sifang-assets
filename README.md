# sifang-assets

私房日本（[@sifang.riben](https://www.threads.com/@sifang.riben)）の Threads 投稿用・公開画像アセット。

Threads API は画像のバイナリアップロードを受け付けず、`image_url` に指定された
**公開HTTPS URL を Meta のサーバ側が取りに来る**仕様のため、投稿する画像は
公開ホストに置く必要がある。このリポジトリがその置き場。

- `cards/` — 図卡（データカード）画像。`投稿キュー/post-NNNN_*.yaml` の `images:` から参照する
- 参照URL形式: `https://raw.githubusercontent.com/goodkenfree2/sifang-assets/main/cards/<file>.png`
- 投稿前に必ず `python3 engine/threads_publisher.py checkimg <URL>` で Meta 側から取得できるか確認する

戦略ドキュメントや `.env` は非公開の `nagataken` リポジトリにある。**ここには公開してよい画像だけ**を置くこと。

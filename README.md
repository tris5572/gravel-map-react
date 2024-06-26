# グラベルマップ

グラベルマップは、自転車・グラベルロードで走れるグラベル（未舗装路）を地図にマッピングした Web アプリです。

https://tris5572.github.io/gravel-map/

## ルートについて

記載のルートは作者が走った記録を元にマッピングしており、現時点では関東平野南部のデータがほとんどです。

各ルートにはグラベルレベル（星の数）を作者の主観で付与し、道の走りにくさを色で示しています。ただし道の整備具合や季節によって大きく変動するため、参考程度です。

|星の数|色|説明|
|--|--|--|
|★|青|耐パンク性の高いタイヤを履いたロードバイクでも走行できる。締まった細かい砂 等|
|★★|緑|グラベルロードで走りやすい。浅い砂利、硬い土、草 等|
|★★★|橙|グラベルロードで走りにくい。深い砂利、浅い凹凸、緩い土 等|
|★★★★|赤|MTBの方が向いている。緩い砂利、深い凸凹、大きめの石 等|
|★★★★★|紫|自転車で走るのに向かない|


## 開発時のコマンド類

事前に `pnpm` の導入が必要です。

### ローカルプレビュー

```sh
pnpm run dev  # or `pnpm dev`
```

### テスト

今のところテストはありません……。

### デプロイ

[完成版](https://tris5572.github.io/gravel-map/)は GitHub Actions を使って GitHub Pages にデプロイしているため、このリポジトリでデプロイする際は `push` するだけで、他にやることはありません。

デプロイ関連の設定はこのあたりにあります。

- https://github.com/tris5572/gravel-map/blob/main/.github/workflows/deploy.yml
- https://github.com/tris5572/gravel-map/blob/main/vite.config.ts

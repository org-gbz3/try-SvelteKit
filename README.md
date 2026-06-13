# sv

[`sv`](https://github.com/sveltejs/cli) によって構築された、Svelte プロジェクト開発に必要な一式です。

## プロジェクトの作成

これを見ているなら、この手順はすでに完了しているはずです。おめでとうございます。

```sh
# 新しいプロジェクトを作成
npx sv create my-app
```

同じ設定でこのプロジェクトを再作成するには:

```sh
# このプロジェクトを再作成
npx sv@0.16.1 create --template demo --types ts --add prettier eslint vitest="usages:unit,component" playwright tailwindcss="plugins:typography" mcp="ide:vscode+setup:remote" --install npm .
```

## 開発

プロジェクトを作成し、`npm install`（または `pnpm install` / `yarn`）で依存関係をインストールしたら、開発サーバーを起動します:

```sh
npm run dev

# またはサーバーを起動し、新しいブラウザータブでアプリを開く
npm run dev -- --open
```

## ビルド

アプリの本番版を作成するには:

```sh
npm run build
```

`npm run preview` で本番ビルドをプレビューできます。

> アプリをデプロイするには、対象環境向けの [adapter](https://svelte.dev/docs/kit/adapters) のインストールが必要になる場合があります。

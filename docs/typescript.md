# typescript 環境について

- lerna と yarn の workspace で各 pakcage を管理します。

## 初期化

```bash

# direnvの準備
# パスとかは適宜書き換えてください
> cp .envrc.tmpl .envrc

> docker-compose build

# dotenvのコピー
> cp apps/backend/.env.tmpl apps/backend/.env

> pnpm install

> pnpm build
```

## サーバースタート

```bash

# DBの起動
> docker-compose up -d

# nestjs serverの起動
> pnpm workspace @typescript-plane-boilerplate/backend start:dev

# nextjs 管理画面起動
> pnpm workspace @typescript-plane-boilerplate/admin start:dev

# erd更新
> docker-compose up -d

# erd起動
> pnpm workspace @typescript-plane-boilerplate/erd start
```

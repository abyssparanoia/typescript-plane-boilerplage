# DB schema migration について

- typeORM の migration 機能で管理しています。

## usage

- migration file 作成

```sh
> yarn workspace @toyota-catalog/backend migration:generate -n added_displayname
```

- migration を走らせる

```sh
> yarn workspace @toyota-catalog/backend migration:run
```

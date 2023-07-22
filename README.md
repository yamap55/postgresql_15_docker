# postgresql_15_docker

本リポジトリはPostgreSQLのVersion15をDockerで使用するリポジトリです

## 特徴

- timezone: Asia/Tokyo
- language: ja_JP.UTF-8
- ログ
  - 実行されたSQLを含むすべてのログをホストで確認可能
  - 出力先: `./logs/postgresql`
  - 日毎のローテーション
  - 自動削除は行わないので定期的に手動削除することを想定

## 起動コマンド

```bash
docker compose up
```

## 接続情報
- Host: localhost
- Database: database-name
- Port: 5432
- User: root
- Password: change-me

## 初期化SQL

- 以下にサンプルが設定されているので変更か削除を行うこと
  - `database\sql\init.sql` 

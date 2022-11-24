phpを使って掲示板を作りました

Dockerを使ってMysqlをインストールしています。

# フォルダの構成
- `private/database.php`... DBの設定が入っております
- `private/exception_handler.php`... エラー画面用のファイルです
- `private/helper.php`... ヘルパー関数が定義されたファイルです
- `confirm.php`... 投稿時の確認画面です
- `confirm_delete.php`... 削除時の確認画面です
- `deleted.php`... 削除完了画面です
- `edit_complete.php`... 編集完了画面です
- `editing.php`... 編集画面です
- `index.php`... トップ画面です
- `register.php`... 登録完了画面です

# 開発環境の立ち上げ
```shell
docker-compose up -d
```
ブラウザで [http://localhost/index.php](http://localhost/index.php) にアクセスしてください



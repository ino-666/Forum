# 掲示板

## 使用技術

- PHP: 7.4.12
- データベース: MySQL 5.7
- ウェブサーバー: Apache

これらを用いる際に Docker を使用しています。

## フォルダの構成

- `private/database.php`... DB の設定が入っております
- `private/exception_handler.php`... エラー画面用のファイルです
- `private/helper.php`... ヘルパー関数が定義されたファイルです
- `confirm.php`... 投稿時の確認画面です
- `confirm_delete.php`... 削除時の確認画面です
- `deleted.php`... 削除完了画面です
- `edit_complete.php`... 編集完了画面です
- `editing.php`... 編集画面です
- `index.php`... トップ画面です
- `register.php`... 登録完了画面です

## 開発環境の立ち上げ

1. このリポジトリをクローンします。

```bash
git clone https://github.com/ino-666/Forum.git
```

2.Docker Compose を使用してアプリケーションを起動します。

```shell
docker-compose up -d
```

3.ブラウザで [http://localhost/index.php](http://localhost/index.php) にアクセスしてください

＊Docker を立ち上げてすぐだとエラーが出る場合があります。エラーが出た場合 10 秒ほど待ってサイトをリロードしてください。

## スクリーンショット

![スクリーンショット](/screenshots/screenshot1.png.png)

# 掲示板

## 使用技術
- PHP: 7.4.12
- データベース: MySQL 5.7
- ウェブサーバー: Apache

これらを用いる際にDockerを使用しています。

## フォルダの構成
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

## 開発環境の立ち上げ
1. このリポジトリをクローンします。
```bash
git clone https://github.com/Takumi-666/docker-php-keiziban.git
```
2. プロジェクトディレクトリに移動します。
```shell
cd docker-php-keiziban
```
3.Docker Composeを使用してアプリケーションを起動します。
```shell
docker-compose up -d
```
4.ブラウザで [http://localhost/index.php](http://localhost/index.php) にアクセスしてください

＊Dockerを立ち上げてすぐだとエラーが出る場合があります。エラーが出た場合10秒ほど待ってサイトをリロードしてください。

## デモ動画


https://github.com/Takumi-666/Forum/assets/108921895/2c3446fd-5bb8-4f4f-a743-130ece4f544c




[https://www.youtube.com/watch?v=U2eRuuZvf5Y](https://www.youtube.com/watch?v=U2eRuuZvf5Y)

## スクリーンショット

![スクリーンショット](/screenshots/screenshot1.png.png)


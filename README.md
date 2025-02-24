# 掲示板

## 使用技術

- PHP: 8.2
- データベース: MySQL 8.0
- ウェブサーバー: Apache

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

### 1. このリポジトリをクローンします。

```bash
git clone https://github.com/ino-666/Forum.git
```

### 2. プロジェクトディレクトリに移動します.。

```shell
cd Forum
```

### 3. .env ファイルを作成する。

プロジェクトのルートディレクトリに .env ファイルを作成し、以下の内容をコピー＆ペーストしてください。

```.env
DB_HOST=db
DB_PORT=3306
DB_NAME=bbs
DB_USER=user
DB_PASSWORD=password
```

###### ※DB_PASSWORD の項目はあくまで一例です。自分が分かりやすいものに修正して使ってください。

###### ※パスワード 12 文字以上、大文字と小文字、数字を含める、!, @, #, $, %, ^, &, \*などの特殊文字を含めるとセキュリティ的に良いです。

### 4. Docker Compose を使用してアプリケーションを起動します

・build

```shell
docker compose build --no-cache
```

・Doker の立ち上げ

```shell
docker-compose up -d
```

### 5.ブラウザで [http://localhost/index.php](http://localhost/index.php) にアクセスしてください。

## スクリーンショット

![スクリーンショット](/screenshots/screenshot1.png.png)

## デモ動画

https://github.com/user-attachments/assets/69f4fd8e-0c7d-4a21-a582-fce57692ec13

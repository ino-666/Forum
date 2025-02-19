# PHP 8.2 Apache イメージをベースにする
FROM php:8.2-apache

# 必要なPHP拡張をインストール
RUN docker-php-ext-install -j$(nproc) pdo_mysql \
    && docker-php-ext-enable opcache

# Gitのインストール
RUN apt-get update && apt-get install -y git

# 作業ディレクトリを設定
WORKDIR /var/www/html

# プロジェクトのファイルをコンテナにコピー
COPY . /var/www/html

# Composerのインストール
RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

# Composerで依存関係をインストール
RUN composer install

# 必要に応じて、権限の設定
RUN chown -R www-data:www-data /var/www/html

# ポート80を公開
EXPOSE 80

# アプリケーションの起動 (Apache)
CMD ["apache2-foreground"]
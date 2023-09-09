# 使用イメージの指定
FROM php:7.4-fpm

# composer イメージ内から特定のファイルをコピー
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# コマンドの実行
# apt-getコマンドのアップデートと必要なライブラリやドライバのインストール
#RUN apt-get update && apt-get install -y \git \&& zip unzip \
#&& docker-php-ext-install pdo_mysql

RUN apt-get update && apt-get install -y git zip unzip \
&& docker-php-ext-install pdo_mysql

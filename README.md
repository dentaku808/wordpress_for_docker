# wordpress for docker

## 概要

* WordPressのDocker環境
* メール送信はMailCatcherで確認できる

## 前提条件
* Dockerがインストール済であること  

## コンテナ

* db: MySQL latest
* wordpress: WordPress latest
* phpmyadmin
* mailcatcher

## ビルド

* 起動  
`$ cd (インストールディレクトリ)`  
`$ docker-compose up -d`  
* 停止  
`$ docker-compose down`  

## 使い方

### Web
* http://localhost/

### WordPress
* http://localhost/wp-login.php
  * WordPress本体は/var/www/html以下に設置すること

### phpMyAdmin
* http://localhost:8888/  
  * DB NAME: wordpress_db
  * USER: wordpress_user
  * PASS: wordpress_password
  * HOST: db

### MailCatcher (メール送信確認)
* http://localhost:1080/  
  * メーラー: その他のSMTP
  * SMTPホスト: mailcatcher
  * 暗号化: なし
  * SMTPポート: 1025
  * 認証: Disable
  * WordPressにWP Mail SMTPプラグインを追加
  * WordPressから送信したメールはMailCatcherの管理画面に溜まる  

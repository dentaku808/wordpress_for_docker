# wordpress for docker

## Overview

* WordPressのDocker環境  
* Docker Desktop使用  

## Container

* db: MySQL latest  
* wordpress: WordPress latest  
* phpmyadmin  

## Build

* 起動  
`$ cd (インストールディレクトリ)`  
`$ docker-compose up -d`  
* 停止  
`$ docker-compose down`  

## Usage

### Web
* http://localhost/

### WordPress
* http://localhost/wp-login.php  

### phpMyAdmin
* http://localhost:8888/  
DB NAME: wordpress_db  
USER: wordpress_user  
PASS: wordpress_password

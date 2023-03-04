# docker-laravel-auth
Laravelの認証サーバー。
## 環境構築
1.コンテナのビルド
```
docker compose up -d --build
```
2.コンテナに入る
```
docker container exec -it docker-laravel-auth-php-1 bash
```
3.ライブライをインストール(2回目以降は不要)
```
composer install
```
4.マイグレーションを実行
```
php artisan migrate
```

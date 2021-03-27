# Docker PHP Laravel

## App Detail

```bash
├── code
├── docker-compose.yml
├── nginx
│   └── conf.d
│       └── app.conf
├── php
│   └── local.ini
└── README.md
```

### Docker Images

- Nginx Alpine
- MySQL 8
- PHP 7.4 FPM Alpine With Composer

## Code

All coding files must be saved in the `code` folder

## Nginx

Because here we use laravel, the directory bidding is in `code/public`.

## Folder Permission (Development Only)

If there is an error in the storage folder, just give permission like this:

```bash
sudo chmod 777 -R storage/
sudo chmod 777 -R bootstrap/cache/
```

## Laravel Setup

```
docker exec -i php_laravel sh -c "exec php artisan:generate"
```

### Database & Redis ENV

```
DB_CONNECTION=mysql
DB_HOST=db_laravel
DB_PORT=3306
DB_DATABASE=laravel_dock
DB_USERNAME=laravel
DB_PASSWORD=laravel

REDIS_HOST=redis_laravel
REDIS_PASSWORD=null
REDIS_PORT=6379
```

# Docker PHP Laravel

## App Detail

### Folder Tree

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
- PHP 7.4 FPM Alpine
- Composer

## Code

Semua file coding harus di simpan di folder `code`

## Nginx

Karena disini pakai laravel, maka bidding directorynya di `code/public`.

## Folder Permission (Development Only)

Kalau ada error di folder storage, kasi aja permission seperti ini :

```bash
sudo chmod 777 -R storage/
sudo chmod 777 -R bootstrap/cache/
```

## Reference

- [http://geekyplatypus.com/dockerise-your-php-application-with-nginx-and-php7-fpm/](https://web.archive.org/web/20200924175739/http://geekyplatypus.com/dockerise-your-php-application-with-nginx-and-php7-fpm/)
- [http://geekyplatypus.com/making-your-dockerised-php-application-even-better/](https://web.archive.org/web/20200310195111/http://geekyplatypus.com/making-your-dockerised-php-application-even-better/)
- https://medium.com/@sreejithezhakkad/how-i-set-up-laravel-in-docker-container-f80987559bc6

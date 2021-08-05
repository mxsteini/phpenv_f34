# phpenv_f34
PHP 7.2.34 / 7.4.20
on my Fedory 34 laptop I install some packages to get php 7.4 compiled:

```bash
 sudo dnf install \
 libxml2-devel \
 sqlite-devel \
 bzip2-devel \
 libcurl-devel \
 libpng-devel \
 libjpeg-devel \
 libicu-devel \
 oniguruma-devel \
 readline-devel \
 libtidy-devel \
 libxslt-devel \
 libzip-devel \
 php-devel \
 php-pear \
 libdb-devel \
 libcurl4-openssl-devel \
 libXpm-devel \
 libmysqlclient-devel \
 libpq-devel \
 freetype-devel \
 libdb-devel

 sudo pecl install xdebug
 
```
# install redis for phpenv
```bash
export version=7.4.20
pecl install -R ~/.phpenv/versions/${version}/lib/php/extensions -o -f redis
echo "extension=redis" > ~/.phpenv/versions/${version}/etc/conf.d/redis.ini
```

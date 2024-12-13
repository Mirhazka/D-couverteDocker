# Découverte de Docker

## 1. Généralités
Après la découverte du logiciel **Docker**, voici un petit challenge :
  * Exécute l'image docker *php* puis lance là dans un conteneur **interactif**
  * Dans l'interpréteur php alors disponible, exécute la fonction : `php > phpinfo(INFO_GENERAL);`

## 2. Résultat du challenge
```bash
root@sybill-x555ub:/home/sybill# docker run -i php
Interactive shell

php > phpinfo(INFO_GENERAL);
phpinfo(INFO_GENERAL);
phpinfo()
PHP Version => 8.4.1

System => Linux b7593f20cb88 6.8.0-49-generic #49-Ubuntu SMP PREEMPT_DYNAMIC Mon Nov  4 02:06:24 UTC 2024 x86_64
Build Date => Nov 21 2024 17:57:18
Build System => Linux - Docker
Build Provider => https://github.com/docker-library/php
Configure Command =>  './configure'  '--build=x86_64-linux-gnu' '--with-config-file-path=/usr/local/etc/php' '--with-config-file-scan-dir=/usr/local/etc/php/conf.d' '--enable-option-checking=fatal' '--with-mhash' '--with-pic' '--enable-mbstring' '--enable-mysqlnd' '--with-password-argon2' '--with-sodium=shared' '--with-pdo-sqlite=/usr' '--with-sqlite3=/usr' '--with-curl' '--with-iconv' '--with-openssl' '--with-readline' '--with-zlib' '--enable-phpdbg' '--enable-phpdbg-readline' '--with-pear' '--with-libdir=lib/x86_64-linux-gnu' '--enable-embed' 'build_alias=x86_64-linux-gnu' 'PHP_UNAME=Linux - Docker' 'PHP_BUILD_PROVIDER=https://github.com/docker-library/php'
Server API => Command Line Interface
Virtual Directory Support => disabled
Configuration File (php.ini) Path => /usr/local/etc/php
Loaded Configuration File => (none)
Scan this dir for additional .ini files => /usr/local/etc/php/conf.d
Additional .ini files parsed => /usr/local/etc/php/conf.d/docker-php-ext-sodium.ini

PHP API => 20240924
PHP Extension => 20240924
Zend Extension => 420240924
Zend Extension Build => API420240924,NTS
PHP Extension Build => API20240924,NTS
PHP Integer Size => 64 bits
Debug Build => no
Thread Safety => disabled
Zend Signal Handling => enabled
Zend Memory Manager => enabled
Zend Multibyte Support => provided by mbstring
Zend Max Execution Timers => disabled
IPv6 Support => enabled
DTrace Support => disabled

Registered PHP Streams => https, ftps, compress.zlib, php, file, glob, data, http, ftp, phar
Registered Stream Socket Transports => tcp, udp, unix, udg, ssl, tls, tlsv1.0, tlsv1.1, tlsv1.2, tlsv1.3
Registered Stream Filters => zlib.*, convert.iconv.*, string.rot13, string.toupper, string.tolower, convert.*, consumed, dechunk

This program makes use of the Zend Scripting Language Engine:
Zend Engine v4.4.1, Copyright (c) Zend Technologies
php > 
```

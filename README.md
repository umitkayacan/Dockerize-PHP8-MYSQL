
# Dockerize PHP8 - MYSQL - GIT - COMPOSER 

PHP'yi ve Mysql Docker üzerinden kullanmak için kullanılır. 

# Kurulum
Repository'i bir dizine clonlayın ve docker-compose.yml dosyasının olduğu dizine cd komutu ile geçip
```bash
  docker-compose up -d 
```
komutu ile php8, mysql 5.7 kurulumu tamamlanır ve containerlar ayağı kalkar
[http://127.0.0.1:8080](http://127.0.0.1:8080/) veya 
[http://localhost:8080](http://localhost:8080/) veya adresi ile erişim sağlayabilirsiniz.



# Docker üzerinde çalışan containerları listeleme

```bash
  docker ps
```
komutu ile aşağıda gördüğümüz gibi containerlar listelenecektir. 

Şimdi de PHP container'ının içine girip Word kütüphanesini yükleyelim. 

![Uygulama Ekran Görüntüsü](https://img.onl/kbNxXZ)

```bash
  docker exec -it da4a05820326 bash
```
komutu ile container içine girdik. Burada `composer require phpoffice/phpword` komutu ile phpWord kütüphanesini indirebiliriz.

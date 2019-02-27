# docker-php7.2-nginx-mysql-phpmyadmin


localhost:8080/hogehoge.php = docker-php7.2-nginx-mysql-phpmyadmin/www/html/hogehoge.php



## Installation
```
# After git clone 
$ cd docker-php7.2-nginx-mysql-phpmyadmin && docker-compose up -d
```


## nginx server
```
open http://localhost:8080
```

## phpmyadmin
```
open http://localhost:8888
```


## Connect mysql container
```
$ docker exec -it docker-php72-nginx-mysql-phpmyadmin_db_1 /bin/bash

# password = secret
$ mysql -u root -p
```

## Connect mysql contaner by external tool
![](https://drive.google.com/uc?export=view&id=1bctVVekgWRDOKNgBwti-tEBllUKzjnEo)


## Connect PHP7.2 container
```
$ docker exec -it ocker-php72-nginx-mysql-phpmyadmin_php_1 /bin/bash
```



## Usage
| Command | Result |
| docker-compose up -d | Create containers on detach mode |
| docker-compose start | Containers run |
| docker-compose stop  | Containers stop | 
| docker-compose down  | Stop container and remove container |

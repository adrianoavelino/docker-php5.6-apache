# Container Docker com Apache e PHP 5.6
> Neste repositório está incluso o PHP 5.6, Apache 2.4.10 e o Mysql 5.7

Dependências:
- Composer
- Docker
- docker-compose

Instalação:
```sh
$ git clone https://github.com/adrianoavelino/docker-php5.6-apache.git # clona o projeto
$ cd docker-php5.6-apache # entra no diretório clonado
$ composer install # instala as depedências PHP
$ docker-compose build # cria as imagens docker necessárias
$ docker-compose up -d # inicia servidor
```
Outros comando uteis:
```bash
$ docker logs dockerphp56apache_php_1 # verifica os logs do servidor PHP
$ docker logs dockerphp56apache_db_1 # verifica os logs do servidor Mysql
$ docker exec -it dockerphp56apache_php_1 hostname -i # verifica o ip do container PHP
docker exec -it dockerphp56apache_php_1 bash # acessa o terminal via linha de comando
```



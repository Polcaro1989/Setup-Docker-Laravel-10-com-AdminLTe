# Projeto Laravel 10 com AdminLTe:
<div style="display: flex; align-items: center;">
<img src="https://github.com/abraao69/abraao69/blob/main/Navy%20Blue%20Geometric%20Technology%20LinkedIn%20Banner%20(2).png" alt="Logo">
  <br><br>
</div>

### Passo a passo
Clone Repositório
```sh
https://github.com/abraao69/Setup-Docker-Laravel-10-com-AdminLTe.git
```
```sh
cd app-laravel
```


Crie o Arquivo .env
```sh
cp .env.example .env
```


Atualize as variáveis de ambiente do arquivo .env
```dosini
APP_NAME=EspecializaTi
APP_URL=http://localhost:8989

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=nome_usuario
DB_PASSWORD=senha_aqui

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acesse o container app
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```


Gere a key do projeto Laravel
```sh
php artisan key:generate
```


Acesse o projeto
[http://localhost:8989](http://localhost:8989)

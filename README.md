
# Setup Docker Laravel 11 com PHP 8.3

### Passo a passo
Clone Repositório
```sh
git clone https://github.com/falaprodavi/laravel-11.git
```
```sh
cd setup-docker-laravel-11
```
Suba os containers do projeto
```sh
docker-compose up -d
```
Crie o Arquivo .env
```sh
cp .env.example .env
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

Rodar as migrations
```sh
php artisan migrate
```

Acesse o projeto
[http://localhost:8000](http://localhost:8000)


Instalar Beezer
```sh
composer require laravel/breeze --dev
```
```sh
php artisan breeze:install 
```
```sh
blade alpine
```
```sh
yes
```
```sh
pest
```
Intalar dependências Node
```sh
npm install
```
rodar run dev
```sh
npm run dev
```
Build arquivos estáticos e manifest
```sh
npm run build
```

Migrations
```sh
php artisan make:model Organization -m
php artisan make:model OrganizationUser -m -p
php artisan make:model Media -m   
php artisan make:model MediaOrganization -m -p
php artisan make:model Content -m
```



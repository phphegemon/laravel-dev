
## Kontener bazowy ngnix,mysql,php8,composer,laravel

Projekt kontenera bazowego do rozwoju oprogramowania: Laravel

### Instalacja

Skopiować plik docker-compose i ustawić porty i hasło do mysql 

> cp docker-compose-default.yml docker-compose.yml

Zbudowanie i start kontenerów

*problem z uprawnieniami do folderu mysql*

> sudo chown -R tomasz:docker mysql/
> docker-compose up --build

composer update

> docker-compose run --rm composer update

npm instalacja npm

> docker-compose run --rm npm install

artisan migracja poczatkowa

> docker-compose run --rm artisan migrate:fresh

### TO_DO

*Dodać po kolei kroki do uruchomienia kontenera*

*Dodać kroki jak uzywac*

### Jak używać

#### composer

> docker-compose run --rm composer update
> docker-compose run --rm composer require doctrine/dbal

#### npm

> docker-compose run --rm npm run dev
> docker-compose run --rm npm run prod

#### artisan

> docker-compose run --rm artisan migrate


 





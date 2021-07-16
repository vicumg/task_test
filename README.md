## Command flow

curl -s "https://laravel.build/test_task?with=mysql,mailhog" | bash

alias sail='bash vendor/bin/sail'

cd test_task

sail up -d

sail artisan migrate

sail npm install

sail composer require laravel/breeze --dev

sail artisan breeze:install

sail npm install

sail npm run dev

git commit -m "add auth by laravel/breeze"

add the interface MustVerifyEmail to User model

add a middleware to routes where need auth

edit .env add MAIL_FROM_ADDRESS value

php artisan make:observer UserObserver --model=User

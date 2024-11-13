Comando creazione progetto da git bash:
laravel new project_name

composer install

*Se il progetto è importato*
1) cp .env.example .env
2) php artisan key:generate



npm i bootstrap (installa componenti bootstrap)

Cartella components nella view 
Layout con {{$slot}} al centro di layout
componenti navbar e footer da inserire in layout

Importare bootstrap, fine della head in layout:
@vite(['resources/css/app.css', 'resources/js/app.js'])
aggiustare i file rimuovendo le dipendenze di tailwind, aggiungere @import 'bootstrap' in app.css e import 'bootstrap' in app.js


importare con x-layout nella welcome

inserire password in .env per il database
*Se inlcude dei seeders*
php artisan db:seed

php artisan migrate
(avviare creazione del database, fare yes per creare) 


npm run dev (avviare npm)
php artisan serve (avviare selfhost:

configurare rotte parametriche

php artisan storage:link per linkare le immagini del database

Installare [[Fortify]]
Comando creazione progetto da git bash:
laravel new project_name

npm i bootstrap (installa componenti bootstrap)

Cartella components nella view 
Layout con {{$slot}} al centro di layout
componenti navbar e footer da inserire in layout

Importare bootstrap, fine della head in layout:
@vite(['resources/css/app.css', 'resources/js/app.js'])

importare con x-layout nella welcome

inserire password in .env per il database
php artisan migrate
(avviare creazione del database, fare yes per creare) 

aggiustare i file rimuovendo le dipendenze di tailwind, aggiungere @import 'bootstrap' in app.css e import 'bootstrap' in app.js

npm run dev (avviare npm)
php artisan serve (avviare selfhost:

configurare rotte parametriche
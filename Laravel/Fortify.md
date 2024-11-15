Fortify è il sistema di autenticazione di Laravel.

Installazione:
composer require laravel/fortify

php artisan fortify:install

php artisan migrate

Configurazioni:
E' consigliabile modificare nella config fortify.php mettendo come link della home '/' 

la rotta di Login è preimpostata dai valori, possiamo usare 
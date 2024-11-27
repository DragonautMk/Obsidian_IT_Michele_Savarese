Creare Controller:
php artisan make:controller PublicController

Linkare immagini nella public:
php artisan storage:link

Creare componenti per crud
php artisan make:model nome -mc   (m=model, c=controller)
Convenzioni: nome del modello, iniziale maiuscola, singolare, evitare camelcase, underscore etc per evitare problemi

abilitare revisore:
php artisan app:make-user-revisor <emailUtente>
php artisan app:make-user-revisor prova@gmail.com
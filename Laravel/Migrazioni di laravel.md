La migrazione permette di gestire il database.
La funzione up saranno le modifiche che effettueremo, 
la funzione down invece servirà per il rollback del database.

Comandi:
php artisan migrate (effettua una migrazione)
php artisan migrate:rollback (ritorna indietro di una migrazione)

schema:
title è il nome della colonna che creeremo, unique è un attributo che impedirà agli utenti di caricare un'entità con un nome già presente.
            $table->string(column: 'title')->unique();
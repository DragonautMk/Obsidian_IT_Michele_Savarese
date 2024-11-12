1: Create
-- 
Creare Route::get in web php
(ES: Route::get('/create',[PostController::class, 'create'])->name('post.create');)
Creare cartella nella view relativa alla post per fare il crud
creare nella relativa cartella: create.blade.php
inserire nel controlla la view della create, es:

public function create(){

    return view("post.create");

}

Nei form di submit la direttiva livewire che si usa è: wire:submit="nomedellafunzione"

Nella funzione store se vogliamo avere un messaggio di conferma di avvenuto inserimento dobbiamo inserire: 
        session()->flash('success','Inserito correttamente nel database');




Puoi controllare campi in real time evitando di inserire input con il metodo .live e inserendo #[Validate] nel modello del form relativo per ciascun attributo del form. in alternativa a .live è possibile usare .blur. Il vantaggio di questo metodo è che esegue il controllo solo dopo che l'utente è uscito dalla casella di inserimento, riducendo il numero di richiesta al server e quindi alleggerendo il programma.

2: Reed
--
3: Update
--
4: Delete
--
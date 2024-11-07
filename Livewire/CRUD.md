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
2: Reed
--
3: Update
--
4: Delete
--
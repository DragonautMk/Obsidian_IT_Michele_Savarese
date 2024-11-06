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


2: Reed
--
3: Update
--
4: Delete
--
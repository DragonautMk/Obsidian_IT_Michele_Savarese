Welcome:
function () {

    return view('welcome');

}
spostare da web.php a PublicController.php, aggiungere ->name(' ') come etichetta della rotta. Aggiungere [nomedelcontroller::class, 'nomefunzione]
Es di correzzione:
Route::get('/',[PublicController::class, 'homepage'])->name('homepage');

aggiungendo public e il nome, esempio:
public function homepage() {

    return view('welcome');

}

A questo punto l'indirizzo della pagina diventerà: {{route('homepage')}}
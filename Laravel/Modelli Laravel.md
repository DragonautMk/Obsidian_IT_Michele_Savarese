esempio:
class Post extends Model

{
    //
}

Aggiungo nelle graffe: 
Title e content sono i nomi delle colonne che andremo ad usare per salvare i dati.
In seguito dovremo inserire questi valori nella tabella delle migrazioni che avremo creato.
protected $fillable = [
'title', 'content'
];
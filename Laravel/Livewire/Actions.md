Le azioni sono le funzioni utilizzate in limewire, è possibile visualizzarle nella classe nel relativo file php.
Queste possono essere attivate dal click di un bottone o da un submit di un form.
wire:click="nomedellafunzione" (direttiva click di un bottone, all'interno degli attributi di un bottone)
Generalmente le funzioni di Livewire hanno già delle variabili di appoggio, questo processo è detto data binding.
Tuttavia se vogliamo dare all'utente la possibilità di inserire dei valori custom dobbiamo inserire un altro databinding tramite un input

Per fare data binding  di un valore custom bisogna usare un attributo html chiamato:
wire:model="" all'interno di un tag input
wire:model.live permette alle variabili di aggiornarsi in tempo reale, ad esempio se un bottone cambia dinamicamente il testo in baso a cosa inseriamo in un input
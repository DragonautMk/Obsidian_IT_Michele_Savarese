Livewire è un framwork di php di [[Laravel]] che ti permette di utilizzare il php nel lato frontend, quindi non è necessario integrare il javascript al suo posto. Livewire permette di realizzare un FullStack php creando one page application e permettendo il controllo degli elementi senza inviare dati.
Può controllare campi in real time. Vedi [[Laravel/Livewire/CRUD|CRUD]]

## Prerequisites

Before we start, make sure you have the following installed:

- Laravel version 10 or later
- PHP version 8.1 or later

composer require livewire/livewire 
(otterremo 2 file, 1 nella view nella cartella livewire, l'altro in app/livewire)
(Make sure AlpineJS isn't already installed)

Richiamare componente livewire
<livewire:nomecomponente /> o 
@livewire('nomecomponente')


lnseriamo il codice del componente preso dalla documentazione app/livewire, nel relativo file. Per convenzione la funzione render resta per ultima. Le variabili (meglio dette [[Properties]]) sono automaticamente disponibili, quindi è possibile richiamarle con {{$nome}}. 
Queste vengono utilizzate nelle funzioni (dette [[Actions]]).

E' possibile realizzare un [[Laravel/Livewire/CRUD|CRUD]] usando limewire per risparmiare tempo rispetto ai form.
Il mio primo linguaggio di programmazione, orientato al lato Front End. Permette di eseguire operazioni lato client.
Per utilizzare Javascript rispettando i principi della SEO creiamo in file .js, ad esempio main.js altrimenti possiamo scrivere codice in linea sempre nella sezione script a fine pagina.

Javascript non ha bisogno di terminare le esecuzioni con ; tuttavia è utile farlo perché permette di leggere più facilmente il codice e ci tiene allenati per gli altri linguaggi di programmazione.

Per essere sicuri che il nostro codice venga eseguito dobbiamo richiamare il file js alla fine del body, quindi come ultima linea del body metteremo:
    <script src="./main.js"></script>

Funzioni built in:
alert(' Messaggio a schermo ');

prompt(); - Permette all'utente di inserire un contenuto testuale in una finestra di dialogo.

let nomevariabile = prompt();  Utilizzando let possiamo salvare un valore inserito in un cassetto, in questo caso salveremo il contenuto testuale inserito dall'utente in prompt

usando:
alert(nomevariabile);  (quindi senza apici, richiameremo il valore della variabile)

Possiamo inserire delle variabili nelle stringe, es:
let name = promp(); ES: Mark
let saluto = 'Piacere di conoscerti ' + name; 
Otterremo come risultato: Piacere di conoscerti Mark

Per visualizzare quello che succede utilizzeremo la console log del browser:

Possiamo sovrascrivere una variabile richiamandola con 
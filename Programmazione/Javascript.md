Il mio primo linguaggio di programmazione, orientato agli eventi, lato Front End. Permette di eseguire operazioni lato client.
Per utilizzare Javascript rispettando i principi della SEO creiamo in file .js, ad esempio main.js altrimenti possiamo scrivere codice in linea sempre nella sezione script a fine pagina.

Javascript non ha bisogno di terminare le esecuzioni con ; tuttavia è utile farlo perché permette di leggere più facilmente il codice e ci tiene allenati per gli altri linguaggi di programmazione.

Per essere sicuri che il nostro codice venga eseguito dobbiamo richiamare il file js alla fine del body, quindi come ultima linea del body metteremo:
    <script src="./main.js"></script>

[[Variabili e tipi di dato]]

Funzioni built in:
console.log(variabile); 
==Visualizza nella console il valore di una variabile.==
alert(' Messaggio a schermo ');
\n ==(Manda a capo nell'alert)==

prompt(); - Permette all'utente di inserire un contenuto testuale in una finestra di dialogo.

let nomevariabile = prompt();  Utilizzando let possiamo salvare un valore inserito in un cassetto, in questo caso salveremo il contenuto testuale inserito dall'utente in prompt

usando:
alert(nomevariabile);  (quindi senza apici, richiameremo il valore della variabile)

Possiamo inserire delle variabili nelle stringe, es:
let name = promp(); ES: Mark
let saluto = 'Piacere di conoscerti ' + name; 
Otterremo come risultato: Piacere di conoscerti Mark

Per visualizzare quello che succede utilizzeremo la console log del browser:

Possiamo sovrascrivere una variabile richiamandola.

Utilizzando una condizione è possibile creare un codice che reagisce a seconda di una situazione, es:
let age = prompt('Quanti anni hai?');
if (age >= 18)
==Utilizzando la condizione iniziale definiamo il parametro della comparazione==
{  
alert('puoi bere');}   
else if ( age <18)
==Utilizzando else if diamo una condizione specifica in cui succedono cose diverse dalla prima.==
{ 

alert('sei troppo giovane');
}
else
==Utilizzando else diamo come condizione una situazione in cui le condizioni precedenti non sono verificate==
{ 
alert('Risposta errata)
}

==In un else if la condizione verificata, se ci sono dichiarazioni che possono entrare in più condizioni la condizione verrà verificata sempre nel caso più in alto verificato.==

Possiamo annidare un if dentro un if per verifiche più specifiche

do/while -  il ciclo do while non fa andare avanti finché una condizione non è verificata.
è possibile inserire un ciclo if nel do while.
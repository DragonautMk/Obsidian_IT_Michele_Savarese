let firstName = 'Marco';
Abbiamo inizializzato una variabile e le abbiamo dato un valore 
**Inizializzare la variabili**
Usando let ==la variabile non è sovrascrivibile==
Usando var ==è sovrascrivibile==

**Inizializzare le costanti**
const PIGRECO = 3.13;

Le costanti non possono cambiare valore e devono essere inizializzate, quindi va assegnato un valore di default.

**Tipi di dato**
In javascript possiamo usare questo codice per  riconoscere un tipo di dato che stiamo analizzando.
console.log(typeof nomeVariabile);

- **Non primitivi o strutturali**  (Gli oggetti)
- **Primitivi (dati semplici)** (Number, string, boolean, null, undefined, symbol)


**Primitivi**
- **String:** Valori alfanumerici, ossia lettere o numeri inseriti all'interno di ' ', " " o    \` \` (alt+96 per le backtick).
let stinga = 'ciao';
let stinga2 = "ciao";
let stinga3 = \`ciao\`;

Le backtick si usano per la **string interpolation**, ovvero un processo in cui js all'interno di una stringa riconosce delle variabili e le riempie con il suo valore. 
Utilizzando + posso concatenare le stringhe.

utilizzando $(nome variabile) posso rendere funzionante una variabile in una stringa. 
es:
let age 17
let compleanno = \` ciao a tutti ho $(age) anni. \`

**Type cohertion**:  concatena e rende sottoforma di stringa un valore non string. Implicita quando JS la converte in autonomia, esplicita quando lo facciamo noi con i metodi come toString.
es:
let a =4; (è un numero)
let b = '5'; (è una stringa)
let d= '6ciao'
console.log(typeof (a + b));
Otterremo 45, javascript ha inserito entrambi i valori in una stringa. Dal typeof otterremo che il valore è una stringa.

console.log (a + number(b)); In questo caso stiamo dicendo a js di considerare b un numero, quindi come risultato otterremo la somma, non la concatenazione.
console.log(a + d); = 46ciao
console.log(a \* d); = Nan 
**NaN = Not a Number**
console.log(typeof(a \* d)); = Number. Not a number è un dato di tipo number. 
Bootstrap è un framework css che permette un buon livello di personalizzazione usando le sue [[Classi di bootstrap]] integrate, permette una facile gestione dello spazio grazia al suo [[Grid system]] e permette di importare parti di sito già fatte con i suoi [[Componenti]].

Installare bootstrap su node:
npm i bootstrap@5.3.3

icone di bootstrap:
npm i bootstrap-icons

composer:
composer require twbs/bootstrap-icons

Sass:
Sass è un sistema di personalizzazione del css.
npm install bootstrap
npm install -g sass

installare sass:
### **1. Configurazione predefinita di Laravel**

Quando crei un nuovo progetto Laravel, troverai già una configurazione di base per SASS:

- La directory `resources/sass` contiene un file chiamato `app.scss`.
- Questo file è il punto di partenza per il tuo SASS.

Percorso:

plaintext

Copia codice

`resources/sass/app.scss`

---

### **2. Creare un file SASS personalizzato**

Se vuoi aggiungere un nuovo file SASS, puoi crearlo direttamente nella directory `resources/sass`.

#### Passaggi:

1. Vai alla directory `resources/sass`.
2. Crea un nuovo file `.scss`:
    
    bash
    
    Copia codice
    
    `touch resources/sass/custom.scss`
    

---

### **3. Modificare il file `webpack.mix.js`**

Laravel Mix è configurato per compilare il file `resources/sass/app.scss` per impostazione predefinita. Se aggiungi un nuovo file, puoi aggiornare il file `webpack.mix.js` per includerlo.

#### Esempio `webpack.mix.js`:

javascript

Copia codice

`const mix = require('laravel-mix');  // Compilazione del file predefinito mix.sass('resources/sass/app.scss', 'public/css');  // Aggiungi il file personalizzato mix.sass('resources/sass/custom.scss', 'public/css');`

Dopo aver aggiornato `webpack.mix.js`, ricorda di eseguire la compilazione.

---

### **4. Compilazione del file SASS**

Per compilare i file SASS, usa uno dei seguenti comandi nel terminale:

- **Per compilare in modalità di sviluppo (più veloce):**
    
    bash
    
    Copia codice
    
    `npm run dev`
    
- **Per compilare in modalità di produzione (ottimizzata):**
    
    bash
    
    Copia codice
    
    `npm run prod`
    

Il file CSS risultante verrà generato nella directory `public/css`.

---

### **5. Importare Bootstrap o altri stili nel tuo SASS**

Se stai usando Bootstrap o altri framework, puoi importarli direttamente nel tuo file SASS.

#### Esempio per importare Bootstrap in `app.scss` o `custom.scss`:

scss

Copia codice

`// Importa Bootstrap SASS @import '~bootstrap/scss/bootstrap';  // Aggiungi i tuoi stili personalizzati body {   background-color: #f8f9fa; }  .navbar {   background-color: #343a40; }`

Il simbolo `~` indica a Laravel Mix di cercare il pacchetto nel percorso `node_modules`.

---

### **6. Includere il file CSS compilato nel layout Blade**

Una volta compilato il file SASS in CSS, includilo nel layout Blade del tuo progetto.

#### Esempio in `resources/views/layouts/app.blade.php`:

html

Copia codice

`<link href="{{ asset('css/custom.css') }}" rel="stylesheet">`

Se stai usando il file predefinito `app.scss`, includilo come segue:

html

Copia codice

`<link href="{{ asset('css/app.css') }}" rel="stylesheet">`

---

### **7. Struttura consigliata per i file SASS**

Puoi organizzare i tuoi file SASS per una migliore gestione, utilizzando importazioni e moduli:

#### Esempio struttura:

plaintext

Copia codice

`resources/sass/ ├── app.scss        // File principale che importa tutti gli altri ├── _variables.scss // Variabili personalizzate ├── _mixins.scss    // Mixin riutilizzabili ├── _navbar.scss    // Stili specifici per la navbar ├── _footer.scss    // Stili specifici per il footer`

#### Esempio `app.scss`:

scss

Copia codice

`@import 'variables'; @import 'mixins'; @import 'navbar'; @import 'footer';`

Laravel Mix compilerà tutti i file importati in un unico file CSS.

---

### **8. Installare Bootstrap con Laravel Mix (facoltativo)**

Se stai utilizzando Bootstrap con SASS, assicurati che il pacchetto sia installato nel progetto:

bash

Copia codice

`npm install bootstrap`

Poi importalo nel file `app.scss` o in un file SASS personalizzato come descritto sopra.

---

### **Conclusione**

- Crea i tuoi file SASS in `resources/sass`.
- Configura il file `webpack.mix.js` per includere i file personalizzati.
- Compila i file con `npm run dev` o `npm run prod`.
- Collega i file CSS compilati nel tuo layout Blade.

Questa configurazione ti permette di utilizzare SASS in Laravel in modo efficiente, sfruttando la potenza di Laravel Mix per personalizzare il tuo progetto.
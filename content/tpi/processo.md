[[index]]
[[TPI]]

Un processo è un'istanza in esecuzione di un programma, comprendente sia il codice che i dati necessari per la sua esecuzione. Ogni processo è composto da:

- **Codice**: le istruzioni del programma.
- **Dati**: suddivisi in variabili globali, locali, temporanee e allocate dinamicamente.

I processi possono essere classificati in:

- **Indipendenti**: operano autonomamente senza scambi di dati con altri processi.
- **Cooperanti**: necessitano di scambi di informazioni per funzionare.
- **Competitori**: competono per le stesse risorse, rischiando conflitti.

Ogni programma può generare più processi, ma ogni processo è associato a un solo programma. Esistono due tipi di processi:

- **Processo utente**: generato da un programma scritto dall'utente.
- **Processo supervisore**: generato da un programma del sistema operativo, come il gestore delle attività.

Quando un programma viene eseguito, il [[sistema_operativo]] crea un processo memorizzato in memoria centrale. Ogni processo è rappresentato da una struttura chiamata PCB (Process Control Block), che contiene informazioni cruciali per l'esecuzione di esso.
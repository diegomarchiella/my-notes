[[index]]
## Rilocazione della Memoria

La **rilocazione della memoria** è un processo fondamentale nella gestione della memoria dei sistemi operativi, che consente di tradurre indirizzi virtuali in indirizzi fisici. Esistono due principali modalità di rilocazione: **statica** e **dinamica**.

### Rilocazione Statica

- **Definizione**: La rilocazione statica avviene durante il caricamento del programma. Gli indirizzi virtuali vengono convertiti in indirizzi fisici dal loader, che somma un valore fisso (indirizzo di base) a ciascun indirizzo logico.
- **Vantaggi**:
  - Semplicità nell'implementazione.
  - Non richiede hardware complesso per la traduzione degli indirizzi.
- **Svantaggi**:
  - Limitata flessibilità: una volta caricato, un programma non può essere spostato in un'altra area di memoria.
  - Inefficienza in caso di swapping, poiché richiede una nuova rilocazione se il programma deve essere ricaricato[1][2].

### Rilocazione Dinamica

- **Definizione**: Nella rilocazione dinamica, gli indirizzi virtuali vengono tradotti in indirizzi fisici durante l'esecuzione del programma. Questo avviene attraverso l'uso di una Memory Management Unit (MMU), che gestisce la traduzione in tempo reale.
- **Vantaggi**:
  - Maggiore flessibilità: i programmi possono essere spostati liberamente in memoria, facilitando operazioni di swapping e compattamento della memoria.
  - Riduzione della frammentazione esterna grazie alla possibilità di compattare aree di memoria libere[2][3].
- **Svantaggi**:
  - Maggiore complessità e overhead dovuti alla necessità di hardware per la gestione degli indirizzi[4].

### Tecniche di Allocazione della Memoria

Nella gestione della memoria, le tecniche di allocazione possono essere classificate come segue:

1. **Partizioni Fisse**: La memoria è suddivisa in partizioni di dimensioni fisse. Questo metodo può portare a frammentazione interna.
2. **Partizioni Variabili**: Le partizioni sono allocate in base alle esigenze dei processi, riducendo la frammentazione interna ma aumentando il rischio di frammentazione esterna.
3. **Paginazione**: La memoria è suddivisa in pagine di dimensioni fisse, permettendo una gestione più efficiente e flessibile della memoria virtuale. Le pagine possono essere allocate in qualsiasi area libera della memoria fisica, migliorando l'utilizzo complessivo[3][4].
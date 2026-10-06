# Definizioni
**Corrente elettrica**: grandezza fisica che indica la quantità di carica elettrica che attraversa una determinata superficie nell'unità di tempo.

**Tensione elettrica**: grandezza fisica proporzionale alla quantità di energia richiesta per muovere una carica elettrica tra due punti nello spazio

**Resistenza elettrica**: grandezza fisica che misura la tendenza di un corpo ad opporsi al passaggio di una corrente elettrica

**Funzione**: relazione tra due insiemi, chiamati dominio e codominio della funzione, che associa a ogni elemento del dominio un solo elemento del codominio.

# Legge di Ohm
$$V_{[V]} = I_{[A]} \times R_{[\Omega]}$$
**Forma più corretta per esprimerla**
$$I_{[A]} = \frac {V_{[V]}} {R_{[\Omega]}}$$
**_28/09/2026_**
# Diversi tipi di sistemi
- **Sistema naturale**: Sistema indipendente dall'uomo (es. corpo umano).
- **Sistema artificiale**: Diventa un sistema dall'interazione del corpo umano (es. computer)
- **Sistema misto**: Un orto che presenta un sistema di irrigazione o una serra.

### La distinzione dei sistemi avviene anche tramite il tempo: 
- **Sistemi discreti**: Posso definire lo stato del sistema tramite valori definiti per tutto il tempo in cui esiste. (Es. un circuito con un interruttore posso definire sempre che lo stato può essere acceso o spento sempre)
- **Sistemi continui**: Non può passare da un valore definito ad un altro in un singolo istante di tempo.

# Staticità di un sistema
- **Sistema statico**: Il cui funzionamento non dipende da un qualcosa di esterno, per esempio una ROM. Il sistema dove i valori non possono variare.
- **Sistema dinamico**: Il cui funzionamento puo' dipendere da un input esterno, esempio la RAM. Quando il suo stato non e' definito ma soggetto a variazioni, temporanee e reversibili.

# Sistemi aperti o chiusi
- **Sistema aperto**: Il suo funzionamento vive della relazione con l'esterno.
- **Sistema chiuso**: Un sistema che non comunica/scambia informazioni con l'esterno.

# Sistemi deterministici o probabilistici
- **Sistema deterministico**: Un sistema dove per lo stesso input, l'output sara' sempre uguale. Quindi un sistema prevedibile.
- **Sistema probabilistico**: Un sistema dove per lo stesso input, output non e' certo.

# Sistemi combinatori o sequenziali
- **Sistema combinatorio**: Sistemi che non hanno una memoria.
- **Sistema sequenziale**: Sistemi che hanno una memoria.

Todo: definire il personal computer come un sistema, perche lo e'? Che sistema e'?
		+ ricerca su sistema operativo, cos'e?

**Personal computer**: Il personal computer e' un sistema artificiale, discreto, dinamico, aperto, deterministico e sequenziale.

## Ricerca sistema operativo
Un sistema operativo si può definire come artificiale, discreto, dinamico, aperto, deterministico e sequenziale. Consiste di molteplici sottosistemi, ognuno con un ruolo definito per arrivare ad un obiettivo comune come eseguire un programma, comunicare con periferiche o mostrare qualcosa a schermo.

### Kernel
Il kernel e' quella parte del sistema operativo che comunica effettivamente con l'hardware e gestisce tutte le componentistiche a basso livello del sistema operativo, per comunicarci si usano le syscall.

### La divisione
Il sistema operativo e' diviso in due parti principali, il kernel-space e lo user space, più nel dettaglio il sistema operativo e' diviso ad anelli di permessi (rings).

![[Pasted image 20261006091117.png|465]]

### Driver
I driver sono l'unica parte introducibile dall'utente sul sistema che può comunicare quasi direttamente con l'hardware. Questi, se scritti male, posso portare ad un crash del sistema oppure essere pericolosi se provenienti da siti non ufficiali dei produttori.

'_01/10/2026_
# Connettori
I connettori sono tutti codificati: sono fatti in modo tale dal non poter essere messi al contrario.

## Connettori di alimentazione
### 20/24 pin slotted connector di scheda madre principale
> Tutte le schede madri moderne hanno 24 pin. Ci sono cavi di colore uguale perché linee della stessa tensione usano più cavi per portare più corrente. Le tensioni che portano sono: 5V, 12V, 3.3V. 
>![[Pasted image 20261001123646.png]]

### Alimentazione SATA
> Connettori di alimentazione per dischi SATA.
> ![[Pasted image 20261001124245.png]]

### Connettori alimentazione MOLEX
> Usati in sistemi legacy per alimentazione dischi e sistemi attaccati tramite SATA/ATA
> ![[Pasted image 20261001124212.png]]

### Connettore 8 pin ausiliario
> Diviso in due sezioni da 4 pin usato per portare alimentazione supplementare alla CPU

### Connettore 6+2 pin PCIe
> Usato per alimentare componentistica come schede grafiche più potente

## Connettori trovati sulle schede madri data

### ATA
> Acronimo di Advanced Technology Attachment.
### SATA
> Serial ATA, dati trasmessi in maniera seriale.
### PATA
> Parallel ATA, dati trasmessi in maniera parallela.
### IDE
> (Integrated Drive Electronics) Vecchio connettore dati.
### Internal USB
> Connettore a 19 pin usati per connettere il bus USB alla porta frontale del case per espansione e accessibilità.

# Schede madri
Un supporto che da la possibilità di collegare in modo opportuno componenti tra di loro.
Possono anche essere multistrato. E' il componente più' importante del computer, dopo la corrente.

La scheda madre ha diverse parti usate per connettere componenti e parti fondamentali del computer:
- **Socket CPU**: Usato per connettere la CPU alla scheda madre
- **Alimentazione locale**: Vicino alla CPU, usata per gestire alimentazione interna con dissipatori.
- **Slot RAM**: Connettori dove si possono installare i banchi di memoria, sono di due colori distinti per il dual channel, non tutte le memorie possono avere questa funzione.
- **USB interna**: Usati per portare le porte USB sul davanti del case
- **Chipset**: Uno dei componenti più importanti, mette in comunicazione la CPU con tutto il resto.
- **Chip BIOS/UEFI**: Chip dove risiede il BIOS/UEFI che gestisce la prima parte dell'avvio del computer e la configurazione a basso livello sulla scheda.
- **Slot di espansione**: Servono a collegare carte di espansione come schede video o schede di rete.

![[83.png]]
# Chipset
Il chipset e' quella parte del sistema che mette in comunicazione il processore e le altre componenti del computer attraverso i due bridge integrati dentro esso, la loro posizione e' strategica.
![[84.png]]
## Northbridge
Parte più vicina alla CPU, gestisce i dispositivi che necessitano una performance più elevata come RAM e slot PCI di priorità.

## Southbridge
Parte più lontana dalla CPU, si occupa di gestire i componenti meno performanti come Hard disk, USB, networking etc..

# Fattori di forma
Ci sono diversi standard di fattori di forma, sia per schede madri, che per alimentatori che per schede madri e sono in standard ATX, DTX e ITX.
![[Pasted image 20261001132435.png|453]]

# CPU
La CPU (Central Processing Unit) e' il componente "principale" se integrato con altri componenti e il suo compito e' eseguire istruzioni.

**Diversi tipi di connettori del processore (socket):**
Il connettore e' _codificato_, questo vuol dire che la CPU puo' essere inserita in un solo modo. Il socket usa il principio Zero Impression Force (ZIF), quindi non bisogna fare forza per inserirli. 
### Pin Grid Array  (PGA)
>In questa configurazione i pin escono dalla CPU mentre il socket presenta dei buchi ed una leva usata per bloccarli dentro.
>![[85.png]]

## Land Grid Array (LGA)
>In questa configurazione i pin sono posizionati sul socket mentre la CPU presenta dei pad per avere un contatto al tocco con i pin del socket. La leva in questo caso blocca la posizione della CPU con la scocca metallica che possiede.
>![[86.png]]

# Sistemi di raffreddamento
I sistemi di raffreddamento della CPU si dividono principalmente in 3 tipi: 
## Sistema passivo
>E' un sistema che non ha parti in movimento, come quello rappresentato in figura. Generalmente questi sistemi sono montati a sbalzo, cioè montato perpendicolarmente alla scheda madre.
>![[Pasted image 20261008124325.png]]

## Sistema attivo
>E' un dissipatore che ha una parte attiva/in movimento, come una ventola per spostare il caldo e portare aria fresca. In questo caso il dissipatore può
 avere una dimensione più ridotta.![[Pasted image 20261008124924.png]]

## Sistema a liquido (ibrido)
>I dissipatori a liquido sono chiamati ibridi perché la parte di contatto della CPU e' passiva mentre il radiatore raffredda il liquido e viene spinto sulla parte passiva.
>![[Pasted image 20261008125042.png]]

# Memoria
## Tipi di memoria
Esistono generalmente due tipi di memoria che vengono utilizzate all'interno di un computer.

### ROM (Read-only memory)
>La memoria ROM e' una memoria **non volatile** che viene utilizzata generalmente per mantenere dati anche dopo lo spegnimento del computer. Generalmente viene scritta in fabbrica e che non puo' essere sovrascritta.
### RAM (Random access memory)
>La memoria RAM e' una memoria **volatile** ad accesso casuale. Viene usata per eseguire programmi, e' scrivibile e molto veloce.

## Tipi di ROM

### ROM
>Questa e' una memoria read-only scritta in fabbrica e non puo' essere cambiata. E' usata per funzioni generali read-only
>![[Pasted image 20261008131618.png]]

### PROM
>Questi tipi di ROM escono dalla fabbrica vuote ma possono essere scritte solo una volta, successivamente diventano read-only.
>![[Pasted image 20261008131722.png]]

### EPROM
>Questo tipo di memorie può essere cancellato ma solo posizionandola sotto un forte raggio ultravioletto. In definitiva, possono essere riprogrammate, ma non facilmente.
>![[Pasted image 20261008131832.png]]

### EEPROM
>Questo tipo di memoria e' il piu' moderno e puo essere letta e riscritta completamente in modo elettronico. Questi tipi di memoria possono anche essere chiamate _flash_.
>![[Pasted image 20261008131919.png]]

## Tipi di RAM

### RAM dinamica
>Vecchia tecnologia degli anni '90. Usate per memoria di sistema, guardualmente scaricano l'energia e devono essere costantemente aggiornate.

### RAM statica
>Richiede alimentazione costante per funzionare, usate come cache, bassi consumi, piu' veloci delle RAM dinamiche e costano di piu.

### SDRAM
>RAM rinamiche che operano in sincrono con i banchi di memoria. Possono gestire istruzioni in parallelo e sono piu' veloci rispetto alle precedenti.

### DDR SDRAM
>RAM dinamiche (Double Data Rate Syncrounous Dynamic RAM), trasportano dati due volte piu veloci delle SDRAM normali, possono supportare due scritture e due letture ogni ciclo del clock. Il connettore ha 184 pin, usano 2.5V (Famiglia DDR2, DDR3, DDR4) 

### DDR2 SDRAM
>Trasferisce due volte piu veloce di SDRAM, funziona a velocita' di clock maggiori (533 MHz vs. DDR a 200MHz). Ha 240 pin e usa 1.8V

### DDR3 SDRAM
>Raddoppia la velocita del clock di DDR2, funziona a 1.5V, genera meno calore, funziona fino a 800MHz ed ha un connettore a 240 pin.

### DDR4 SDRAM
>Possiede quattro volte la capacita di DDR3, consuma 1.2V, funziona fino a 1600MHz, ha 288 pin.

### GDDR SDRAM
>Graphics DDR SDRAM, creata per le schede grafiche, usata assieme alla GPU, famiglia GDDR, GDDR2, GDDR3, GDDR4, GDDR5. La performance aumenta per ogni step.

### DDR5
>Piu del doppio della velocita dei moduli DDR4, 4x la capacita, consuma 1.1V, connettore a 288 pin ma con un pattern diverso da quello del DDR4, la grandezza massima per modulo e' 128GB

## Moduli di memoria
Ogni banco di memoria possiede i moduli effettivi sulla scheda:
### DIP
> Dual Inline Package e' un modulo di memoria individuale, generalmente i DIP hanno 2 linee di pin utilizzati per essere attaccati alla scheda madre.
> ![[Pasted image 20261008133613.png]]

### SIMM
> Single Inline Memory Module e' una piccola PCB che contiene piu moduli di memoria. Hanno connettori a 30 o 72 pin a seconda della configurazione.
> ![[Pasted image 20261008133719.png]]

### DIMM
> Dual Inline Memory Module e' una PCB che tiene SDDRAM, DDR SDDRAM ecc... fino alla DDR4. Ci sono da 168 pin a 288.
> ![[Pasted image 20261008133815.png]]

### SODIMM
> Small Outline DIMM e' una piccola versione della DIMM, generalmente usata in portatili, stampanti e device dove lo spazio e' chiave.
> ![[Pasted image 20261008133946.png]]


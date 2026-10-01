_01/10/2026_
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

# Chipset
Il chipset e' quella parte del sistema che mette in comunicazione il processore e le altre componenti del computer attraverso i due bridge integrati dentro esso, la loro posizione e' strategica.
![[Pasted image 20261001131701.png]]
## Northbridge
Parte più vicina alla CPU, gestisce i dispositivi che necessitano una performance più elevata come RAM e slot PCI di priorità.

## Southbridge
Parte più lontana dalla CPU, si occupa di gestire i componenti meno performanti come Hard disk, USB, networking etc..

# Fattori di forma
Ci sono diversi standard di fattori di forma, sia per schede madri, che per alimentatori che per schede madri e sono in standard ATX, DTX e ITX.
![[Pasted image 20261001132435.png|453]]


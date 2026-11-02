# Caratteristiche di un istruzione
- **Non ambiguità**: la stessa istruzione eseguita da esecutori diversi deve dare lo stesso risultato.
- **Finita**: l'istruzione deve terminare.
- **Deterministica**: se eseguita più' volte da lo stesso risultato.
- **Elementare**: l'istruzione non deve essere ulteriormente scomponibile o particolarmente complessa.
# Caratteristiche di un algoritmo
Un algoritmo deve essere:
- **Generale**: deve risolvere una categoria di problemi, non solo una parte.

# Descrizione di un algoritmo
- linguaggi di programmazione
- pseudo codice
- diagramma di flusso

# Diagrammi di flusso
Utilizziamo le figure geometriche per contenere le istruzioni

![[326.jpg]]

# Costrutti

![[327.jpg]]

# Teorema di Bohm-Jacopini
Qualsiasi problema sia risolvibile lo si può' implementare con le strutture di sequenza, selezione e iterazione.


# Operazioni/Algoritmi sulla gestione degli array
- Caricamento o popolazione di un array
- Ricerca di un elemento
- Ordinamento
- Aggiunta o eliminazione di un elemento
- Fusione di due array

## Caricamento o popolazione di un array di dimensione fisica DIM e dimensione logica scelta dall'utente 
```c
#define DIM ...

int main() { // INIZIO
	int numeri[DIM];
	
	do {
		printf("Quanti numeri vuoi caricare:");
		scanf("%d", &n);
	} while (n <= 0 || n >= DIM);
	
	for (int i = 0; i < n; i++) {
		printf("Inserisci il numero di posizione i:");
		scanf("%d", numeri[i]);
	}
	
	return 0; // FINE
}
```

## Ricerca di un elemento in un array
**Ricerca sequenziale**
```c
#define DIM ...
int main() {
	int numeri[DIM];
	int n, K;
	
	// Caricamento array (sottoproblema)
	carica_array(numeri, &n);
	
	printf("Inserisci il numero da cercare: ");
	scanf("%d", K);
	
	int i = 0;
	while (i < n && numeri[i] != K) i++;
	
	if (i == n) printf("Il valore non e' nell'array");
	else printf("L'elemento e' nell'array nella posizione %d", i);
	
	return 0;
}
```


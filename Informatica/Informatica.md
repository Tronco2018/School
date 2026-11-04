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

## Ordinamento di un array
Gli array possono essere ordinati in numerosi modi. Alcuni sono:
- Per selezione (Selection sort)
- A bolle (Bubble sort)
- Quick sort

### Implementazioni
**Selection Sort in ordine crescente**
```c
#define DIM ...
int main() {
	int arr[DIM], min, pos, temp, n = DIM;
	// arr esempio => 7 1 4 8 3 5 7 4 9
	
	// 1. Cercare il minimo e scambiarlo con il primo elemento
	// 2. Cercare il minimo a partire dalla posizione successiva
	// 3. Scambiarlo con l'elemento da cui si e' partiti
	
	// Carica array
	for (int i = 0; i < n; i++) scanf("%d", &arr[i]);
	
	for (int i = 0; i < n - 1; i++) {
		// Minimo di base
		min = arr[i];
		pos = i;
		
		// Cerca minimo
		for (int j = i; j < n; j++) {
			if (arr[j] < min) {
				min = arr[j];
				pos = j;
			}
		}
		
		// Scambia minimo con arr[i]
		temp = arr[i];
		arr[i] = arr[pos];
		arr[pos] = temp;
	}
	
	// Stampa risultato
	for (int i = 0; i < n; i++) {
		printf("%d ", arr[i]);
	}
	
	return 0;
}
```

**Bubble sort**
```c
#include <stdio.h>

#define DIM ...
int main() { 
	int arr[DIM], temp, n = DIM;
	
	// 1. Confronta due elementi adiacenti
	// 2. Se il precedente e' maggiore del successivo li scambio
	
	for (int i = 0; i < n; i++) scanf("%d", &arr[i]);
	
	for (int i = 0; i < n-1; i++) {
		if (arr[i] > arr[i+1]){
			temp = arr[i];
			arr[i] = arr[i+1];
			arr[i+1] = temp;
		}
	}
	
	for (int i = 0; i < n; i++) printf("%d ", arr[i]);
	
	return 0;
}
```
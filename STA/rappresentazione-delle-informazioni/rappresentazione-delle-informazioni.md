# Rappresentazione delle Informazioni Numeriche 🔢

## Concetti Base
La rappresentazione (codifica) delle informazioni numeriche avviene in unità base chiamate **byte**. 
Nella pratica si utilizzano potenze di 2:
- 1 byte (8 bit)
- 2 byte (16 bit)
- 4 byte (32 bit)
- 8 byte (64 bit)

## 1. Rappresentazione dei Numeri Naturali ℕ

Per rappresentare un numero naturale, occorre:
1. Convertire il numero in base binaria
2. Inserirlo in una quantità "adeguata" di byte

### Esempio di Conversione
Numero decimale: 53
```
Conversione binaria: 110101 (6 bit)
Opzioni di memorizzazione:
✅ 1 byte (8 bit)  - Ottimale
⬜ 2 byte (16 bit) - Spazio eccessivo
⬜ 4 byte (32 bit) - Spazio eccessivo
```

### Limiti della Rappresentazione
Con 1 byte (8 bit):
- Valore massimo: `11111111` = 255
- Se si supera: overflow a `00000000`

## 2. Rappresentazione dei Numeri Interi (con segno) ℤ

Il bit più significativo viene utilizzato per il segno:
- 0 → Positivo (+)
- 1 → Negativo (-)

### Due Metodologie di Rappresentazione

#### A. Modulo e Segno
Struttura:
```
|S|V|V|V|V|V|V|V|
 ↑ └──────────┘
segno  valore
```

Esempio: -5
```
1 00000101
↑ └──────┘
- valor 5
```

#### B. Complemento a 2
Per numeri negativi:
1. Convertire il valore assoluto
2. Fare il complemento a 1 (invertire tutti i bit)
3. Sommare 1

Esempio: -5
```
Valore assoluto:  00000101
Complemento a 1:  11111010
Somma 1:         11111011
```

## 3. Operazioni con Numeri Binari

### Somma
```
  00100101 (37)
+ 00110110 (54)
──────────
  01011011 (91)
```

### Sottrazione (usando complemento a 2)
```
  01100001 (97)
+ 11001111 (-48)
──────────
  00110001 (49)
```

## 4. Numeri con Virgola 

### Processo di Conversione
Esempio: 107.375

1. Parte intera: 107 → 1101011
2. Parte decimale: 
   ```
   0.375 × 2 = 0.75  → 0
   0.75  × 2 = 1.5   → 1
   0.5   × 2 = 1.0   → 1
   ```

Risultato: `1101011.011`

## 5. Standard IEEE 754 🔍

### Rappresentazione in Virgola Mobile
1. **Normalizzazione**: spostare la virgola dopo il primo 1
2. **Caratteristica**: esponente + bias
   - 32 bit: bias = 127
   - 64 bit: bias = 1023

### Formato
```
32 bit: |S|EEEEEEEE|MMMMMMMMMMMMMMMMMMMMMMM|
        ↑ └───────┘└───────────────────────┘
      segno   esp.        mantissa

64 bit: |S|EEEEEEEEEEE|MMMM...MMMM|
        ↑ └──────────┘└───────────┘
      segno   esp.     mantissa
```

> **Nota**: La rappresentazione in virgola mobile permette di gestire un'ampia gamma di numeri con diversa precisione.

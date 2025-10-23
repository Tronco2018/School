# Rappresentazione delle informazioni numeriche
La rappresentazione (codifica/traduzione) avviene in un formato base detto byte.
In realtà si utilizzano potenze di 2, ossia 1 byte, 2 byte, 4 byte, 8 byte, ...

## Rappresentazione dei numeri naturali
Per rappresentare un numero naturale si deve convertire il numero in base _Z_ e lo si deve inserire (scrivere) in una quantità "adeguata" di byte.
>Esempio
>Rappresentazione del numero 53 --> 110101 (6 bit)
>1 byte = 8 bit <--- scelta migliore perché utilizziamo meno spazio e rientra dentro gli 8 bit
>2 byte = 16 bit
>4 byte = 32 bit

```
Esercizio
Rappresentare il numero 341 (101010101) --> 9 bit
1 byte (8 bit) troppo piccolo
2 byte (16 bit) Abbastanza <--- scelta giusta
```
Un numero naturale rappresentato su 1 byte quali numeri si possono rappresentare
1 byte = 8 bit
Massimo valore (11111111) = 255
Se aggiungiamo 1 il valore diventa (00000000) perché abbiamo massimo 1 byte

## Rappresentazione dei numeri interi (con segno)
Si deve considerare la rappresentazione del segno che verrà gestita con 1 bit assegnando 0 per il **+** oppure 1 per il **-**.
Nella rappresentazione il bit di segno sarà sempre il bit più significativo.

Esistono due modalità di rappresentazione dei numeri interi.
- **Modulo e segno**: non molto usato, più in elettronica e basso livello
- **Complemento**: vale per qualsiasi base numerica, lo chiamiamo "complemento a 2" perché usiamo il binario.

### Modulo e segno
- bit più significativo per il segno
- bit rimanenti per il valore assoluto del numero (modulo del numero |a|)

**Esempio** -5
`|1|0|0|0|0|1|0|1|`
^   {--------------} <--- numero
|
(segno)

**Esercizio**
Rappresentare il +150 in modulo e segno
`|0|0|0|0|0|0|0|0|1|0|0|1|0|1|1|0|`

### Complemento a 2
I seguenti passaggi si applicano per la rappresentazione dei numeri negativi (per quelli positivi il complemento a due è identico a modulo e segno):
- Convertire e rappresentare il valore assoluto del numero
- Fare il complemento a 1 (gli 0 diventano 1 e gli 1 diventano 0)
- Sommare 1

**Esempio** -5
```java
[00000101]
 11111010
        1+
----------
[11111011] //Rappresetazione complemento a 2 di 5, il primo bit continua ad essere il segno
```

## Operazioni con i numeri binari
### Somma
37 + 54

37 = `[00100101]` (1 byte)
54 = `[00110110]` (1 byte)

result = `[01011011]`

### Differenza
97 - 48

97 = `[01100001]` (1 byte)

Negativo! da rappresentare in complemento a due
48 = `[00110000]` (1 byte)
-------`[11001111]` (complemento a due)

result = `[00110001]`

**Esempi**
35 - 71 = -36

35 = `[0110001]`

---
97+84

97 = `[01100001]`
84 = `[01010100]`

result = `[10110101]`

## Coversione dei numeri con la virgola
**Esempio**
$107.375$
|Parte intera|Parte decimale|
|------------|--------------|
|107|375|

### Parte intera
(Conversione classica)
$107 = 1101011$

### Parte decimale
$0.375\times2 = 0.75$
$0.75\times2 = 1.5$
$0.5\times2 = 1.0$

|Parte intera|Parte decimale|
|--|--|
|0|75|
|1|5|
|1|0|

!Le prendiamo in ordine inverso

### Risultato
$107.375_{10} => 1101011.011$

---

**Esempio 2**
_38.3_
$38 = 011001$
$0.3\times2 = 0.6$
$0.6\times2 = 1.2$ *
$0.2\times2 = 0.4$
$0.4\times2 = 0.8$
$0.8\times2 = 1.6$
$0.6\times2 = 1.2$ *

\* si vanno a ripetere: infinito

Result = $100110.01001$


## Rappresentazione dei numeri "reali"
- **Convertire il numero reale**
- **Normalizzazione** -> spostare la virgola subito dopo il primo 1 più significativo e moltiplicare per una potenza del due con esponente (positivo o negativo) corrispondente al numero di posti in cui la virgola è stata spostata
($1101011.011 => 1.101011011\times2^{+6}$)

---
- La **caratteristica** (esponente del due) verrà sempre rappresentata con un numero positivo. Si ottiene sommando il bias che varia in base al tipo di rappresentazione scelta:
 * Rappresentazione a 32 bit -> 127
 * Rappsesentazione a 64 bit -> 1023

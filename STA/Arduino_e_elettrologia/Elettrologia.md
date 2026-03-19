### Atomo
Fatto da:
- Protone (+) => interno (nucleo) [Carica positiva]
- Neutrone (\*) => interno (nucleo) [Neutro]
- Elettrone (-) => esterno (anelli) [Carica negativa]

In un atomo stabile => $nProtoni = nElettroni$
In un atomo con carica positiva => $nProtoni > nElettroni$
In un atomo con carica negativa => $nProtoni < nElettroni$

La **carica elettrica** si misura in *Coulomb*.

_**Attrazione**_
Due particelle di carica opposta di attraggono reciprocamente, come l'attrazione gravitazionale. Questo si chiama **attrazione elettrica**. La più grande attrae di più rispetto a quella più piccola. Cariche uguali **si respingono**.

Una carica elettrica può attirare o respingere oggetti, generando un campo elettrico.

_**Differenza di potenziale**_
In presenza di cariche elettriche fra due punti distinti e' presente una differenza di potenziale (capacita' di attrarre/respingere altre cariche elettriche).
Questa grandezza fisica si misura in Volt (simbolo $V$) e si può chiamare anche tensione o forza elettromotrice ($t.e.m$).

**Tipi di differenza di potenziale**
- DC => (Continua)
- AC => (Alternata)

### Corrente elettrica
E' il movimento ordinato di cariche elettriche. L'Intensità della corrente e' data da $$I=\frac{\Delta{Q}}{\Delta{t}}$$
$\Delta{Q}$ => variazione di carica elettrica
$\Delta{t}$ => variazione di tempo

L'Intensità di corrente elettrica di misura in Ampere
$$Ampere = \frac{Coulomb}{secondo}$$
**Conduttori**
I materiali che permettono il passaggio di corrente elettrica si dicono conduttori (es. rame, argento, oro, tungsteno, ecc...), mentre i materiali che si "oppongono" al movimento di cariche si dicono isolanti (es. gomma, vetro, legno, ecc...).
Esistono materiali semiconduttori, esistono anche superconduttori.

### Potenza elettrica
E' l'energia applicata per un intervallo di tempo e si misura in Watt 
$$P=V\times I$$
Potenza {W} = Differenza di potenziale {V} * Intensità di corrente {A}

### Resistenza elettrica
Si parla di resistenza elettrica quando un materiale tende ad opporsi al movimento delle cariche elettriche.
Prima legge di Ohm
$$R=\frac{\Delta{V}}{\Delta{I}}$$
Variazione di differenza di potenziale / variazione di corrente elettrica.
$R$ = resistenza elettrica (Misurata in Ohm $\ohm$ [Omega]).

### Circuiti elettrici
Un circuito elettrico e' costituito da, un generatore (di tensione), un carico (resistenza), dei conduttori (e un interruttore).

### Resistenze commerciali
In commercio esistono solo resistenze di misura limitata (1, 1.2, 1.5, 1.8, 2.2, 2.7, ecc...).
Il valore di una resistenza viene individuato tramite una serie di "bande" colorate.
Le resistenze possono essere a 4 bande o 5 bande.
![[Pasted image 20260312124311.png|255]]
![[Pasted image 20260316114112.png|253]]

**Resistenza a 4 bande**
Bande:
1. Prima cifra della resistenza
2. Seconda cifra della resistenza
3. Moltiplicatore (Potenza di 10)
4. Tolleranza (Percentuale)

**Resistenza a 5 bande**
Bande:
1. Prima cifra della resistenza
2. Seconda cifra della resistenza
3. Terza cifra della resistenza
4. Moltiplicatore (Potenza base 10)
5. Tolleranza (Percentuale)

### Collegamento di resistenze
Esistono due tipologie di collegamento di resistenze:
- In serie
- In parallelo

Collegandole in questi modi possiamo creare un valore di resistenza che non sono presenti in commercio.

**Collegamento di resistenze in serie**
Due o più resistenze sono collegate in serie quando vengono attraversate dalla stessa intensità di corrente (la "fine" di una resistenza viene collegata con l'"inizio" delll'altra).
![[Pasted image 20260316115828.png]]
$V_1$ ed $V_2$ sono la differenza di potenziale misurata rispettivamente ai capi della resistenza 1 e 2. $I$ e' l'intensità di corrente.
$$V_1 = R_1\times I$$
$$V_2 = R_2\times I$$
$$V = V_1+V_2$$
$$V=R_T\times I$$
$$V = R_T\times I \rightarrow R_1\times I + R_2\times I$$
$$R_T\times I = I\times (R_1 + R_2) \rightarrow R_T = R_1 + R_2$$
Abbiamo dimostrato che quando due resistenze sono in serie, la risultante $R_T$ e' uguale alla somma dei valori delle resistenze in serie.

**Collegamento di resistenze in parallelo**
Due più resistenze sono collegate in parallelo ai loro capi si ha la stessa differenza di potenziale.
![[Pasted image 20260316121329.png]]
$$I = I_1 + I_2$$
$$R_T = R_1 - R_2$$
$$I_1 = \frac{V}{R_1};\space I_2 =\frac{V}{R_2}; \space I = \frac{V}{R_T}$$
$$\frac{V}{R_T} = \frac{V}{R_1} + \frac{V}{R_2} \rightarrow \frac{V}{R_T} = V\times(\frac{1}{R_1} + \frac{1}{R_2})$$
$$\frac{1}{R_T} = \frac{1}{R_1} + \frac{1}{R_2}\rightarrow R_T = \frac{1}{\frac{1}{R_1} + \frac{1}{R_2}}$$
Quindi il reciproco di $R_T$ e' uguale ai reciproci delle resistenze presenti in parallelo sommati.

**Caso particolare** (Precisamente due resistenze in parallelo)
$$\frac{1}{R_T} = \frac{1}{R_1} + \frac{1}{R_2} \rightarrow \frac{1}{R_T}=\frac{R_2 + R_1}{R_1 \times R_2}$$
Facciamo il reciproco (ribaltiamo)
$$R_T = \frac{R_1\times R_2}{R_1 + R_2}$$

Esercizi sul quaderno.
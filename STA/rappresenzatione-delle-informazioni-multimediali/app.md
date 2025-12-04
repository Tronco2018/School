# Rappresentazione delle informazioni multimediali
- **Immagini**
- **Video**
- **Suoni**
- **Simboli afanumerici**

## 1. Rappresentazione dei simboli alfanumerici
- **Codifica ASCII standard**   
usa 7 bit (il bit piu significativo e' zero)  
>Esempio:  
`A <---> 01000001`  
`@ <---> 01000000`  
`a <---> 01100001`

- **Codifica ASCII esteso**  
usa 8 bit (non e' standard)

- **UNICODE**  
usa 16 bit, i primi 128 simboli sono ASCII standart (per retrocompatibilita)
>Esempio:  
`A <---> 0000000001000001`

**Esercizio**
il simbolo 0 (zero) ha codifica decimale `48`, qual e' la sua rappresentazione UNICODE?
```
48 = 1100000  
UNICODE = 00000000000110000  
```


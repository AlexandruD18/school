# Manuale di Ripasso

## MATRICE

### Obiettivo

Trovare le incognite con il metodo dei determinanti.

### Procedimento

1. Copia la **Matrice A** tante volte quante sono le sue **colonne**.
2. In ogni copia sostituisci **una colonna** della Matrice A con la **Matrice B**.
3. Calcola `=MATR.DETERM(A)` per verificare che il determinante della matrice principale non sia 0.
4. Calcola il determinante di ogni matrice modificata.
5. Trova le incognite con la formula:  
   **x = (determinante matrice con B) / (determinante matrice A)**

---

## RANGO

### Obiettivo

Determinare il rango di una matrice.

### Procedimento

1. Prendi le matrici **A** e **B**.
2. Calcola `=MATR.DETERM` per diverse combinazioni (3 o 4 prove).
3. Se ottieni un numero diverso da 0, quello è il rango.
4. Se il determinante è **0**, riduci la dimensione della matrice (es. da 5x5 a 4x4) e ripeti.

---

## STATISTICA

### Obiettivo

Calcolare frequenze e indici statistici.

### Passaggi

#### Frequenze

- **Frequenza assoluta:**  
  `=FREQUENZA(tabella; estremo_sup)`
- **Totale frequenze assolute:** somma di tutte le frequenze.
- **Frequenza relativa:**  
  `=frequenza_assoluta / totale_frequenze`
- **Frequenza cumulata assoluta:**
  - Prima classe = frequenza assoluta
  - Dalla seconda = frequenza cumulata precedente + frequenza assoluta della classe
- **Frequenza cumulata relativa:**  
  `=frequenza_cumulata_assoluta / totale_frequenze`

#### Indici di tendenza centrale

- **Media:** `=MEDIA(tabella)`
- **Mediana:** `=MEDIANA(tabella)`
- **Minimo:** `=MIN(tabella)`
- **Massimo:** `=MAX(tabella)`
- **I quartile:** `=INC.QUARTILE(tabella;1)`
- **II quartile:** `=INC.QUARTILE(tabella;2)`
- **III quartile:** `=INC.QUARTILE(tabella;3)`
- **IV quartile:** `=INC.QUARTILE(tabella;4)`

#### Indici di dispersione

- **Varianza:** `=VAR.P(tabella)`
- **Deviazione standard:** `=DEV.ST.P(tabella)`
- **Coefficiente di variazione:**  
  `=deviazione_standard / media`

#### Indici di forma

- **Asimmetria:** `=ASIMMETRIA.P(tabella)`

---

## TEOREMA DI BAYES

### Obiettivo

Calcolare probabilità condizionate.

### Procedimento

1. Parti da una tabella con **N** e **N GUASTI**.
2. Calcola il totale di entrambe le colonne.
3. Probabilità totale:  
   `=N GUASTI / N`
4. Probabilità condizionata (P(T|G)):
   - Tipo 1 → `=valore_1_N_GUASTI / totale_N_GUASTI`
   - Tipo 2 → `=valore_2_N_GUASTI / totale_N_GUASTI`
   - Tipo 3 → `=valore_3_N_GUASTI / totale_N_GUASTI`
   - Continua allo stesso modo per gli altri tipi.

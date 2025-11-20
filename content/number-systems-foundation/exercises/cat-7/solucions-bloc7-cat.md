# Solucions Bloc 7 – Primers, Compostos i Garbell d'Eratòstenes

---

## 📌 Part 1: Comprensió de Primers i Compostos — SOLUCIONS

### 1.1 Completa les Definicions

**Nombre Primer:** Un nombre natural major que 1 que té exactament **DOS** divisors.

**Nombre Compost:** Un nombre que té **MÉS** de dos divisors.

**Nombre 1:** El nombre 1 és **NI** primer **NI** compost.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 2 és un nombre primer | **VERTADER** | Els seus únics divisors són 1 i 2. |
| 1 és un nombre primer | **FALS** | Per definició, primers han de tenir exactament 2 divisors. 1 només en té 1. |
| 9 és un nombre primer | **FALS** | 9 = 3 × 3, té divisors: 1, 3, 9 (tres divisors). |
| Tot nombre parell és compost | **FALS** | 2 és parell i primer! (Els altres parells són compostos) |
| Els primers negatius no existeixen | **VERTADER** | Els primers es defineixen només per a nombres naturals positius. |

---

## 📌 Part 2: Identificar Divisors — SOLUCIONS

### 2.1 Llista tots els Divisors

| Nombre | Divisors | Quants? | Primer o Compost? |
|--------|----------|---------|------------------|
| 5 | 1, 5 | 2 | **PRIMER** |
| 8 | 1, 2, 4, 8 | 4 | **COMPOST** |
| 7 | 1, 7 | 2 | **PRIMER** |
| 15 | 1, 3, 5, 15 | 4 | **COMPOST** |
| 20 | 1, 2, 4, 5, 10, 20 | 6 | **COMPOST** |
| 13 | 1, 13 | 2 | **PRIMER** |

---

### 2.2 Classifica els Números

De: 2, 3, 4, 6, 9, 11, 15, 17, 20, 23, 25, 29

**P (Primers):** **2, 3, 11, 17, 23, 29**

**C (Compostos):** **4, 6, 9, 15, 20, 25**

---

## 📌 Part 3: El Garbell d'Eratòstenes — SOLUCIONS

### 3.1 Aplica el Garbell fins 20

| Número | Marcar? | Per què? |
|--------|---------|---------|
| 2 | **NO** | És el primer nombre primer |
| 3 | **NO** | És primer (3 × 1 = 3) |
| 4 | **SÍ** | Múltiple de 2 (2 × 2) |
| 5 | **NO** | És primer |
| 6 | **SÍ** | Múltiple de 2 (2 × 3) |
| 7 | **NO** | És primer |
| 8 | **SÍ** | Múltiple de 2 (2 × 4) |
| 9 | **SÍ** | Múltiple de 3 (3 × 3) |
| 10 | **SÍ** | Múltiple de 2 (2 × 5) |
| 11 | **NO** | És primer |
| 12 | **SÍ** | Múltiple de 2 (2 × 6) |
| 13 | **NO** | És primer |
| 14 | **SÍ** | Múltiple de 2 (2 × 7) |
| 15 | **SÍ** | Múltiple de 3 (3 × 5) |
| 16 | **SÍ** | Múltiple de 2 (2 × 8) |
| 17 | **NO** | És primer |
| 18 | **SÍ** | Múltiple de 2 (2 × 9) |
| 19 | **NO** | És primer |
| 20 | **SÍ** | Múltiple de 2 (2 × 10) |

**Primers fins a 20:** **2, 3, 5, 7, 11, 13, 17, 19**

---

### 3.2 Completa el Garbell fins 30

Seguint el mateix procés:

**Primers fins a 30:** **2, 3, 5, 7, 11, 13, 17, 19, 23, 29**

**Nous primers (21-30):** 23, 29

---

## 📌 Part 4: Propietats de Primers — SOLUCIONS

### 4.1 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 2 és l'únic nombre primer parell | **VERTADER** | Tots els altres nombres parells són divisibles per 2. |
| Tots els nombres primers són senars | **FALS** | 2 és primer i parell! |
| Els primers són infinits | **VERTADER** | Euclides ho va provar fa 2300 anys. |
| Cap nombre parell pot ser primer | **FALS** | 2 és parell i primer. |

---

### 4.2 Investiga Patrons

Primers: 2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31

| Pregunta | Resposta | Explicació |
|----------|----------|-----------|
| Quants primers parells? | **1** (només 2) | Tots els altres parells són divisibles per 2. |
| Quin és el més petit? | **2** | Per definició, primer > 1. |
| Els primers 5 primers? | **2, 3, 5, 7, 11** | Els primers nombres primers. |
| Quin patró veus? | **Els primers són cada cop més rars, però segueixen apareixent.** | Els primers es raren a mesura que augmentem. |

---

## 📌 Part 5: Diferenciar Primer vs Compost — SOLUCIONS

### 5.1 Explica per què Cadascun

| Nombre | Primer o Compost? | Explicació |
|--------|------------------|-----------|
| 21 | **COMPOST** | 21 = 3 × 7. Divisors: 1, 3, 7, 21 |
| 23 | **PRIMER** | Els seus únics divisors són 1 i 23 |
| 27 | **COMPOST** | 27 = 3 × 9 = 3 × 3 × 3. Divisors: 1, 3, 9, 27 |
| 31 | **PRIMER** | Els seus únics divisors són 1 i 31 |
| 35 | **COMPOST** | 35 = 5 × 7. Divisors: 1, 5, 7, 35 |

---

### 5.2 Problemes Aplicats

**Pregunta 1:** Si tens 17 estudiants, pots fer grups iguals?

**Resposta:** **NO (o sí: només 1 grup de 17 o 17 grups d'1).** Perquè 17 és primer i només té divisors 1 i 17.

---

**Pregunta 2:** Si tens 16 estudiants, quantes formes pots fer grups iguals?

**Resposta:** **16 = 2⁴ té divisors: 1, 2, 4, 8, 16. Per tant, pots fer:**
- 1 grup de 16
- 2 grups de 8
- 4 grups de 4
- 8 grups de 2
- 16 grups d'1
**Total: 5 formes**

---

## 📌 Part 6: Factoritzacions Incompletes — SOLUCIONS

### 6.1 Continua fins a Primers

| Factorització Incompleta | Continua | Factorització Completa |
|--------------------------|----------|----------------------|
| 12 = 2 × 6 | 2 × (2 × 3) | **12 = 2 × 2 × 3** |
| 20 = 2 × 10 | 2 × (2 × 5) | **20 = 2 × 2 × 5** |
| 18 = 2 × 9 | 2 × (3 × 3) | **18 = 2 × 3 × 3** |
| 30 = 3 × 10 | 3 × (2 × 5) | **30 = 2 × 3 × 5** |
| 24 = 4 × 6 | (2 × 2) × (2 × 3) | **24 = 2 × 2 × 2 × 3** |

---

### 6.2 Arbres de Factors

**20:**
```
       20
      /  \
     2   10
        /  \
       2    5
```
Resultat: **2 × 2 × 5**

**24:**
```
       24
      /  \
     4    6
    / \  / \
   2  2 2   3
```
Resultat: **2 × 2 × 2 × 3** o **2³ × 3**

---

## 📌 Part 7: Repte — Problemes de Lògica — SOLUCIONS

### 7.1 Pensa Críticament

**Pregunta 1:** Quants nombres primers hi ha entre 1 i 100?

**Resposta:** **25 nombres primers:**
2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97

---

**Pregunta 2:** Per què el 2 és especial entre els números primers?

**Resposta:** **Perquè és l'únic nombre primer parell.** Tots els altres nombres parells són divisibles per 2, per tant són compostos. El 2 és l'excepció.

---

**Pregunta 3:** Si multipliques dos nombres primers, el resultat pot ser primer?

**Resposta:** **NO, mai.** Si multipliques dos nombres primers p i q (ambdós > 1), el resultat p × q té almenys quatre divisors: 1, p, q, i p×q. Per tant, és sempre compost.

---

### 7.2 Casos Especials

**Pregunta 1:** El número 51 es pot dividir per 3. És primer?

**Resposta:** **NO, és compost.** Perquè 51 = 3 × 17. Si es pot dividir per 3 (i 3 ≠ 1 ni 51), aleshores té més de dos divisors: 1, 3, 17, 51.

---

**Pregunta 2:** El número 91 = 7 × 13. És primer?

**Resposta:** **NO, és compost.** Perquè 91 = 7 × 13. Té divisors: 1, 7, 13, 91. No és primer.

---

## 📌 Part 8: El Garbell Aplicat — SOLUCIONS

### 8.1 Usa el Garbell per Trobar Primers

**Primers fins a 50:**

**2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47**

(Total: 15 nombres primers)

---

### 8.2 Compte els Primers

| Pregunta | Resposta | Explicació |
|----------|----------|-----------|
| Quants primers fins a 20? | **8** | 2, 3, 5, 7, 11, 13, 17, 19 |
| Quants entre 20 i 40? | **5** | 23, 29, 31, 37 (34, 35, 36, 38, 39, 40 són compostos) |
| Més comuns: petits o grans? | **Més comuns en números petits** | Primer densidade disminueix amb números més grans. |

---

## 📌 Part 9: Crea els Teus Números — SOLUCIONS (EXEMPLAR)

### 9.1 Escull i Classifica

**Exemple:**

| Número | Primer? | Divisors |
|--------|---------|----------|
| 7 | **SÍ** | 1, 7 |
| 12 | **NO** | 1, 2, 3, 4, 6, 12 |
| 19 | **SÍ** | 1, 19 |
| 20 | **NO** | 1, 2, 4, 5, 10, 20 |
| 23 | **SÍ** | 1, 23 |

---

### 9.2 Crea un Problema Real

**Exemple de Problema:** 

"Si tens **19 euros** per a comprar **llibres**, pots repartir equitativament entre grups iguals? (sense deixar euros sense repartir)"

**Resposta:** No (només es pot fer 1 grup de 19 euros, perquè 19 és primer).

---

## 🎯 Claus del Bloc 7

| Concepte | Descripció |
|----------|-----------|
| **Nombre Primer** | Natural > 1 amb exactament 2 divisors (1 i ell mateix) |
| **Nombre Compost** | Natural > 1 amb més de 2 divisors |
| **Nombre 1** | Ni primer ni compost (cas especial) |
| **Garbell d'Eratòstenes** | Algoritme per trobar primers marcant múltiples |
| **2 és especial** | Únic nombre primer parell |
| **Infinitud** | Hi ha infinitament molts primers (Euclides) |

---

## 📊 Resumen de Respostes Correctes

**Part 1:** Definicions correctes de primer, compost, i 1.
**Part 2:** Identificació correcta de divisors i classificació.
**Part 3:** Aplicació correcta del Garbell d'Eratòstenes.
**Part 4:** Propietats correctes de primers (2 és parell, primers són infinits, etc.).
**Part 5:** Diferenciació entre primers i compostos amb explicacions.
**Part 6:** Factoritzacions completes fins a primers.
**Part 7:** Pensament crític sobre casos especials i propietats.
**Part 8:** Compte correcte de primers en intervals.
**Part 9:** Creació de problemes amb números primer/compost.
**Part 10:** Reflexió sobre importància de primers.

---

**Felicitats! Has completat Bloc 7. Ara dominas els nombres primers!** 🌟

Els primers són els blocs de construcció de tota la matemàtica! Els científics els usen per a criptografia, internet, i seguretat! 🔐


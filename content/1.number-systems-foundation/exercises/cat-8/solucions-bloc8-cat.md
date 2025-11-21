# Solucions Bloc 8 – Aplicacions MCD i Algoritme d'Euclides

---

## 📌 Part 1: Comprensió del MCD — SOLUCIONS

### 1.1 Completa les Definicions

**MCD (Màxim Comú Divisor):** El nombre **MÉS GRAN** que divideix dos nombres sense resta.

**Algoritme d'Euclides:** Un mètode per trobar el MCD usant **DIVISIÓ** repetida.

**Divisor Comú:** Un nombre que divideix **AMBDÓS NOMBRES** sense deixar resta.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| MCD(6, 9) = 3 | **VERTADER** | Divisors comuns: 1, 3. El màxim és 3. |
| MCD(10, 20) = 10 | **VERTADER** | 10 divideix tant 10 com 20. |
| MCD(7, 11) = 1 | **VERTADER** | Els únics divisor comú és 1 (són primers). |
| MCD sempre menor que els números | **FALS** | Si a divideix b, MCD(a, b) = a, que és igual a a. |

---

## 📌 Part 2: Trobar Divisors Comuns — SOLUCIONS

### 2.1 Llista Divisors Comuns

| Parella | Divisors 1r | Divisors 2n | Comuns | MCD |
|---------|------------|------------|--------|-----|
| MCD(12, 18) | 1,2,3,4,6,12 | 1,2,3,6,9,18 | 1,2,3,6 | **6** |
| MCD(20, 30) | 1,2,4,5,10,20 | 1,2,3,5,6,10,15,30 | 1,2,5,10 | **10** |
| MCD(8, 12) | 1,2,4,8 | 1,2,3,4,6,12 | 1,2,4 | **4** |
| MCD(9, 15) | 1,3,9 | 1,3,5,15 | 1,3 | **3** |

---

## 📌 Part 3: Algoritme d'Euclides — SOLUCIONS

### 3.1 Completa els Passos

| Operació | Divisió | Residu | MCD |
|----------|---------|--------|-----|
| MCD(24, 36) | 36 = 24 × **1** + **12** | 12 | **12** (però...) |
|  | 24 = 12 × **2** + **0** | 0 | |
| MCD(50, 30) | 50 = 30 × **1** + **20** | 20 | **10** |
|  | 30 = 20 × **1** + **10** | 10 | |
|  | 20 = 10 × **2** + **0** | 0 | |
| MCD(100, 60) | 100 = 60 × **1** + **40** | 40 | **20** |
|  | 60 = 40 × **1** + **20** | 20 | |
|  | 40 = 20 × **2** + **0** | 0 | |

---

### 3.2 Practica l'Algoritme

**MCD(56, 35):**
- 56 = 35 × **1** + **21**
- 35 = **21** × **1** + **14**
- **21** = **14** × **1** + **7**
- **14** = **7** × **2** + **0**
- **MCD = 7**

---

**MCD(72, 48):**
- 72 = 48 × **1** + **24**
- 48 = **24** × **2** + **0**
- **MCD = 24**

---

## 📌 Part 4: MCD en Problemes Reals — SOLUCIONS

### 4.1 Distribució Equitativa

**Problema 1:** Tens 24 nens i 36 nenes. Vols fer grups iguals.

- Divisors de 24: 1, 2, 3, 4, 6, 8, 12, 24
- Divisors de 36: 1, 2, 3, 4, 6, 9, 12, 18, 36
- MCD(24, 36) = **12**
- **Resposta:** **12 grups** (cada grup amb **2 nens i 3 nenes**)

---

**Problema 2:** Tens 48 maçanes i 36 taronges.

- MCD(48, 36) = **12**
- **Resposta:** **12 cistelles** (cada una amb **4 maçanes i 3 taronges**)

---

### 4.2 Enrajolat de Rectangle

Vols cobrir 60 × 45 cm amb rajoles quadrades.

- MCD(60, 45) = **15**
- **Resposta:** Rajoles de **15 × 15 cm**

**Verificació:** 60 ÷ 15 = 4 rajoles horitals, 45 ÷ 15 = 3 rajoles verticals. 4 × 3 = 12 rajoles totals. ✓

---

## 📌 Part 5: Propietats del MCD — SOLUCIONS

### 5.1 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| MCD(a, b) = MCD(b, a) | **VERTADER** | La divisió és commutativa en aquest sentit. |
| MCD(a, b) ≤ min(a, b) | **VERTADER** | El MCD no pot ser més gran que el més petit nombre. |
| MCD(a, a) = a | **VERTADER** | El màxim divisor de a és a mateix. |
| Si a divideix b, MCD(a, b) = a | **VERTADER** | Llavors a és el màxim comú divisor. |

---

### 5.2 Relació amb MCM

**Identitat:** a × b = MCD(a, b) × MCM(a, b)

| a | b | MCD(a, b) | a × b | MCM(a, b) |
|---|---|-----------|-------|-----------|
| 12 | 18 | 6 | 216 | 36 |
| 20 | 30 | **10** | **600** | **60** |
| 8 | 12 | **4** | **96** | **24** |
| 15 | 25 | **5** | **375** | **75** |

**Verificacions:**
- 12 × 18 = 216; 6 × 36 = 216 ✓
- 20 × 30 = 600; 10 × 60 = 600 ✓

---

## 📌 Part 6: Simplificació de Fraccions — SOLUCIONS

### 6.1 Simplifica usant MCD

| Fracció | MCD | Simplificada |
|---------|-----|-------------|
| 20/30 | **10** | **2/3** |
| 36/48 | **12** | **3/4** |
| 15/25 | **5** | **3/5** |
| 18/24 | **6** | **3/4** |

**Exemple detallat (20/30):**
- MCD(20, 30) = 10
- 20/30 = (20÷10)/(30÷10) = 2/3 ✓

---

### 6.2 Verifica si es pot Simplificar

Una fracció es pot simplificar si MCD > 1.

| Fracció | MCD | Es pot simplificar? |
|---------|-----|------------------|
| 7/11 | **1** | **NO** (ja està simplificada) |
| 14/21 | **7** | **SÍ** → 2/3 |
| 13/17 | **1** | **NO** (primers) |
| 25/40 | **5** | **SÍ** → 5/8 |

---

## 📌 Part 7: Problemes de Sincronització — SOLUCIONS

### 7.1 Cicles Que Es Sincronitzen

**Problema:** Dos semàfors. Un cada 12 segons, altre cada 18 segons. Quan parpellegen junts?

- MCD(12, 18) = **6**
- MCM(12, 18) = (12 × 18) / MCD(12, 18) = **216 / 6 = 36**
- **Resposta:** Cada **36 segons** parpellegen junts

**Verificació:** Múltiples de 12: 12, 24, 36, 48... Múltiples de 18: 18, 36, 54... Primer comú: 36 ✓

---

### 7.2 Buses que Arriben

Un bus cada 15 minuts, altre cada 20 minuts. Quan arriben junts?

- MCD(15, 20) = **5**
- MCM(15, 20) = (15 × 20) / **5** = **300 / 5 = 60**
- **Resposta:** Cada **60 minuts (1 hora)** arriben junts

---

## 📌 Part 8: Repte — Problemes Avançats — SOLUCIONS

### 8.1 Pensa Críticament

**Pregunta 1:** Què és MCD(0, n)?

**Resposta:** **MCD(0, n) = n.** Perquè tot nombre divideix 0 (0 = n × 0), i el màxim divisor de 0 i n és n.

---

**Pregunta 2:** Si MCD(a, b) = 1, què significa?

**Resposta:** **Els nombres són coprims (primers entre ells).** No comparteixen divisors comuns excepte 1. Per exemple, 7 i 11 són coprims.

---

**Pregunta 3:** Quan MCD(a, b) = a? Quan MCD(a, b) = b?

**Resposta:** 
- **MCD(a, b) = a quan a divideix b** (per exemple, MCD(5, 20) = 5)
- **MCD(a, b) = b quan b divideix a** (per exemple, MCD(20, 5) = 5)

---

### 8.2 Casos Especials

**Pregunta 1:** MCD(12, 18, 24)?

- MCD(12, 18) = **6**
- MCD(6, 24) = **6**
- **MCD(12, 18, 24) = 6**

---

**Pregunta 2:** MCD(100, 50, 75)?

- MCD(100, 50) = **50**
- MCD(50, 75) = **25**
- **MCD(100, 50, 75) = 25**

(Nota: L'ordre importa! MCD(a, b, c) = MCD(MCD(a, b), c))

---

## 📌 Part 9: Crea els Teus Exercicis — SOLUCIONS (EXEMPLAR)

### 9.1 Disseny de Problemes

**Exemple d'Exercici 1:**

"Tens **60 caramels** i **45 xocolates** per repartir equitativament. Quants grups pots fer?"

**Solució:** MCD(60, 45) = **15 grups**

---

**Exemple d'Exercici 2:**

"Simplifica la fracció **24/36**"

**Solució:** **2/3** (dividint per MCD = 12)

---

### 9.2 Reflexió

**Pregunta 1:** On vas veure MCD en la vida real?

**Resposta Possible:** En distribuir classes en grups iguals, repartir menjar equitativament, trobar mides comunes per a enrajolats, etc.

---

**Pregunta 2:** Per què és important l'Algoritme d'Euclides?

**Resposta Possible:** **Perquè és ràpid i eficient,** funciona fins i tot per a números enormes, i es va usar fa 2300 anys. Avui es va usar en criptografia RSA per a protegir Internet!

---

## 🎯 Claus del Bloc 8

| Concepte | Descripció |
|----------|-----------|
| **MCD** | El nombre més gran que divideix dos nombres |
| **Algoritme d'Euclides** | Divisió repetida amb restes fins a 0 |
| **Divisors Comuns** | Nombres que divideixen ambdós nombres |
| **Identitat MCD-MCM** | a × b = MCD(a, b) × MCM(a, b) |
| **Aplicacions** | Simplificació de fraccions, distribució equitativa |
| **Coprims** | MCD(a, b) = 1 (sense divisors comuns) |

---

## 📊 Resumen de Respostes Correctes

**Part 1:** Definicions correctes i propietats del MCD.
**Part 2:** Llista correcta de divisors comuns i identificació del MCD.
**Part 3:** Aplicació correcta de l'Algoritme d'Euclides.
**Part 4:** Resolució correcta de problemes reals.
**Part 5:** Propietats correctes i relació MCD-MCM.
**Part 6:** Simplificació correcta de fraccions.
**Part 7:** Càlcul correcte de MCM usant MCD.
**Part 8:** Pensament crític sobre casos especials.
**Part 9:** Creació de problemes i reflexió significativa.

---

**Felicitats! Has completat Bloc 8. Ara dominas el MCD i l'Algoritme d'Euclides!** 🌟

L'Algoritme d'Euclides és un dels algoritmes més importants de tota la matemàtica! 🔐


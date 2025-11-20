# Exercicis Bloc 8 – Aplicacions MCD i Algoritme d'Euclides

---

## 📌 Part 1: Comprensió del MCD

### 1.1 Completa les Definicions

**MCD (Màxim Comú Divisor):** El nombre _________________ que divideix dos nombres sense resta.

**Algoritme d'Euclides:** Un mètode per trobar el MCD usant _________________ repetida.

**Divisor Comú:** Un nombre que divideix _________________  sense deixar resta.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| MCD(6, 9) = 3 | | |
| MCD(10, 20) = 10 | | |
| MCD(7, 11) = 1 | | |
| El MCD és sempre menor que els números originals | | |

---

## 📌 Part 2: Trobar Divisors Comuns

### 2.1 Llista Divisors Comuns

**Exemple:** MCD(12, 18)
- Divisors de 12: 1, 2, 3, 4, 6, 12
- Divisors de 18: 1, 2, 3, 6, 9, 18
- Divisors comuns: 1, 2, 3, 6
- **MCD = 6**

| Parella | Divisors 1r | Divisors 2n | Comuns | MCD |
|---------|------------|------------|--------|-----|
| MCD(12, 18) | | | | |
| MCD(20, 30) | | | | |
| MCD(8, 12) | | | | |
| MCD(9, 15) | | | | |

---

## 📌 Part 3: Algoritme d'Euclides

### 3.1 Completa els Passos

**Pas 1:** Divideix el nombre més gran per el més petit.
**Pas 2:** El divisor es converteix en dividend, el residu en divisor.
**Pas 3:** Repeteix fins que la resta sigui 0. El darrer divisor és el MCD.

Exemple: MCD(48, 18)
- 48 = 18 × 2 + 12
- 18 = 12 × 1 + 6
- 12 = 6 × 2 + 0
- **MCD = 6**

| Operació | Divisió | Residu | MCD |
|----------|---------|--------|-----|
| MCD(24, 36) | 36 = 24 × __ + __ | | |
| MCD(50, 30) | | | |
| MCD(100, 60) | | | |

---

### 3.2 Practica l'Algoritme

Calcula MCD usant Euclides:

**MCD(56, 35):**
- 56 = 35 × ___ + ___
- 35 = ___ × ___ + ___
- ___ = ___ × ___ + ___
- **MCD = ___**

---

**MCD(72, 48):**
- 72 = 48 × ___ + ___
- 48 = ___ × ___ + ___
- ___ = ___ × ___ + ___
- **MCD = ___**

---

## 📌 Part 4: MCD en Problemes Reals

### 4.1 Distribució Equitativa

**Problema 1:** Tens 24 nens i 36 nenes. Vols fer grups iguals. Quin és el màxim nombre de grups?

- Divisors de 24: _______________
- Divisors de 36: _______________
- MCD(24, 36) = ___
- **Resposta:** ___ grups (cada grup amb ___ nens i ___ nenes)

---

**Problema 2:** Tens 48 maçanes i 36 taronges. Vols fer cistelles iguals sense mesclar. Quantes cistelles pots fer?

- MCD(48, 36) = ___
- **Resposta:** ___ cistelles (cada una amb ___ maçanes i ___ taronges)

---

### 4.2 Enrajolat de Rectangle

Vols cobrir un rectangle de 60 × 45 cm amb rajoles quadrades de la mateixa mida, sense tallar.

- Quina és la mida més gran de rajola quadrada?
- MCD(60, 45) = ___
- **Resposta:** Rajoles de ___ × ___ cm

---

## 📌 Part 5: Propietats del MCD

### 5.1 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| MCD(a, b) = MCD(b, a) | | |
| MCD(a, b) ≤ min(a, b) | | |
| MCD(a, a) = a | | |
| Si a divideix b, MCD(a, b) = a | | |

---

### 5.2 Relació amb MCM

Recorda: **a × b = MCD(a, b) × MCM(a, b)**

| a | b | MCD(a, b) | a × b | MCM(a, b) |
|---|---|-----------|-------|-----------|
| 12 | 18 | 6 | 216 | 36 |
| 20 | 30 | | | |
| 8 | 12 | | | |
| 15 | 25 | | | |

---

## 📌 Part 6: Simplificació de Fraccions

### 6.1 Simplifica usant MCD

**Exemple:** 24/36
- MCD(24, 36) = 12
- 24/36 = (24÷12)/(36÷12) = 2/3

| Fracció | MCD | Simplificada |
|---------|-----|-------------|
| 20/30 | | |
| 36/48 | | |
| 15/25 | | |
| 18/24 | | |

---

### 6.2 Verifica si es pot Simplificar

Una fracció es pot simplificar si MCD(numerador, denominador) > 1.

| Fracció | MCD | Es pot simplificar? |
|---------|-----|------------------|
| 7/11 | | |
| 14/21 | | |
| 13/17 | | |
| 25/40 | | |

---

## 📌 Part 7: Problemes de Sincronització

### 7.1 Cicles Que Es Sincronitzen

**Problema:** Dos semàfors parpadegen. Un cada 12 segons, altre cada 18 segons. Quan parpellegen junts novament?

(Pista: Necessites MCM, no MCD, però MCD us ajuda a trobar-lo)

- MCD(12, 18) = ___
- MCM(12, 18) = (12 × 18) / MCD(12, 18) = _____  / _____ = _____
- **Resposta:** Cada _____ segons parpellegen junts

---

### 7.2 Buses que Arriben

Un bus passa cada 15 minuts, un altre cada 20 minuts. Quan arriben al mateix temps?

- MCD(15, 20) = ___
- MCM(15, 20) = ___
- **Resposta:** Cada _____ minuts arriben junts

---

## 📌 Part 8: Repte — Problemes Avançats

### 8.1 Pensa Críticament

**Pregunta 1:** Què és MCD(0, n)?

**Resposta:** _________________________________________________________________

---

**Pregunta 2:** Si MCD(a, b) = 1, què significa?

**Resposta:** _________________________________________________________________

---

**Pregunta 3:** Quan MCD(a, b) = a? Quan MCD(a, b) = b?

**Resposta:** _________________________________________________________________

---

### 8.2 Casos Especials

**Pregunta 1:** MCD de tres nombres: MCD(12, 18, 24)?

(Pista: MCD(12, 18) primer, després MCD(resultat, 24))

- MCD(12, 18) = ___
- MCD(6, 24) = ___
- **MCD(12, 18, 24) = ___**

---

**Pregunta 2:** MCD(100, 50, 75)?

- MCD(100, 50) = ___
- MCD(50, 75) = ___
- **MCD(100, 50, 75) = ___**

---

## 📌 Part 9: Crea els Teus Exercicis

### 9.1 Disseny de Problemes

**Exercici 1 (Distribució):**

"Tens __________ i __________ per repartir equitativament. Quant pots fer de cada grup?"

**Solució:** MCD = ___

---

**Exercici 2 (Simplificació):**

"Simplifica la fracció __________/__________"

**Solució:** ___________/___________

---

### 9.2 Reflexió

**Pregunta 1:** On vas veure MCD en la vida real?

_________________________________________________________________

---

**Pregunta 2:** Per què és important l'Algoritme d'Euclides?

_________________________________________________________________

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Divisors comuns): ✓
- [ ] Part 3 (Algoritme d'Euclides): ✓
- [ ] Part 4 (Problemes reals): ✓
- [ ] Part 5 (Propietats): ✓
- [ ] Part 6 (Simplificació): ✓
- [ ] Part 7 (Sincronització): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Creació): ✓

**Puntuació:** Si has marcat 7 o més, dominas el MCD! 🎉

---

**Recorda:** El MCD és el nombre més gran que divideix sense deixar resta! 🔍


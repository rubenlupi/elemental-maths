# Solucions Bloc 6 – Pràctica de Regles de Divisibilitat

---

## 📌 Part 1: Comprensió Bàsica de Divisibilitat — SOLUCIONS

### 1.1 Completa les Definicions

**Divisibilitat:** Un nombre `a` es divideix per un nombre `b` si la divisió `a ÷ b` dóna un nombre enter (sense resta).

**Regla de Divisibilitat:** Una regla de divisibilitat és una drecera o patró que permet determinar si un nombre és divisible per un altre només mirant els dígits, sense fer la divisió completa.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 24 és divisible per 2 | **VERTADER** | Acaba en 4 (parell). 24 ÷ 2 = 12 ✓ |
| 15 és divisible per 3 | **VERTADER** | Suma de dígits: 1+5 = 6, múltiple de 3. 15 ÷ 3 = 5 ✓ |
| 20 és divisible per 5 | **VERTADER** | Acaba en 0. 20 ÷ 5 = 4 ✓ |
| 17 és divisible per 2 | **FALS** | Acaba en 7 (senar). 17 ÷ 2 = 8.5 (no enter) ✗ |
| 100 és divisible per 9 | **FALS** | Suma de dígits: 1+0+0 = 1, no és múltiple de 9. 100 ÷ 9 = 11.11... ✗ |

---

## 📌 Part 2: Regla de Divisibilitat per 2 — SOLUCIONS

### 2.1 Identifica si és Divisible per 2

| Nombre | Últim Dígit | Divisible per 2? |
|--------|------------|-----------------|
| 346 | 6 | **SÍ** (6 és parell) |
| 123 | 3 | **NO** (3 és senar) |
| 2,000 | 0 | **SÍ** (0 és parell) |
| 789 | 9 | **NO** (9 és senar) |
| 1,244 | 4 | **SÍ** (4 és parell) |
| 5,555 | 5 | **NO** (5 és senar) |

---

### 2.2 Marca els Parells

De: 45, 128, 2,001, 3,456, 7, 9,999, 5,000, 333

**Resposta:** **128, 3,456, 5,000**

**Explicació:** Només aquests acaben en dígit parell (8, 6, 0).

---

## 📌 Part 3: Regla de Divisibilitat per 3 — SOLUCIONS

### 3.1 Suma de Dígits per 3

| Nombre | Suma de Dígits | Múltiple de 3? | Divisible per 3? |
|--------|---------------|----------------|------------------|
| 123 | 1+2+3 = 6 | SÍ (6÷3=2) | **SÍ** |
| 456 | 4+5+6 = 15 | SÍ (15÷3=5) | **SÍ** |
| 789 | 7+8+9 = 24 | SÍ (24÷3=8) | **SÍ** |
| 1,234 | 1+2+3+4 = 10 | NO | **NO** |
| 5,005 | 5+0+0+5 = 10 | NO | **NO** |
| 222 | 2+2+2 = 6 | SÍ (6÷3=2) | **SÍ** |

---

### 3.2 Completa els Blancs

**1. En el nombre 2_5:**
- Suma actual: 2 + **?** + 5 = 7 + **?**
- Per ser múltiple de 3, la suma ha de ser: **9** (o 12, 15, 18...)
- La xifra ha de ser: **2** (ja que 7 + 2 = 9)
- Verificació: 225 ÷ 3 = 75 ✓

**2. En el nombre 51_:**
- Suma actual: 5 + 1 + **?** = 6 + **?**
- Per ser múltiple de 3, la suma ha de ser: **9** (o 12, 15...)
- La xifra ha de ser: **3** (ja que 6 + 3 = 9)
- Verificació: 513 ÷ 3 = 171 ✓

**Altres respostes vàlides:**
- Per 2_5: 8 (2+8+5=15), ...
- Per 51_: 6 (5+1+6=12), 9 (5+1+9=15), ...

---

## 📌 Part 4: Regla de Divisibilitat per 5 — SOLUCIONS

### 4.1 Últim Dígit per 5

| Nombre | Últim Dígit | Divisible per 5? |
|--------|------------|-----------------|
| 345 | 5 | **SÍ** |
| 1,000 | 0 | **SÍ** |
| 2,342 | 2 | **NO** |
| 3,575 | 5 | **SÍ** |
| 1,001 | 1 | **NO** |

---

### 4.2 Busca els Divisibles per 5

De: 22, 45, 100, 123, 505, 777, 1,000

**Divisibles per 5:** **45, 100, 505, 1,000**

**Explicació:** Els únics que acaben en 0 o 5.

---

## 📌 Part 5: Regla de Divisibilitat per 9 — SOLUCIONS

### 5.1 Suma per 9

| Nombre | Suma | Múltiple de 9? | Divisible per 9? |
|--------|------|----------------|------------------|
| 108 | 1+0+8 = 9 | **SÍ** | **SÍ** (108÷9=12) |
| 999 | 9+9+9 = 27 | **SÍ** (27÷9=3) | **SÍ** (999÷9=111) |
| 225 | 2+2+5 = 9 | **SÍ** | **SÍ** (225÷9=25) |
| 1,234 | 1+2+3+4 = 10 | **NO** | **NO** |
| 2,700 | 2+7+0+0 = 9 | **SÍ** | **SÍ** (2,700÷9=300) |

---

### 5.2 Vertader o Fals?

- 99 és divisible per 9: **VERTADER** (comprovació: 9+9=18, 18÷9=2 ✓)
- 100 és divisible per 9: **FALS** (comprovació: 1+0+0=1, 1÷9✗)
- 1,111 és divisible per 9: **FALS** (comprovació: 1+1+1+1=4, 4÷9✗)

---

## 📌 Part 6: Regla de Divisibilitat per 4 — SOLUCIONS

### 6.1 Últims Dos Dígits per 4

| Nombre | Últims 2 Dígits | Divisible per 4? |
|--------|----------------|-----------------|
| 124 | 24 (24÷4=6) | **SÍ** |
| 123 | 23 (23÷4=5.75) | **NO** |
| 516 | 16 (16÷4=4) | **SÍ** |
| 1,000 | 00 (00÷4=0) | **SÍ** |
| 2,345 | 45 (45÷4=11.25) | **NO** |

---

### 6.2 Escull la Resposta Correcta

Per fer que 23__ sigui divisible per 4:
- Nombre: 23**2**
- Opcions: 2, 4, 6, 8
- Resposta: **Qualsevol dels: 2, 6** funcionen

**Comprovacions:**
- 232: últims 2 dígits = 32 ÷ 4 = 8 ✓
- 234: últims 2 dígits = 34 ÷ 4 = 8.5 ✗
- 236: últims 2 dígits = 36 ÷ 4 = 9 ✓
- 238: últims 2 dígits = 38 ÷ 4 = 9.5 ✗

---

## 📌 Part 7: Divisibilitat per 6 — SOLUCIONS

### 7.1 Recorda: 6 = 2 × 3

| Nombre | Divisible per 2? | Divisible per 3? | Divisible per 6? |
|--------|------------------|------------------|-----------------|
| 12 | **SÍ** (acaba en 2) | **SÍ** (1+2=3) | **SÍ** |
| 18 | **SÍ** (acaba en 8) | **SÍ** (1+8=9) | **SÍ** |
| 24 | **SÍ** (acaba en 4) | **SÍ** (2+4=6) | **SÍ** |
| 15 | **NO** (acaba en 5) | **SÍ** (1+5=6) | **NO** (falta divisibilitat per 2) |
| 30 | **SÍ** (acaba en 0) | **SÍ** (3+0=3) | **SÍ** |
| 100 | **SÍ** (acaba en 0) | **NO** (1+0+0=1) | **NO** (falta divisibilitat per 3) |

---

### 7.2 Corregeix l'Error

**Afirmació Falsa:** "15 és divisible per 6 perquè és divisible per 3."

**Per què és falsa?** Perquè 6 = 2 × 3. Un nombre ha de ser divisible **tant per 2 COM per 3** per ser divisible per 6. 15 és divisible per 3, però NO és divisible per 2 (acaba en 5).

**Resposta correcta:** "15 NO és divisible per 6 perquè, tot i ser divisible per 3, no és divisible per 2."

---

## 📌 Part 8: Problemes Aplicats de Divisibilitat — SOLUCIONS

### 8.1 Distribució Equitativa

**Problema 1:** Tens 48 caramels i els vols distribuir entre grups iguals.

| Pregunta | Resposta | Per què? |
|----------|----------|---------|
| Pots fer 2 grups? | **SÍ** | 48 acaba en 8 (parell). 48÷2 = 24 ✓ |
| Pots fer 3 grups? | **SÍ** | 4+8 = 12 (múltiple de 3). 48÷3 = 16 ✓ |
| Pots fer 4 grups? | **SÍ** | Últims 2 dígits: 48÷4 = 12. 48÷4 = 12 ✓ |
| Pots fer 5 grups? | **NO** | 48 no acaba en 0 ni 5. 48÷5 = 9.6 ✗ |

---

**Problema 2:** Tens 126 estudiants per a una activitat.

| Pregunta | Resposta | Comprovació |
|----------|----------|-----------|
| Pots fer 6 grups iguals? | **SÍ** | Divisible per 2? **SÍ** (acaba en 6). Divisible per 3? **SÍ** (1+2+6=9). Conclusió: **Sí, 126÷6 = 21** |
| Quants estudiants per grup? | **21** | 126 ÷ 6 = 21 |

---

### 8.2 Supermercat i Codis de Barres

**Problema:** Un codi termina en 5. Per a ser vàlid, ha de passar la prova de divisibilitat per 5.

- El codi: 123456789**5**
- Es divisible per 5? **SÍ** Per què? **Acaba en 5** (la regla per a divisibilitat per 5 és que acabi en 0 o 5) ✓

---

## 📌 Part 9: Repte — Problemes de Lògica — SOLUCIONS

### 9.1 Pensa Críticament

**Pregunta 1:** Si un nombre és divisible per 9, és SEMPRE divisible per 3?

**Resposta:** **SÍ, SEMPRE.** Perquè 9 = 3 × 3. Si la suma de dígits és múltiple de 9, aleshores és múltiple de 3. Per exemple: 99 és divisible per 9 (9+9=18÷9=2). 99 és divisible per 3 (18÷3=6). **La regla:** Si divisor més gran (9) divideix un nombre, aleshores els seus factors (3) també el dividixen.

---

**Pregunta 2:** Si un nombre és divisible per 6, quins dos nombres el dividen NECESSÀRIAMENT?

**Resposta:** **2 i 3.** Perquè 6 = 2 × 3. Per a ser divisible per 6, ha de ser divisible tant per 2 (acaba en parell) com per 3 (suma de dígits múltiple de 3).

---

**Pregunta 3:** Troча un nombre de 4 dígits que sigui divisible per 2, 3, i 5.

**Exemple vàlid:** **1,230**

**Comprovació:**
- Divisible per 2? **SÍ** (acaba en 0, que és parell) ✓
- Divisible per 3? **SÍ** (1+2+3+0 = 6, múltiple de 3) ✓
- Divisible per 5? **SÍ** (acaba en 0) ✓

**Altres exemples:** 1,200, 1,320, 2,010, 3,000, etc. (tots acaben en 0 i la suma de dígits és múltiple de 3)

---

### 9.2 Identifica el Patró

Estudia: **6, 12, 18, 24, 30, 36, 42, ...**

| Pregunta | Resposta |
|----------|----------|
| Quin és el patró? | **Cada nombre és 6 més que l'anterior** (o "múltiples de 6") |
| Quin serà el següent? | **48** (42 + 6 = 48) |
| El 100 és en aquesta seqüència? | **NO** (100 ÷ 6 = 16.67..., no és enter) |
| Per què no? | Perquè 100 no és múltiple de 6. No passa la prova de divisibilitat per 6 (acaba en 0, divisible per 2, però 1+0+0=1, no divisible per 3). |

---

## 📌 Part 10: Crea els Teus Exercicis — SOLUCIONS (EXEMPLAR)

### 10.1 Crea 3 Exercicis de Divisibilitat

**Exemple d'Exercici 1** (per 2, 3, o 5):

"El nombre **246** és divisible per **2** perquè **acaba en 6, que és un dígit parell**"

(Altres opcions: per 3 perquè 2+4+6=12, múltiple de 3)

---

**Exemple d'Exercici 2** (per 4, 6, o 9):

"El nombre **324** és divisible per **6** perquè **és divisible tant per 2 (acaba en 4) com per 3 (3+2+4=9)**"

---

**Exemple d'Exercici 3** (Problema aplicat):

"Si tens **60** caramels i els distribuïxes entre **5** grups, quantes coses per grup? **12 caramels per grup**"

---

### 10.2 Reflexió

**Pregunta 1:** Quina regla de divisibilitat és la més fàcil d'usar? Per què?

**Resposta:** **La regla del 2 (mirar l'últim dígit)** és molt simple i ràpida. Només cal veure si acaba en parell.

(Altres respostes vàlides: 5 también és simple per la mateixa raó)

---

**Pregunta 2:** Com ha ajudat la divisibilitat en un problema real?

**Resposta:** **En distribuir els caramels equitativament entre grups, la divisibilitat et permet saber ràpidament si es pot fer sense deixar caramels sense repartir.**

(Altres: códis de barres, distribució de classes, etc.)

---

## 🎯 Claus del Bloc 6

| Regla | Prova Ràpida |
|-------|-------------|
| **Divisibilitat per 2** | Últim dígit parell (0, 2, 4, 6, 8) |
| **Divisibilitat per 3** | Suma de dígits múltiple de 3 |
| **Divisibilitat per 4** | Últims 2 dígits divisibles per 4 |
| **Divisibilitat per 5** | Últim dígit 0 o 5 |
| **Divisibilitat per 6** | Divisible per 2 **I** per 3 |
| **Divisibilitat per 9** | Suma de dígits múltiple de 9 |

---

## 📊 Resumen de Respostes Correctes

**Part 1:** Comprensió de les definicions i verificació de divisibilitat.
**Part 2-7:** Aplicació correcta de cada regla de divisibilitat.
**Part 8:** Resolució de problemes aplicats usant les regles.
**Part 9:** Pensament crític sobre patrons i excepcions.
**Part 10:** Creació de problemes propis i reflexió sobre l'aprenentatge.

---

**Felicitats! Has completat Bloc 6. Ara dominas les regles de divisibilitat!** 🌟

Les regles de divisibilitat són eines poderoses que els matemàtics, els comerciants i els sistemes informàtics usan cada dia!


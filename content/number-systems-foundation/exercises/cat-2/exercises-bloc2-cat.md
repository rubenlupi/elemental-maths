# Exercicis Bloc 2 – Subconjunts i Diagrames de Venn

---

## 📌 Part 1: Introducció a Subconjunts

Identifica si les afirmacions són correctes.

**Exemple:** A = {1, 2}, B = {1, 2, 3} → A ⊆ B? **SÍ**, perquè 1 i 2 estan en B.

---

### 1.1 Relacions Bàsiques

Completa amb **⊆** (és subconjunt) o **⊄** (no és subconjunt):

| A | B | Relació | Correcte? |
|---|---|---------|-----------|
| {1, 2} | {1, 2, 3} | A ___ B | |
| {a, b, c} | {a, c} | A ___ B | |
| {5} | {1, 2, 3, 4, 5} | A ___ B | |
| {gat, gos} | {gat, gos, peix} | A ___ B | |
| {1, 2} | {2, 3, 4} | A ___ B | |
| ∅ | {1, 2, 3} | A ___ B | |

---

### 1.2 Subconjunt Propi vs Subconjunt

Usa **⊂** (subconjunt propi) o **⊆** (subconjunt):

| A | B | Simbol | Explicació |
|---|---|--------|-----------|
| {1, 2} | {1, 2, 3} | | |
| {1, 2, 3} | {1, 2, 3} | | |
| {a} | {a, b, c} | | |
| {red, blue} | {red, blue} | | |

---

## 📌 Part 2: Casos Especials

### 2.1 Conjunt Buit

Marca V (Vertader) o F (Fals):

| Afirmació | V/F | Explicació (si és fals) |
|-----------|-----|------------------------|
| ∅ ⊆ {1, 2, 3} | | |
| ∅ ⊂ {a, b} | | |
| ∅ ⊆ ∅ | | |
| {∅} = ∅ | | |
| \|\∅\| = 0 | | |

---

### 2.2 Reflexivitat (Un conjunt és subconjunt de si mateix)

Marca V o F:

| Afirmació | V/F |
|-----------|-----|
| {1, 2} ⊆ {1, 2} | |
| {a, b, c} ⊂ {a, b, c} | |
| A ⊆ A (per a qualsevol A) | |

---

## 📌 Part 3: Comptatge de Subconjunts

Un conjunt amb **n elements** té exactament **2^n subconjunts**.

### 3.1 Calcula

| Conjunt | Elements | 2^n | Subconjunts |
|---------|----------|-----|-----------|
| {1} | 1 | | |
| {a, b} | 2 | | |
| {1, 2, 3} | 3 | | |
| {x, y, z, w} | 4 | | |

---

### 3.2 Enumera tots els Subconjunts

Per al conjunt **A = {1, 2}**, enumera tots els subconjunts (inclou ∅ i el conjunt sencer):

Subconjunts: ___, ___, ___, ___

(Total: ___?)

---

Per al conjunt **B = {a, b, c}**, enumera tots els subconjunts:

Subconjunts: ___, ___, ___, ___, ___, ___, ___, ___

(Total: ___?)

---

## 📌 Part 4: Diagrames de Venn

### 4.1 Interpreta Diagrames

Sigui A = {1, 2, 3} i B = {2, 3, 4, 5}.

Dibuixa un diagrama de Venn amb dos cercles:
- Cercle A (gos): 1, 2, 3
- Cercle B (gat): 2, 3, 4, 5

Escriu:
1. Què està DINS d'A? _______________
2. Què està DINS de B? _______________
3. Què està en TOTS DOS (intersecció)? _______________
4. Què està FORA de tots dos? _______________

---

### 4.2 Interpreta el Diagrama Donat

Sigui el diagrama:

```
    ____________________
   /                    \
  /         B            \
 /  _________________    \
|  /                 \    |
| /        A          \   |
| | 1      2,3    4   |   |
| \                 /  5  |
|  \_________________/    |
 \                        /
  \____________________/
```

Identifica:
- Elements només en A: _______________
- Elements només en B: _______________
- Elements en A i B: _______________
- Elements fora de tots dos: _______________

---

### 4.3 Crea el Teu Diagrama de Venn

Dibuixa un diagrama de Venn per:
- A = {fruites: poma, plàtan, taronja}
- B = {colors: vermell, groc, taronja}

Etiqueta les regions.

---

## 📌 Part 5: Transitivitat

Si A ⊆ B i B ⊆ C, aleshores A ⊆ C.

### 5.1 Verifica la Transitivitat

Completa les afirmacions:

| A | B | C | A ⊆ B? | B ⊆ C? | A ⊆ C? | Transitivitat es compleix? |
|---|---|---|--------|--------|--------|---------------------------|
| {1} | {1, 2} | {1, 2, 3} | | | | |
| {a} | {a, b} | {a, b, c} | | | | |
| {5} | {1, 2, 5} | {1, 2, 3, 4, 5} | | | | |

---

### 5.2 Crea una Cadena de Subconjunts

Crea una cadena on A ⊂ B ⊂ C ⊂ D:

- D (conjunt més gran): _______________
- C: _______________
- B: _______________
- A (conjunt més petit): _______________

---

## 📌 Part 6: Aplicacions Reals

### 6.1 Jerarquies de la Vida Real

Completa les cadenes de subconjunts amb ⊆:

| Cadena | Escriu amb ⊆ |
|--------|-------------|
| Gats ⊆ Felins ⊆ Mamífers ⊆ Animals | |
| Quadrats ⊆ Rectangles ⊆ ? | |
| Telèfons intel·ligents ⊆ ? ⊆ Electrodomèstics | |
| Divendres ⊆ ? ⊆ Temps | |

---

### 6.2 Organització de Dades

Una empresa té empleats. Classifica:

- **Empleats totals:** 100
- **Gerents:** 10
- **Programadors:** 30
- **Gerents que són programadors:** 2

Preguntes:
1. Els gerents ⊆ Empleats? (V/F) ___
2. Els programadors ⊆ Empleats? (V/F) ___
3. Els gerents-programadors ⊆ Gerents? (V/F) ___
4. Els gerents-programadors ⊆ Programadors? (V/F) ___

---

## 📌 Part 7: Propietats de Subconjunts

### 7.1 Marca V o F

| Afirmació | V/F | Si és F, dona un contraexemple |
|-----------|-----|---------|
| Si A ⊂ B, aleshores A ⊆ B | | |
| Si A ⊆ B i B ⊆ A, aleshores A = B | | |
| Si A ⊆ B i A ⊆ C, aleshores A ⊆ (B ∩ C) | | |
| Tot conjunt és subconjunt de si mateix | | |

---

### 7.2 Completa la Definició

- Un subconjunt propi A ⊂ B significa: _____________________________
- El conjunt buit ∅ és subconjunt de: _____________________________
- La reflexivitat significa: _____________________________

---

## 📌 Part 8: Repte — Problemes de Lògica

### 8.1 Pensar Críticament

**Pregunta 1:** Si A ⊂ B ⊂ C, quina és la relació entre A i C?

**Resposta:** _______________

---

**Pregunta 2:** Quants subconjunts propis té un conjunt de 4 elements?

Ajuda: El conjunt sencer no és propi, però el buit sí.

**Resposta:** ___ (Fórmula: 2^n − 1 si excloem el conjunt sencer, o 2^n − 1 si excloem el propi)

---

**Pregunta 3:** Per a quins conjunts A és cert que A ⊂ A?

**Resposta:** _______________

---

### 8.2 Paradoxa del Conjunt Buit

El conjunt buit ∅ pot semblar estrany:
- ∅ ⊆ ∅? (sí o no?) ___
- ∅ ⊂ ∅? (sí o no?) ___
- Per què?

---

## 📌 Part 9: Casos Combinats

### 9.1 Diagrames de Venn + Subconjunts

Sigui A = {1, 2, 3}, B = {2, 3}, C = {2}.

Identifica les relacions:
- C ___ B ___ A (omple amb ⊆ o ⊂)
- Verifica: C ⊆ B ⊆ A? (V/F) ___

---

### 9.2 Jerarquies de Números

Recordem: ℕ ⊂ ℤ ⊂ ℚ (naturals ⊂ enters ⊂ racionals)

Marca V o F:

| Afirmació | V/F |
|-----------|-----|
| 5 ∈ ℕ, 5 ∈ ℤ, 5 ∈ ℚ | |
| -3 ∈ ℕ | |
| 1/2 ∈ ℤ | |
| 1/2 ∈ ℚ | |
| ℕ ⊆ ℚ (tots els naturals són racionals)? | |

---

## 📌 Part 10: Crea els Teus Conjunts

### 10.1 Dibuixa Diagrames de Venn

Crea 2 diagrames de Venn amb:

**Diagrama 1:**
- Conjunt A: ___________
- Conjunt B: ___________
- (Dibuixa els cercles i etiqueta)

---

**Diagrama 2:**
- Conjunt X: ___________
- Conjunt Y: ___________
- (Dibuixa els cercles i etiqueta)

---

### 10.2 Crea Cadenes de Subconjunts

Crea 2 cadenes de subconjunts:

**Cadena 1:** A ⊂ B ⊂ C
- A = ___________
- B = ___________
- C = ___________

---

**Cadena 2:** X ⊂ Y ⊂ Z
- X = ___________
- Y = ___________
- Z = ___________

---

## 🎯 Autoavaluació

Marca quines parts vas respondre correctament:

- [ ] Part 1 (Introducció): ✓
- [ ] Part 2 (Casos Especials): ✓
- [ ] Part 3 (Comptatge): ✓
- [ ] Part 4 (Diagrames de Venn): ✓
- [ ] Part 5 (Transitivitat): ✓
- [ ] Part 6 (Aplicacions): ✓
- [ ] Part 7 (Propietats): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Casos Combinats): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, domines Bloc 2! 🎉

---

**Bona sort! Recorda: els diagrames de Venn són la millor forma de veure subconjunts!** 🎓


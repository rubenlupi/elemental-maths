# Exercicis Bloc 2.5 – Operacions de Conjunts i Cardinalitat

---

## 📌 Part 1: Cardinalitat Bàsica

Compte els elements i escriu la cardinalitat de cada conjunt.

**Exemple:** A = {poma, pera, plàtan} → |A| = 3

---

### 1.1 Conjunts Simples

| Conjunt | Cardinalitat |
|---------|--------------|
| A = {1, 2, 3, 4, 5} | |
| B = {gat, gos} | |
| C = ∅ (conjunt buit) | |
| D = {7} | |
| E = {a, b, c, d, e, f} | |
| F = {10, 20, 30, 40} | |

---

### 1.2 Cardinalitat Implícita

Quants elements té cada conjunt?

| Conjunt | Cardinalitat |
|---------|--------------|
| G = {nombres parells entre 1 i 10} | |
| H = {vocals de "elemental"} | |
| I = {mesos de l'any} | |
| J = {dies de la setmana que comencen amb "d"} | |

---

## 📌 Part 2: Unió (A ∪ B)

Calcula la unió i la seva cardinalitat.

**Exemple:** A = {1, 2, 3}, B = {2, 3, 4} → A ∪ B = {1, 2, 3, 4}, |A ∪ B| = 4

---

### 2.1 Unió Simple

| A | B | A ∪ B | \|A ∪ B\| |
|---|---|-------|----------|
| {1, 2} | {3, 4} | | |
| {a, b, c} | {b, c, d} | | |
| {5, 10} | {5, 10} | | |
| {gat} | {gos, conill} | | |
| {1, 3, 5} | {2, 4, 6} | | |

---

### 2.2 Usa la Fórmula: \|A ∪ B\| = \|A\| + \|B\| − \|A ∩ B\|

Calcula la cardinalitat sense enumerar tots els elements:

| \|A\| | \|B\| | \|A ∩ B\| | \|A ∪ B\| |
|-------|-------|----------|----------|
| 5 | 3 | 1 | |
| 10 | 7 | 4 | |
| 6 | 6 | 2 | |
| 8 | 5 | 0 | |
| 4 | 4 | 4 | |

---

## 📌 Part 3: Intersecció (A ∩ B)

Calcula la intersecció i la seva cardinalitat.

**Exemple:** A = {1, 2, 3}, B = {2, 3, 4} → A ∩ B = {2, 3}, |A ∩ B| = 2

---

### 3.1 Intersecció Simple

| A | B | A ∩ B | \|A ∩ B\| |
|---|---|-------|----------|
| {1, 2, 3} | {2, 3, 4} | | |
| {a, e, i, o, u} | {a, b, c} | | |
| {gat, gos} | {gat, gos} | | |
| {1, 2} | {3, 4} | | |
| {5, 10, 15} | {10, 15, 20} | | |

---

### 3.2 Interpreta els Casos

Completa la taula:

| A | B | Cas | A ∩ B |
|---|---|-----|-------|
| {1, 2, 3} | {1, 2, 3} | Idèntics | |
| {1, 2} | {3, 4} | Disjunts (sense elements comuns) | |
| {1, 2, 3} | {2, 3, 4, 5} | Parcialment comuns | |
| {1} | {1, 2, 3, 4} | Subconjunt | |

---

## 📌 Part 4: Diferència (A − B)

Calcula la diferència i la seva cardinalitat.

**Exemple:** A = {1, 2, 3, 4}, B = {2, 4, 5} → A − B = {1, 3}, |A − B| = 2

---

### 4.1 Diferència Simple

| A | B | A − B | \|A − B\| |
|---|---|-------|----------|
| {1, 2, 3, 4} | {2, 4} | | |
| {a, b, c, d} | {b, d} | | |
| {1, 2, 3} | {1, 2, 3} | | |
| {5, 6, 7} | {1, 2, 3} | | |
| {gat, gos, peix} | {gos} | | |

---

### 4.2 Diferència Inversa (B − A)

Per als mateixos pairs, calcula B − A. Observa com difereix de A − B!

| A | B | B − A | A − B | Són iguals? |
|---|---|-------|-------|----------|
| {1, 2} | {2, 3} | | | |
| {a, b} | {a, b, c} | | | |
| {5} | {1, 2} | | | |

---

### 4.3 Usa la Fórmula: \|A − B\| = \|A\| − \|A ∩ B\|

| \|A\| | \|A ∩ B\| | \|A − B\| |
|-------|----------|----------|
| 7 | 3 | |
| 5 | 0 | |
| 10 | 4 | |
| 6 | 6 | |

---

## 📌 Part 5: Complemento (A^c)

Calcula el complemento d'un conjunt respecte a un univers U.

**Exemple:** U = {1, 2, 3, 4, 5}, A = {1, 3, 5} → A^c = {2, 4}, |A^c| = 2

---

### 5.1 Complemento Simple

| U (Univers) | A | A^c | \|A^c\| |
|----------|---|-----|---------|
| {1, 2, 3, 4, 5} | {1, 3} | | |
| {a, e, i, o, u} | {a, e} | | |
| {1, 2, 3, 4} | {1, 2, 3, 4} | | |
| {Mon, Tue, Wed, Thu, Fri} | {Mon, Fri} | | |
| {1, 2, 3, 4, 5, 6} | ∅ | | |

---

### 5.2 Usa la Fórmula: \|A^c\| = \|U\| − \|A\|

| \|U\| | \|A\| | \|A^c\| |
|-------|-------|---------|
| 10 | 3 | |
| 8 | 8 | |
| 15 | 6 | |
| 20 | 12 | |

---

## 📌 Part 6: Diferència Simètrica (A Δ B)

La diferència simètrica inclou elements que estan en A o en B, però **NO en ambdós**.

**Exemple:** A = {1, 2, 3}, B = {2, 3, 4} → A Δ B = {1, 4}, |A Δ B| = 2

---

### 6.1 Diferència Simètrica Simple

| A | B | A Δ B | \|A Δ B\| |
|---|---|-------|----------|
| {1, 2, 3} | {2, 3, 4} | | |
| {a, b} | {a, b} | | |
| {1, 2} | {3, 4} | | |
| {gat, gos, peix} | {gos, ocell} | | |
| {1} | {1, 2, 3} | | |

---

### 6.2 Relació amb Diferència Ordinària

Recorda: **A Δ B = (A − B) ∪ (B − A)**

Verifica aquesta relació amb els exemples anteriors. Completa la taula:

| A | B | A − B | B − A | (A − B) ∪ (B − A) | A Δ B | Coincideix? |
|---|---|-------|-------|------------------|-------|-----------|
| {1, 2} | {2, 3} | | | | | |
| {a, b, c} | {b, c, d} | | | | | |

---

## 📌 Part 7: Operacions Combinades

Calcula operacions més complexes en ordre.

---

### 7.1 Dos Passos

**Exemple:** A = {1, 2, 3}, B = {2, 3, 4}, C = {3, 4, 5}

Calcula:
1. (A ∪ B) ∩ C
2. A ∩ (B ∪ C)
3. (A − B) ∪ (B − A)

---

### 7.2 Amb Complemento

Sigui U = {1, 2, 3, 4, 5, 6}, A = {1, 2, 3}, B = {3, 4, 5}.

Calcula:
1. A^c
2. B^c
3. (A ∪ B)^c
4. A^c ∩ B^c
5. Compara (A ∪ B)^c i A^c ∩ B^c. Són iguals? (Llei de De Morgan)

---

## 📌 Part 8: Problemes Reals

### 8.1 Enquesta de Preferències

En una classe de 20 nens:
- 12 prefereixen pizza
- 8 prefereixen hamburguesa
- 3 prefereixen ambdós

Calcula:
1. Quants prefereixen pizza o hamburguesa? (usa la fórmula de la unió)
2. Quants prefereixen només pizza?
3. Quants prefereixen només hamburguesa?
4. Quants NO prefereixen ni pizza ni hamburguesa?

---

### 8.2 Biblioteca

Una biblioteca té:
- 150 llibres de ficció
- 100 llibres de no-ficció
- 30 llibres que són ambdós (per ex., novel·les históriques)

Calcula:
1. Quants llibres són ficció O no-ficció?
2. Quants llibres són NOMÉS ficció?
3. Si la biblioteca té 500 llibres totals, quants no són ficció ni no-ficció (altres categories)?

---

### 8.3 Xarxes Socials

Dels 100 estudiants:
- 60 usen Instagram
- 50 usen TikTok
- 25 usen ambdós

Calcula:
1. Quants usen Instagram o TikTok?
2. Quants usen només Instagram?
3. Quants NO usen ni Instagram ni TikTok?

---

## 📌 Part 9: Repte — Problemes de Lògica

### 9.1 Lleis de De Morgan

**Llei 1:** (A ∪ B)^c = A^c ∩ B^c
**Llei 2:** (A ∩ B)^c = A^c ∪ B^c

Verifica aquestes lleis amb:
- U = {1, 2, 3, 4, 5}
- A = {1, 2, 3}
- B = {2, 3, 4}

Completa:
1. A ∪ B = ___
2. (A ∪ B)^c = ___
3. A^c = ___
4. B^c = ___
5. A^c ∩ B^c = ___
6. Compara: (A ∪ B)^c = A^c ∩ B^c? ✓ o ✗

---

### 9.2 Propietats Comutatives

Completa la taula. Si dues operacions donen el mateix resultat, són commutatives (A op B = B op A).

| Operació | A | B | A op B | B op A | Commutativa? |
|----------|---|---|--------|--------|-------------|
| Unió (∪) | {1,2} | {2,3} | | | |
| Intersecció (∩) | {1,2} | {2,3} | | | |
| Diferència (−) | {1,2} | {2,3} | | | |

---

### 9.3 Pensar Críticament

**Pregunta 1:** Per a quins casos és (**A ∪ B) ∩ C = A ∪ (B ∩ C)**?
- Sempre? Només de vegades? Mai?

Dona un exemple o contraexemple.

---

**Pregunta 2:** Si A ⊂ B, quina és la diferència A − B?

---

**Pregunta 3:** Si A ∩ B = ∅ (els conjunts són disjunts), quina és |A ∪ B|?

---

## 📌 Part 10: Crea els Teus Problemes

Crea tres problemes de conjunts (similar als de Part 8):

1. **Problema 1 (amb Unió):**

   Enunciat: ___________________________
   
   Pregunta: ___________________________
   
   Solució: ___________________________

---

2. **Problema 2 (amb Diferència):**

   Enunciat: ___________________________
   
   Pregunta: ___________________________
   
   Solució: ___________________________

---

3. **Problema 3 (combinat):**

   Enunciat: ___________________________
   
   Pregunta: ___________________________
   
   Solució: ___________________________

---

## 🎯 Autoavaluació

Marca quines parts vas respondre correctament:

- [ ] Part 1 (Cardinalitat): ✓
- [ ] Part 2 (Unió): ✓
- [ ] Part 3 (Intersecció): ✓
- [ ] Part 4 (Diferència): ✓
- [ ] Part 5 (Complemento): ✓
- [ ] Part 6 (Diferència Simètrica): ✓
- [ ] Part 7 (Operacions Combinades): ✓
- [ ] Part 8 (Problemes Reals): ✓
- [ ] Part 9 (Repte): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, domines Bloc 2.5! 🎉

---

**Bona sort! Recorda: les operacions de conjunts són com "combinar", "trobar comunes" i "separar" grups!** 🎓


# Solucions Bloc 2.5 – Operacions de Conjunts i Cardinalitat

---

## 📌 Part 1: Cardinalitat Bàsica

### 1.1 Conjunts Simples

| Conjunt | Cardinalitat |
|---------|--------------|
| A = {1, 2, 3, 4, 5} | **5** |
| B = {gat, gos} | **2** |
| C = ∅ (conjunt buit) | **0** |
| D = {7} | **1** |
| E = {a, b, c, d, e, f} | **6** |
| F = {10, 20, 30, 40} | **4** |

---

### 1.2 Cardinalitat Implícita

| Conjunt | Cardinalitat | Explicació |
|---------|--------------|-----------|
| G = {nombres parells entre 1 i 10} | **5** | {2, 4, 6, 8, 10} |
| H = {vocals de "elemental"} | **3** | {e, a} (e apareix dues vegades però es compta una) |
| I = {mesos de l'any} | **12** | Gener, febrer, ..., desembre |
| J = {dies de la setmana que comencen amb "d"} | **2** | {dilluns, dimecres} o {dilluns, dimarts, dimecres} depenent de l'idioma |

---

## 📌 Part 2: Unió (A ∪ B)

### 2.1 Unió Simple

| A | B | A ∪ B | \|A ∪ B\| |
|---|---|-------|----------|
| {1, 2} | {3, 4} | **{1, 2, 3, 4}** | **4** |
| {a, b, c} | {b, c, d} | **{a, b, c, d}** | **4** |
| {5, 10} | {5, 10} | **{5, 10}** | **2** |
| {gat} | {gos, conill} | **{gat, gos, conill}** | **3** |
| {1, 3, 5} | {2, 4, 6} | **{1, 2, 3, 4, 5, 6}** | **6** |

---

### 2.2 Usa la Fórmula: \|A ∪ B\| = \|A\| + \|B\| − \|A ∩ B\|

| \|A\| | \|B\| | \|A ∩ B\| | \|A ∪ B\| | Càlcul |
|-------|-------|----------|----------|--------|
| 5 | 3 | 1 | **7** | 5 + 3 − 1 = 7 |
| 10 | 7 | 4 | **13** | 10 + 7 − 4 = 13 |
| 6 | 6 | 2 | **10** | 6 + 6 − 2 = 10 |
| 8 | 5 | 0 | **13** | 8 + 5 − 0 = 13 |
| 4 | 4 | 4 | **4** | 4 + 4 − 4 = 4 (A = B) |

---

## 📌 Part 3: Intersecció (A ∩ B)

### 3.1 Intersecció Simple

| A | B | A ∩ B | \|A ∩ B\| |
|---|---|-------|----------|
| {1, 2, 3} | {2, 3, 4} | **{2, 3}** | **2** |
| {a, e, i, o, u} | {a, b, c} | **{a}** | **1** |
| {gat, gos} | {gat, gos} | **{gat, gos}** | **2** |
| {1, 2} | {3, 4} | **∅** | **0** |
| {5, 10, 15} | {10, 15, 20} | **{10, 15}** | **2** |

---

### 3.2 Interpreta els Casos

| A | B | Cas | A ∩ B |
|---|---|-----|-------|
| {1, 2, 3} | {1, 2, 3} | Idèntics | **{1, 2, 3}** (tots els elements) |
| {1, 2} | {3, 4} | Disjunts (sense elements comuns) | **∅** (cap element) |
| {1, 2, 3} | {2, 3, 4, 5} | Parcialment comuns | **{2, 3}** (només els comuns) |
| {1} | {1, 2, 3, 4} | Subconjunt | **{1}** (l'element del conjunt menor) |

---

## 📌 Part 4: Diferència (A − B)

### 4.1 Diferència Simple

| A | B | A − B | \|A − B\| |
|---|---|-------|----------|
| {1, 2, 3, 4} | {2, 4} | **{1, 3}** | **2** |
| {a, b, c, d} | {b, d} | **{a, c}** | **2** |
| {1, 2, 3} | {1, 2, 3} | **∅** | **0** |
| {5, 6, 7} | {1, 2, 3} | **{5, 6, 7}** | **3** |
| {gat, gos, peix} | {gos} | **{gat, peix}** | **2** |

---

### 4.2 Diferència Inversa (B − A)

| A | B | B − A | A − B | Són iguals? |
|---|---|-------|-------|----------|
| {1, 2} | {2, 3} | **{3}** | **{1}** | **NO** |
| {a, b} | {a, b, c} | **{c}** | **∅** | **NO** |
| {5} | {1, 2} | **{1, 2}** | **{5}** | **NO** |

**Conclusió:** La diferència NO és commutativa! A − B ≠ B − A (en general).

---

### 4.3 Usa la Fórmula: \|A − B\| = \|A\| − \|A ∩ B\|

| \|A\| | \|A ∩ B\| | \|A − B\| | Càlcul |
|-------|----------|----------|--------|
| 7 | 3 | **4** | 7 − 3 = 4 |
| 5 | 0 | **5** | 5 − 0 = 5 (cap element comú) |
| 10 | 4 | **6** | 10 − 4 = 6 |
| 6 | 6 | **0** | 6 − 6 = 0 (A ⊆ B) |

---

## 📌 Part 5: Complemento (A^c)

### 5.1 Complemento Simple

| U (Univers) | A | A^c | \|A^c\| |
|----------|---|-----|---------|
| {1, 2, 3, 4, 5} | {1, 3} | **{2, 4, 5}** | **3** |
| {a, e, i, o, u} | {a, e} | **{i, o, u}** | **3** |
| {1, 2, 3, 4} | {1, 2, 3, 4} | **∅** | **0** |
| {Mon, Tue, Wed, Thu, Fri} | {Mon, Fri} | **{Tue, Wed, Thu}** | **3** |
| {1, 2, 3, 4, 5, 6} | ∅ | **{1, 2, 3, 4, 5, 6}** | **6** |

---

### 5.2 Usa la Fórmula: \|A^c\| = \|U\| − \|A\|

| \|U\| | \|A\| | \|A^c\| | Càlcul |
|-------|-------|---------|--------|
| 10 | 3 | **7** | 10 − 3 = 7 |
| 8 | 8 | **0** | 8 − 8 = 0 (A = U) |
| 15 | 6 | **9** | 15 − 6 = 9 |
| 20 | 12 | **8** | 20 − 12 = 8 |

---

## 📌 Part 6: Diferència Simètrica (A Δ B)

### 6.1 Diferència Simètrica Simple

| A | B | A Δ B | \|A Δ B\| | Explicació |
|---|---|-------|----------|-----------|
| {1, 2, 3} | {2, 3, 4} | **{1, 4}** | **2** | 1 només en A, 4 només en B |
| {a, b} | {a, b} | **∅** | **0** | Cap element diferent |
| {1, 2} | {3, 4} | **{1, 2, 3, 4}** | **4** | Tots són diferent (disjunts) |
| {gat, gos, peix} | {gos, ocell} | **{gat, peix, ocell}** | **3** | Només gos és comú |
| {1} | {1, 2, 3} | **{2, 3}** | **2** | 2 i 3 només en B |

---

### 6.2 Relació amb Diferència Ordinària

**Recorda:** A Δ B = (A − B) ∪ (B − A)

| A | B | A − B | B − A | (A − B) ∪ (B − A) | A Δ B | Coincideix? |
|---|---|-------|-------|------------------|-------|-----------|
| {1, 2} | {2, 3} | {1} | {3} | {1, 3} | {1, 3} | ✓ **SÍ** |
| {a, b, c} | {b, c, d} | {a} | {d} | {a, d} | {a, d} | ✓ **SÍ** |

---

## 📌 Part 7: Operacions Combinades

### 7.1 Dos Passos

**Donnats:** A = {1, 2, 3}, B = {2, 3, 4}, C = {3, 4, 5}

**1. (A ∪ B) ∩ C**

- A ∪ B = {1, 2, 3} ∪ {2, 3, 4} = {1, 2, 3, 4}
- (A ∪ B) ∩ C = {1, 2, 3, 4} ∩ {3, 4, 5} = **{3, 4}**

---

**2. A ∩ (B ∪ C)**

- B ∪ C = {2, 3, 4} ∪ {3, 4, 5} = {2, 3, 4, 5}
- A ∩ (B ∪ C) = {1, 2, 3} ∩ {2, 3, 4, 5} = **{2, 3}**

---

**3. (A − B) ∪ (B − A)**

- A − B = {1, 2, 3} − {2, 3, 4} = {1}
- B − A = {2, 3, 4} − {1, 2, 3} = {4}
- (A − B) ∪ (B − A) = {1} ∪ {4} = **{1, 4}** (diferència simètrica!)

---

### 7.2 Amb Complemento

**Donnats:** U = {1, 2, 3, 4, 5, 6}, A = {1, 2, 3}, B = {3, 4, 5}

**1. A^c**

A^c = U − A = {1, 2, 3, 4, 5, 6} − {1, 2, 3} = **{4, 5, 6}**

---

**2. B^c**

B^c = U − B = {1, 2, 3, 4, 5, 6} − {3, 4, 5} = **{1, 2, 6}**

---

**3. (A ∪ B)^c**

- A ∪ B = {1, 2, 3} ∪ {3, 4, 5} = {1, 2, 3, 4, 5}
- (A ∪ B)^c = U − (A ∪ B) = {1, 2, 3, 4, 5, 6} − {1, 2, 3, 4, 5} = **{6}**

---

**4. A^c ∩ B^c**

A^c ∩ B^c = {4, 5, 6} ∩ {1, 2, 6} = **{6}**

---

**5. Compara (A ∪ B)^c i A^c ∩ B^c**

- (A ∪ B)^c = {6}
- A^c ∩ B^c = {6}

**Són iguals? ✓ SÍ!**

**Conclusió:** Aquesta és la **Llei de De Morgan: (A ∪ B)^c = A^c ∩ B^c**

---

## 📌 Part 8: Problemes Reals

### 8.1 Enquesta de Preferències

**Donnats:**
- Total: 20 nens
- Pizza: 12
- Hamburguesa: 8
- Ambdós: 3

**Calcula:**

**1. Quants prefereixen pizza o hamburguesa?** (usa la fórmula de la unió)

|Pizza ∪ Hamburguesa| = |Pizza| + |Hamburguesa| − |Pizza ∩ Hamburguesa|
= 12 + 8 − 3 = **17 nens**

---

**2. Quants prefereixen només pizza?**

|Pizza − Hamburguesa| = |Pizza| − |Pizza ∩ Hamburguesa|
= 12 − 3 = **9 nens**

---

**3. Quants prefereixen només hamburguesa?**

|Hamburguesa − Pizza| = |Hamburguesa| − |Pizza ∩ Hamburguesa|
= 8 − 3 = **5 nens**

---

**4. Quants NO prefereixen ni pizza ni hamburguesa?**

Univers − (Pizza ∪ Hamburguesa) = 20 − 17 = **3 nens**

---

### 8.2 Biblioteca

**Donnats:**
- Ficció: 150
- No-ficció: 100
- Ambdós: 30
- Total de llibres: 500

**Calcula:**

**1. Quants llibres són ficció O no-ficció?**

|Ficció ∪ No-ficció| = 150 + 100 − 30 = **220 llibres**

---

**2. Quants llibres són NOMÉS ficció?**

|Ficció − No-ficció| = 150 − 30 = **120 llibres**

---

**3. Quants no són ficció ni no-ficció (altres categories)?**

Total − (Ficció ∪ No-ficció) = 500 − 220 = **280 llibres**

---

### 8.3 Xarxes Socials

**Donnats:**
- Total: 100 estudiants
- Instagram: 60
- TikTok: 50
- Ambdós: 25

**Calcula:**

**1. Quants usen Instagram o TikTok?**

|Instagram ∪ TikTok| = 60 + 50 − 25 = **85 estudiants**

---

**2. Quants usen només Instagram?**

|Instagram − TikTok| = 60 − 25 = **35 estudiants**

---

**3. Quants NO usen ni Instagram ni TikTok?**

Total − (Instagram ∪ TikTok) = 100 − 85 = **15 estudiants**

---

## 📌 Part 9: Repte — Problemes de Lògica

### 9.1 Lleis de De Morgan

**Donnats:**
- U = {1, 2, 3, 4, 5}
- A = {1, 2, 3}
- B = {2, 3, 4}

**Verifica:** (A ∪ B)^c = A^c ∩ B^c

**Completa:**

1. A ∪ B = **{1, 2, 3, 4}**
2. (A ∪ B)^c = **{5}**
3. A^c = **{4, 5}**
4. B^c = **{1, 5}**
5. A^c ∩ B^c = **{5}**
6. **(A ∪ B)^c = A^c ∩ B^c? ✓ SÍ**

---

### 9.2 Propietats Comutatives

| Operació | A | B | A op B | B op A | Commutativa? |
|----------|---|---|--------|--------|-------------|
| Unió (∪) | {1,2} | {2,3} | {1,2,3} | {1,2,3} | **✓ SÍ** |
| Intersecció (∩) | {1,2} | {2,3} | {2} | {2} | **✓ SÍ** |
| Diferència (−) | {1,2} | {2,3} | {1} | {3} | **✗ NO** |

---

### 9.3 Pensar Críticament

**Pregunta 1:** Per a quins casos és (A ∪ B) ∩ C = A ∪ (B ∩ C)?

**Resposta:** **Només de vegades!** (No sempre, no mai.)

**Contraexemple:** A = {1}, B = {2}, C = {2}
- (A ∪ B) ∩ C = {1, 2} ∩ {2} = {2}
- A ∪ (B ∩ C) = {1} ∪ {2} = {1, 2}
- {2} ≠ {1, 2}, per tant **NO és sempre cert**.

**Cas que SÍ funciona:** Si C ⊆ A.

---

**Pregunta 2:** Si A ⊂ B, quina és la diferència A − B?

**Resposta:** **∅** (el conjunt buit)

**Explicació:** Si tot element de A està en B, aleshores no hi ha cap element en A que no sigui en B.

---

**Pregunta 3:** Si A ∩ B = ∅ (els conjunts són disjunts), quina és |A ∪ B|?

**Resposta:** |A ∪ B| = |A| + |B|

**Explicació:** Si no tenen elements comuns, la unió és simplement la suma de les cardinalitats.

---

## 📌 Part 10: Crea els Teus Problemes

*(Les solucions variaran segons l'estudiant. Aquí hi ha exemples de resposta correcta.)*

---

**1. Problema 1 (amb Unió):**

Enunciat: 
*En un centre de sants, 15 nens practiquen futbol i 10 practiquen baloncest. Si 5 practiquen ambdós, quants nens practiquen ALMENYS un esport?*

Pregunta: *Quants nens practiquen futbol o baloncest (o ambdós)?*

Solució: 
|Futbol ∪ Baloncest| = 15 + 10 − 5 = **20 nens**

---

**2. Problema 2 (amb Diferència):**

Enunciat:
*Una tenda té 100 productes: 60 són roba i 40 són electrodomèstics. Si 15 són ambdós (ex., maniquís amb sensors), quants productes són NOMÉS roba?*

Pregunta: *Quants productes són només roba?*

Solució:
|Roba − Electrodomèstics| = 60 − 15 = **45 productes**

---

**3. Problema 3 (combinat):**

Enunciat:
*Una biblioteca té 500 llibres totals: 200 de ficció, 150 de ciència, i 50 de ficció científica (ambdós). Quants llibres NO són ficció ni ciència?*

Pregunta: *Quants llibres són d'altres categories?*

Solució:
|Ficció ∪ Ciència| = 200 + 150 − 50 = 300
Altres = 500 − 300 = **200 llibres**

---

## 🎯 Autoavaluació

Marca quines parts vas respondre correctament:

- [ ] Part 1 (Cardinalitat): Esperem 10/10
- [ ] Part 2 (Unió): Esperem 13/13
- [ ] Part 3 (Intersecció): Esperem 9/9
- [ ] Part 4 (Diferència): Esperem 10/10
- [ ] Part 5 (Complemento): Esperem 9/9
- [ ] Part 6 (Diferència Simètrica): Esperem 7/7
- [ ] Part 7 (Operacions Combinades): Esperem 6/6
- [ ] Part 8 (Problemes Reals): Esperem 11/11
- [ ] Part 9 (Repte): Esperem 5/5
- [ ] Part 10 (Creació): Autocreació

**Puntuació Esperada:**
- 9/10 parts correctes: **Mestre de Bloc 2.5!** 🎉
- 7/10 parts correctes: **Molt bé! Repassa les parts que fallaren.** 👍
- 5/10 parts correctes: **Bé, però necessites practicar més.** 📚

---

## 📝 Notes Addicionals

**Punts Clau a Recordar:**

1. **Cardinalitat** = nombre d'elements d'un conjunt
2. **Unió (A ∪ B)** = tots els elements (unió-exclusió: no comptar dues vegades)
3. **Intersecció (A ∩ B)** = només els comuns
4. **Diferència (A − B)** = els de A que NO estan en B
5. **Complemento (A^c)** = tot allò que NO és en A (dins d'un univers U)
6. **Diferència Simètrica (A Δ B)** = els que són en un o altre, però no ambdós

**Fórmules Clau:**
- |A ∪ B| = |A| + |B| − |A ∩ B|
- |A − B| = |A| − |A ∩ B|
- |A^c| = |U| − |A|
- A Δ B = (A − B) ∪ (B − A)

**Lleis de De Morgan:**
- (A ∪ B)^c = A^c ∩ B^c
- (A ∩ B)^c = A^c ∪ B^c

---

**Molt bé pels exercicis! Domina les operacions de conjunts!** 🎓


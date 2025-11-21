# Solucions Bloc 1 – Conjunts i Notació Bàsica

---

## 📌 Part 1: Identificar Elements i Pertinença

### 1.1 Pertinença Bàsica

| Conjunt | Pregunta | V/F | Explicació |
|---------|----------|-----|-----------|
| A = {poma, plàtan, taronja} | poma ∈ A? | **V** | poma apareix a la llista |
| B = {1, 2, 3, 4, 5} | 6 ∈ B? | **F** | 6 no està a la llista |
| C = {a, e, i, o, u} | a ∈ C? | **V** | a és una vocal |
| D = {vermell, blau, verd} | groc ∈ D? | **F** | groc no està a la llista |
| E = {cat, dog, bird} | gat ∈ E? | **F** | "gat" en català no apareix (només "cat" en anglès) |
| F = {5, 10, 15, 20} | 12 ∈ F? | **F** | 12 no és múltiple de 5 en aquest conjunt |

---

### 1.2 No Pertinença (∉)

| Conjunt | Element | Símbol | Correcte? | Explicació |
|---------|---------|--------|-----------|-----------|
| {1, 2, 3} | 4 | **∉** | **SÍ** | 4 no pertany al conjunt |
| {a, b, c} | b | **∈** | **SÍ** | b pertany al conjunt |
| {vermell, blau} | groc | **∉** | **SÍ** | groc no pertany |
| {gat, gos, peix} | peix | **∈** | **SÍ** | peix pertany |
| {2, 4, 6, 8} | 5 | **∉** | **SÍ** | 5 és senar, no està |

---

## 📌 Part 2: Escriure Conjunts

### 2.1 Enumera Elements

| Descripció | Conjunt |
|-----------|---------|
| Vocals de l'alfabet catalan | **{a, e, i, o, u}** |
| Nombres parells entre 1 i 10 | **{2, 4, 6, 8, 10}** o **{2, 4, 6, 8}** (depenent si incluïm 10) |
| Colors primaris | **{vermell, groc, blau}** |
| Dies de la setmana que comencen amb "d" | **{dilluns, dimarts, dimecres}** |
| Primeres 3 lletres de l'alfabet | **{a, b, c}** |

---

### 2.2 Usa Notació de Condició

| Descripció | Conjunt |
|-----------|---------|
| Nombres enters entre 0 i 5 | **{n \| n ∈ ℤ, 0 < n < 5}** o **{1, 2, 3, 4}** |
| Vocals | **{x \| x és vocal}** o **{a, e, i, o, u}** |
| Nombres parells | **{n \| n = 2k, k ∈ ℤ}** o **{n \| n és parell}** |

---

## 📌 Part 3: Conjunt Buit i Casos Especials

### 3.1 Vertader o Fals?

| Afirmació | V/F | Explicació |
|-----------|-----|-----------|
| ∅ és un conjunt vàlid | **V** | El conjunt buit és un conjunt perfectament valid |
| \|∅\| = 0 | **V** | El buit té 0 elements |
| {∅} és buit | **F** | {∅} NO és buit; conté 1 element: el conjunt buit |
| {∅} = ∅ | **F** | {∅} és un conjunt que CONTÉ el buit; ∅ NO conté res |
| ∅ és igual a {0} | **F** | ∅ no conté res; {0} conté el nombre zero |
| \|{∅}\| = 1 | **V** | {∅} té 1 element (el buit) |

---

### 3.2 Identifica Conjunts Buits

| Descripció | Resultat |
|-----------|----------|
| Nombres enters entre 0 i 1 | **∅** (no hi ha enters entre 0 i 1) |
| Nens de la classe amb 10 anys | **Depèn del context** (pot tenir elements si hi ha nens de 10 anys) |
| Gats que volen | **∅** (els gats no volen naturalment) |
| Lletres de la paraula "casa" | **{c, a, s}** (c apareix una vegada, a dues, s una) |
| Nombres positius menors que 0 | **∅** (cap nombre positiu és menor que 0) |

---

## 📌 Part 4: Cardinalitat (|A|)

### 4.1 Compte Elements

| Conjunt | Cardinalitat | Explicació |
|---------|--------------|-----------|
| A = {1, 2, 3} | **3** | Tres elements |
| B = {a, b, c, d, e} | **5** | Cinc elements |
| C = {gat, gos} | **2** | Dos elements |
| D = ∅ | **0** | El buit no té elements |
| E = {∅} | **1** | Conté un element: el buit |
| F = {10} | **1** | Un element |

---

### 4.2 Cardinalitat de Conjunts amb Duplicats

| Conjunt | Cardinalitat | Per què? |
|---------|--------------|---------|
| {1, 2, 2, 3, 3, 3} | **3** | Els duplicats es col·lapsen: {1, 2, 3} |
| {a, a, a, b, b} | **2** | Es col·lapsa a {a, b} |
| {5, 5, 5, 5} | **1** | Es col·lapsa a {5} |
| {gat, gos, gat} | **2** | Es col·lapsa a {gat, gos} |

---

## 📌 Part 5: Propietats dels Conjunts

### 5.1 L'Ordre NO Importa

| Conjunt 1 | Conjunt 2 | Mateix? | Explicació |
|-----------|-----------|--------|-----------|
| {1, 2, 3} | {3, 2, 1} | **SÍ** | Mateixos elements, ordre diferent |
| {a, b, c} | {c, b, a} | **SÍ** | Mateixos elements |
| {5, 10, 15} | {15, 5, 10} | **SÍ** | Mateixos elements |
| {vermell, blau} | {blau, vermell} | **SÍ** | Mateixos elements |

---

### 5.2 Marca les Afirmacions Correctes

| Afirmació | V/F |
|-----------|-----|
| Els conjunts són iguals si tene els mateixos elements (independentment de l'ordre) | **V** |
| Les repeticions es col·lapsen en una sola entrada | **V** |
| Un conjunt pot tenir infinits elements | **V** |
| El conjunt {1, 2, 3} té 3 elements | **V** |

---

## 📌 Part 6: Unió (A ∪ B) i Intersecció (A ∩ B)

### 6.1 Calcula Unions

| A | B | A ∪ B | \|A ∪ B\| | Explicació |
|---|---|-------|----------|-----------|
| {1, 2} | {3, 4} | **{1, 2, 3, 4}** | **4** | Tots els elements |
| {a, b, c} | {b, c, d} | **{a, b, c, d}** | **4** | Col·lapsem duplicats |
| {5} | {5, 10} | **{5, 10}** | **2** | Duplicat es col·lapsa |
| {gat} | {gos, peix} | **{gat, gos, peix}** | **3** | Tots els elements |

---

### 6.2 Calcula Interseccions

| A | B | A ∩ B | \|A ∩ B\| | Explicació |
|---|---|-------|----------|-----------|
| {1, 2, 3} | {2, 3, 4} | **{2, 3}** | **2** | Elements comuns |
| {a, b, c} | {d, e, f} | **∅** | **0** | Cap element comú |
| {5, 10, 15} | {5, 10} | **{5, 10}** | **2** | Tots els de B estan en A |
| {gat, gos} | {gat, gos, peix} | **{gat, gos}** | **2** | Tots els de A estan en B |

---

### 6.3 Commutativitat

| A | B | A ∪ B | B ∪ A | Iguals? | A ∩ B | B ∩ A | Iguals? |
|---|---|-------|-------|---------|-------|-------|---------|
| {1, 2} | {2, 3} | {1, 2, 3} | {1, 2, 3} | **SÍ** | {2} | {2} | **SÍ** |
| {a, b} | {c, d} | {a, b, c, d} | {a, b, c, d} | **SÍ** | ∅ | ∅ | **SÍ** |

**Conclusió:** La unió i la intersecció són **commutatives**: A ∪ B = B ∪ A i A ∩ B = B ∩ A.

---

## 📌 Part 7: Casos Especials amb Unió i Intersecció

### 7.1 Unió i Intersecció amb el Conjunt Buit

| Operació | Resultat | Cardinalitat | Explicació |
|----------|----------|--------------|-----------|
| {1, 2} ∪ ∅ | **{1, 2}** | **2** | El buit no afegeix res |
| {a, b, c} ∩ ∅ | **∅** | **0** | No hi ha elements comuns |
| {5} ∪ ∅ | **{5}** | **1** | El buit no afegeix res |
| ∅ ∩ {1, 2, 3} | **∅** | **0** | El buit no té elements comuns |

---

### 7.2 Unió i Intersecció de Conjunts Idèntics

| Operació | Resultat | Explicació |
|----------|----------|-----------|
| {1, 2, 3} ∪ {1, 2, 3} | **{1, 2, 3}** | La unió amb si mateix és ell mateix |
| {a, b} ∩ {a, b} | **{a, b}** | La intersecció amb si mateix és ell mateix |
| {5} ∪ {5} | **{5}** | Mateixa lògica |

---

## 📌 Part 8: Problemes Aplicats

### 8.1 Escoles i Clubs

**Donnats:**
- Club d'Escacs: {Anna, Biel, Carles, Dina}
- Club de Ciència-Ficció: {Biel, Eva, Ferran, Gina}

**Calcula:**

1. Qui està en el Club d'Escacs O en el de Ciència-Ficció? (Unió)
   
   **A ∪ CF = {Anna, Biel, Carles, Dina, Eva, Ferran, Gina}**

2. Qui està en AMBDÓS clubs? (Intersecció)
   
   **A ∩ CF = {Biel}**

3. Quants nens estan almenys en un club?
   
   **7 nens** (tots els mencionats)

---

### 8.2 Fruites

**Donnats:**
- Fruites verdes: {pistatxo, kiwi, llima}
- Fruites que són cítrics: {llima, taronja, llimona}

**Calcula:**

1. Fruites verdes O cítrics:
   
   **V ∪ C = {pistatxo, kiwi, llima, taronja, llimona}**

2. Fruites que són verdes I cítrics:
   
   **V ∩ C = {llima}** (només la llima és ambdues)

---

## 📌 Part 9: Repte — Problemes de Lògica

### 9.1 Pensa Críticament

**Pregunta 1:** Per a quins casos és A ∪ B = A?

**Resposta:** **Quan B ⊆ A** (B és subconjunt de A, o B ⊆ A, o B = ∅)

**Explicació:** Si tots els elements de B ja estan en A, llavors A ∪ B = A.

---

**Pregunta 2:** Per a quins casos és A ∩ B = ∅?

**Resposta:** **Quan A i B no tienen elementos comuns** (disjunts)

**Explicació:** Si cap element de A apareix en B, la intersecció és buida.

---

**Pregunta 3:** Si A ⊆ B (A és subconjunt de B), quina és la relació entre A ∪ B i B?

**Resposta:** **A ∪ B = B**

**Explicació:** Si tots els elements d'A ja estan en B, llavors la unió no afegeix res nou.

---

### 9.2 Cardinalitat i Duplicats

Un estudiant escriu: `{1, 2, 2, 3, 3, 3} té cardinalitat 6`.

**És correcte? (V/F)** **F** (FALS)

**Quina és la cardinalitat correcta?** **3**

**Explicació:** Els duplicats es col·lapsen en una sola entrada: {1, 2, 2, 3, 3, 3} = {1, 2, 3}, que té 3 elements.

---

## 📌 Part 10: Crea els Teus Conjunts

*(Les solucions variaran segons l'estudiant. Aquí hi ha exemples de resposta correcta.)*

---

### 10.1 Defineix 3 Conjunts de la Vida Real

**Conjunt 1:** Nom: **Fruites de color vermell** | Elements: **{poma, maduixa, cereza, taronja}**

**Conjunt 2:** Nom: **Transports amb rodes** | Elements: **{cotxe, bicicleta, moto, camió}**

**Conjunt 3:** Nom: **Matèries escolars** | Elements: **{matemàtiques, català, anglès, educació física}**

---

### 10.2 Usa els Teus Conjunts

Usant els conjunts de dalt, calcula:

- Unió de Conjunt 1 i Conjunt 2: **{poma, maduixa, cereza, taronja, cotxe, bicicleta, moto, camió}**
- Intersecció de Conjunt 2 i Conjunt 3: **∅** (cap element comú entre transports i matèries)
- Cardinalitat de cada conjunt: **|C1| = 4, |C2| = 4, |C3| = 4**

---

## 🎯 Autoavaluació

Marca quines parts vas respondre correctament:

- [ ] Part 1 (Pertinença): Esperem 11/11 correctes
- [ ] Part 2 (Escriure Conjunts): Esperem 8/8 correctes
- [ ] Part 3 (Conjunt Buit): Esperem 11/11 correctes
- [ ] Part 4 (Cardinalitat): Esperem 10/10 correctes
- [ ] Part 5 (Propietats): Esperem 8/8 correctes
- [ ] Part 6 (Unió i Intersecció): Esperem 12/12 correctes
- [ ] Part 7 (Casos Especials): Esperem 8/8 correctes
- [ ] Part 8 (Problemes Aplicats): Esperem 5/5 correctes
- [ ] Part 9 (Repte): Esperem 5/5 correctes
- [ ] Part 10 (Creació): Autocreació (bé si són coherents)

**Puntuació Esperada:**
- 9/10 parts correctes: **Mestre de Bloc 1!** 🎉
- 7/10 parts correctes: **Molt bé! Repassa les parts que fallaren.** 👍
- 5/10 parts correctes: **Bé, però necessites practicar més.** 📚

---

## 📝 Notes Addicionals

**Punts Clau a Recordar:**

1. **Conjunt:** Col·lecció ben definida d'objectes (elements)
2. **Pertinença (∈):** Indica que un element està al conjunt
3. **No pertinença (∉):** Indica que un element NO està al conjunt
4. **Conjunt buit (∅):** No conté cap element (cardinalitat 0)
5. **Cardinalitat (\|A\|):** Nombre d'elements
6. **Duplicats:** Es col·lapsen en una sola entrada (no es permeten)
7. **Ordre:** NO importa en conjunts
8. **Unió (A ∪ B):** Tots els elements de A o B
9. **Intersecció (A ∩ B):** Només els elements comuns
10. **Commutativitat:** A ∪ B = B ∪ A i A ∩ B = B ∩ A

**Símbols Clau:**
- ∈ : pertany a
- ∉ : no pertany a
- ∅ : conjunt buit
- \|A\| : cardinalitat de A
- ∪ : unió
- ∩ : intersecció

**Fórmula Clau:**
- \|A ∪ B\| = \|A\| + \|B\| − \|A ∩ B\| (inclusió-exclusió)

---

**Molt bé pels exercicis! Els conjunts són la base de totes les matemàtiques!** 🎓


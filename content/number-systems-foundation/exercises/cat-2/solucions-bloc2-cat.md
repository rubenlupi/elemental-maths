# Solucions Bloc 2 – Subconjunts i Diagrames de Venn

---

## 📌 Part 1: Introducció a Subconjunts

### 1.1 Relacions Bàsiques

| A | B | Relació | Correcte? | Explicació |
|---|---|---------|-----------|-----------|
| {1, 2} | {1, 2, 3} | A **⊆** B | **SÍ** | 1 i 2 estan en B |
| {a, b, c} | {a, c} | A **⊄** B | **SÍ** | b no està en B |
| {5} | {1, 2, 3, 4, 5} | A **⊆** B | **SÍ** | 5 està en B |
| {gat, gos} | {gat, gos, peix} | A **⊆** B | **SÍ** | gat i gos estan en B |
| {1, 2} | {2, 3, 4} | A **⊄** B | **SÍ** | 1 no està en B |
| ∅ | {1, 2, 3} | A **⊆** B | **SÍ** | el buit és subconjunt de tot |

---

### 1.2 Subconjunt Propi vs Subconjunt

| A | B | Simbol | Explicació |
|---|---|--------|-----------|
| {1, 2} | {1, 2, 3} | **⊂** | A és subconjunt PROPI (més petit que B) |
| {1, 2, 3} | {1, 2, 3} | **⊆** | A és igual a B, per tant és subconjunt però NO propi |
| {a} | {a, b, c} | **⊂** | A és subconjunt propi (més petit) |
| {red, blue} | {red, blue} | **⊆** | A és igual a B, per tant ⊆ pero no ⊂ |

---

## 📌 Part 2: Casos Especials

### 2.1 Conjunt Buit

| Afirmació | V/F | Explicació |
|-----------|-----|-----------|
| ∅ ⊆ {1, 2, 3} | **V** | El buit és subconjunt de tots els conjunts |
| ∅ ⊂ {a, b} | **V** | El buit és subconjunt propi (més petit) |
| ∅ ⊆ ∅ | **V** | Tot conjunt és subconjunt de si mateix, inclòs el buit |
| {∅} = ∅ | **F** | {∅} és un conjunt que CONTÉ el buit; ∅ NO conté res |
| \|\∅\| = 0 | **V** | El buit té 0 elements |

---

### 2.2 Reflexivitat

| Afirmació | V/F | Explicació |
|-----------|-----|-----------|
| {1, 2} ⊆ {1, 2} | **V** | Tot conjunt és subconjunt de si mateix |
| {a, b, c} ⊂ {a, b, c} | **F** | NO és subconjunt propi (seria igual, no més petit) |
| A ⊆ A (per a qualsevol A) | **V** | Sempre és cert (reflexivitat) |

---

## 📌 Part 3: Comptatge de Subconjunts

### 3.1 Calcula

| Conjunt | Elements | 2^n | Subconjunts |
|---------|----------|-----|-----------|
| {1} | 1 | 2^1 = **2** | **∅, {1}** |
| {a, b} | 2 | 2^2 = **4** | **∅, {a}, {b}, {a,b}** |
| {1, 2, 3} | 3 | 2^3 = **8** | **∅, {1}, {2}, {3}, {1,2}, {1,3}, {2,3}, {1,2,3}** |
| {x, y, z, w} | 4 | 2^4 = **16** | **16 subconjunts** |

---

### 3.2 Enumera tots els Subconjunts

**Per a A = {1, 2}:**

Subconjunts: **∅, {1}, {2}, {1,2}**

(Total: **4 subconjunts** = 2^2)

---

**Per a B = {a, b, c}:**

Subconjunts: **∅, {a}, {b}, {c}, {a,b}, {a,c}, {b,c}, {a,b,c}**

(Total: **8 subconjunts** = 2^3)

---

## 📌 Part 4: Diagrames de Venn

### 4.1 Interpreta Diagrames

**Donnats:** A = {1, 2, 3}, B = {2, 3, 4, 5}

Diagrama de Venn:

```
     A             B
   ┌───┐         ┌───┐
   │ 1 │─┬─────┬─│ 5 │
   │   ├─┼─{2,3}┼─┤   │
   │   │ │     │ │ 4 │
   └───┘─┴─────┴─└───┘
        (intersecció)
```

**Escriu:**

1. Què està DINS d'A? **{1, 2, 3}**
2. Què està DINS de B? **{2, 3, 4, 5}**
3. Què està en TOTS DOS (intersecció)? **{2, 3}**
4. Què està FORA de tots dos? **Res (depenent de l'univers)**

---

### 4.2 Interpreta el Diagrama Donat

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

**Identifica:**

- Elements només en A: **{1}**
- Elements només en B: **{4, 5}**
- Elements en A i B: **{2, 3}**
- Elements fora de tots dos: **(cap)**

---

### 4.3 Crea el Teu Diagrama de Venn

**Donnats:**
- A = {fruites: poma, plàtan, taronja}
- B = {colors: vermell, groc, taronja}

**Diagrama:**

```
        A (Fruites)           B (Colors)
       ┌─────────┐           ┌─────────┐
       │ poma    │───┬───────│ vermell │
       │ plàtan  │─┬─┼─{taronja}┬─│ groc    │
       └─────────┘ │ └───────│         │
                   └─────────┴─────────┘
           (intersecció: taronja)
```

---

## 📌 Part 5: Transitivitat

### 5.1 Verifica la Transitivitat

| A | B | C | A ⊆ B? | B ⊆ C? | A ⊆ C? | Transitivitat es compleix? |
|---|---|---|--------|--------|--------|---------------------------|
| {1} | {1, 2} | {1, 2, 3} | **V** | **V** | **V** | **✓ SÍ** |
| {a} | {a, b} | {a, b, c} | **V** | **V** | **V** | **✓ SÍ** |
| {5} | {1, 2, 5} | {1, 2, 3, 4, 5} | **V** | **V** | **V** | **✓ SÍ** |

**Conclusió:** La transitivitat SEMPRE es compleix: Si A ⊆ B i B ⊆ C, aleshores A ⊆ C.

---

### 5.2 Crea una Cadena de Subconjunts

**Exemple de resposta:**

- D (conjunt més gran): **{1, 2, 3, 4, 5, 6}**
- C: **{1, 2, 3, 4, 5}**
- B: **{1, 2, 3}**
- A (conjunt més petit): **{1}**

**Verificació:** {1} ⊂ {1,2,3} ⊂ {1,2,3,4,5} ⊂ {1,2,3,4,5,6} ✓

---

## 📌 Part 6: Aplicacions Reals

### 6.1 Jerarquies de la Vida Real

| Cadena | Escriu amb ⊆ |
|--------|-------------|
| Gats ⊆ Felins ⊆ Mamífers ⊆ Animals | **{gats} ⊆ {felins} ⊆ {mamífers} ⊆ {animals}** |
| Quadrats ⊆ Rectangles ⊆ ? | **Quadrats ⊆ Rectangles ⊆ Paral·lelograms** |
| Telèfons intel·ligents ⊆ ? ⊆ Electrodomèstics | **Telèfons ⊆ Dispositius mòbils ⊆ Electrodomèstics** |
| Divendres ⊆ ? ⊆ Temps | **Divendres ⊆ Dies de la setmana ⊆ Temps** |

---

### 6.2 Organització de Dades

**Donnats:**
- Empleats totals: 100
- Gerents: 10
- Programadors: 30
- Gerents-programadors: 2

**Preguntes:**

1. Els gerents ⊆ Empleats? **(V)** Tots els gerents són empleats
2. Els programadors ⊆ Empleats? **(V)** Tots els programadors són empleats
3. Els gerents-programadors ⊆ Gerents? **(V)** Els gerents que programen són gerents
4. Els gerents-programadors ⊆ Programadors? **(V)** Els gerents que programen són programadors

---

## 📌 Part 7: Propietats de Subconjunts

### 7.1 Marca V o F

| Afirmació | V/F | Explicació |
|-----------|-----|-----------|
| Si A ⊂ B, aleshores A ⊆ B | **V** | Tot subconjunt propi és subconjunt |
| Si A ⊆ B i B ⊆ A, aleshores A = B | **V** | Definició d'igualtat de conjunts |
| Si A ⊆ B i A ⊆ C, aleshores A ⊆ (B ∩ C) | **V** | A està en B i en C, per tant en la seva intersecció |
| Tot conjunt és subconjunt de si mateix | **V** | Reflexivitat: A ⊆ A |

---

### 7.2 Completa la Definició

- Un subconjunt propi A ⊂ B significa: **Tots els elements d'A estan en B, però A ≠ B (A és més petit)**

- El conjunt buit ∅ és subconjunt de: **TOTS els conjunts**

- La reflexivitat significa: **Tot conjunt és subconjunt de si mateix**

---

## 📌 Part 8: Repte — Problemes de Lògica

### 8.1 Pensar Críticament

**Pregunta 1:** Si A ⊂ B ⊂ C, quina és la relació entre A i C?

**Resposta:** **A ⊂ C** (per transitivitat)

---

**Pregunta 2:** Quants subconjunts propis té un conjunt de 4 elements?

**Resposta:** **15** 

**Explicació:** 
- Un conjunt de 4 elements té 2^4 = 16 subconjunts totals
- Els subconjunts propis són tots excepte el conjunt sencer
- 16 − 1 = **15 subconjunts propis**

---

**Pregunta 3:** Per a quins conjunts A és cert que A ⊂ A?

**Resposta:** **Cap conjunt!** (Ningú és subconjunt propi de si mateix)

**Explicació:** Per ser A ⊂ A seria necessari que A fos diferent de A (més petit), cosa impossible.

---

### 8.2 Paradoxa del Conjunt Buit

- ∅ ⊆ ∅? **(sí)** El buit és subconjunt de si mateix (reflexivitat)
- ∅ ⊂ ∅? **(no)** El buit NO és subconjunt propi de si mateix (seria igual, no més petit)

**Per què?** El buit és un conjunt especial que és subconjunt de tot, però no és mai un subconjunt PROPI de si mateix perquè "propi" significa més petit.

---

## 📌 Part 9: Casos Combinats

### 9.1 Diagrames de Venn + Subconjunts

**Donnats:** A = {1, 2, 3}, B = {2, 3}, C = {2}

**Identifica les relacions:**

- C **⊂** B **⊂** A (omple amb ⊆ o ⊂)
- Verifica: C ⊆ B ⊆ A? **(V) SÍ**

**Explicació:**
- C = {2} és subconjunt propi de B = {2, 3} ✓
- B = {2, 3} és subconjunt propi de A = {1, 2, 3} ✓

---

### 9.2 Jerarquies de Números

**Recordem:** ℕ ⊂ ℤ ⊂ ℚ (naturals ⊂ enters ⊂ racionals)

| Afirmació | V/F | Explicació |
|-----------|-----|-----------|
| 5 ∈ ℕ, 5 ∈ ℤ, 5 ∈ ℚ | **V** | 5 és natural, per tant enter, per tant racional (5 = 5/1) |
| -3 ∈ ℕ | **F** | -3 no és natural (els naturals són positius) |
| 1/2 ∈ ℤ | **F** | 1/2 no és enter |
| 1/2 ∈ ℚ | **V** | 1/2 és racional (fracció) |
| ℕ ⊆ ℚ? | **V** | Tot natural és racional (per la cadena ℕ ⊂ ℤ ⊂ ℚ) |

---

## 📌 Part 10: Crea els Teus Conjunts

### 10.1 Dibuixa Diagrames de Venn

**Diagrama 1 (Exemple):**

- Conjunt A: Esports amb pilota
- Conjunt B: Esports en equip

```
    A (Pilota)      B (Equip)
   ┌──────────┐   ┌──────────┐
   │ tennis   │───┼─ bàsquet │
   │ bàsbol   │─┬─┼─ futbol  │
   │ golf     │ │ │ voleibol │
   └──────────┘─┴─└──────────┘
      (intersecció: bàsbol, bàsquet)
```

---

**Diagrama 2 (Exemple):**

- Conjunt X: Fruites
- Conjunt Y: Colors vermells

```
    X (Fruites)      Y (Vermell)
   ┌──────────┐     ┌──────────┐
   │ poma     │──┬──│ taronja  │
   │ plàtan   │─ ├─ │ maduixa  │
   │ kiwi     │  │  │          │
   └──────────┘──┴──└──────────┘
        (intersecció: poma, taronja, maduixa)
```

---

### 10.2 Crea Cadenes de Subconjunts

**Cadena 1 (Exemple):** A ⊂ B ⊂ C

- A = {1}
- B = {1, 2}
- C = {1, 2, 3}

**Verificació:** {1} ⊂ {1,2} ⊂ {1,2,3} ✓

---

**Cadena 2 (Exemple):** X ⊂ Y ⊂ Z

- X = {gats}
- Y = {gats, gossos}
- Z = {gats, gossos, ous}

**Verificació:** {gats} ⊂ {gats, gossos} ⊂ {gats, gossos, ous} ✓

---

## 🎯 Autoavaluació

Marca quines parts vas respondre correctament:

- [ ] Part 1 (Introducció): Esperem 6/6 correctes
- [ ] Part 2 (Casos Especials): Esperem 8/8 correctes
- [ ] Part 3 (Comptatge): Esperem 4+2+2 correctes
- [ ] Part 4 (Diagrames de Venn): Esperem 3 diagrames correctes
- [ ] Part 5 (Transitivitat): Esperem 4+2 correctes
- [ ] Part 6 (Aplicacions): Esperem 8+4 correctes
- [ ] Part 7 (Propietats): Esperem 4+3 correctes
- [ ] Part 8 (Repte): Esperem 4+2 correctes
- [ ] Part 9 (Casos Combinats): Esperem 2+5 correctes
- [ ] Part 10 (Creació): Autocreació (2 diagrames + 2 cadenes)

**Puntuació Esperada:**
- 9/10 parts correctes: **Mestre de Bloc 2!** 🎉
- 7/10 parts correctes: **Molt bé! Repassa les parts que fallaren.** 👍
- 5/10 parts correctes: **Bé, però necessites practicar més.** 📚

---

## 📝 Notes Addicionals

**Punts Clau a Recordar:**

1. **Subconjunt (⊆):** Tots els elements d'A estan en B (pot ser A = B)
2. **Subconjunt propi (⊂):** Tots els elements d'A estan en B, i A ≠ B (A més petit)
3. **Conjunt buit (∅):** Subconjunt de tots els conjunts (inclòs ell mateix)
4. **Comptatge:** Un conjunt de n elements té 2^n subconjunts
5. **Diagrama de Venn:** Visual per veure subconjunts, interseccions, unions
6. **Transitivitat:** Si A ⊆ B i B ⊆ C, aleshores A ⊆ C
7. **Reflexivitat:** A ⊆ A per a qualsevol conjunt A

**Símbols Clau:**
- ⊆ : subconjunt
- ⊂ : subconjunt propi
- ⊄ : no és subconjunt
- ∅ : conjunt buit
- ∈ : pertany a
- ∉ : no pertany a

---

**Molt bé pels exercicis! Els diagrames de Venn són la clau!** 🎓


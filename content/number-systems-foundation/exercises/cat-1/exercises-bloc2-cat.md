# Exercicis - Mòdul 1: Bloc 2 – Subconjunts i Visualitzacions de Venn

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Aplicació Directa: Símbol de Subconjunt

**Enunciat:**

Considera els conjunts:
- `U = {1, 2, 3, 4, 5, 6}`
- `V = {2, 4, 6}`
- `W = {1, 2, 3, 4, 5, 6, 7}`

Escriu les afirmacions correctes utilitzant `⊆`, `⊂`, o `⊄`:

a) `V` i `U`
b) `U` i `W`
c) `U` i `U`
d) `∅` i `V`

**Solució:**

a) `V ⊆ U` (de fet, `V ⊂ U` és més precís perquè `V ≠ U`, però `⊆` és correcte)
   - Justificació: Tots els elements de `V` (`2, 4, 6`) apareixen a `U`.

b) `U ⊂ W` (subconjunt propi, perquè `U` és més petit i `W` conté 7)
   - Justificació: Tots els elements de `U` apareixen a `W`, però `U ≠ W`.

c) `U ⊆ U` (és a dir, cada conjunt és subconjunt de si mateix)
   - Justificació: Per definició, tot conjunt és un subconjunt de si mateix.

d) `∅ ⊆ V` (el conjunt buit és subconjunt de tot conjunt)
   - Justificació: El conjunt buit no conté cap element que no estigui en `V`.

**Concepte avaluat:** Interpretació de símbols `⊆` i `⊂`, diferència entre subconjunt i subconjunt propi.

---

### **Exercici 2** 🟦 (1.1 punts) – Llistatge de Subconjunts

**Enunciat:**

Donada `A = {a, b}`:

a) Llista tots els subconjunts de `A`.

b) Verifica que el nombre total de subconjunts correspon a la fórmula `2^n`, on `n` és el nombre d'elements.

c) Entre tots els subconjunts que has llistat, quins són subconjunts propis de `A`?

**Solució:**

a) Tots els subconjunts de `A = {a, b}`:
   - `∅` (el conjunt buit)
   - `{a}`
   - `{b}`
   - `{a, b}` (el mateix conjunt `A`)
   - Total: **4 subconjunts**

b) Verificació:
   - `A` té `n = 2` elements.
   - Fórmula: `2^n = 2^2 = 4` ✓
   - Efectivament, hem llistat 4 subconjunts.

c) Subconjunts propis (tot subconjunt excepte el mateix `A`):
   - `∅ ⊂ A` ✓
   - `{a} ⊂ A` ✓
   - `{b} ⊂ A` ✓
   - `{a, b}` **NO és propi** perquè `{a, b} = A`.

**Concepte avaluat:** Enumeració sistemàtica de subconjunts, fórmula `2^n`, distinció entre subconjunt i subconjunt propi.

---

### **Exercici 3** ⭐ (0.9 punts) – Verificació de Membership en Subconjunts

**Enunciat:**

Determina si les següents afirmacions són **verdaderes** o **falses**. Justifica brevement.

a) `∅ ⊆ {1, 2, 3}`

b) `{1, 2} ⊆ {1, 2, 3}`

c) `{1, 2, 3} ⊆ {1, 2}`

d) `3 ⊆ {1, 2, 3}` (nota: s'usa `⊆` incorrectament aquí)

**Solució:**

a) **Vertadera.** El conjunt buit és subconjunt de qualsevol conjunt per definició (no conté elements que contradiguin la pertinença).

b) **Vertadera.** Tots els elements de `{1, 2}` (que són `1` i `2`) apareixen a `{1, 2, 3}`.

c) **Falsa.** L'element `3` pertany a `{1, 2, 3}` però no apareix a `{1, 2}`, així que `{1, 2, 3}` no és subconjunt de `{1, 2}`.

d) **Falsa i errònea en notació.** L'error és que `3` és un **element** i `⊆` s'usa per a **conjunts**. L'afirmació correcta seria `3 ∈ {1, 2, 3}` (amb `∈`, no `⊆`).

**Concepte avaluat:** Distinció entre element (`∈`) i subconjunt (`⊆`), aplicació correcta de símbols.

---

### **Exercici 4** 🟦 (1.2 punts) – Visualització de Venn i Relacions

**Enunciat:**

Considera els conjunts:
- `E = {estudiants de l'escola}`
- `M = {estudiants que fan Matemàtiques}`
- `C = {estudiants que fan Cuina}`

a) Dibuixa un diagrama de Venn que mostri la relació entre `M`, `C`, i `E`.

b) En el teu diagrama, marca les regions per a:
   - Només Matemàtiques
   - Només Cuina
   - Ambdós (Matemàtiques i Cuina)
   - Cap dels dos

c) Justifica per què `M ⊆ E` i `C ⊆ E`.

**Solució:**

a) Diagrama de Venn (representació ASCII):

```
         ___________E___________
        /                       \
       /                         \
      |   ___M___    ___C___     |
      |  /       \  /       \    |
      | | M only | \  Both / | C|
      |  \       /  \     /     |
      |   \_____/    \___/      |
      |                   Cap   |
      |_________________________|
```

b) Regions marcades:
   - **Només Matemàtiques**: Estudiants que fan Matemàtiques però no Cuina.
   - **Només Cuina**: Estudiants que fan Cuina però no Matemàtiques.
   - **Ambdós**: La regió de intersecció (tant Matemàtiques com Cuina).
   - **Cap dels dos**: Estudiants que no fan ni Matemàtiques ni Cuina.

c) Justificacions:
   - `M ⊆ E` perquè **tots els estudiants que fan Matemàtiques** són also estudiants de l'escola `E`.
   - `C ⊆ E` perquè **tots els estudiants que fan Cuina** són also estudiants de l'escola `E`.

**Concepte avaluat:** Representació visual amb diagrames de Venn, interpretació de relacions de subconjunts en contextos reals.

---

### **Exercici 5** ⭐ (0.8 punts) – Conjunt Buit com a Subconjunt

**Enunciat:**

Explica per què `∅ ⊆ A` és vertader per a **qualsevol conjunt** `A`. (Pista: Pensa en la definició de subconjunt.)

**Solució:**

Per definició, `X ⊆ Y` significa que **tot element de `X` pertany a `Y`**.

Per al conjunt buit `∅`:
- El conjunt buit no conté **cap element**.
- Per tant, hi ha **0 elements** de `∅` que no pertanyen a `A`.
- Així que la condició "tot element de `∅` pertany a `A`" és **vertadera de manera "vacua"** (és a dir, es compleix per defecte perquè no hi ha contraexemples).

**Conclusió:** `∅ ⊆ A` per a **qualsevol conjunt** `A`, incloent `A = ∅`.

**Concepte avaluat:** Comprensió de la definició formal de subconjunt, raonament lògic amb el conjunt buit.

---

### **Exercici 6** 🟦 (1.1 punts) – Transitivitat de Subconjunts

**Enunciat:**

Verifica que la relació de subconjunt és **transitiva**. Donats:
- `P = {1, 3}`
- `Q = {1, 2, 3, 5}`
- `R = {1, 2, 3, 4, 5, 6}`

a) Comprova que `P ⊆ Q` i `Q ⊆ R`.

b) Usa la transitivitat per concloure que `P ⊆ R`.

c) Verifica directament que `P ⊆ R` verifiant que cada element de `P` pertany a `R`.

**Solució:**

a) Comprovació:
   - `P ⊆ Q`: Els elements de `P` són `1` i `3`. Ambdós apareixen a `Q = {1, 2, 3, 5}`. ✓
   - `Q ⊆ R`: Els elements de `Q` són `1, 2, 3, 5`. Tots apareixen a `R = {1, 2, 3, 4, 5, 6}`. ✓

b) Per transitivitat (si `A ⊆ B` i `B ⊆ C`, llavors `A ⊆ C`):
   - Aplicant: Si `P ⊆ Q` i `Q ⊆ R`, aleshores **`P ⊆ R`**. ✓

c) Verificació directa:
   - Elements de `P`: `1, 3`.
   - `1 ∈ R`? Sí, `1` apareix a `R`. ✓
   - `3 ∈ R`? Sí, `3` apareix a `R`. ✓
   - Per tant, **`P ⊆ R`** directament verificat. ✓

**Concepte avaluat:** Propietat transitiva de subconjunts, lògica de relacions encadenades.

---

### **Exercici 7** 🟦 (1.0 punt) – Aplicació Real: Classificació de Figures Geomètriques

**Enunciat:**

En geometria, sabem que:
- Quadrat = figura amb 4 costats iguals i 4 angles rectes.
- Paral·lelogram = figura amb costats oposats paral·lels.
- Rectangle = figura amb 4 angles rectes.

a) Completa les afirmacions usant `⊆` o `⊄`:

   - `{quadrats} ___ {rectangles}`
   - `{rectangles} ___ {paral·lelograms}`
   - `{quadrats} ___ {paral·lelograms}`

b) Justifica la primera relació.

c) Dibuixa un diagrama de Venn simple que mostri aquestes relacions.

**Solució:**

a) Completacions:
   - `{quadrats} ⊆ {rectangles}` (tot quadrat és un rectangle)
   - `{rectangles} ⊆ {paral·lelograms}` (tot rectangle és un paral·lelogram)
   - `{quadrats} ⊆ {paral·lelograms}` (per transitivitat, tot quadrat és paral·lelogram)

b) Justificació de la primera:
   - Un quadrat té 4 angles rectes (per definició de quadrat).
   - Un rectangle es defineix com una figura amb 4 angles rectes.
   - Per tant, **tot quadrat compleix la definició de rectangle**, és a dir, `{quadrats} ⊆ {rectangles}`.

c) Diagrama de Venn:

```
       _______________________
      /    Paral·lelograms    \
     /                          \
    |    ___________________    |
    |   /    Rectangles    \   |
    |  |   _____________    |  |
    |  |  /   Quadrats  \   |  |
    |  |  |             |   |  |
    |  |  |_____________|   |  |
    |  |___________________|  |
    |_________________________|
```

**Concepte avaluat:** Aplicació de subconjunts a contextos geomètrics, construcció de jerarquies de conceptes.

---

### **Exercici 8** 🟦 (1.3 punts) – Distinció entre Subconjunt i Igual

**Enunciat:**

Considera els conjunts:
- `A = {2, 4, 6, 8}`
- `B = {2, 4, 6, 8}`
- `C = {2, 4, 6}`
- `D = {x | x és nombre parell positiu menor que 10}`

a) Completa les afirmacions:
   - `A ⊆ B` → **Vertader o Fals?**
   - `A ⊂ B` → **Vertader o Fals?**
   - `A = B` → **Vertader o Fals?**
   - `A ⊆ D` → **Vertader o Fals?**

b) Explica per què `A ⊆ B` és vertader mentre que `A ⊂ B` és fals.

c) Verifica que `D = {2, 4, 6, 8}` i per tant `D = A`.

**Solució:**

a) Completacions:
   - `A ⊆ B` → **Vertader** (tots els elements de `A` pertanyen a `B`)
   - `A ⊂ B` → **Fals** (no és un subconjunt propi perquè `A = B`)
   - `A = B` → **Vertader** (ambdós conjunts tenen exactament els mateixos elements)
   - `A ⊆ D` → **Vertader** (tots els elements de `A` són nombres parells positius menors de 10)

b) Distinció:
   - `A ⊆ B` és vertader perquè: cada element de `A` pertany a `B`.
   - `A ⊂ B` és fals perquè: tot i que `A ⊆ B`, tenim que `A = B` (no és una relació "pròpia" és a dir, no hi ha desigualtat).

c) Verificació de `D`:
   - `D = {x | x és nombre parell positiu menor que 10}`
   - Nombres parells positius menors de 10: `2, 4, 6, 8`
   - Per tant, `D = {2, 4, 6, 8}`
   - Comparant amb `A = {2, 4, 6, 8}`, es veu que **`D = A`**. ✓

**Concepte avaluat:** Distinció subtil entre `⊆`, `⊂`, i `=`; relació entre notació de comprensió i enumeració.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Construcció de Subconjunts amb Restriccions

**Enunciat:**

Donada `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}` (conjunt universal):

a) Construeix dos subconjunts `A` i `B` de manera que:
   - `A ⊂ B` (és a dir, `A` és subconjunt propi de `B`)
   - `B ⊂ U`
   - `A` conté almenys dos nombres parells
   - `B` conté almenys tres nombres imparells

b) Per als subconjunts que has construït, verifica la **transitivitat**: si `A ⊂ B` i `B ⊂ U`, aleshores `A ⊂ U`.

c) Quants subconjunts propis té `U`? (Pista: Usa la fórmula `2^n - 1`, on `n = |U|`.)

**Solució:**

a) Un exemple de construcció:
   - `A = {2, 4, 6}` (té dos nombres parells: `2` i `4` ✓, de fet en té 3)
   - `B = {1, 2, 3, 4, 5, 6}` (conté tres nombres imparells: `1, 3, 5` ✓)
   - Verificació: `A ⊂ B`? Tots els elements de `A` pertanyen a `B`, i `A ≠ B`. ✓
   - Verificació: `B ⊂ U`? Tots els elements de `B` pertanyen a `U`, i `B ≠ U`. ✓

b) Verificació de transitivitat:
   - `A = {2, 4, 6}` i `U = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10}`
   - Tots els elements de `A` apareixen a `U`, i `A ≠ U`.
   - Per tant, **`A ⊂ U`**. ✓
   - Aquesta és la conclusió de la transitivitat aplicada correctament.

c) Nombre de subconjunts propis de `U`:
   - `|U| = 10`, així que `2^{10} = 1024` subconjunts en total.
   - Subconjunts propis = Tots els subconjunts excepte `U` mateix.
   - Nombre = `2^{10} - 1 = 1024 - 1 = 1023` subconjunts propis.

**Concepte avaluat:** Construcció de subconjunts amb restriccions múltiples, verificació de propietats, fórmula `2^n - 1`.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Venn Avançat amb Tres Conjunts

**Enunciat:**

En una biblioteca, els estudiants s'agrupen segons els tipus de llibres que llegeixen:
- `T = {estudiants que llegeixen llibres de Tecnologia}`
- `H = {estudiants que llegeixen llibres d'História}`
- `F = {estudiants que llegeixen llibres de Ficció}`

A més, saps que:
- `T ⊆ S` (on `S` és el conjunt de tots els estudiants)
- `H ⊆ S`
- `F ⊆ S`
- No tots els estudiants llegeixen tecnologia.
- Alguns estudiants llegeixen historia i ficció alhora.
- Cap estudiant llegeix només tecnologia (és a dir, qui llegeix tecnologia llegeix almenys un altre gènere).

a) Dibuixa un diagrama de Venn que mostri `T`, `H`, `F` dins de `S`.

b) En el diagrama, marca i etiqueta:
   - La regió de `T` (estudiants de tecnologia)
   - La regió de `H ∩ F` (estudiants que llegeixen história i ficció)
   - La regió de estudiants que **no** llegeixen cap dels tres gèneres.

c) Justifica per què `T ≠ S` basat en la informació "No tots els estudiants llegeixen tecnologia."

d) Explica per què la condició "Cap estudiant llegeix només tecnologia" significa que `T` no té elements que estiguin exclusivament en `T` (és a dir, `T` és dins de la unió `H ∪ F`).

**Solució:**

a) Diagrama de Venn (representació ASCII):

```
       __________________S__________________
      /                                      \
     /   ________________  ________________  \
    |   /      T         \/        H       \ |
    |  | \                /\               / |
    |  |  \______________/  \             /  |
    |  |     (Tec)      |     \           /   |
    |  |                |      \___  ____/    |
    |  |________________|          \/         |
    |  /(Ficció) _________________(H∩F)______\|
    | /  F                                   |
    |/________________________  ______________\
    |        (Cap dels tres)                 |
    |______________________________________|
```

b) Regions marcades:
   - **Regió de `T`**: Estudiants que llegeixen tecnologia (però que també llegeixen altra cosa).
   - **Regió de `H ∩ F`**: La intersecció entre história i ficció (estudiants que llegeixen ambdós).
   - **Regió de cap dels tres**: Estudiants que no llegeixen tecnologia, historia, ni ficció.

c) Justificació de `T ≠ S`:
   - Per definició, `T = S` significaria que **tots els estudiants** llegeixen tecnologia.
   - Però la informació diu "No tots els estudiants llegeixen tecnologia."
   - Per tant, hi ha almenys un estudiant en `S` que **no** pertany a `T`.
   - Conclusió: **`T ⊂ S`** (és a dir, `T ≠ S` i `T ⊆ S`).

d) Justificació de "Cap estudiant llegeix només tecnologia":
   - Si algú llegeix "només tecnologia", estarien en `T` però **no** en `H` i **no** en `F`.
   - La condició diu que és **impossible** (cap estudiant és en aquesta situació).
   - Per tant, **tots els elements de `T` pertanyen a `H ∪ F`** (és a dir, `T ⊆ (H ∪ F)`).
   - Matemàticament: No hi ha cap "regió exclusiva de `T`" en el diagrama; `T` està completament dins de la unió de `H` i `F`.

**Concepte avaluat:** Diagrames de Venn amb múltiples conjunts, interseccions, unió, subconjunts amb restriccions complexes, raonament lògic avançat.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Símbols `⊆`, `⊂`, `⊄` | Moderat |
| 2 | Enumeració de subconjunts, `2^n` | Intermedi |
| 3 | Element vs subconjunt | Moderat |
| 4 | Diagrames de Venn | Intermedi |
| 5 | Conjunt buit com a subconjunt | Moderat |
| 6 | Transitivitat | Intermedi |
| 7 | Aplicació a formes geomètriques | Intermedi |
| 8 | Distinció `⊆` vs `⊂` vs `=` | Intermedi |
| 9 | Construcció amb restriccions | Desafiador |
| 10 | Venn avançat amb interseccions | Desafiador |

---

## 🎯 Consells per als Estudiants

- **Exercicis 1–3, 5:** Practica identificant correctament `⊆`, `⊂`, i distingint entre element i conjunt.
- **Exercicis 2, 4, 6–8:** Treballa amb enumeracions sistemàtiques, diagrames de Venn, i propietats com transitivitat.
- **Exercicis 9–10:** Consolida amb problemes multi-nivell que requereixen construcció, restriccions, i raonament lògic complex.

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre `⊆` amb `∈`**: Recorda que `⊆` és per a conjunts, `∈` és per a elements.
2. **Oblidar que tot conjunt és subconjunt de si mateix**: `A ⊆ A` sempre és vertader.
3. **Confondre subconjunt amb subconjunt propi**: `A ⊂ B` és més restringit que `A ⊆ B`.
4. **Neglect the empty set**: `∅ ⊆ A` per a qualsevol `A`.
5. **Diagrama de Venn**: Assegura't que els cercles es superposen correctament per representar les relacions.


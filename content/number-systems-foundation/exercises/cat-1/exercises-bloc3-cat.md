# Exercicis - Mòdul 1: Bloc 3 – Jerarquia de Conjunts Numèrics ℕ→ℤ→ℚ

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Aplicació Directa: Classificació de Nombres

**Enunciat:**

Classifica els següents nombres assenyalant si pertanyen a `ℕ`, `ℤ`, `ℚ`, o cap dels anteriors:

a) `5`
b) `-3`
c) `0`
d) `1/2`
e) `√2`

Per a cada nombre, escriu la notació correcta usant `∈` o `∉`.

**Solució:**

a) `5 ∈ ℕ` (és un nombre natural positiu)
   - `5 ∈ ℤ` (tots els naturals són enters)
   - `5 ∈ ℚ` (es pot escriure com `5/1`)

b) `-3 ∉ ℕ` (els naturals no inclouen negatius)
   - `-3 ∈ ℤ` (és un nombre enter negatiu)
   - `-3 ∈ ℚ` (es pot escriure com `-3/1`)

c) `0 ∉ ℕ` (per convencionalitat, ℕ comença en 1; algunes convencions inclouen 0)
   - `0 ∈ ℤ` (zero és un nombre enter)
   - `0 ∈ ℚ` (es pot escriure com `0/1`)

d) `1/2 ∉ ℕ` (no és un nombre natural)
   - `1/2 ∉ ℤ` (no és un nombre enter)
   - `1/2 ∈ ℚ` (és una fracció amb numerador i denominador enters)

e) `√2 ∉ ℕ`, `√2 ∉ ℤ`, `√2 ∉ ℚ` (√2 és irracional; no es pot escriure com `a/b`)

**Concepte avaluat:** Comprensió de les definicions de ℕ, ℤ, ℚ; classificació precisa de nombres.

---

### **Exercici 2** 🟦 (1.1 punts) – Jerarquia i Inclusió

**Enunciat:**

Usa els símbols `⊆`, `⊂`, o `⊄` per completar:

a) `ℕ ___ ℤ`

b) `ℤ ___ ℚ`

c) `ℕ ___ ℚ`

d) `ℤ ___ ℕ`

Per a cada afirmació, justifica breument per què és correcta.

**Solució:**

a) `ℕ ⊂ ℤ` (subconjunt propi)
   - Justificació: Tot nombre natural és enter, però existeixen enters (com `-1`) que no són naturals.

b) `ℤ ⊂ ℚ` (subconjunt propi)
   - Justificació: Tot nombre enter `n` es pot escriure com `n/1`, però existeixen racionals (com `1/2`) que no són enters.

c) `ℕ ⊂ ℚ` (subconjunt propi)
   - Justificació: Per transitivitat (`ℕ ⊂ ℤ` i `ℤ ⊂ ℚ`, així `ℕ ⊂ ℚ`). Un nombre natural `n` és racional perquè `n = n/1`.

d) `ℤ ⊄ ℕ` (no és subconjunt)
   - Justificació: Existeixen enters (com `-1`) que **no** pertanyen a ℕ.

**Concepte avaluat:** Jerarquia de conjunts numèrics, relacions de subconjunt, transitivitat.

---

### **Exercici 3** ⭐ (0.9 punts) – Representació en la Recta Numèrica

**Enunciat:**

Dibuixa una recta numèrica i marca les posicions dels següents nombres:

`-2, -1/2, 0, 1, 3/2, 2, 5/2`

a) Indica quins pertanyen a `ℕ`, quins a `ℤ` (però no a `ℕ`), i quins a `ℚ` (però no a `ℤ`).

b) Ordena els nombres de menor a major.

**Solució:**

a) Recta numèrica:

```
─────┼─────┼─────┼─────┼─────┼─────┼─────
    -2   -1/2  0    1    3/2   2   5/2
     │     │    │    │    │    │    │
  (ℤ,ℚ) (ℚ)  (ℤ,ℚ) (ℕ,ℤ,ℚ) (ℚ) (ℕ,ℤ,ℚ) (ℚ)
```

- **En ℕ**: `1, 2`
- **En ℤ (però no ℕ)**: `-2, 0`
- **En ℚ (però no ℤ)**: `-1/2, 3/2, 5/2`

b) Ordre de menor a major:
   
   `-2 < -1/2 < 0 < 1 < 3/2 < 2 < 5/2`

**Concepte avaluat:** Visualització espacial de nombres, ordenació, classificació simultània en múltiples conjunts.

---

### **Exercici 4** 🟦 (1.2 punts) – Representació de la Jerarquia

**Enunciat:**

Dibuixa un diagrama de jerarquia (tipus "caixes anidades") que mostri les relacions:

`ℕ ⊂ ℤ ⊂ ℚ`

a) Etiqueta cada nivell amb exemples de nombres que pertanyen a cada conjunt.

b) Per a cada exemple, verifica que pertany a tots els conjunts del seu nivell cap amunt.

c) Identifica la regió que conté números que estan en `ℚ` però **no** en `ℤ`.

**Solució:**

a) Diagrama de jerarquia:

```
      ┌─────────────────────────────────┐
      │  ℚ (Racionals)                 │
      │  Exemples: 1/2, -3/4, 2, -1   │
      │                                 │
      │  ┌──────────────────────────┐  │
      │  │ ℤ (Enters)               │  │
      │  │ Exemples: -2, -1, 0, 1, 2│  │
      │  │                          │  │
      │  │  ┌─────────────────────┐│  │
      │  │  │ ℕ (Naturals)        ││  │
      │  │  │ Exemples: 1, 2, 3  ││  │
      │  │  └─────────────────────┘│  │
      │  │                          │  │
      │  └──────────────────────────┘  │
      │                                 │
      └─────────────────────────────────┘
```

b) Verificació per a cada exemple:
   - `1/2 ∈ ℚ` ✓ (és una fracció)
   - `-3/4 ∈ ℚ` ✓, però `-3/4 ∉ ℤ`
   - `2 ∈ ℚ` ✓, `2 ∈ ℤ` ✓, `2 ∈ ℕ` ✓
   - `-1 ∈ ℚ` ✓, `-1 ∈ ℤ` ✓, però `-1 ∉ ℕ`

c) Regió en `ℚ` però **no** en `ℤ`:
   - Aquesta regió és la **corona externa** del rectangle `ℚ` que està fora de `ℤ`.
   - Conté fraccions com `1/2, 3/7, -5/3`, és a dir, nombres racionals no enters.

**Concepte avaluat:** Visualització de jerarquies, relacions d'inclusió encadenades, interpretació de diagrames.

---

### **Exercici 5** ⭐ (0.8 punts) – Conversió entre Representacions

**Enunciat:**

Converteix els següents nombres enters a fraccions (és a dir, representa'ls en forma `a/b`):

a) `7 = ___/___`

b) `-4 = ___/___`

c) `0 = ___/___`

Explica per què aquesta conversió demostra que tot enter és racional.

**Solució:**

a) `7 = 7/1` (o qualsevol múltiple: `14/2`, `21/3`, etc.)

b) `-4 = -4/1` (o `-8/2`, `-12/3`, etc.)

c) `0 = 0/1` (o `0/2`, `0/5`, etc.)

Explicació:
- Per definició, un nombre racional és qualsevol nombre de la forma `a/b` on `a` i `b` són enters i `b ≠ 0`.
- Cada enter `n` pot escriure's com `n/1` (amb `b = 1 ≠ 0`).
- Per tant, **cada enter compleix la definició de racional**, és a dir, `ℤ ⊂ ℚ`.

**Concepte avaluat:** Connexió entre notació fraccionaria i membership, demostració de relacions d'inclusió.

---

### **Exercici 6** 🟦 (1.0 punt) – Densitat de Racionals

**Enunciat:**

Una de les propietats clau dels racionals és que són **densos**: entre qualsevol parell de nombres racionals, hi ha un altre nombre racional.

a) Donats `r = 1/4` i `s = 1/2`, troba **almenys tres** nombres racionals estrictament entre ells.

b) Verifica que els nombres que has trobat estan efectivament entre `r` i `s` (és a dir, `1/4 < ? < 1/2`).

c) Com explica aquesta propietat de densitat que els racionals són "innumerables" en quant a ordre (tot i que matemàticament són numerables)?

**Solució:**

a) Nombres entre `1/4` i `1/2`:

Estratègia: Convertir a denominador comú o usar la mitjana.

- Mitja de `1/4` i `1/2`: `(1/4 + 1/2) / 2 = (1/4 + 2/4) / 2 = (3/4) / 2 = 3/8`
- Mitja de `1/4` i `3/8`: `(1/4 + 3/8) / 2 = (2/8 + 3/8) / 2 = (5/8) / 2 = 5/16`
- Mitja de `3/8` i `1/2`: `(3/8 + 1/2) / 2 = (3/8 + 4/8) / 2 = (7/8) / 2 = 7/16`

Tres nombres racionals: `5/16, 3/8, 7/16` (o qualsevol altre combinació vàlida).

b) Verificació:
   - `1/4 = 4/16`
   - `5/16` (és a dir, `4/16 < 5/16 < 8/16`) ✓
   - `3/8 = 6/16` (és a dir, `4/16 < 6/16 < 8/16`) ✓
   - `7/16` (és a dir, `4/16 < 7/16 < 8/16`) ✓
   - `1/2 = 8/16`

c) Explicació de densitat:
   - Densitat significa que **entre qualsevol parell de racionals, hi ha infinits més**.
   - Això fa que els racionals semblin "omplir tot l'espai", però...
   - Matemàticament, ℚ és **numerable** (es pot listar en una seqüència), mentre que ℝ (que inclou irracionals) és **no numerable**.
   - La densitat reflecteix que ℚ és molt "ric" en estructura, tot i ser menys abundant que ℝ.

**Concepte avaluat:** Propietats de densitat, construcció de racionals intermedis, diferència entre estructura ordem i cardinalitat.

---

### **Exercici 7** 🟦 (1.1 punts) – Classificació de Nombres: Decisió Multiple

**Enunciat:**

Per a cada nombre, marca tots els conjunts als quals pertany (ℕ, ℤ, ℚ):

| Nombre | ℕ | ℤ | ℚ |
|--------|---|---|---|
| a) 3   |   |   |   |
| b) -2  |   |   |   |
| c) 2/5 |   |   |   |
| d) 0   |   |   |   |
| e) -7/3|   |   |   |

**Solució:**

| Nombre | ℕ | ℤ | ℚ |
|--------|---|---|---|
| a) 3   | ✓ | ✓ | ✓ |
| b) -2  | ✗ | ✓ | ✓ |
| c) 2/5 | ✗ | ✗ | ✓ |
| d) 0   | ✗ | ✓ | ✓ |
| e) -7/3| ✗ | ✗ | ✓ |

Justificacions:
- **a) 3**: Natural (enter positiu), enter, i racional (`3/1`).
- **b) -2**: No és natural (negatiu), però és enter i racional (`-2/1`).
- **c) 2/5**: No és enter (és fracció), però és racional per definició.
- **d) 0**: No és natural (per convencionalitat), és enter, i racional (`0/1`).
- **e) -7/3**: No és enter (no es pot simplificar a un enter), però és racional (fracció amb denominador no zero).

**Concepte avaluat:** Classificació sistemàtica, aplicació de definicions a diversos casos.

---

### **Exercici 8** 🟦 (1.3 punts) – Transitivitat i Cadena de Relacions

**Enunciat:**

Donats els nombres `2`, `1/3`, i `-5`:

a) Classifica cada nombre en un o més dels conjunts ℕ, ℤ, ℚ.

b) Escriu una cadena de relacions d'inclusió que inclogui els conjunts als quals pertanyen aquests nombres.

c) Verifica la **transitivitat**: si el nombre pertany a ℕ, llavors pertany a ℤ i a ℚ per la cadena `ℕ ⊂ ℤ ⊂ ℚ`.

d) Per a aquells nombres que pertanyen a ℤ però no a ℕ, explica per què la transitivitat assegura que sí pertanyen a ℚ.

**Solució:**

a) Classificació:
   - `2 ∈ ℕ`, `2 ∈ ℤ`, `2 ∈ ℚ`
   - `1/3 ∉ ℕ`, `1/3 ∉ ℤ`, `1/3 ∈ ℚ`
   - `-5 ∉ ℕ`, `-5 ∈ ℤ`, `-5 ∈ ℚ`

b) Cadena de relacions:
   - `ℕ ⊂ ℤ ⊂ ℚ`
   
   Això significa:
   - Tots els nombres naturals són enters.
   - Tots els enters són racionals.

c) Verificació de transitivitat per a `2`:
   - `2 ∈ ℕ`
   - Per la relació `ℕ ⊂ ℤ`, es dedueix `2 ∈ ℤ` ✓
   - Per la relació `ℤ ⊂ ℚ`, es dedueix `2 ∈ ℚ` ✓

d) Explicació per a `-5` (a ℤ però no a ℕ):
   - `-5 ∈ ℤ` (és enter)
   - Per la relació `ℤ ⊂ ℚ`, es dedueix `-5 ∈ ℚ` ✓
   - La transitivitat garanteix que qualsevol enter, tant si és natural com si no, és racional.

**Concepte avaluat:** Aplicació de transitivitat a casos concrets, deducció sistemàtica.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Jerarquia amb Exclusions

**Enunciat:**

Considera els conjunts:
- `A = {nombres que pertanyen a ℚ però no a ℤ}`
- `B = {nombres que pertanyen a ℤ però no a ℕ}`
- `C = {nombres que pertanyen a ℕ}`

a) Proporciona **almenys dos exemples** per a cada conjunt `A`, `B`, i `C`.

b) Expressa els conjunts `A` i `B` en notació de diferència de conjunts:
   - `A = ℚ \ ___`
   - `B = ℤ \ ___`

c) Verifica que els tres conjunts `A`, `B`, `C` són **disjunts** (és a dir, no comparteixen elements).

d) Verifica que la unió `A ∪ B ∪ C = ℚ` (és a dir, cobreixen tots els racionals).

**Solució:**

a) Exemples:
   - **`A` (racionals no enters)**: `1/2, 3/4, -2/5, 7/3`
   - **`B` (enters no naturals)**: `-1, -2, 0`
   - **`C` (naturals)**: `1, 2, 3, 5`

b) Expressió en diferència de conjunts:
   - `A = ℚ \ ℤ` (racionals menys enters)
   - `B = ℤ \ ℕ` (enters menys naturals)

c) Verificació de disjunció:
   - `A ∩ B = ∅` perquè `A` conté només no-enters i `B` conté només enters.
   - `A ∩ C = ∅` perquè `A` conté només no-enters i `C` conté enters.
   - `B ∩ C = ∅` perquè `B` conté enters no naturals (negatius o zero) i `C` conté naturals positius.

d) Verificació que `A ∪ B ∪ C = ℚ`:
   - Per jerarquia: `ℕ ⊂ ℤ ⊂ ℚ`
   - Tots els racionals es classifiquen en una de tres categories:
     1. Naturals (ℕ) → pertanyen a `C`
     2. Enters no naturals → pertanyen a `B`
     3. Racionals no enters → pertanyen a `A`
   - Per tant, `A ∪ B ∪ C` cobreix tots els racionals, és a dir, `A ∪ B ∪ C = ℚ` ✓

**Concepte avaluat:** Jerarquies amb exclusions, operacions de diferència, disjunció i unió, particions de conjunts.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Irracionals i Extensió de Jerarquia

**Enunciat:**

Fins ara hem estudiat `ℕ ⊂ ℤ ⊂ ℚ`. Però la jerarquia continua:

`ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ` (on ℝ representa els **nombres reals**, que inclouen tant racionals com irracionals).

Donats els nombres: `2, √2, 0, π, 1/3, -5`

a) Classifica cada nombre en els conjunts `ℕ`, `ℤ`, `ℚ`, `ℝ`.

b) Identifica quins nombres pertanyen a `ℝ` però **no** a `ℚ` (aquests són els **irracionals**).

c) Dibuixa una jerarquia expandida que mostri `ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ` i localitza els nombres irracionals.

d) Explica per què `ℚ ⊂ ℝ` però `ℚ ≠ ℝ` (és a dir, per què els reals són més gran que els racionals).

**Solució:**

a) Classificació:

| Nombre | ℕ | ℤ | ℚ | ℝ |
|--------|---|---|---|---|
| 2      | ✓ | ✓ | ✓ | ✓ |
| √2     | ✗ | ✗ | ✗ | ✓ |
| 0      | ✗ | ✓ | ✓ | ✓ |
| π      | ✗ | ✗ | ✗ | ✓ |
| 1/3    | ✗ | ✗ | ✓ | ✓ |
| -5     | ✗ | ✓ | ✓ | ✓ |

b) Nombres en `ℝ` però **no** en `ℚ` (irracionals):
   - `√2` (no es pot escriure com fracció de sencers)
   - `π` (constant irracional, aproximadament 3.14159...)

c) Diagrama jeràrquic expandit:

```
      ┌─────────────────────────────────────────────────┐
      │  ℝ (Nombres Reals)                             │
      │  Exemples: Tots els anteriors + √2, π, e, ... │
      │                                                 │
      │  ┌───────────────────────────────────────────┐ │
      │  │ ℚ (Racionals)                             │ │
      │  │ Exemples: 2, 0, 1/3, -5                  │ │
      │  │                                            │ │
      │  │  ┌────────────────────────────────────┐  │ │
      │  │  │ ℤ (Enters)                         │  │ │
      │  │  │ Exemples: 2, 0, -5                 │  │ │
      │  │  │                                    │  │ │
      │  │  │  ┌──────────────────────────────┐ │  │ │
      │  │  │  │ ℕ (Naturals)                 │ │  │ │
      │  │  │  │ Exemples: 2                  │ │  │ │
      │  │  │  └──────────────────────────────┘ │  │ │
      │  │  │                                    │  │ │
      │  │  └────────────────────────────────────┘  │ │
      │  │                                            │ │
      │  └───────────────────────────────────────────┘ │
      │                                                 │
      │  **Irracionals** (ℝ \ ℚ):                     │
      │  Ubicats fora de ℚ però dins ℝ              │
      │  Exemples: √2, π                             │
      │                                                 │
      └─────────────────────────────────────────────────┘
```

d) Explicació de `ℚ ⊂ ℝ` però `ℚ ≠ ℝ`:
   - `ℚ ⊂ ℝ` perquè tots els racionals són reals (tot nombre que es pot expressar com fracció és un nombre real).
   - `ℚ ≠ ℝ` perquè existeixen nombres reals que **no** són racionals, anomenats **irracionals** (com `√2` i `π`).
   - Els irracionals no es poden escriure com `a/b` amb `a, b` enters. Més bé, les seves representacions decimals són infinites i no periòdiques.
   - Per tant, **els reals són una extensió dels racionals** que inclou aquesta nova classe de nombres.

**Concepte avaluat:** Extensió de jerarquies, introducció a irracionals, diferència entre `⊂` i `=`, comprensió de jerarquies multinivelades.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Classificació de nombres en ℕ, ℤ, ℚ | Moderat |
| 2 | Jerarquia i inclusió (`⊂`, `⊆`) | Intermedi |
| 3 | Recta numèrica i ordenació | Moderat |
| 4 | Diagrama de jerarquia visual | Intermedi |
| 5 | Conversió a representació fraccionaria | Moderat |
| 6 | Densitat de racionals | Intermedi |
| 7 | Classificació múltiple en taula | Intermedi |
| 8 | Transitivitat de relacions | Intermedi |
| 9 | Jerarquies amb exclusions i particions | Desafiador |
| 10 | Extensió a ℝ, introducció a irracionals | Desafiador |

---

## 🎯 Consells per als Estudiants

- **Exercicis 1, 3, 5**: Practica la classificació de nombres individuals i la representació en rectes numèriques.
- **Exercicis 2, 4, 6–8**: Enteneu profundament la jerarquia `ℕ ⊂ ℤ ⊂ ℚ` i les propietats de cada conjunt.
- **Exercicis 9–10**: Consolideu amb conceptes avançats: particions, extensions de jerarquies, i introducció als irracionals.

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre `0 ∈ ℕ` amb `0 ∉ ℕ`**: Depén de la convencionalitat; verifica sempre en el context del curs.
2. **Pensar que les fraccions no són racionals**: Les fraccions (`a/b` amb `b ≠ 0`) **són la definició** de racionals.
3. **Creure que tot enter és natural**: Els enters negatius (`-1, -2, ...`) i zero no són naturals (en la majoria de convencions).
4. **Negligir que els naturals es poden escriure com fraccions**: Recordeu que `5 = 5/1`, per tant `5 ∈ ℚ`.
5. **Ignorar la densitat de racionals**: Entre qualsevol parell de racionals hi ha infinits més; això és important per entendre per què ℚ és tan "ric".
6. **No distingir irracionals de racionals**: Alguns nombres reals (com `√2` i `π`) **no** es poden escriure com fraccions; aquests són irracionals.

---

## 🔗 Connexions amb altres Blocs

- **Bloc 1 (Conjunts i Notació)**: Usa subconjunts per expressar jerarquies numèriques.
- **Bloc 2 (Subconjunts i Venn)**: Els diagrames de Venn es poden usar per visualitzar aquestes jerarquies.
- **Bloc 4 (Irracionals)**: Exposa la limitació dels racionals i la necessitat dels reals.
- **Mòdul 3 (Decimals)**: Connecta racionals amb representacions decimals finites o periòdiques.


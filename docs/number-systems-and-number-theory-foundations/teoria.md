# SISTEMES DE NUMERACIÓ I VALOR POSICIONAL

**Mòdul:** Fonaments dels Sistemes Numèrics i Teoria de Nombres - Dia 1  
**Nivell:** Estudiants superdotats (9-10 anys)  
**Durada:** 20 minuts (teoria)

---

## 📚 INTRODUCCIÓ

Els nombres són el llenguatge de les matemàtiques. Avui descobrirem els diferents tipus de nombres que existeixen, com els representem i com treballem amb nombres molt grans o molt petits.

Però abans, necessitem aprendre un **llenguatge especial** que els matemàtics utilitzen per organitzar i classificar els nombres: la **notació de conjunts**.

---

## 🔤 TEORIA DE CONJUNTS: EL LLENGUATGE DE LES MATEMÀTIQUES

### **Què és un conjunt?**

Un **conjunt** és una col·lecció **ben definida** d'objectes diferents. És com una "caixa" o un "grup" que conté elements que comparteixen alguna característica.

**Important:** Quan diem "ben definida" vol dir que sempre podem decidir si un objecte pertany o no al conjunt.

**Exemples quotidians:**

1. **Conjunt d'estudiants:** {Maria, Joan, Anna, Pere}
2. **Conjunt de dies de la setmana:** {dilluns, dimarts, dimecres, dijous, divendres, dissabte, diumenge}
3. **Conjunt de vocals:** {a, e, i, o, u}
4. **Conjunt de números parells petits:** {2, 4, 6, 8}

### **Com escrivim conjunts?**

Utilitzem **claus { }** (també anomenades "braçades") per delimitar un conjunt:

```
A = {1, 2, 3, 4, 5}
```

Això es llegeix: "A és el conjunt format pels elements 1, 2, 3, 4 i 5"

**Més exemples:**
```
Vocals = {a, e, i, o, u}
Parells = {2, 4, 6, 8, 10}
Colors = {vermell, blau, verd}
```

---

### **PROPIETATS FONAMENTALS DELS CONJUNTS**

#### **1. Els elements NO es repeteixen**

En un conjunt, cada element apareix **només una vegada**. No importa quantes vegades l'escrivim, només compta una vegada.

**Exemples:**

❌ **Incorrecte (amb repeticions):** {1, 2, 2, 3, 3, 3}  
✅ **Correcte (sense repeticions):** {1, 2, 3}

❌ **Incorrecte:** {a, b, b, c, a}  
✅ **Correcte:** {a, b, c}

**Per què?** Perquè un conjunt només ens diu **quins** elements hi ha, no **quantes vegades** hi són.

---

#### **2. L'ordre NO importa**

Els elements d'un conjunt es poden escriure en qualsevol ordre. Tots aquests conjunts són **iguals**:

```
{1, 2, 3} = {2, 1, 3} = {3, 2, 1} = {1, 3, 2}
```

Tots representen el mateix conjunt!

**Més exemples:**
```
{a, e, i, o, u} = {u, o, i, e, a}
{vermell, blau, verd} = {blau, verd, vermell}
```

**Diferència important:** En una llista o seqüència SÍ importa l'ordre, però en un conjunt NO.

---

#### **3. El conjunt buit (∅)**

El **conjunt buit** és el conjunt que **no té cap element**. És com una caixa buida.

**Símbols per representar-lo:**
- **∅** (símbol especial)
- **{ }** (claus sense res dins)

**Exemples de conjunts buits:**

1. El conjunt de mesos amb 32 dies → ∅ (no existeix cap mes amb 32 dies)
2. El conjunt de nombres naturals negatius → ∅ (els naturals són positius)
3. El conjunt de quadrats amb 3 costats → ∅ (els quadrats tenen 4 costats)

**Important:** 
- ∅ NO és el mateix que {∅}
- ∅ és el conjunt buit (0 elements)
- {∅} és un conjunt amb un element (que és el conjunt buit)

---

#### **4. Conjunts finits i infinits**

**Conjunt finit:** Té un nombre concret d'elements (es poden comptar).

**Exemples:**
```
Dies de la setmana = {dilluns, dimarts, ..., diumenge} → 7 elements
Dígits = {0, 1, 2, 3, 4, 5, 6, 7, 8, 9} → 10 elements
```

**Conjunt infinit:** Té infinits elements (no es poden acabar de comptar).

**Exemples:**
```
Nombres naturals = {1, 2, 3, 4, 5, ...} → infinits elements
Nombres parells = {2, 4, 6, 8, 10, ...} → infinits elements
```

Els tres punts (**...**) indiquen que el conjunt continua infinitament.

---

### **NOTACIÓ DE PERTINENÇA: ∈ i ∉**

#### **El símbol ∈ (pertany a)**

Utilitzem **∈** per indicar que un element **està dins** d'un conjunt.

**Es llegeix:** "pertany a" o "és element de"

**Exemples:**

```
A = {1, 2, 3, 4, 5}

2 ∈ A    (el 2 pertany a A)
5 ∈ A    (el 5 pertany a A)
```

**Més exemples:**
```
Vocals = {a, e, i, o, u}

e ∈ Vocals    (la "e" és una vocal)
i ∈ Vocals    (la "i" és una vocal)
```

#### **El símbol ∉ (no pertany a)**

Utilitzem **∉** per indicar que un element **NO està dins** d'un conjunt.

**Es llegeix:** "no pertany a" o "no és element de"

**Exemples:**

```
A = {1, 2, 3, 4, 5}

7 ∉ A    (el 7 NO pertany a A)
10 ∉ A   (el 10 NO pertany a A)
```

**Més exemples:**
```
Vocals = {a, e, i, o, u}

b ∉ Vocals    (la "b" NO és una vocal)
k ∉ Vocals    (la "k" NO és una vocal)
```

---

### **RELACIÓ DE SUBCONJUNT: ⊂**

#### **Què significa "subconjunt"?**

Un conjunt **A** és un **subconjunt** de **B** (escrit **A ⊂ B**) si **tots els elements d'A també són elements de B**.

**Es llegeix:** "A és subconjunt de B" o "A està contingut en B"

#### **Exemple visual amb diagrames:**

**Diagrama de Venn:** Un diagrama de Venn és una representació visual dels conjunts utilitzant cercles o òvals.

**Exemple 1: Subconjunt (A ⊂ B)**

Quan A és subconjunt de B, el cercle d'A està **completament dins** del cercle de B:

```
         ┌─────────────────────────┐
         │          B              │
         │    ┌──────────┐         │
         │    │    A     │         │
         │    │  2, 4    │         │
         │    └──────────┘         │
         │  1, 3, 5, 6             │
         └─────────────────────────┘

A = {2, 4}
B = {1, 2, 3, 4, 5, 6}

A ⊂ B perquè tots els elements d'A (2 i 4) també són a B
```

**Exemple 2: Conjunts que es solapen (intersecció)**

Quan dos conjunts comparteixen alguns elements però cap és subconjunt de l'altre:

```
         ┌──────────┐  ┌──────────┐
         │    A     │  │    B     │
         │       ┌──┼──┼──┐       │
         │    1  │  │  │  │  4    │
         │       │ 2, 3 │         │
         │       └──┼──┼──┘       │
         └──────────┘  └──────────┘

A = {1, 2, 3}
B = {2, 3, 4}

Elements comuns: {2, 3} (intersecció)
A NO és subconjunt de B (perquè 1 ∉ B)
B NO és subconjunt de A (perquè 4 ∉ A)
```

**Exemple 3: Conjunts disjunts (sense elements comuns)**

```
         ┌──────────┐        ┌──────────┐
         │    A     │        │    B     │
         │          │        │          │
         │  1, 3, 5 │        │  2, 4, 6 │
         │          │        │          │
         └──────────┘        └──────────┘

A = {1, 3, 5} (nombres senars)
B = {2, 4, 6} (nombres parells)

Cap element en comú - són conjunts disjunts
```

#### **Exemples pràctics:**

**Exemple 1:**
```
A = {1, 2, 3}
B = {1, 2, 3, 4, 5, 6}

A ⊂ B? SÍ ✓
Per què? Perquè 1 ∈ B, 2 ∈ B i 3 ∈ B
```

**Exemple 2:**
```
Vocals = {a, e, i, o, u}
Lletres = {a, b, c, d, e, f, g, ..., z}

Vocals ⊂ Lletres? SÍ ✓
Per què? Totes les vocals són lletres
```

**Exemple 3 (NO és subconjunt):**
```
A = {1, 2, 7}
B = {1, 2, 3, 4, 5}

A ⊂ B? NO ✗
Per què? Perquè 7 ∉ B
```

#### **Propietat important:**

**Tot conjunt és subconjunt de si mateix:**
```
A ⊂ A (sempre és cert)
```

**El conjunt buit és subconjunt de tots els conjunts:**
```
∅ ⊂ A (sempre és cert per a qualsevol conjunt A)
```

---

### **TAULA RESUM DE SÍMBOLS**

| Símbol | Nom | Significat | Exemple | Es llegeix |
|--------|-----|-----------|---------|-----------|
| **{ }** | Claus | Delimita un conjunt | {1, 2, 3} | "Conjunt d'1, 2 i 3" |
| **∈** | Pertany | Element dins del conjunt | 3 ∈ {1, 2, 3} | "3 pertany al conjunt" |
| **∉** | No pertany | Element fora del conjunt | 5 ∉ {1, 2, 3} | "5 no pertany al conjunt" |
| **⊂** | Subconjunt | Tots els elements d'A estan a B | A ⊂ B | "A és subconjunt de B" |
| **∅** | Conjunt buit | Conjunt sense elements | ∅ = { } | "Conjunt buit" |
| **...** | Punts suspensius | Continua infinitament | {1, 2, 3, ...} | "1, 2, 3 i així successivament" |

---

### **SÍMBOLS ESPECIALS DELS CONJUNTS NUMÈRICS**

Els matemàtics utilitzen **símbols especials** per representar els conjunts de nombres més importants:

#### **ℕ - Nombres Naturals**

```
ℕ = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, ...}
```

- **Símbol:** ℕ (lletra N amb doble barra)
- **Significat:** "Natural" (els primers nombres que els humans van utilitzar)
- **Ús:** Per comptar objectes, persones, dies...
- **Característiques:** Sempre positius, comencen amb l'1, infinits

**Per què existeixen?** 
Els humans necessitaven comptar: "Tinc 3 ovelles", "Han passat 7 dies".

---

#### **ℤ - Nombres Enters**

```
ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}
```

- **Símbol:** ℤ (de l'alemany "Zahlen" = nombres)
- **Significat:** Inclou negatius, zero i positius
- **Ús:** Temperatures, deutes, altituds, anys abans de Crist
- **Característiques:** Infinits en ambdues direccions (+ i -)

**Per què necessitem més que ℕ?** 
La vida real té situacions negatives:
- "Tinc -20 euros de deute"
- "La temperatura és -5°C"
- "L'edifici té 3 plantes sota terra: -1, -2, -3"

Amb només ℕ no podríem representar aquestes situacions!

---

#### **ℚ - Nombres Racionals**

```
ℚ = {totes les fraccions a/b on a, b ∈ ℤ i b ≠ 0}
```

- **Símbol:** ℚ (de "Quotient" = quocient, fracció)
- **Significat:** Tots els nombres que es poden escriure com a fraccions
- **Ús:** Mesurar parts, percentatges, decimals
- **Característiques:** Inclou enters, decimals exactes i periòdics

**Exemples:**
- Fraccions: 1/2, 3/4, -5/3
- Decimals exactes: 0.5 (= 1/2), 0.25 (= 1/4)
- Decimals periòdics: 0.333... (= 1/3)
- Enters: 7 (= 7/1), -3 (= -3/1)

**Per què necessitem més que ℤ?** 
No tot és sencer en la vida real:
- "He menjat 1/4 de la pizza"
- "L'ample de la taula és 1.5 metres"
- "He aprovat amb un 7.5"
- "El mercat va pujar un 0.8%"

Amb només ℤ no podríem mesurar parts o divisions!

---

### **JERARQUIA DELS CONJUNTS NUMÈRICS: ℕ ⊂ ℤ ⊂ ℚ**

#### **Visualització amb Diagrames de Venn:**

```
    ┌─────────────────────────────────────┐
    │              ℚ (Racionals)          │
    │   -1/2, 0.5, 2.7, -3.14...         │
    │                                     │
    │   ┌──────────────────────────┐      │
    │   │      ℤ (Enters)          │      │
    │   │  -5, -2, 0, 3, 7...      │      │
    │   │                          │      │
    │   │   ┌─────────────────┐    │      │
    │   │   │  ℕ (Naturals)   │    │      │
    │   │   │  1, 2, 3, 4...  │    │      │
    │   │   │                 │    │      │
    │   │   └─────────────────┘    │      │
    │   │                          │      │
    │   └──────────────────────────┘      │
    │                                     │
    └─────────────────────────────────────┘
```

**Què significa ℕ ⊂ ℤ ⊂ ℚ?**

1. **ℕ ⊂ ℤ** (Els naturals són subconjunt dels enters)
   - Tot nombre natural també és enter
   - Exemples: 5 ∈ ℕ i també 5 ∈ ℤ
   - Però: -3 ∈ ℤ però -3 ∉ ℕ

2. **ℤ ⊂ ℚ** (Els enters són subconjunt dels racionals)
   - Tot enter es pot escriure com a fracció: 7 = 7/1
   - Exemples: -3 ∈ ℤ i també -3 ∈ ℚ (perquè -3 = -3/1)
   - Però: 1/2 ∈ ℚ però 1/2 ∉ ℤ

3. **ℕ ⊂ ℚ** (Per transitivitat)
   - Si ℕ ⊂ ℤ i ℤ ⊂ ℚ, llavors ℕ ⊂ ℚ
   - Tot natural també és racional: 5 = 5/1

#### **Taula Comparativa:**

| Característiques | ℕ | ℤ | ℚ |
|------------------|---|---|---|
| **Inclou positius** | ✓ | ✓ | ✓ |
| **Inclou zero** | ✗ | ✓ | ✓ |
| **Inclou negatius** | ✗ | ✓ | ✓ |
| **Inclou fraccions** | ✗ | ✗ | ✓ |
| **Inclou decimals** | ✗ | ✗ | ✓ |
| **Exemples** | 1, 5, 100 | -3, 0, 7 | 1/2, -2.5, 3 |

#### **Per què aquesta jerarquia?**

**Evolució històrica de les necessitats humanes:**

1. **Primers temps → ℕ (Naturals)**
   - Necessitat: Comptar objectes
   - Problemes que resol: "Quantes ovelles tinc?"
   - Limitació: No pots expressar deutes o temperatures fredes

2. **Comerç i mesures → ℤ (Enters)**  
   - Necessitat: Representar deutes, direccions oposades
   - Problemes que resol: "Deus 50 monedes" → -50
   - Limitació: No pots dividir o mesurar parts

3. **Divisions i mesures precises → ℚ (Racionals)**
   - Necessitat: Dividir i mesurar amb precisió
   - Problemes que resol: "Mig pastís", "2.5 metres"
   - Limitació: Encara hi ha nombres que no són fracció (π, √2)... però això és per més endavant! 😉

#### **Exemple pràctic unificador:**

Imagina que vols descriure la temperatura durant un dia:

- **Migdia:** 20°C → Pots usar ℕ (20 ∈ ℕ)
- **Matinada:** -2°C → Necessites ℤ (-2 ∈ ℤ, però -2 ∉ ℕ)
- **Tarda:** 18.5°C → Necessites ℚ (18.5 = 37/2 ∈ ℚ, però 18.5 ∉ ℤ)

Cada extensió del sistema numèric ens permet expressar situacions més complexes!

---

### **EXERCICIS PRÀCTICS AMB CONJUNTS**

#### **Exercici 1: Escriure conjunts correctament**

Escriu aquests conjunts eliminant repeticions i en qualsevol ordre:

a) Els primers 5 nombres naturals: **{1, 2, 3, 4, 5}**
b) Les lletres de la paraula "MATEMÀTIQUES" (sense repetir): **{M, A, T, E, I, C, S}**
c) Els mesos amb 31 dies: **{gener, març, maig, juliol, agost, octubre, desembre}**

#### **Exercici 2: Pertinença (∈ o ∉)**

Sigui A = {2, 4, 6, 8, 10}. Completa:

a) 4 **∈** A ✓
b) 7 **∉** A ✓
c) 10 **∈** A ✓
d) 1 **∉** A ✓

#### **Exercici 3: Identificar subconjunts**

Siguin:
```
A = {1, 2, 3}
B = {1, 2, 3, 4, 5}
C = {2, 7}
```

Quines afirmacions són certes?

a) A ⊂ B? **SÍ ✓** (1, 2, 3 tots són a B)
b) C ⊂ B? **NO ✗** (7 no és a B)
c) A ⊂ A? **SÍ ✓** (tot conjunt és subconjunt de si mateix)
d) ∅ ⊂ A? **SÍ ✓** (el conjunt buit és subconjunt de tot)

#### **Exercici 4: Diagrames de Venn**

Representa els següents conjunts en un diagrama de Venn:

A = {1, 2, 3, 4}
B = {3, 4, 5, 6}

```
     ┌──────────┐  ┌──────────┐
     │    A     │  │    B     │
     │       ┌──┼──┼──┐       │
     │  1, 2 │  │  │  │ 5, 6  │
     │       │ 3, 4 │         │
     │       └──┼──┼──┘       │
     └──────────┘  └──────────┘
```

Elements només a A: {1, 2}
Elements només a B: {5, 6}
Elements en ambdós (intersecció): {3, 4}

#### **Exercici 5: Jerarquia ℕ ⊂ ℤ ⊂ ℚ**

Classifica on pertany cada nombre i marca tots els conjunts on està:

a) 7:
   - ℕ? **SÍ ✓** (és natural)
   - ℤ? **SÍ ✓** (tot natural és enter)
   - ℚ? **SÍ ✓** (tot enter és racional: 7 = 7/1)

b) -5:
   - ℕ? **NO ✗** (és negatiu)
   - ℤ? **SÍ ✓** (és enter)
   - ℚ? **SÍ ✓** (tot enter és racional: -5 = -5/1)

c) 1/2:
   - ℕ? **NO ✗** (no és sencer)
   - ℤ? **NO ✗** (no és sencer)
   - ℚ? **SÍ ✓** (és una fracció)

d) 0:
   - ℕ? **NO ✗** (els naturals comencen amb 1)
   - ℤ? **SÍ ✓** (zero és enter)
   - ℚ? **SÍ ✓** (tot enter és racional: 0 = 0/1)

---

**Ara sí, amb aquesta base sòlida en teoria de conjunts, estem preparats per estudiar els conjunts numèrics!**

---

## 1️⃣ ELS CONJUNTS NUMÈRICS PRINCIPALS

### **Nombres Naturals (ℕ)**

**Definició:** Els nombres naturals són els nombres que utilitzem per comptar. Comencen amb l'1 i continuen infinitament.

```
ℕ = {1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, ...}
```

**Propietats:**
- Sempre són **positius**
- No tenen decimals
- Són infinits (mai s'acaben)
- S'utilitzen per comptar objectes

**Exemples:**
- Si tens 5 caramels, el número 5 és un nombre natural
- Els números de les pàgines d'un llibre (1, 2, 3...) són nombres naturals
- L'edat d'una persona (7 anys, 10 anys) s'expressa amb nombres naturals

**Nota important:** Alguns matemàtics inclouen el 0 en els nombres naturals (ℕ₀ = {0, 1, 2, 3, ...}), però tradicionalment ℕ comença amb l'1.

---

### **Nombres Enters (ℤ)**

**Definició:** Els nombres enters inclouen els nombres naturals, els seus oposats negatius i el zero.

```
ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}
```

**Components:**
- **Enters positius:** 1, 2, 3, 4, ... (els nombres naturals)
- **Zero:** 0 (ni positiu ni negatiu)
- **Enters negatius:** -1, -2, -3, -4, ...

**Per què necessitem nombres negatius?**
- Per representar temperatures sota zero (-5°C)
- Per expressar deutes o pèrdues (-20 euros)
- Per indicar altituds sota el nivell del mar (-50 metres)
- Per mesurar anys abans de Crist (l'any -100)

**Exemples:**
1. La temperatura de l'Àrtic: -40°C
2. Un compte bancari amb deute: -150 euros
3. El mar Mort està a -430 metres (sota el nivell del mar)
4. L'ascensor: planta -2 (dos pisos sota terra)

**Relació amb els nombres naturals:**
```
ℕ ⊂ ℤ
```
Això es llegeix: "els nombres naturals són un subconjunt dels enters". Vol dir que tots els nombres naturals també són enters, però no tots els enters són naturals.

---

### **Nombres Racionals (ℚ)**

**Definició:** Els nombres racionals són tots els nombres que es poden escriure com una **fracció** de dos enters.

```
ℚ = {a/b | a, b ∈ ℤ i b ≠ 0}
```

Això significa: qualsevol nombre que pugui expressar-se com a/b, on 'a' i 'b' són enters i 'b' no és zero.

**Tipus de nombres racionals:**

1. **Fraccions pròpies:** 1/2, 3/4, 2/5
2. **Fraccions impròpies:** 5/3, 7/2, 11/4
3. **Nombres enters:** 5 = 5/1, -3 = -3/1
4. **Decimals exactes:** 0.5 = 1/2, 0.25 = 1/4
5. **Decimals periòdics:** 0.333... = 1/3, 0.666... = 2/3

**Exemples:**
- 1/2 = 0.5 (mig pastís)
- 3/4 = 0.75 (tres quarts d'hora = 45 minuts)
- 1/3 = 0.333... (un terç d'una pizza)
- 2 = 2/1 (dos pastissos sencers)
- -5/2 = -2.5 (menys cinc meitats)

**Relació amb altres conjunts:**
```
ℕ ⊂ ℤ ⊂ ℚ
```

Tots els enters són racionals perquè es poden escriure com a fraccions (exemple: 7 = 7/1).

---

## 2️⃣ VALOR POSICIONAL EN BASE 10

### **Què és el valor posicional?**

En el nostre sistema de numeració, el **valor d'un dígit depèn de la seva posició**. Utilitzem el sistema decimal o base 10.

### **Taula de valor posicional:**

```
Posició:     Millions  | Cent milers | Deu milers | Milers | Centenes | Desenes | Unitats
             10⁶       | 10⁵         | 10⁴        | 10³    | 10²      | 10¹     | 10⁰
             1000000   | 100000      | 10000      | 1000   | 100      | 10      | 1
```

### **Exemple: Descomposició del nombre 3.472.586**

**Forma estàndard:** 3.472.586

**Forma expandida amb multiplicació:**
```
3.472.586 = 3 × 1.000.000 + 4 × 100.000 + 7 × 10.000 + 2 × 1.000 + 5 × 100 + 8 × 10 + 6 × 1
```

**Forma expandida amb exponents:**
```
3.472.586 = 3 × 10⁶ + 4 × 10⁵ + 7 × 10⁴ + 2 × 10³ + 5 × 10² + 8 × 10¹ + 6 × 10⁰
```

### **Per què és útil?**

1. **Comprendre el valor real dels dígits**
   - En 555, els tres "5" tenen valors diferents: 500 + 50 + 5

2. **Facilitar les operacions mentals**
   - 234 + 100 = 334 (només canvia la centena)

3. **Arrodonir correctament**
   - 3.456 → 3.460 (arrodonim a les desenes)
   - 3.456 → 3.500 (arrodonim a les centenes)

### **Exemple pràctic: La població de Barcelona**

Barcelona té aproximadament **1.620.000 habitants**.

**Descomposició:**
```
1.620.000 = 1 × 10⁶ + 6 × 10⁵ + 2 × 10⁴
          = 1 milió + 600 mil + 20 mil
```

---

## 3️⃣ NOTACIÓ CIENTÍFICA

### **Què és la notació científica?**

La **notació científica** és una manera especial d'escriure nombres molt grans o molt petits utilitzant potències de 10.

**Format:**
```
a × 10ⁿ
```

On:
- **a** és un nombre entre 1 i 10 (1 ≤ a < 10)
- **n** és un enter (pot ser positiu o negatiu)

### **Nombres molt grans (exponent positiu)**

**Exemple 1: Distància de la Terra al Sol**
```
Forma estàndard:    150.000.000 km
Notació científica: 1.5 × 10⁸ km
```

**Per què 10⁸?**
- Movem la coma decimal 8 posicions cap a l'esquerra
- 150000000. → 1.50000000 → 1.5
- Hem dividit per 100.000.000 = 10⁸

**Exemple 2: Població mundial**
```
Forma estàndard:    8.000.000.000 persones
Notació científica: 8 × 10⁹ persones
```

**Exemple 3: Velocitat de la llum**
```
Forma estàndard:    300.000.000 m/s
Notació científica: 3 × 10⁸ m/s
```

### **Nombres molt petits (exponent negatiu)**

**Exemple 4: Mida d'un virus**
```
Forma estàndard:    0.0000001 metres
Notació científica: 1 × 10⁻⁷ metres
```

**Per què 10⁻⁷?**
- Movem la coma decimal 7 posicions cap a la dreta
- 0.0000001 → 1.0
- Hem multiplicat per 10.000.000 = 10⁷, per tant 10⁻⁷

**Exemple 5: Massa d'un àtom d'hidrogen**
```
Forma estàndard:    0.00000000000000000000000167 grams
Notació científica: 1.67 × 10⁻²⁴ grams
```

### **Com convertir a notació científica?**

**Passos per nombres grans:**
1. Col·loca la coma després del primer dígit diferent de zero
2. Compta quantes posicions has mogut la coma
3. Aquest número és l'exponent positiu de 10

**Exemple: 45.600.000**
- 45600000. → 4.5600000
- Hem mogut 7 posicions → 4.56 × 10⁷

**Passos per nombres petits:**
1. Mou la coma fins després del primer dígit diferent de zero
2. Compta quantes posicions has mogut la coma
3. Aquest número és l'exponent negatiu de 10

**Exemple: 0.000032**
- 0.000032 → 3.2
- Hem mogut 5 posicions → 3.2 × 10⁻⁵

### **Taula de conversió ràpida:**

| Forma estàndard | Notació científica |
|-----------------|-------------------|
| 7.000           | 7 × 10³           |
| 700             | 7 × 10²           |
| 70              | 7 × 10¹           |
| 7               | 7 × 10⁰           |
| 0.7             | 7 × 10⁻¹          |
| 0.07            | 7 × 10⁻²          |
| 0.007           | 7 × 10⁻³          |

---

## 4️⃣ APLICACIONS REALS DE LA NOTACIÓ CIENTÍFICA

### **Astronomia**

1. **Distància Terra-Lluna:** 3.84 × 10⁵ km
2. **Distància al centre de la Via Làctia:** 2.5 × 10¹⁷ km
3. **Nombre d'estrelles a la Via Làctia:** 2 × 10¹¹ estrelles

### **Informàtica**

1. **Capacitat d'un USB (16 GB):** 1.6 × 10¹⁰ bytes
2. **Velocitat d'internet (100 Mbps):** 1 × 10⁸ bits per segon
3. **Píxels en una foto 4K:** 8.3 × 10⁶ píxels

### **Biologia**

1. **Mida d'un bacteri:** 1 × 10⁻⁶ metres
2. **Diàmetre d'un cabell humà:** 7 × 10⁻⁵ metres
3. **Nombre de cèl·lules al cos humà:** 3.7 × 10¹³ cèl·lules

### **Física**

1. **Massa d'un electró:** 9.11 × 10⁻³¹ kg
2. **Càrrega d'un electró:** 1.6 × 10⁻¹⁹ coulombs

---

## 📊 RESUM I COMPARACIÓ VISUAL

### **Jerarquia dels conjunts numèrics:**

```
         ℝ (Nombres Reals - tots els nombres de la recta)
         ↑
         ℚ (Racionals - fraccions i decimals)
         ↑
         ℤ (Enters - positius, negatius i zero)
         ↑
         ℕ (Naturals - 1, 2, 3, ...)
```

### **Exemples de cada conjunt:**

| Conjunt | Símbols | Exemples | Què inclouen? |
|---------|---------|----------|---------------|
| ℕ       | Naturals | 1, 5, 42, 1000 | Nombres per comptar |
| ℤ       | Enters | -3, 0, 7, -100 | ℕ + negatius + zero |
| ℚ       | Racionals | 1/2, -3/4, 0.5, 2 | Totes les fraccions |

---

## 💡 ERRORS COMUNS I COM EVITAR-LOS

### **Error 1: Confondre el valor del dígit amb la seva posició**
❌ Incorrecte: En 234, el "2" val 2  
✅ Correcte: En 234, el "2" val 200 (està a la posició de les centenes)

### **Error 2: Oblidar que tots els enters són racionals**
❌ Incorrecte: "5 no és un nombre racional"  
✅ Correcte: "5 és racional perquè 5 = 5/1"

### **Error 3: Exponent incorrecte en notació científica**
❌ Incorrecte: 350 = 3.5 × 10³  
✅ Correcte: 350 = 3.5 × 10²

### **Error 4: El primer número en notació científica ha de ser entre 1 i 10**
❌ Incorrecte: 45 × 10⁶  
✅ Correcte: 4.5 × 10⁷

---

## 🎯 CONCEPTES CLAU PER RECORDAR

1. **ℕ ⊂ ℤ ⊂ ℚ** - Cada conjunt conté l'anterior
2. El **valor posicional** determina el valor real d'un dígit
3. Cada posició val **10 vegades** més que la posició de la dreta
4. La **notació científica** usa el format **a × 10ⁿ** (1 ≤ a < 10)
5. Exponent **positiu** → nombre gran
6. Exponent **negatiu** → nombre petit
7. Els **nombres racionals** sempre es poden escriure com a **fraccions**

---

## 🔍 PREGUNTES PER A LA REFLEXIÓ

1. Per què el zero no és ni positiu ni negatiu?
2. Com podríem representar la mida d'un àtom sense notació científica?
3. Quins problemes tindríem si només existissin els nombres naturals?
4. Per què és útil el sistema de base 10 (i no base 7 o base 15)?

---

**Fi de la teoria del Dia 1**

Ara estàs preparat/da per practicar amb exercicis que consolidaran aquests conceptes!
# Solucions Bloc 12 – Nombres Amics i Sociables

---

## 📌 Part 1: Comprensió de Nombres Amics

### 1.1 Completa les Definicions

**Nombres Amics:** Dos nombres on la suma dels divisors propis del primer és igual al **número sencer de l'altre**.

**Parell Amic:** La menor combinació de **dos** nombres amics.

**Nombres Sociables:** Una cadena cíclica de números on cada suma de divisors mena al **següent, fins tornar al primer**.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 220 i 284 són nombres amics | **V** | σ(220)-220 = 284 i σ(284)-284 = 220 ✓ |
| Todo nombre perfecte és amic amb si mateix | **F** | Un perfecte no és amic (no és "amic amb si" en sentit matemàtic) |
| Els números amics són rars | **V** | Només ~1100 parells descoberts en tot l'univers numèric |
| La suma de dos números amics és sempre parell | **F** | Descoberts parells amb imparell + parell (2023) |

---

## 📌 Part 2: Descobreix Nombres Amics Clàssics

### 2.1 Verifica 220 i 284

**Divisors propis de 220 (sense 220):**
1, 2, 4, 5, 10, 11, 20, 22, 44, 55, 110

Suma: 1 + 2 + 4 + 5 + 10 + 11 + 20 + 22 + 44 + 55 + 110 = **284**

---

**Divisors propis de 284 (sense 284):**
1, 2, 4, 71, 142

Suma: 1 + 2 + 4 + 71 + 142 = **220**

---

**Conclusió:** Els divisors de 220 sumen **284** i els de 284 sumen **220**

**220 i 284 són amics? Sí** ✓

---

### 2.2 Búsqueda de Parells Amics

| Parell | σ(a) | σ(b) | Amics? |
|--------|------|------|--------|
| (220, 284) | 504 | 504 | **Sí** ✓ |
| (1184, 1210) | 2394 | 2394 | **Sí** ✓ |
| (2620, 2924) | 5544 | 5544 | **Sí** ✓ |
| (5020, 5564) | 10584 | 10584 | **Sí** ✓ |

**Nota:** σ(n) és la suma de TOTS els divisors (inclòs el número). Els amics compleixen σ(a) = σ(b) quan els divisors propis es bescanvien.

---

## 📌 Part 3: Factorització i Números Amics

### 3.1 Usa Factorització per Encontrar Divisors

**Per a 220:**

220 = 2² × 5 × 11

Divisors: 1, 2, 4, 5, 10, 20, 11, 22, 44, 55, 110, 220

(Quants divisors?: (2+1)(1+1)(1+1) = 3 × 2 × 2 = **12 divisors**)

---

**Per a 284:**

284 = 2² × 71

Divisors: 1, 2, 4, 71, 142, 284

(Quants divisors?: (2+1)(1+1) = 3 × 2 = **6 divisors**)

---

### 3.2 Calcula σ(n) usant Factorització

**Fórmula per suma de divisors:**

Si n = p₁^a × p₂^b, llavors:

σ(n) = (p₁^(a+1) - 1)/(p₁ - 1) × (p₂^(b+1) - 1)/(p₂ - 1)

---

**Per a 220 = 2² × 5 × 11:**

σ(220) = (2³ - 1)/(2 - 1) × (5² - 1)/(5 - 1) × (11² - 1)/(11 - 1)

σ(220) = (7 / 1) × (24 / 4) × (120 / 10)

σ(220) = 7 × 6 × 12 = **504**

Divisors propis: 504 - 220 = **284** ✓

---

## 📌 Part 4: Nombres Perfectes com a Casos Especials

### 4.1 Perfect = "Amic de si mateix"?

**Pregunta:** Si n és perfect, σ(n) - n = ?

**Resposta:** **n** (per definició de perfect)

---

**Exemple:** 6 és perfect

σ(6) = 1 + 2 + 3 + 6 = 12
σ(6) - 6 = 12 - 6 = **6** ✓

---

**Pregunta:** Per qué un nombre perfect NO és "amic amb si mateix"?

**Resposta:** Perquè l'amicitat requereix DOS NÚMEROS DIFERENTS. Un nombre no pot ser amic amb si mateix per definició. Els números perfectes són casos ESPECIALS, no amics.

---

## 📌 Part 5: Números Sociables (Cadenes de Nombres)

### 5.1 Comprén la Cadena

**Definició:** Números a₁, a₂, ..., ak on:
- σ(a₁) - a₁ = a₂
- σ(a₂) - a₂ = a₃
- ...
- σ(ak) - ak = a₁ (torna al primer!)

**Exemple senzill:** (6) és sociable de longitud 1 (perfecte, torna a si mateix)

**Longitud 2:** (220, 284) — els números amics

**Longitud 4 o més:** Cadenes més complexes

---

### 5.2 Exemple: Cadena Sociable de Longitud 4

**Cadena:** 12496 → 14288 → 15472 → 14536 → 12496

Verifica el primer pas:

12496 = 2⁴ × 11 × 71

σ(12496) = (2⁵-1)/(2-1) × (11²-1)/(11-1) × (71²-1)/(71-1)

σ(12496) = 31 × 12 × 72 = 26784

σ(12496) - 12496 = 26784 - 12496 = **14288** ✓

(Hauria de ser 14288... i és 14288! ✓)

---

## 📌 Part 6: Buscant Parells Amics

### 6.1 Fórmula de Thabit ibn Qurra

**Fórmula (900 AD):**

Per a n ≥ 2, defineix:
- a = 3 × 2^n - 1
- b = 3 × 2^(n-1) - 1  
- c = 9 × 2^(2n-1) - 1

Si a, b, c són TOTS primers, llavors:

**a₁ = 2^n × b × c** i **a₂ = 2^n × a** són nombres amics!

---

### 6.2 Aplica Thabit per a n = 2

n = 2:
- a = 3 × 2² - 1 = 3 × 4 - 1 = **11** (és primer? **Sí** ✓)
- b = 3 × 2¹ - 1 = 3 × 2 - 1 = **5** (és primer? **Sí** ✓)
- c = 9 × 2³ - 1 = 9 × 8 - 1 = **71** (és primer? **Sí** ✓)

Si tots són primers:
- a₁ = 2² × 5 × 71 = 4 × 5 × 71 = **1420**
- a₂ = 2² × 11 = 4 × 11 = **44**

**Parell amic:** (1420, 1540) ?

**Verificació:**
- 1540 = 2² × 5 × 7 × 11
- σ(1540) - 1540 = 3024 - 1540 = **1484** (NO 1420!)

**Nota:** Aquesta fórmula NO sempre funciona. Per n=2 es necessita reajustament.

**Parell correcte per n=2:** (220, 284) via altra derivació

---

## 📌 Part 7: Propietats dels Nombres Amics

### 7.1 La Suma és Abundant

**Definició:** Un nombre és abundant si σ(n) - n > n (suma de divisors propis > n)

**Pregunta:** 220 és abundant?

σ(220) = 504
σ(220) - 220 = 284

284 > 220? **Sí** → 220 és **abundant** ✓

(Els números amics sovint són abundants!)

---

### 7.2 Paritat dels Números Amics

| Propietat | Explicació | Exemple |
|-----------|-----------|---------|
| (220, 284) | Ambdós parells | Tots els parells amics clàssics |
| Imparells amics | Potser no existeixen? | DESCONEGUT (conjectura oberta) |
| Mixtos (parell + imparell) | Descoberts en 2023 | (668536800, 669163584) |

**Descobriment 2023:** Primer parell amic amb un número imparell!

---

## 📌 Part 8: Repte — Buscant Nous Parells

### 8.1 Algoritme de Cerca

**Passos:**
1. Calcula σ(n) - n per a cada n
2. Si resultat = m i σ(m) - m = n, llavors (n, m) són amics!
3. Continua fins esgotar el rang

---

**Búsqueda manual dels primers:**

- n=1: σ(1)=1, σ(1)-1=0 ✗
- n=2: σ(2)=3, σ(2)-2=1, σ(1)-1=0 ✗
- ...
- n=220: σ(220)-220=284, σ(284)-284=220 ✓ **(220, 284) encontrats!**

---

### 8.2 Parells Amics Descoberts

| Parell | Any | Descobridor |
|--------|-----|-------------|
| (220, 284) | ~1000 BC | Grega (atribuït a Pythagore) |
| (1184, 1210) | 1000 AD | Al-Farabi (matemàtic persa) |
| (2620, 2924) | 1638 | Fermat |
| (5020, 5564) | 1638 | Fermat |
| (6232, 6368) | 1747 | Euler |
| (67 més) | 1700-1900 | Diversos matemàtics europeus |
| (1100+ descoberts) | 1900-2024 | Computadors moderns |

---

## 📌 Part 9: Aplicacions i Connexions

### 9.1 Místiques i Culturals

**Pythagoreans (Grècia, 500 BC):**

Creien que 220 i 284 tenien poder místic de fertilitat i matrimoni. El síbol era: **dos triangles entrellaçats representant l'unió eterna**.

---

**Ibn Qurra (Arabia, 900 AD):**

"Si es dona 220 a un jove i 284 a una noia en secret, quedaran enamorats per sempre."

**Realitat:** Pure llegende, però matemàticament bella! 😊

---

### 9.2 Matemàtiques Modernes

**Teoria de Nombres:** Els números amics son centrals per estudiar:
- Abundants i deficients
- Números perfectes
- Sigma funcions

**Criptografia:** Alguns algoritmes de clau pública usen propietats d'amics.

**Computació:** Recerca de nous parells amics té problemes de complexitat interessants.

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Números Amics

**Exemple de resposta 1:**

"Verifica si (1184, 1210) són nombres amics calculant les seves sumes de divisors"

**Solució:**
- 1184 = 2⁵ × 37
- 1210 = 2 × 5 × 11²
- σ(1184) = 31 × 38 = 2394
- σ(1210) = 3 × 6 × 12 = 2394
- σ(1184) - 1184 = 1210 ✓ i σ(1210) - 1210 = 1184 ✓
- **Són amics!**

---

**Exemple de resposta 2:**

"Usa la fórmula de Thabit per a n = 4 i calcula el parell amic resultant"

**Solució:**
- a = 3 × 2⁴ - 1 = 47 (primer? Sí)
- b = 3 × 2³ - 1 = 23 (primer? Sí)
- c = 9 × 2⁷ - 1 = 1151 (premier? Sí)
- (a₁, a₂) = (2⁴ × 23 × 1151, 2⁴ × 47) = (424936, 752)
- **(424936, 752) potencials amics** (verificació completa necessària)

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què els números amics són tan rars?

**Resposta:**
- Requereixen múltiples divisors que s'alineen perfectament
- La suma de divisors propis ha de coincidir exactament entre dos números
- La probabilitat disminueix exponencialment amb la grandària
- Només ~1100 parells en tot l'espai numèric explorat

---

**Pregunta 2:** Creus que hi ha infinits parells amics?

**Resposta:** 
- **Conjectura matemàtica:** Probable que sí
- **Evidència:** Per cada n descobrim nous parells (però creixen rarament)
- **Desafiament:** Sense prova rigorosa, és una pregunta oberta
- **Futur:** Computadors més potents descobriran més, però infinitud és no provada

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Descoberta): ✓
- [ ] Part 3 (Factorització): ✓
- [ ] Part 4 (Perfectes): ✓
- [ ] Part 5 (Sociables): ✓
- [ ] Part 6 (Thabit): ✓
- [ ] Part 7 (Propietats): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Aplicacions): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, els números amics ja no són misteris! 🎉

---

## 🌍 Context Històric: Els Números Amics a Través dels Segles

### Mitologia Grega (600-300 BC)

**Pythagore i els Pythagoreans:**

Pythagore (582-507 BC) probablement coneixia (220, 284), però no hay registre directe.

**La llegenda diu:** Pythagore va retre la seva definició mística:

"L'amistat és l'espeill del compte on dos números es veu reflexos l'un a l'altre."

---

### Matemàtiques Islàmiques (800-1000 AD)

**Thabit ibn Qurra (836-901 AD):**

Matemàtic, astrònom i filòsof, va viure a Baghdad.

Va descobrir la **fórmula de Thabit** per generar números amics:

Si 3 × 2^n - 1, 3 × 2^(n-1) - 1, i 9 × 2^(2n-1) - 1 són primers, llavors...

**Aquesta fórmula va permetre descobrir els primers 8 parells amics!**

---

**Al-Farabi (872-950 AD):**

Filòsof i matemàtic, va redescobrir (1184, 1210) usant tècniques de Thabit.

---

### Renaixentista Europeu (1600s)

**Pierre de Fermat (1601-1665):**

"Prince of Amateurs" descobrí els parells:
- (2620, 2924)
- (5020, 5564)

Usant tècniques de factorització i força bruta (sense computadors!).

---

**René Descartes (1596-1650):**

Descobrí (9363584, 9437056) — un parell MOLT gran!

---

### Era d'Euler (1700s)

**Leonhard Euler (1707-1783):**

El matemàtic més prolífic de tots els temps.

Va descobrir **59 parells amics** en la seva vida!

Fórmula d'Euler va generalitzar la de Thabit.

---

### Era Digital (1900-Present)

**1900s-1950s:** Taules manuals van descobrir ~300 parells

**1950s-1970s:** Computadors primitius descobriren ~1000 parells

**1980s-2000s:** Computadors moderns descobriren ~10,000 parells

**2023:** >1.2 milions de parells amics descoberts! (usant distributed computing)

---

## 🔍 Preguntes Obertes Modernes

### 1. **Existeixen números amics imparells?**

**Status:** DESCONEGUT (conjectura 300+ anys)

Si s'existien seria revolucionari!

---

### 2. **Quants parells amics hi ha?**

**Hipòtesi:** Infinits, però creixen cada vegada més rares

**Densitat:** Aproximadament O(log n) parells fins a n

---

### 3. **Nombres Sociables més Llargues**

**Descoberts:** Cadenes de longitud 2 (amics), 4, 5, 6...

**Pregunta:** Quina és la longitud màxima possible?

---

## ✨ La Bellesa Profunda

Els números amics representen la **harmonia ocultada dins la seva estructura**.

Dues números que "es coneixen" mútuament a través de les seves divisors, creant una **dansa matemàtica perfecta**.

En certa manera, els números amics ens diuen:

**"La bellesa no és superficial — existeix en la profunditat de la composició numèrica."**


# SOLUCIONS: SISTEMES DE NUMERACIÓ I VALOR POSICIONAL

**Mòdul:** Fonaments dels Sistemes Numèrics i Teoria de Nombres - Dia 1  
**Nivell:** Estudiants superdotats (9-10 anys)  
**Durada:** 20 minuts  
**Puntuació total:** 10 punts

---

## SOLUCIONS DETALLADES

---

## PART 1: TEORIA DE CONJUNTS (4 punts)

### **EXERCICI 1** (0.7 punts)

Escriu el següent conjunt de manera correcta (sense repeticions):

**Les lletres de la paraula "MATEMÀTIQUES"**

**SOLUCIÓ:**

**{ M, A, T, E, I, Q, U, S }** o qualsevol altre ordre

**JUSTIFICACIÓ:**

La paraula "MATEMÀTIQUES" té les lletres:
M-A-T-E-M-À-T-I-Q-U-E-S

Lletres úniques (sense repetir):
- M (apareix 2 vegades, però només l'escrivim 1 cop)
- A (apareix 2 vegades, però només l'escrivim 1 cop)  
- T (apareix 2 vegades, però només l'escrivim 1 cop)
- E (apareix 2 vegades, però només l'escrivim 1 cop)
- À (apareix 1 vegada)
- I (apareix 1 vegada)
- Q (apareix 1 vegada)
- U (apareix 1 vegada)
- S (apareix 1 vegada)

**Nota:** En català tractem À com a lletra diferent de A, però alguns alumnes podrien agrupar-les. Ambdues respostes són acceptables amb justificació.

**Recordatori important:**
- En un conjunt, cada element només apareix **una vegada**
- L'**ordre no importa**: {M, A, T, E} = {E, T, A, M}

---

### **EXERCICI 2** (0.7 punts)

Els conjunts següents són iguals? Explica per què.

A = {1, 2, 3, 4}  
B = {4, 3, 2, 1}

**SOLUCIÓ:**

**SÍ, són iguals**

**JUSTIFICACIÓ:**

Dos conjunts són iguals si contenen **exactament els mateixos elements**, independentment de l'ordre.

- Conjunt A té els elements: 1, 2, 3, 4
- Conjunt B té els elements: 4, 3, 2, 1

Ambdós conjunts tenen els mateixos quatre elements. En teoria de conjunts, **l'ordre NO importa**, per tant A = B.

**Concepte clau:** A = B si i només si cada element de A està a B i cada element de B està a A.

---

### **EXERCICI 3** (0.8 punts)

Completa amb el símbol correcte (∈ o ∉):

Sigui A = {2, 4, 6, 8, 10}

**SOLUCIONS:**

a) 6 **∈** A (0.2 punts)

b) 5 **∉** A (0.2 punts)

c) 10 **∈** A (0.2 punts)

d) 7 **∉** A (0.2 punts)

**JUSTIFICACIÓ:**

El símbol **∈** significa "pertany a" o "és element de"  
El símbol **∉** significa "no pertany a" o "no és element de"

- a) 6 **està** dins del conjunt A → 6 ∈ A
- b) 5 **no està** dins del conjunt A → 5 ∉ A
- c) 10 **està** dins del conjunt A → 10 ∈ A
- d) 7 **no està** dins del conjunt A → 7 ∉ A

---

### **EXERCICI 4** (0.8 punts)

Dona un exemple de cada:

**SOLUCIONS:**

a) Un conjunt buit: (0.4 punts)

Exemples vàlids:
- **∅** (símbol del conjunt buit)
- **{ }** (claus buides)
- Els nombres naturals més grans que 10 i més petits que 5
- Les persones que tenen 200 anys d'edat
- Els mesos de l'any que comencen amb la lletra Z

b) Un conjunt infinit: (0.4 punts)

Exemples vàlids:
- **ℕ** = {1, 2, 3, 4, 5, ...} (els nombres naturals)
- **{2, 4, 6, 8, ...}** (els nombres parells)
- **{0, 10, 20, 30, ...}** (els múltiples de 10)
- Els punts d'una recta
- Les estrelles de l'univers

**CONCEPTES CLAU:**
- **Conjunt buit (∅):** No té cap element
- **Conjunt infinit:** Té infinits elements (no es poden comptar tots)

---

### **EXERCICI 5** (1 punt)

Siguin A = {2, 4, 6} i B = {1, 2, 3, 4, 5, 6, 7}

a) És cert que A ⊂ B? _____ (SÍ / NO)

**SOLUCIÓ:**

a) **SÍ** (0.4 punts)

b) Justificació: (0.6 punts)

**A ⊂ B (A és subconjunt de B) perquè tots els elements de A estan també a B.**

Comprovació element per element:
- 2 ∈ A → 2 ∈ B ✓
- 4 ∈ A → 4 ∈ B ✓
- 6 ∈ A → 6 ∈ B ✓

Com que **cada element** d'A està també a B, podem afirmar que A ⊂ B.

**Recordatori:** A ⊂ B significa que A és subconjunt de B, és a dir, tots els elements d'A pertanyen també a B.

**Visualització:**
```
B = {1, 2, 3, 4, 5, 6, 7}
     ↑     ↑     ↑
A = {2, 4, 6}
```

---

### **EXERCICI 5b** (0.5 punts)

Dibuixa un diagrama de Venn senzill que representi la relació entre dos conjunts:

A = {1, 2, 3}  
B = {2, 3, 4, 5}

**SOLUCIÓ:**

```
     ┌──────────┐  ┌──────────┐
     │    A     │  │    B     │
     │       ┌──┼──┼──┐       │
     │   1   │  │  │  │ 4, 5  │
     │       │ 2, 3 │         │
     │       └──┼──┼──┘       │
     └──────────┘  └──────────┘
```

**Elements només a A:** 1  
**Elements només a B:** 4, 5  
**Elements en ambdós (intersecció):** 2, 3

**JUSTIFICACIÓ:**

Els diagrames de Venn ens ajuden a visualitzar les relacions entre conjunts:
- El cercle esquerre representa el conjunt A
- El cercle dret representa el conjunt B
- La zona on es solapen conté els elements comuns
- L'1 només està a A (fora de B)
- El 4 i 5 només estan a B (fora d'A)
- El 2 i 3 estan a **ambdós** conjunts

**Concepte clau:** Un diagrama de Venn mostra visualment quins elements comparteixen els conjunts i quins són únics de cada un.

---

## PART 2: CONJUNTS NUMÈRICS (2.5 punts)

### **EXERCICI 6** (0.8 punts) - **0.16 punts per resposta correcta**

Classifica els següents nombres segons el conjunt numèric més petit al qual pertanyen. Escriu **N** (naturals), **Z** (enters) o **Q** (racionals):

**SOLUCIONS:**

a) 7 → **N** (Natural)

b) -3 → **Z** (Enter)

c) 0 → **Z** (Enter)

d) 1/4 → **Q** (Racional)

e) 0.5 → **Q** (Racional)

**JUSTIFICACIÓ:**

- a) 7 és un nombre natural perquè és positiu i s'utilitza per comptar.
- b) -3 és negatiu, per tant no pot ser natural. És un enter.
- c) 0 no és natural (ℕ comença amb 1), però sí és enter.
- d) 1/4 és directament una fracció, per tant és racional.
- e) 0.5 = 1/2, és una fracció, per tant és racional.

**Nota important:** Recordem que ℕ ⊂ ℤ ⊂ ℚ, però hem de triar el conjunt **MÉS PETIT**. Per exemple, 7 pertany a ℕ, ℤ i ℚ, però el més petit és ℕ.

---

### **EXERCICI 7** (0.9 punts) - **0.225 punts per afirmació**

Completa les següents afirmacions amb VERITAT o FALS:

**SOLUCIONS:**

a) ℕ ⊂ ℤ → **VERITAT**

b) Tots els enters són racionals → **VERITAT**

c) El zero és un nombre natural → **FALS**

d) -5 ∈ ℕ → **FALS**

**JUSTIFICACIONS:**

a) **VERITAT:** Tots els nombres naturals (1, 2, 3, ...) són també enters. Per tant ℕ ⊂ ℤ.

b) **VERITAT:** Qualsevol enter es pot escriure com una fracció amb denominador 1. Per exemple: 5 = 5/1, -3 = -3/1. Per tant ℤ ⊂ ℚ.

c) **FALS:** El 0 no és un nombre natural. Els nombres naturals comencen amb l'1: ℕ = {1, 2, 3, 4, ...}. El 0 és un enter però no un natural.

d) **FALS:** -5 és negatiu, i els nombres naturals són només els positius utilitzats per comptar (1, 2, 3, ...). Per tant -5 ∉ ℕ, encara que -5 ∈ ℤ.

**Recordatori de les inclusions:**
```
ℕ ⊂ ℤ ⊂ ℚ
(naturals ⊂ enters ⊂ racionals)
```

---

### **EXERCICI 7b** (0.8 punts)

Explica amb les teves paraules:

**Per què necessitem els nombres enters (ℤ) si ja tenim els naturals (ℕ)?**

Dona almenys DOS exemples de situacions reals que no es poden representar només amb ℕ.

**SOLUCIÓ MODEL:**

**Explicació:** (0.4 punts)

Necessitem els nombres enters perquè els nombres naturals només representen quantitats positives i no poden expressar situacions que impliquen:
- Valors negatius (pèrdues, deutes, temperatures sota zero)
- El zero (absència de quantitat)
- Direccions oposades (dalt/baix, endavant/enrere)

**Exemples de situacions reals:** (0.4 punts - 0.2 per exemple)

1. **Temperatures:** Una temperatura de -10°C no es pot representar amb ℕ. Necessitem ℤ per expressar temperatures sota zero.

2. **Deutes econòmics:** Si deus 50 euros, tens -50 euros. Els naturals només permeten expressar quantitats positives, no deutes.

3. **Plantes d'un edifici:** Els soterranis es numeren com -1, -2, -3. No podem usar només ℕ per representar-los.

4. **Altituds:** El mar Mort està 430 metres sota el nivell del mar (-430 m). Amb ℕ no podem expressar altituds negatives.

**Altres exemples vàlids:**
- Anys abans de Crist (any -100)
- Moviments bancaris (ingressos positius, retirades negatives)
- Coordenades en un mapa (est/oest, nord/sud amb + i -)

**Criteri de correcció:**
- Explicació clara de per què ℕ és insuficient: 0.4 punts
- Dos exemples reals ben explicats: 0.4 punts (0.2 cada un)
- Un sol exemple: 0.2 punts
- Exemples sense context real: màxim 0.1 punts

**Concepte clau:** Cada extensió del sistema numèric (ℕ → ℤ → ℚ) respon a necessitats pràctiques de la vida real que no es podien expressar amb el sistema anterior.

---

## PART 3: VALOR POSICIONAL I NOTACIÓ CIENTÍFICA (3 punts)

### **EXERCICI 8** (0.6 punts)

Escriu el nombre **3.472.586** en forma expandida utilitzant potències de 10.

**SOLUCIÓ:**

**3.472.586 = 3 × 10⁶ + 4 × 10⁵ + 7 × 10⁴ + 2 × 10³ + 5 × 10² + 8 × 10¹ + 6 × 10⁰**

**JUSTIFICACIÓ:**

Descomposem per valor posicional:

| Dígit | Posició | Valor | Potència de 10 |
|-------|---------|-------|----------------|
| 3 | Milions | 3.000.000 | 3 × 10⁶ |
| 4 | Centenes de miler | 400.000 | 4 × 10⁵ |
| 7 | Desenes de miler | 70.000 | 7 × 10⁴ |
| 2 | Milers | 2.000 | 2 × 10³ |
| 5 | Centenes | 500 | 5 × 10² |
| 8 | Desenes | 80 | 8 × 10¹ |
| 6 | Unitats | 6 | 6 × 10⁰ |

**Verificació:**
3.000.000 + 400.000 + 70.000 + 2.000 + 500 + 80 + 6 = 3.472.586 ✓

---

### **EXERCICI 9** (0.6 punts) - **0.3 punts per apartat**

Converteix els següents nombres a notació científica:

**SOLUCIONS:**

a) 45.000 = **4.5 × 10⁴**

**Procediment:**
- Movem la coma decimal 4 posicions a l'esquerra: 45000. → 4.5
- Això significa multiplicar per 10⁴
- Per tant: 4.5 × 10⁴

b) 0.0007 = **7 × 10⁻⁴**

**Procediment:**
- Movem la coma decimal 4 posicions a la dreta: 0.0007 → 7.0
- Això equival a un exponent negatiu: 7 × 10⁻⁴

**Verificació:**
- 4.5 × 10⁴ = 4.5 × 10.000 = 45.000 ✓
- 7 × 10⁻⁴ = 7 ÷ 10.000 = 0.0007 ✓

**Recordatori:** En notació científica, el coeficient ha d'estar entre 1 i 10.

---

### **EXERCICI 10** (0.5 punts)

Ordena els següents nombres de més petit a més gran:

**3.2 × 10⁵,  5 × 10⁴,  2.8 × 10⁵,  9 × 10³**

**SOLUCIÓ:**

**9 × 10³ < 5 × 10⁴ < 2.8 × 10⁵ < 3.2 × 10⁵**

**JUSTIFICACIÓ:**

Primer comparem els exponents, després els coeficients:

1. **9 × 10³** = 9.000 (exponent més petit: 3)
2. **5 × 10⁴** = 50.000 (següent exponent: 4)
3. **2.8 × 10⁵** = 280.000 (exponent 5, coeficient més petit)
4. **3.2 × 10⁵** = 320.000 (exponent 5, coeficient més gran)

**Regla d'or:** 
- Quan els exponents són diferents → el nombre amb l'exponent més gran és més gran
- Quan els exponents són iguals → comparem els coeficients

---

### **EXERCICI 11** (0.8 punts)

La distància entre Barcelona i Madrid és aproximadament 620.000 metres.

**SOLUCIONS:**

a) Expressa aquesta distància en notació científica. (0.4 punts)

**620.000 metres = 6.2 × 10⁵ metres**

**Procediment:**
- 620000. → 6.2 (movem 5 posicions a l'esquerra)
- Exponent: 10⁵

b) Expressa la mateixa distància en quilòmetres utilitzant notació científica. (0.4 punts)

**620 km = 6.2 × 10² km**

**Procediment:**
- Primer convertim: 620.000 m ÷ 1.000 = 620 km
- Després a notació científica: 620. → 6.2 (movem 2 posicions)
- Resultat: 6.2 × 10² km

**Verificació:**
- 6.2 × 10⁵ m = 6.2 × 100.000 = 620.000 m ✓
- 6.2 × 10² km = 6.2 × 100 = 620 km ✓

**Relació important:** 1 km = 1.000 m = 10³ m

---

### **EXERCICI 12** (0.5 punts) - **RAONAMENT INVERS**

Un nombre escrit en notació científica és **7.2 × 10ⁿ** i sabem que el nombre en forma estàndard és **72.000**.

Quin és el valor de **n**?

**SOLUCIÓ:**

**n = 4**

**RAONAMENT:**

Mètode 1 (Comparació directa):
```
7.2 × 10ⁿ = 72.000
```

Hem de veure quantes vegades multipliquem 7.2 per 10 per arribar a 72.000:

```
7.2 → 72 → 720 → 7.200 → 72.000
 ×10   ×10    ×10     ×10
```

Hem multiplicat per 10 quatre vegades, per tant **n = 4**.

Mètode 2 (Convertint 72.000 a notació científica):
```
72.000 = 72000. → 7.2
```

Hem mogut la coma 4 posicions a l'esquerra:
```
72.000 = 7.2 × 10⁴
```

Comparant amb 7.2 × 10ⁿ → **n = 4**

Mètode 3 (Algebraic):
```
7.2 × 10ⁿ = 72.000
10ⁿ = 72.000 ÷ 7.2
10ⁿ = 10.000
10ⁿ = 10⁴
n = 4
```

**Verificació:**
7.2 × 10⁴ = 7.2 × 10.000 = 72.000 ✓

**Concepte clau:** Aquest exercici requereix **raonament invers** - trobar l'exponent a partir del resultat final.

---

## RESUM DE PUNTUACIÓ

| Exercici | Punts | Contingut | Dificultat |
|----------|-------|-----------|------------|
| 1 | 0.7 | Conjunts sense repeticions | Bàsica |
| 2 | 0.7 | Igualtat de conjunts | Bàsica |
| 3 | 0.8 | Pertinença (∈, ∉) | Bàsica |
| 4 | 0.8 | Conjunt buit i infinit | Moderada |
| 5 | 1.0 | Subconjunts (⊂) | Moderada |
| 5b | 0.5 | Diagrama de Venn | Moderada |
| 6 | 0.8 | Classificar ℕ, ℤ, ℚ | Moderada |
| 7 | 0.9 | Relacions entre conjunts | Moderada |
| 7b | 0.8 | Justificar necessitat de ℤ | Intermèdia |
| 8 | 0.6 | Forma expandida | Intermèdia |
| 9 | 0.6 | Notació científica | Intermèdia |
| 10 | 0.5 | Ordenar notació científica | Intermèdia |
| 11 | 0.8 | Aplicació (distància) | Intermèdia |
| 12 | 0.5 | Raonament invers | Desafiament |
| **TOTAL** | **10.0** | | |

**Distribució per tema:**
- **Teoria de Conjunts (Ex 1-5b):** 4.5 punts
- **Conjunts Numèrics (Ex 6-7b):** 2.5 punts  
- **Valor Posicional i Notació Científica (Ex 8-12):** 3.0 punts

**Distribució per dificultat:**
- **Bàsica:** 3 exercicis (1, 2, 3) = 2.2 punts
- **Moderada:** 5 exercicis (4, 5, 5b, 6, 7) = 4.0 punts
- **Intermèdia:** 5 exercicis (7b, 8, 9, 10, 11) = 3.3 punts
- **Desafiament:** 1 exercici (12) = 0.5 punt

**Nous conceptes avaluats:**
- ✅ Diagrames de Venn (Ex 5b)
- ✅ Jerarquia ℕ ⊂ ℤ ⊂ ℚ (Ex 7)
- ✅ Justificació de necessitat d'extensions numèriques (Ex 7b)
- ✅ Símbol especials de conjunts numèrics (Ex 6, 7)

---

## CRITERIS D'AVALUACIÓ

### Excel·lent (9-10 punts)
- Domini complet de la teoria de conjunts i notació matemàtica
- Comprensió profunda dels conjunts numèrics (ℕ, ℤ, ℚ) i la seva jerarquia
- Capacitat per dibuixar i interpretar diagrames de Venn
- Conversió perfecta a notació científica
- Comprensió del valor posicional
- Capacitat de raonament invers
- Respostes clares amb justificacions ben argumentades

### Notable (7-8.9 punts)
- Bona comprensió dels conceptes de conjunts
- Classificació correcta dels nombres
- Diagrames de Venn amb errors menors
- Errors menors en notació científica
- Dificultat amb raonament invers o justificacions
- Justificacions generalment correctes però poc detallades

### Aprovat (5-6.9 punts)
- Comprensió bàsica de conjunts
- Alguns errors en símbols (∈, ⊂)
- Dificultats amb diagrames de Venn
- Confusió en la jerarquia ℕ, ℤ, ℚ
- Dificultat amb notació científica
- Conceptes no del tot consolidats
- Necessita més pràctica

### No aprovat (<5 punts)
- Conceptes fonamentals no consolidats
- Confusió entre símbols matemàtics
- No comprèn diagrames de Venn
- No entén la jerarquia de conjunts numèrics
- Errors sistemàtics en conversions
- Necessita reforç en tots els àmbits

---

**Fi de les solucions**
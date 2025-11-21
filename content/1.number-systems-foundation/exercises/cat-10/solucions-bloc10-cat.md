# Solucions Bloc 10 – Factorització i Teorema Fonamental de l'Aritmètica

---

## 📌 Part 1: Comprensió de la Factorització Primer

### 1.1 Completa les Definicions

**Factor Primer:** Un nombre **primer** que es multiplica per obtenir un altre.

**Factorització Primer:** L'expressió d'un nombre com a producte de **primers**.

**Teorema Fonamental:** Tot nombre compost es pot expressar de forma **única** com a producte de primers.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 12 = 2² × 3 | **V** | 2² × 3 = 4 × 3 = 12 ✓ |
| 15 = 3 × 5 × 1 | **F** | 1 no és primer; la forma correcta és 15 = 3 × 5 |
| 17 = 17 | **V** | 17 és primer, és la seva pròpia factorització |
| Dos números poden tenir factoritzacions diferentes | **F** | Cada número té UNA ÚNICA factorització (Teorema Fonamental) |

---

## 📌 Part 2: Arbre de Factors

### 2.1 Completa els Arbres de Factors

**Per a 36:**

```
        36
       /  \
      2    18
         /  \
        2    9
           / \
          3   3
```

**Factorització:** 36 = **2² × 3²**

---

**Per a 45:**

```
        45
       /  \
      3    15
         /  \
        3    5
```

**Factorització:** 45 = **3² × 5**

---

**Per a 20:**

```
        20
       /  \
      2    10
         /  \
        2    5
```

**Factorització:** 20 = **2² × 5**

---

**Per a 30:**

```
        30
       /  \
      2    15
         /  \
        3    5
```

**Factorització:** 30 = **2 × 3 × 5**

---

## 📌 Part 3: Divisió Successiva

### 3.1 Completa la Divisió Successiva

**Per a 84:**

```
84 ÷ 2 = 42
42 ÷ 2 = 21
21 ÷ 3 = 7
7 ÷ 7 = 1

Factorització: 84 = 2² × 3 × 7
```

---

**Per a 72:**

```
72 ÷ 2 = 36
36 ÷ 2 = 18
18 ÷ 2 = 9
9 ÷ 3 = 3
3 ÷ 3 = 1

Factorització: 72 = 2³ × 3²
```

---

### 3.2 Taula de Divisió Successiva

| Nombre | Pas 1 | Pas 2 | Pas 3 | Pas 4 | Factorització |
|--------|-------|-------|-------|-------|---------------|
| 50 | 50÷2=25 | 25÷5=5 | 5÷5=1 | — | 2 × 5² |
| 100 | 100÷2=50 | 50÷2=25 | 25÷5=5 | 5÷5=1 | 2² × 5² |
| 48 | 48÷2=24 | 24÷2=12 | 12÷2=6 | 6÷2=3 | 2⁴ × 3 |
| 64 | 64÷2=32 | 32÷2=16 | 16÷2=8 | 8÷2=4 | 2⁶ |

(Per a 64, continuem: 4÷2=2, 2÷2=1)

---

## 📌 Part 4: Teorema Fonamental

### 4.1 Unicitat de la Factorització

**Per a 60:**

Factorització 1: 2 × 2 × 3 × 5 = 60
Factorització 2: 2² × 3 × 5 = 60

Són iguals? **Sí** (és la mateixa factorització, només escrita diferent)

---

**Per a 84:**

Factorització 1: 2 × 2 × 3 × 7 = 84
Factorització 2: 2² × 3 × 7 = 84

Són iguals? **Sí**

---

### 4.2 Per Què No Hi Ha Altres Factoritzacions?

**28 = 4 × 7 = (2 × 2) × 7 = 2² × 7** (factorització primer completa)

---

**Explicació del Teorema Fonamental:**

El Teorema diu que UNA SOLA manera existeix de factoritzar un nombre en primers. Per exemple:

- 30 = 2 × 3 × 5 (única manera)
- No pots escriure 30 = 2 × 2 × ... (2² no divideix 30)
- No pots escriure 30 = 3 × 3 × ... (3² no divideix 30)

**Per què?** Perquè els primers són els "àtoms" dels nombres: no es poden trencar més.

---

## 📌 Part 5: Forma Exponencial

### 5.1 Converteix a Forma Exponencial

| Multiplicació | Forma Exponencial |
|---------------|------------------|
| 2 × 2 × 2 × 3 × 3 | **2³ × 3²** |
| 5 × 5 × 7 | **5² × 7** |
| 2 × 3 × 3 × 3 × 5 | **2 × 3³ × 5** |
| 2 × 2 × 2 × 2 × 5 | **2⁴ × 5** |
| 3 × 7 × 7 × 7 | **3 × 7³** |

---

### 5.2 Calcula el Valor

| Forma Exponencial | Càlcul | Valor |
|------------------|--------|-------|
| 2³ × 3² | 8 × 9 | **72** |
| 2² × 5² | 4 × 25 | **100** |
| 3² × 7 | 9 × 7 | **63** |
| 2⁴ × 3 | 16 × 3 | **48** |

---

## 📌 Part 6: Aplicacions — MCD i MCM usant Factorització

### 6.1 Calcula MCD usant Primers

| Números | Factorització 1 | Factorització 2 | MCD |
|---------|----------------|----------------|-----|
| 60, 84 | 2² × 3 × 5 | 2² × 3 × 7 | 2² × 3 = **12** |
| 72, 96 | 2³ × 3² | 2⁵ × 3 | 2³ × 3 = **24** |
| 100, 150 | 2² × 5² | 2 × 3 × 5² | 2 × 5² = **50** |

**Explicació:** Fem 72 = 8 × 9 = 2³ × 3² i 96 = 32 × 3 = 2⁵ × 3

Per al MCD, agafem la potència MENOR de cada factor comú.

---

### 6.2 Calcula MCM usant Primers

| Números | Factorització 1 | Factorització 2 | MCM |
|---------|----------------|----------------|-----|
| 60, 84 | 2² × 3 × 5 | 2² × 3 × 7 | 2² × 3 × 5 × 7 = **420** |
| 72, 96 | 2³ × 3² | 2⁵ × 3 | 2⁵ × 3² = **288** |
| 100, 150 | 2² × 5² | 2 × 3 × 5² | 2² × 3 × 5² = **300** |

**Explicació:** Per al MCM, agafem la potència MAJOR de cada factor primer que apareix.

Per a 72 i 96: 2⁵ (la major entre 2³ i 2⁵) i 3² (la major entre 3² i 3¹)

---

## 📌 Part 7: Comptador de Divisors

### 7.1 Usa la Factorització per Comptar Divisors

| Nombre | Factorització | Fórmula | Nombre de Divisors |
|--------|--------------|--------|-------------------|
| 12 | 2² × 3 | (2+1)(1+1) | **6** |
| 20 | 2² × 5 | (2+1)(1+1) | **6** |
| 36 | 2² × 3² | (2+1)(2+1) | **9** |
| 48 | 2⁴ × 3 | (4+1)(1+1) | **10** |

**Verificació per a 12:**
- Divisors: 1, 2, 3, 4, 6, 12
- Total: 6 ✓

**Verificació per a 36:**
- Divisors: 1, 2, 3, 4, 6, 9, 12, 18, 36
- Total: 9 ✓

---

### 7.2 Verifica Comptant Divisors

**Per a 20 = 2² × 5:**
- Divisors teòrics = (2+1)(1+1) = **6**
- Divisors reals: 1, 2, 4, 5, 10, 20
- Match? **Sí** ✓

---

## 📌 Part 8: Repte — Propietats Especials

### 8.1 Números Perfectes

**Verifica si 28 és perfect:**

28 = 2² × 7
- Divisors: 1, 2, 4, 7, 14, 28
- Divisors propis: 1, 2, 4, 7, 14
- Suma: 1 + 2 + 4 + 7 + 14 = **28** ✓
- **28 és perfect! Sí**

---

**Números perfectes coneguts:**

Els primers quatre són: **6, 28, 496, 8128**

Euclides va descobrir la fórmula (2000 anys ago):

**Si 2^n - 1 és primer, llavors 2^(n-1) × (2^n - 1) és perfect**

Exemple: n = 2
- 2² - 1 = 3 (primer!)
- 2¹ × 3 = **6** (perfect!) ✓

---

### 8.2 Números Amics

**Per què la factorització primer ajuda a trobar números amics?**

**Resposta:** Perquè la suma dels divisors d'un nombre depèn de la seva factorització primer:

**Fórmula de suma de divisors:** Si n = p₁^a × p₂^b, llavors:

σ(n) = (p₁^(a+1) - 1)/(p₁ - 1) × (p₂^(b+1) - 1)/(p₂ - 1)

Dos nombres són amics si σ(a) = b i σ(b) = a.

---

## 📌 Part 9: Problemes Reals de Factorització

### 9.1 Distribució i Agrupament

**Problema 1:** Tens 60 caramels i 84 fruites. Vols fer paquets iguals amb cada tipus sense sobres. Quants paquets màxim?

- Factoritzacions: 60 = 2² × 3 × 5; 84 = 2² × 3 × 7
- MCD = 2² × 3 = 12
- **Resposta:** 12 paquets màxim

(Cada paquet té 60÷12 = 5 caramels i 84÷12 = 7 fruites)

---

**Problema 2:** Dues sirenes sonen: una cada 18 segons, l'altra cada 24 segons. Quan sonen juntes?

- Factoritzacions: 18 = 2 × 3²; 24 = 2³ × 3
- MCM = 2³ × 3² = 8 × 9 = 72
- **Resposta:** Cada 72 segons sonen juntes

---

### 9.2 Desxiframent de Codis

**Codi secret:** Un nombre es forma multiplicant dos factors primers: ? × ? = 143

143 ÷ 11 = **13**

**Factors:** 11 i 13

Verificació: 11 × 13 = 143 ✓

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Factoritzacions

**Exemple de resposta 1:**

"Factoritza el nombre **60** usant arbre de factors"

**Solució:** 60 = 2² × 3 × 5

---

**Exemple de resposta 2:**

"Si n = **2² × 3 × 5**, quants divisors té?"

**Solució:** (2+1)(1+1)(1+1) = 3 × 2 × 2 = 12 divisors

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què és important que la factorització primer sigui ÚNICA?

**Resposta:** Perquè permet:
- Identificar de forma inequívoca qualsevol nombre (com un "DNI numèric")
- Calcular eficientment MCD, MCM, divisors
- Desenvolupar criptografia (RSA es basa en això!)
- Comprendre l'estructura dels nombres

---

**Pregunta 2:** On vas veure factorització en el món real?

**Resposta:** 
- **Internet/Criptografia:** RSA encriptació es basa en factoritzar nombres grans
- **Música:** harmònics (múltiples de frequencies primeres)
- **Distribució:** dividir recursos equitativament
- **Calendaris:** cicles que es sincronitzen (MCM)

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Arbre de factors): ✓
- [ ] Part 3 (Divisió successiva): ✓
- [ ] Part 4 (Teorema Fonamental): ✓
- [ ] Part 5 (Forma exponencial): ✓
- [ ] Part 6 (MCD i MCM): ✓
- [ ] Part 7 (Comptador de divisors): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Problemes reals): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, dominas la factorització! 🎉

---

## 🌍 Context Històric: El Teorema Fonamental de l'Aritmètica

### Els Grecs Antics (300 BC - Euclides)

Euclides va escriure els **Elementos** (13 llibres, la més influent obra matemàtica de tots els temps).

**Elements, Llibre IX, Proposició 14:**

"Si un nombre és mesurat pels nombres primers, no serà mesurat per cap altre nombre primer."

Això significava: cada nombre té UNA ÚNICA factorització!

Euclides no usava exponents moderns (els grecs no tenia símbols), però el concepte era clar.

---

### Edat Mitjana (1000-1400 AD - Context Perdut)

Tràgicament, durant l'Edat Mitjana occidental, el treball d'Euclides va ser "oblidat". Els matemàtics islàmics, però, el van preservar!

**Al-Khwarizmi** (800 AD, matemàtic persa) va definir sistemes per a factoritzacions.

---

### Renaixentista (1500s - Redescoberta)

Quan els Europeans van redescobrir Euclides, van formalitzar més la teoria dels nombres.

**Cardano (1501-1576)** va desenvolupar el primer sistema d'exponents moderns.

---

### Gauss i la Formalització (1777-1855)

**Carl Friedrich Gauss** (el "Príncep dels Matemàtics") va provar formalment:

**Teorema Fonamental de l'Aritmètica:**
"Tot nombre enter > 1 es pot expressar de forma única com a producte de primers (fins a l'ordre)."

Gauss va provar-ho als seus **Disquisitiones Arithmeticae** (1801), revolucionant la teoria de nombres.

---

### Era de la Criptografia (1900s - Present)

El Teorema Fonamental es va convertir en la **BASE DE TOTA LA CRIPTOGRAFIA MODERNA**.

**RSA Cryptography (1977):**
- **R**ivest, **S**hamir, **A**dleman
- Descobriment: és fàcil multiplicar 2 primers grans, però MOLT DUR factoritzar el producte
- Això protegeix cada transacció online!

**Exemple real:**
- Número de 2048 bits (més de 600 dígits)
- Pots multiplicar dos primers de 1024 bits en **1 millisegon**
- Pots factoritzar el producte en... milions d'anys!

---

## 🔐 Per Què la Unicitat és Crítica per a la Seguretat

### Imagina un Escenari Sense Unicitat

Si 12 pogués ser:
- 12 = 2² × 3
- 12 = 2 × 2 × 3 (escrit diferent)
- 12 = 4 × 3 (però 4 no és primer... per què no podria ser?)

Això ROMPRIA tota la criptografia!

### Com Funciona RSA

1. **Clau Pública:** Un nombre N = p × q (producte de dos nombres primers grans)
2. **Clau Privada:** Els primers p i q
3. **Encriptació:** Qualsevol pot usar N per encriptar
4. **Desencriptació:** SOLS qui coneix p i q pot desencriptar

**Per què funciona?** Perquè el Teorema Fonamental GARANTEIX que N té UNA ÚNICA factorització!

Si no fos única, hi hauria múltiples manera de desencriptar (INSEGURETAT!)

---

## 🎓 Resum: Els Números com a "Àtoms Moleculars"

| Concepte | Analogia | Exemple |
|----------|----------|---------|
| **Primer** | Àtom químic | 2, 3, 5, 7, ... |
| **Número compost** | Molècula | 12 = 2² × 3 (3 àtoms) |
| **Factorització** | Composició molecular | H₂O = 2H + 1O |
| **Unicitat** | Un CO₂ sempre és idèntic | 12 sempre és 2² × 3 |

Aquesta analogia és profunda: els números s'organitzen exactament com els àtoms!

---

## ✅ Aplicacions Modernes del Teorema Fonamental

### 1. **Criptografia RSA** (Internet)
Tots els teus compres online, emails, missatges estan protegits pel Teorema Fonamental.

### 2. **Correctiva de Errors** (Transmissió de Dades)
Els codis per detectar errors usen factoritzacions de nombres cíclics.

### 3. **Compressió de Dades** (ZIP, MP3)
L'algoritme DEFLATE usa factorització per optimitzar compressió.

### 4. **Comptació de Divisors** (Enginyeria)
Quan dissenyem engranatges, usem la fórmula de nombre de divisors.

### 5. **Testeig de Primalitat** (Informàtica)
Determinar si un número és primer (per criptografia) usa factorització.

---

## 🏆 El Futur: Computadors Quàntics

**Repte del Futur:** Els computadors quàntics podran factoritzar números grans en pocs segons!

**Algoritme de Shor (1994):**
Descubert per Peter Shor, demonstra que els computadors quàntics podrien "trencar" RSA.

**Conseqüència:** Els criptògrafs moderns estan desenvolupant criptografia "post-quàntica" que NO es basa en factorització.

El Teorema Fonamental seguirà sent vertader per sempre, però potser ja no serà la base de la seguretat digital!

---

## ✨ La Bellesa Profunda

Euclides va descobrir fa 2300 anys que els números són construïts de "pedretes" indivisibles (els primers).

Aquest descobriment simple:
- Va revolucionar la matemàtica
- Va permetre la criptografia
- Va protegir la privacitat digital
- Segueix sent la base del nostre món connectat

**"Els primers són els àtoms de l'aritmètica."** — Euclides (300 BC)


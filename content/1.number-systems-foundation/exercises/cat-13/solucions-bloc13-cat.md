# Solucions Bloc 13 – Nombres de Mersenne i Primers de Mersenne

---

## 📌 Part 1: Comprensió de Nombres de Mersenne

### 1.1 Completa les Definicions

**Nombre de Mersenne:** Un nombre de la forma **2^p - 1** on p és un nombre premier.

**Primer de Mersenne:** Un nombre de Mersenne que és **premier/primer**.

**Exponent de Mersenne:** El nombre **p** en 2^p - 1.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 2³ - 1 = 7 és un nombre de Mersenne | **V** | 3 és primer i 2³ - 1 = 7 ✓ |
| Tots els 2^p - 1 són premiers | **F** | 2^11 - 1 = 2047 = 23 × 89 (NO premier) |
| Els primers de Mersenne són rars | **V** | Només 52 descoberts fins 2024, mentre primers p-th és infinit |
| Els primers de Mersenne són sempre parells | **F** | Per p > 2, 2^p - 1 sempre és senar (parell - 1) |

---

## 📌 Part 2: Calcula Nombres de Mersenne

### 2.1 Taula de Números de Mersenne

| p | 2^p | 2^p - 1 | Primer? |
|---|-----|---------|---------|
| 2 | 4 | 3 | **Sí** ✓ |
| 3 | 8 | 7 | **Sí** ✓ |
| 5 | 32 | 31 | **Sí** ✓ |
| 7 | 128 | 127 | **Sí** ✓ |
| 11 | 2048 | 2047 | **No** (23 × 89) |
| 13 | 8192 | 8191 | **Sí** ✓ |

---

### 2.2 Completa la Taula

Per a **p = 11:**
- 2^11 = **2048**
- 2^11 - 1 = **2047**
- És premier? **No** (2047 = 23 × 89)

---

Per a **p = 13:**
- 2^13 = **8192**
- 2^13 - 1 = **8191**
- És premier? **Sí** ✓ (primer de Mersenne #5)

---

## 📌 Part 3: Condició Necessària per a Premiers de Mersenne

### 3.1 Comprensió: p ha de ser primer

**Teorema:** Si 2^n - 1 és premier, llavors n ha de ser premier.

**Contraexemple:** Si n és compost, 2^n - 1 NO és primer.

---

| n | Tipus | 2^n - 1 | Factorització |
|---|-------|---------|---------------|
| 4 (compost) | 2² | 15 | **3 × 5** |
| 6 (compost) | 2 × 3 | 63 | **7 × 9** |
| 8 (compost) | 2³ | 255 | **3 × 5 × 17** |
| 9 (compost) | 3² | 511 | **7 × 73** |

---

### 3.2 Per Què no Funciona n Compost?

**Identitat Algebraica (Factorització):**

Si n = a × b, llavors:

**2^(a×b) - 1 = (2^a - 1) × (2^(a(b-1)) + 2^(a(b-2)) + ... + 2^a + 1)**

Per tant **2^a - 1 sempre divideix 2^n - 1**.

---

**Exemple:** n = 6 = 2 × 3
- 2^2 - 1 = 3 (divisor de 2^6 - 1)
- 2^3 - 1 = 7 (divisor de 2^6 - 1)
- 2^6 - 1 = 63 = 3 × 21 = 3 × 7 × 3 ✓

**Conclusió:** n compost → 2^n - 1 compost (sempre!)

Per tant, per a 2^n - 1 ser premier, **n MUST be premier**.

---

## 📌 Part 4: Primers de Mersenne Coneguts

### 4.1 Els Primers 12 Premiers de Mersenne

| # | p | 2^p - 1 | Dígits | Any |
|---|---|---------|--------|-----|
| 1 | 2 | 3 | 1 | Ancient |
| 2 | 3 | 7 | 1 | Ancient |
| 3 | 5 | 31 | 2 | Ancient |
| 4 | 7 | 127 | 3 | 500 BC (Grega) |
| 5 | 13 | 8191 | 4 | 1461 |
| 6 | 17 | 131071 | 6 | 1588 |
| 7 | 19 | 524287 | 6 | 1588 |
| 8 | 31 | 2147483647 | 10 | 1772 (Euler) |
| 9 | 61 | 2^61 - 1 | 19 | 1883 (Pervushin) |
| 10 | 89 | 2^89 - 1 | 27 | 1911 (Powers) |
| 11 | 107 | 2^107 - 1 | 33 | 1914 (Powers) |
| 12 | 127 | 2^127 - 1 | 39 | 1876 (Lucas) |

---

### 4.2 Observa els Patrons

**Pregunta:** Els exponents p (2, 3, 5, 7, 13, 17, 19, 31...) sembla que siguin?

**Resposta:** **TOTS PRIMERS!** (condició necessària provada)

---

**Pregunta:** Quants dígits té 2^127 - 1?

**Resposta:** **39 dígits** (descobert per Lucas el 1876)

Número complet: 170141183460469231731687303715884105727

---

## 📌 Part 5: Proves de Primalitat

### 5.1 Prova de Lucas-Lehmer

**Algoritme eficient per verificar si 2^p - 1 és premier (p > 2):**

Defineix: M_p = 2^p - 1

S₀ = 4

For i = 1 to p-2:
  Sᵢ = (Sᵢ₋₁)² - 2 (mod M_p)

**Si S_{p-2} ≡ 0 (mod M_p), llavors M_p és premier!**

---

**Avantatges:**
- Molt més ràpid que provar divisors
- Permet verificar números ENORMES
- Revolucionà la recerca de primers de Mersenne

---

### 5.2 Aplica para p = 5

M₅ = 2^5 - 1 = **31**

S₀ = 4

**S₁ = (4² - 2) mod 31 = (16 - 2) mod 31 = 14 mod 31 = 14**

**S₂ = (14² - 2) mod 31 = (196 - 2) mod 31 = 194 mod 31 = 8** (194 = 6×31 + 8)

**S₃ = (8² - 2) mod 31 = (64 - 2) mod 31 = 62 mod 31 = 0** (62 = 2×31)

**S₃ = 0, per tant 2^5 - 1 = 31 és premier!** ✓

---

## 📌 Part 6: Relació amb Números Perfectes

### 6.1 Fórmula d'Euclides

**Si 2^p - 1 és premier, llavors:**

**N = 2^(p-1) × (2^p - 1) és un número PERFECT!**

**Gauss provà que TOTS els números perfectes parells són d'aquesta forma.**

---

| p | 2^p - 1 | Primer? | N = 2^(p-1) × (2^p - 1) | Verificació |
|---|---------|--------|----------------------|-----------|
| 2 | 3 | **Sí** | 2¹ × 3 = **6** | σ(6) = 1+2+3+6 = 12; N = 6 ✓ |
| 3 | 7 | **Sí** | 2² × 7 = **28** | σ(28) = 1+2+4+7+14+28 = 56; N = 28 ✓ |
| 5 | 31 | **Sí** | 2⁴ × 31 = **496** | Perfect ✓ |
| 7 | 127 | **Sí** | 2⁶ × 127 = **8128** | Perfect ✓ |

---

### 6.2 Descubre Números Perfectes Nous

**Per a p = 13:**
- 2^13 - 1 = **8191** (és premier? **Sí** ✓)
- N = 2^12 × 8191 = 4096 × 8191 = **33550336**
- **33550336 és un número perfect!** (5è nombre perfecte)

---

**Per a p = 17:**
- 2^17 - 1 = **131071** (primer? Sí)
- N = 2^16 × 131071 = 65536 × 131071 = **8589869056**
- **8589869056 és un número perfect!** (6è nombre perfecte)

---

## 📌 Part 7: La Recerca Moderna

### 7.1 Llista de Descobriments

| # | p | Descoberta | Investigador | Dígits |
|---|---|-----------|---------------|---------| 
| 1-4 | 2,3,5,7 | Ancient | Grecs | 1-3 |
| 5-8 | 13,17,19,31 | 1400-1700 | Vàrios | 4-10 |
| 13 | 521 | **1952** | Computador Robinson | 157 |
| 14 | 607 | 1952 | Computador Robinson | 183 |
| 15 | 1279 | 1952 | Computador Robinson | 386 |
| 20 | 4423 | 1961 | Computador Hurwitz | 1332 |
| 25 | 21701 | 1978 | Noll, Nickel | 6533 |
| 30 | 110503 | 1988 | Colquitt, Welsh | 33265 |
| 52 | **136279279** | **2024** | GIMPS (Great Internet Mersenne Prime Search) | **41,024,320 dígits!** |

---

### 7.2 Creixement dels Exponents

**Els exponents dels primers de Mersenne:**

2, 3, 5, 7, 13, 17, 19, 31, 61, 89, 107, 127, 521, 607, 1279, 4423, ...

---

**Pregunta:** Com creixen els exponents p?

**Resposta:** De forma EXPONENCIAL! Els senyals:
- Primer gap: 3-5 = 2
- Segon: 7-5 = 2
- Tercer: 13-7 = 6
- Quart: 31-19 = 12
- Cinquè: 521-127 = 394 (enorme!)
- Actualment: gaps de milions!

---

**Pregunta:** Quants dígits té 2^136279279 - 1?

**Resposta:** Aproximadament **41,024,320 dígits!**

Per imprimir el número:
- A 1000 dígits per pàgina → 41,024 pàgines
- A 100 pàgines per resma → 410 resmes de paper!

---

## 📌 Part 8: Repte — Propietats Especials

### 8.1 Números de Mersenne Imparells

**Pregunta:** Per a p > 2, 2^p - 1 sempre és senar o parell?

**Resposta:** **SEMPRE SENAR** (imparell)

---

**Pregunta:** Per què? (Pista: 2^p sempre és parell)

**Resposta:** 
- 2^p és parell (qualsevol potència de 2)
- parell - 1 = **senar**
- Per tant 2^p - 1 és sempre senar ✓

---

### 8.2 Suma de Divisors

**Per al primer de Mersenne p = 3:**
- M₃ = 7 (premier)
- Divisors: 1, 7
- σ(7) = 1 + 7 = 8

**Pregunta:** Per a tots els premiers de Mersenne, σ(M) = ?

**Resposta:** **σ(M) = M + 1** (perquè M és premier, els únics divisors són 1 i M!)

---

## 📌 Part 9: Aplicacions i Preguntes Obertes

### 9.1 Usages del Premiers de Mersenne

**Matemàtiques:**
- Teoria de números
- Números perfectes (1-a-1 correspondence)
- Criptografia probabilística
- Distribucions numèriques

---

**Computació:**
- **Testing de Computadors:** CPU/GPU validation (GIMPS usa esto)
- **Algoritmes de computació distribuïda:** Projectes científics globals
- **Distribució de càrrega:** Repartir treballadors per buscar nous primers
- **Benchmarking:** Mesurar velocitat de computadors

---

**Pràctica Real:**
- GIMPS (Great Internet Mersenne Prime Search): Voluntaris de tot el mundo
- Descobriment del #52 (2024): Any de computació compartida!

---

### 9.2 La Gran Pregunta Oberta

**Conjectura Principal (NO RESOLTA):** 

**"Hi ha infinits premiers de Mersenne?"**

---

**Evidència Matemàtica:**
- Només 52 descoberts en 3000 anys
- Creixen cada vegada més rarament
- Però potser infinits? **DESCONEGUT!**

---

**Premi:** 
- Qui provi aquesta conjectura farà história
- Teoriticament podria portar $100M+ de reconeixement

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Mersenne

**Exemple de resposta 1:**

"Per a p = 7, calcula 2^p - 1 i determina si és premier"

**Solució:** 
- 2^7 = 128
- 2^7 - 1 = 127
- Testing: 127 no és divisible per 3, 5, 7, 11 (√127 ≈ 11.3)
- **127 és premier!** (4t primer de Mersenne)

---

**Exemple de resposta 2:**

"Usa la fórmula d'Euclides per generar un número perfect usant p = 13"

**Solució:** 
- 2^13 - 1 = 8191 (és premier)
- N = 2^(13-1) × (2^13 - 1) = 2^12 × 8191 = 4096 × 8191 = **33550336**
- **N és perfect!**

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què els primers de Mersenne són tan importants?

**Resposta:**
1. **Conexió amb números perfectes:** 1-a-1 correspondence
2. **Algoritmes eficients:** Lucas-Lehmer és MOLT ràpid
3. **Benchmarking informàtic:** Prova poder de computadors
4. **Teoria de números:** Ens ensenya sobre l'estructura dels primers
5. **Preguntes obertes:** Encara no sabem si són infinits!

---

**Pregunta 2:** Creus que hi ha infinits premiers de Mersenne?

**Resposta:**
- **Opinió matemàtica:** PROBABLEMENT sí, però no provat
- **Evidència:** Densidade decreix però sembla no-zero
- **Futur:** Potser provarem en aquest segle amb teories noves
- **Conjectura de Artin:** Relacionada, suggereix infinitud
- **La veritat:** DESCONEGUDA! 🔍

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Calcula): ✓
- [ ] Part 3 (Condició Necessària): ✓
- [ ] Part 4 (Coneguts): ✓
- [ ] Part 5 (Lucas-Lehmer): ✓
- [ ] Part 6 (Números Perfectes): ✓
- [ ] Part 7 (Recerca Moderna): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Aplicacions): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, eres un expert en Mersenne! 🎉

---

## 🌍 Context Històric: Els Primers de Mersenne a Través dels Segles

### Antiguitat (500-1000 BC)

**Euclides (300 BC):**

"Si 2^p - 1 és premier, llavors 2^(p-1) × (2^p - 1) és perfect."

Euclides no coneixia si 2^p - 1 era sempre primer quan p és primer, però va establir la connexió.

---

**Mersenne (1588-1648):**

Monjo francés, matemàtic, músic, i filòsof.

Va afirmar (en 1644): Aquests p solen donar primers:

**p = 2, 3, 5, 7, 13, 17, 19, 31, 67, 127, 257**

(Algunes afirmacions eren incorrectes, però va iniciar la recerca sistemàtica)

---

### Era de la Verificació Manual (1600-1800)

**Marin Mersenne (1600s):**
- Definia Mₚ = 2^p - 1
- Els "Primers de Mersenne" van rebre el seu nom

---

**Leonhard Euler (1707-1783):**

Verificà que M₃₁ = 2^31 - 1 = 2147483647 és premier!

(El nombre premier més gran descobert fins aquell moment)

---

**Édouard Lucas (1842-1891):**

Descobrí **Lucas-Lehmer test** (1878):
- Algoritme ràpid per verificar primers de Mersenne
- Revolucionà la recerca

Descobrí que M₁₂₇ és premier (39 dígits!)

---

### Era del Computador (1950s-Present)

**1952:** Computador Robinson verifica:
- M₅₂₁, M₆₀₇, M₁₂₇₉ son premiers!
- Primer cop que computadors descobrien nous primers

---

**Donald Knuth (1940s-present):**
"The Art of Computer Programming" dedica capítols sencers a Mersenne.

---

**GIMPS - Great Internet Mersenne Prime Search (1996-Present):**

Projecte distribuït mundial on voluntaris col·laboren:
- 2024: Descobert el #52 — 2^136279279 - 1
- 41+ milions de dígits!

---

## 💾 Tecnologia & Mersenne

### Per Què Usem Mersenne per a Testing?

1. **Computacionalment eficient:** Operacions en base-2 són rápides
2. **Lucas-Lehmer test:** Algoritme especialitzat ultra-ràpid
3. **Stabilitat:** Les propietats matemàtiques són ben-conegudes
4. **Benchmarking:** Permet comparar directament velocitats de CPUs

---

### GIMPS: Com Funciona

1. **Voluntari descarrega PrimeNet software**
2. **Assignen exponent p a verificar**
3. **Computador corre Lucas-Lehmer test local**
4. **Resultats es retornen (premier o no)**
5. **Si premier → FAMA MUNDIAL + posiblement $$$**

---

## 🔮 Preguntes Obertes (2024)

### 1. **Infinits Primers de Mersenne?**

**Status:** DESCONEGUT (3000 anys sense prova)

### 2. **Quants números perfectes hi ha?**

**Status:** Probablement infinits imparells, cap parell no-Mersenne (DESCONEGUT)

### 3. **Qual és el següent premier de Mersenne?**

**Status:** Buscant activament

---

## ✨ La Bellesa Profunda

Els primers de Mersenne representen la **cerca humana per l'ordre en el caos**.

Números simples (2^p - 1), però extraordinàriament rars.

La seva connexió amb números perfectes i la utilitat per a testeig computacional revela:

**Els patrons matemàtics més simples sovint oculten complexitat profunda.**

---

**"Un premier de Mersenne és com una perlota al fons de l'oceà matemàtic — buscades, belles, i quan es troben, transformem la nostra comprensió."** — Adaptació de Donald Knuth


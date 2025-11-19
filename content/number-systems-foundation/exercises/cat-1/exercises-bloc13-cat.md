# Exercicis - Mòdul 1: Bloc 13 – Exploració de Patrons de Residus

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Patró de Residus Simples

**Enunciat:**

Crea una taula de residus per a potències de `2` mòdul `5`:

| n | 2^n | 2^n mod 5 |
|---|-----|-----------|
| 1 | 2 | ? |
| 2 | 4 | ? |
| 3 | 8 | ? |
| 4 | 16 | ? |
| 5 | 32 | ? |
| 6 | 64 | ? |

a) Completa la taula.
b) Identifica el patró (quina és la longitud del cicle?).

**Solució:**

a) **Taula completada:**

| n | 2^n | 2^n mod 5 |
|---|-----|-----------|
| 1 | 2 | 2 |
| 2 | 4 | 4 |
| 3 | 8 | 3 |
| 4 | 16 | 1 |
| 5 | 32 | 2 |
| 6 | 64 | 4 |

b) **Patró:**
   - Seqüència de residus: `2, 4, 3, 1, 2, 4, 3, 1, ...`
   - **Longitud del cicle: 4** (es repeteix cada 4 passos)
   - Notació: `2^n mod 5` té període `4`.

**Concepte avaluat:** Identificació de cicles en residus, detecció de periodicitat.

---

### **Exercici 2** 🟦 (1.1 punts) – Patró de Múltiples

**Enunciat:**

Crea una taula de residus per a múltiples de `7` mòdul `3`:

| n | 7n | 7n mod 3 |
|---|----|----|
| 1 | 7 | ? |
| 2 | 14 | ? |
| 3 | 21 | ? |
| 4 | 28 | ? |
| 5 | 35 | ? |
| 6 | 42 | ? |

a) Completa la taula.
b) Identifica el patró.
c) Per què es repeteix a partir de `n = 3`?

**Solució:**

a) **Taula completada:**

| n | 7n | 7n mod 3 |
|---|----|----|
| 1 | 7 | 1 |
| 2 | 14 | 2 |
| 3 | 21 | 0 |
| 4 | 28 | 1 |
| 5 | 35 | 2 |
| 6 | 42 | 0 |

b) **Patró:**
   - Seqüència: `1, 2, 0, 1, 2, 0, ...`
   - **Longitud del cicle: 3** (se repeteix cada 3 passos)

c) **Per què es repeteix:**
   - `7 ≡ 1 (mod 3)`, per tant `7n ≡ n (mod 3)`.
   - Els múltiples de 7 mòdul 3 segueixen el patró de `n` mòdul 3.
   - Cicle: `n mod 3` té període 3.

**Concepte avaluat:** Patrons en múltiples, connexió entre base i mòdul.

---

### **Exercici 3** ⭐ (0.9 punts) – Detecció de Cicles

**Enunciat:**

Per a les següents bases i mòduls, determina la longitud del cicle (ordre):

a) Potències de `3` mòdul `7`
b) Potències de `2` mòdul `7`
c) Potències de `4` mòdul `5`

**Solució:**

a) **`3^n mod 7`:**
   - `3^1 = 3 mod 7 = 3`
   - `3^2 = 9 mod 7 = 2`
   - `3^3 = 27 mod 7 = 6`
   - `3^4 = 81 mod 7 = 4`
   - `3^5 = 243 mod 7 = 5`
   - `3^6 = 729 mod 7 = 1`
   - `3^7 = 2187 mod 7 = 3` (cicle comença novament)
   - **Longitud del cicle: 6**

b) **`2^n mod 7`:**
   - `2^1 = 2`, `2^2 = 4`, `2^3 = 1`, `2^4 = 2`, ...
   - **Longitud del cicle: 3**

c) **`4^n mod 5`:**
   - `4^1 = 4`, `4^2 = 16 mod 5 = 1`, `4^3 = 64 mod 5 = 4`, ...
   - **Longitud del cicle: 2**

**Concepte avaluat:** Detecció de cicles en potències, concepte d'ordre modular.

---

### **Exercici 4** 🟦 (1.2 punts) – Teorema d'Euler i Ordre

**Enunciat:**

El **Teorema d'Euler** estableix que si `mcd(a, n) = 1`, aleshores `a^φ(n) ≡ 1 (mod n)`, on `φ(n)` és la funció d'Euler.

a) Per a `a = 2, n = 5`: Calcula `φ(5)` i verifica que `2^φ(5) ≡ 1 (mod 5)`.

b) Per a `a = 3, n = 7`: Calcula `φ(7)` i verifica que `3^φ(7) ≡ 1 (mod 7)`.

(Recorda: `φ(n)` = nombre d'enters menors que `n` que són coprims amb `n`.)

**Solució:**

a) **`a = 2, n = 5`:**
   - `φ(5) = 4` (nombres coprims amb 5: 1, 2, 3, 4)
   - `2^4 = 16 mod 5 = 1` ✓
   - **Verificat**

b) **`a = 3, n = 7`:**
   - `φ(7) = 6` (nombres coprims amb 7: 1, 2, 3, 4, 5, 6)
   - `3^6 = 729 mod 7 = ?`
   - `729 = 7 × 104 + 1`, per tant `729 mod 7 = 1` ✓
   - **Verificat**

**Concepte avaluat:** Teorema d'Euler, funció d'Euler, ordre d'elements.

---

### **Exercici 5** ⭐ (0.8 punts) – Aplicació: Dígits Repetits

**Enunciat:**

Els dígits de certs números es repeteixen de manera periòdica. Per exemple, `0.333... = 1/3`.

a) Per a `1/7`, calcula els dígits decimals repetits usant aritmètica modular.

**Solució:**

a) **Dígits de `1/7`:**
   - Per a aritmètica modular de `10^n mod 7`:
     - `10^1 mod 7 = 3`
     - `10^2 mod 7 = 2`
     - `10^3 mod 7 = 6`
     - `10^4 mod 7 = 4`
     - `10^5 mod 7 = 5`
     - `10^6 mod 7 = 1` (cicle tanca)
   
   - Els dígits de `1/7 = 0.142857142857...` (període 6)
   - Els residus `3, 2, 6, 4, 5, 1` corresponen als dígits `1, 4, 2, 8, 5, 7` (càlculs addicionals)

**Concepte avaluat:** Aplicació de cicles de residus a decimals periòdics.

---

### **Exercici 6** 🟦 (1.0 punt) – Taula de Residus Bidimensional

**Enunciat:**

Crea una taula de `(2^a × 3^b) mod 5`:

| a\b | 0 | 1 | 2 | 3 |
|-----|---|---|---|---|
| 0   | ? | ? | ? | ? |
| 1   | ? | ? | ? | ? |
| 2   | ? | ? | ? | ? |
| 3   | ? | ? | ? | ? |

Completa la taula.

**Solució:**

| a\b | 0 | 1 | 2 | 3 |
|-----|---|---|---|---|
| 0   | 1 | 3 | 4 | 2 |
| 1   | 2 | 1 | 3 | 4 |
| 2   | 4 | 2 | 1 | 3 |
| 3   | 3 | 4 | 2 | 1 |

(Per exemple: `(2^1 × 3^0) mod 5 = 2`, `(2^0 × 3^1) mod 5 = 3`, `(2^2 × 3^2) mod 5 = 4 × 9 mod 5 = 36 mod 5 = 1`, etc.)

**Concepte avaluat:** Taules de residus multidimensionals, visualització de patrons.

---

### **Exercici 7** 🟦 (1.1 punts) – Período de Successió de Residus

**Enunciat:**

Per a cada successió, determina la longitud del cicle:

a) Successió aritmètica: `a_n = 2n + 1` mòdul 7
b) Successió geomètrica: `a_n = 3^n` mòdul 11
c) Successió de Fibonacci: `F_n` mòdul 5

**Solució:**

a) **`a_n = 2n + 1 mod 7`:**
   - `n = 0: 1`, `n = 1: 3`, `n = 2: 5`, `n = 3: 0`, `n = 4: 2`, `n = 5: 4`, `n = 6: 6`, `n = 7: 1`
   - **Longitud del cicle: 7** (igual a 7)

b) **`a_n = 3^n mod 11`:**
   - `3^1 = 3`, `3^2 = 9`, `3^3 = 5`, `3^4 = 4`, `3^5 = 1`, `3^6 = 3`, ...
   - **Longitud del cicle: 5** (ordre de 3 mòdul 11)

c) **`F_n mod 5`:**
   - `0, 1, 1, 2, 3, 0, 3, 3, 1, 4, 0, 4, 4, 3, 2, 0, 2, 2, 4, 1, 0, 1, ...`
   - **Longitud del cicle: 20** (període de Pisano per 5)

**Concepte avaluat:** Períodes de diverses successións, ordre d'elements, període de Pisano.

---

### **Exercici 8** 🟦 (1.3 punts) – Predicció de Residus

**Enunciat:**

Usant els patrons de cicles, prediu residus sense calcular directament:

a) `2^{10} mod 5` (usant que el cicle és de longitud 4)
b) `3^{50} mod 7` (usant que el cicle és de longitud 6)
c) `F_{30} mod 5` (usant que el cicle és de longitud 20)

**Solució:**

a) **`2^{10} mod 5`:**
   - Cicle: longitud 4 (residus: 2, 4, 3, 1 que es repeteixen)
   - `10 = 4 × 2 + 2`, per tant `2^{10} ≡ 2^2 (mod 5) = 4`
   - **Resposta: 4**

b) **`3^{50} mod 7`:**
   - Cicle: longitud 6 (residus: 3, 2, 6, 4, 5, 1 que es repeteixen)
   - `50 = 6 × 8 + 2`, per tant `3^{50} ≡ 3^2 (mod 7) = 9 mod 7 = 2`
   - **Resposta: 2**

c) **`F_{30} mod 5`:**
   - Cicle: longitud 20
   - `30 = 20 × 1 + 10`, per tant `F_{30} ≡ F_{10} (mod 5)`
   - `F_{10} = 55`, i `55 mod 5 = 0`
   - **Resposta: 0**

**Concepte avaluat:** Predicció usant períodes, reduccio de exponents, eficiència computacional.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Període de Pisano

**Enunciat:**

El **Període de Pisano** `π(n)` és la longitud del cicle de Fibonacci mòdul `n`.

a) Calcula els primers termes de Fibonacci mòdul 3 fins que el cicle es complete.
b) Verifica que el período de Pisano per a 3 és `π(3) = 8`.
c) Usa el período per predir `F_{16} mod 3`.

**Solució:**

a) **Fibonacci mòdul 3:**
   - `F_0 = 0`, `F_1 = 1`, `F_2 = 1`, `F_3 = 2`, `F_4 = 0`, `F_5 = 2`, `F_6 = 2`, `F_7 = 1`, `F_8 = 0`, `F_9 = 1`, ...
   - Seqüència: `0, 1, 1, 2, 0, 2, 2, 1, 0, 1, ...`
   - Cicle comença novament a `F_8`

b) **Longitud del cicle:**
   - Des de `F_0` fins `F_7`: longitud 8
   - **`π(3) = 8`** ✓

c) **Predicció de `F_{16} mod 3`:**
   - `16 = 8 × 2 + 0`, per tant `F_{16} ≡ F_0 (mod 3) = 0`
   - **Resposta: 0**

**Concepte avaluat:** Període de Pisano, cicles en successións especials, predicció usant períodes.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Análisis de Cicles Complexes

**Enunciat:**

Investigació: Per a quins mòduls `n` és la longitud del cicle de `2^n` exactament `φ(n)`?

a) Comprova per a `n = 3, 5, 7, 9, 11`.

b) Formula una conjectura.

**Solució:**

a) **Comprovació:**
   
   - `n = 3`: `φ(3) = 2`, longitud del cicle de `2^n mod 3`: `2^1 = 2, 2^2 = 1, 2^3 = 2` → cicle longitud 2 ✓
   - `n = 5`: `φ(5) = 4`, longitud del cicle de `2^n mod 5`: cicle longitud 4 (verificat anteriorment) ✓
   - `n = 7`: `φ(7) = 6`, longitud del cicle de `2^n mod 7`: `2^6 ≡ 1 (mod 7)` → cicle longitud 6 ✓
   - `n = 9`: `φ(9) = 6`, longitud del cicle de `2^n mod 9`: `2^1 = 2, 2^2 = 4, 2^3 = 8, 2^4 = 7, 2^5 = 5, 2^6 = 1` → cicle longitud 6 ✓
   - `n = 11`: `φ(11) = 10`, longitud del cicle de `2^n mod 11`: és 10 (perquè `mcd(2, 11) = 1`) ✓

b) **Conjectura:**
   - Per a primers `p` on `2` és una **arrel primitiva** (generator del grup multiplicatiu), la longitud del cicle és `φ(p) = p - 1`.
   - Els nombres (primers o potències de primers) per als quals es compleix aquesta propietat són aquells on `2` és una arrel primitiva.

**Concepte avaluat:** Investigació de patrons, arrels primitives, teoria de nombres avançada.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Patró de residus simples | Moderat |
| 2 | Patró de múltiples | Intermedi |
| 3 | Detecció de cicles | Moderat |
| 4 | Teorema d'Euler | Intermedi |
| 5 | Aplicació: decimals | Moderat |
| 6 | Taules multidimensionals | Intermedi |
| 7 | Período de successións | Intermedi |
| 8 | Predicció usant períodes | Intermedi |
| 9 | Període de Pisano | Desafiador |
| 10 | Arrels primitives | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Esperar cicles que comencen a n=0**: Els cicles sovint comencen després d'alguns termes inicials.
2. **Negligir que no tots els residus apareixen**: Els cicles seleccionen subconjunts del grup.
3. **Confondre ordre amb període de Pisano**: Són conceptes relacionats però diferents.


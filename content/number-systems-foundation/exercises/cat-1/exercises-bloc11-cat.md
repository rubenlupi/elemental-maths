# Exercicis - Mòdul 1: Bloc 11 – Nombres Especials (Perfectes, Triangulars, Fibonacci)

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Verificació de Nombres Perfectes

**Enunciat:**

Un **nombre perfecte** és igual a la suma dels seus divisors propis (tots els divisors excepte ell mateix).

Verifica si els següents nombres són perfectes:

a) `6`
b) `28`
c) `16`

**Solució:**

a) **`6` és perfecte?**
   - Divisors propis de 6: 1, 2, 3
   - Suma: `1 + 2 + 3 = 6` ✓
   - **SÍ, 6 és perfecte.**

b) **`28` és perfecte?**
   - Divisors propis de 28: 1, 2, 4, 7, 14
   - Suma: `1 + 2 + 4 + 7 + 14 = 28` ✓
   - **SÍ, 28 és perfecte.**

c) **`16` és perfecte?**
   - Divisors propis de 16: 1, 2, 4, 8
   - Suma: `1 + 2 + 4 + 8 = 15 ≠ 16` ✗
   - **NO, 16 no és perfecte.**

**Concepte avaluat:** Definició de nombre perfecte, suma de divisors propis.

---

### **Exercici 2** 🟦 (1.1 punts) – Nombres Triangulars

**Enunciat:**

Un **nombre triangular** `T_n = n(n+1)/2` representa el nombre de punts en un triangle equilàter amb `n` files.

a) Calcula `T_1, T_2, T_3, T_4, T_5`.

b) Dibuixa la representació visual per a `T_4`.

c) Explica la fórmula.

**Solució:**

a) **Nombres triangulars:**
   - `T_1 = 1(1+1)/2 = 1`
   - `T_2 = 2(2+1)/2 = 3`
   - `T_3 = 3(3+1)/2 = 6`
   - `T_4 = 4(4+1)/2 = 10`
   - `T_5 = 5(5+1)/2 = 15`

b) **Representació visual per a `T_4 = 10`:**
   ```
   •
   ••
   •••
   ••••
   ```
   - Total: 1 + 2 + 3 + 4 = 10 punts

c) **Explicació de la fórmula:**
   - `T_n` és la suma de la seqüència `1 + 2 + 3 + ... + n`.
   - La fórmula `n(n+1)/2` és la forma tancada d'aquesta suma (suma aritmètica).

**Concepte avaluat:** Nombres triangulars, fórmula, representació visual, suma aritmètica.

---

### **Exercici 3** ⭐ (0.9 punts) – Seqüència de Fibonacci

**Enunciat:**

La **seqüència de Fibonacci** es defineix com `F_n = F_{n-1} + F_{n-2}` amb `F_0 = 0`, `F_1 = 1`.

a) Calcula els primers 10 termes: `F_0, F_1, ..., F_9`.

b) Identifica quins termes són nombres primers.

**Solució:**

a) **Primers 10 termes:**
   - `F_0 = 0`
   - `F_1 = 1`
   - `F_2 = 0 + 1 = 1`
   - `F_3 = 1 + 1 = 2`
   - `F_4 = 1 + 2 = 3`
   - `F_5 = 2 + 3 = 5`
   - `F_6 = 3 + 5 = 8`
   - `F_7 = 5 + 8 = 13`
   - `F_8 = 8 + 13 = 21`
   - `F_9 = 13 + 21 = 34`

b) **Nombres primers entre els termes:**
   - `F_3 = 2` (primer) ✓
   - `F_4 = 3` (primer) ✓
   - `F_5 = 5` (primer) ✓
   - `F_7 = 13` (primer) ✓
   - `F_8 = 21 = 3 × 7` (compost) ✗
   - `F_9 = 34 = 2 × 17` (compost) ✗

**Concepte avaluat:** Recurrència de Fibonacci, identificació de primers en la seqüència.

---

### **Exercici 4** 🟦 (1.2 punts) – Nombre d'Or en Fibonacci

**Enunciat:**

Els quocients de termes consecutius de Fibonacci s'aproximen al **nombre d'or** `φ ≈ 1.618`.

a) Calcula els quocients `F_n / F_{n-1}` per als següents `n`:
   - `n = 5, 6, 7, 8, 9, 10`

b) Observa com els quocients s'aproximen a `φ`.

**Solució:**

a) **Quocients de Fibonacci:**
   - `F_5 / F_4 = 5 / 3 ≈ 1.667`
   - `F_6 / F_5 = 8 / 5 = 1.600`
   - `F_7 / F_6 = 13 / 8 = 1.625`
   - `F_8 / F_7 = 21 / 13 ≈ 1.615`
   - `F_9 / F_8 = 34 / 21 ≈ 1.619`
   - `F_10 / F_9 = 55 / 34 ≈ 1.618`

b) **Observació:**
   - Els quocients oscil·len al voltant de `φ ≈ 1.618`.
   - A mesura que augmentem `n`, els quocients convergeixen cap al nombre d'or.
   - Això il·lustra la connexió entre Fibonacci i geometria (rectangle d'or, espirals).

**Concepte avaluat:** Convergència de quocients de Fibonacci al nombre d'or, comprensió de límits.

---

### **Exercici 5** ⭐ (0.8 punts) – Comparació de Nombres Especials

**Enunciat:**

Determina quins dels següents nombres pertanyen a cada categoria:

`6, 10, 15, 21, 28, 36, 55`

- Números perfectes
- Números triangulars
- Números de Fibonacci

**Solució:**

| Nombre | Perfecte? | Triangular? | Fibonacci? |
|--------|-----------|-------------|-----------|
| 6 | ✓ (1+2+3) | ✓ (T_3) | ✗ |
| 10 | ✗ | ✓ (T_4) | ✗ |
| 15 | ✗ | ✓ (T_5) | ✗ |
| 21 | ✗ | ✓ (T_6 = 21) | ✗ (però `F_8 = 21`) |
| 28 | ✓ (1+2+4+7+14) | ✗ | ✗ |
| 36 | ✗ | ✓ (T_8) | ✗ |
| 55 | ✗ | ✗ | ✓ (F_10) |

**Concepte avaluat:** Distinció entre tipus de nombres especials, classificació múltiple.

---

### **Exercici 6** 🟦 (1.0 punt) – Propietats de Nombres Triangulars

**Enunciat:**

Verifica les següents propietats de nombres triangulars:

a) `T_n = C(n+1, 2)` (combinacions)
   - Verifica per a `n = 3, 4, 5`.

b) La suma de dos nombres triangulars consecutius és un quadrat perfecte:
   - `T_{n-1} + T_n = n^2`
   - Verifica per a `n = 3, 4, 5`.

**Solució:**

a) **Triangulars com a combinacions:**
   - `T_3 = 6`, `C(4, 2) = 4!/(2!2!) = 6` ✓
   - `T_4 = 10`, `C(5, 2) = 5!/(2!3!) = 10` ✓
   - `T_5 = 15`, `C(6, 2) = 6!/(2!4!) = 15` ✓

b) **Suma de triangulars consecutius:**
   - `T_2 + T_3 = 3 + 6 = 9 = 3^2` ✓
   - `T_3 + T_4 = 6 + 10 = 16 = 4^2` ✓
   - `T_4 + T_5 = 10 + 15 = 25 = 5^2` ✓

**Concepte avaluat:** Propietats avançades de nombres triangulars, connexió amb combinatòria.

---

### **Exercici 7** 🟦 (1.1 punts) – Aplicació: Fibonacci en la Natura

**Enunciat:**

Fibonacci apareix frequentment en la natura. Investigació bàsica:

a) Llista els primers 15 termes de Fibonacci.

b) Identifica patrons: Quins termes són divisibles per 2? Per 3? Per 5?

c) Predicció: Existeix un patró de divisibilitat per a cada posició?

**Solució:**

a) **Primers 15 termes:**
   `0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, 377`

b) **Patrons de divisibilitat:**
   
   | Divisor | Posicions divisibles | Patró? |
   |---------|-----|---|
   | 2 | 3, 6, 9, 12, 15 | Cada 3 posicions ✓ |
   | 3 | 4, 8, 12 | Cada 4 posicions ✓ |
   | 5 | 5, 10, 15 | Cada 5 posicions ✓ |

c) **Predicció:**
   - Sí, `F_n` és divisible per `F_k` si `n` és múltiple de `k`.
   - Pattern: `F_{mk}` és divisible per `F_k`.

**Concepte avaluat:** Investigació de patrons en Fibonacci, descoberta de divisibilitat periòdica.

---

### **Exercici 8** 🟦 (1.3 punts) – Fórmula de Binet

**Enunciat:**

La **Fórmula de Binet** expressa el `n`-èsim terme de Fibonacci sense recurrència:

$$F_n = \frac{\phi^n - \psi^n}{\sqrt{5}}$$

on `φ = (1+√5)/2 ≈ 1.618` (nombre d'or) i `ψ = (1-√5)/2 ≈ -0.618`.

a) Usa la fórmula per calcular `F_5` i `F_6`.

b) Compara amb els valors reals.

c) Explica per què aquesta fórmula és útil.

**Solució:**

a) **Fórmula de Binet per a `F_5` i `F_6`:**

   `φ ≈ 1.618`, `ψ ≈ -0.618`, `√5 ≈ 2.236`
   
   - `F_5 = (1.618^5 - (-0.618)^5) / 2.236 ≈ (11.09 - (-0.09)) / 2.236 ≈ 11.18 / 2.236 ≈ 5` ✓
   - `F_6 = (1.618^6 - (-0.618)^6) / 2.236 ≈ (17.944 - 0.056) / 2.236 ≈ 17.888 / 2.236 ≈ 8` ✓

b) **Comparació:**
   - Fórmula: `F_5 ≈ 5`, Real: `F_5 = 5` ✓
   - Fórmula: `F_6 ≈ 8`, Real: `F_6 = 8` ✓

c) **Utilitat:**
   - Calcula `F_n` directament sense calcular tots els termes anteriors.
   - Permet cercar propietats de Fibonacci usant anàlisi matemàtica.

**Concepte avaluat:** Fórmula tancada de Fibonacci, connexió amb nombres d'or, computació directa.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Nombres Perfectes i Primers de Mersenne

**Enunciat:**

Els nombres perfectes parells segueixen la forma: `P = 2^{p-1}(2^p - 1)` quan `2^p - 1` és primer (primer de Mersenne).

a) Verifica que `p = 2` dóna un nombre perfecte.

b) Verifica que `p = 3` dóna un nombre perfecte.

c) Per a `p = 4`, comprova que `2^4 - 1 = 15` no és primer, i per tant la fórmula no dóna un nombre perfecte.

**Solució:**

a) **`p = 2`:**
   - `2^p - 1 = 2^2 - 1 = 3` (primer) ✓
   - `P = 2^{2-1}(2^2 - 1) = 2^1 × 3 = 2 × 3 = 6`
   - **6 és perfecte** (ja verificat abans) ✓

b) **`p = 3`:**
   - `2^p - 1 = 2^3 - 1 = 7` (primer) ✓
   - `P = 2^{3-1}(2^3 - 1) = 2^2 × 7 = 4 × 7 = 28`
   - **28 és perfecte** (ja verificat abans) ✓

c) **`p = 4`:**
   - `2^p - 1 = 2^4 - 1 = 15 = 3 × 5` (compost, no primer) ✗
   - `P = 2^{4-1}(15) = 8 × 15 = 120`
   - Divisors propis de 120: 1, 2, 3, 4, 5, 6, 8, 10, 12, 15, 20, 24, 30, 40, 60
   - Suma: 1+2+3+4+5+6+8+10+12+15+20+24+30+40+60 = 240 ≠ 120
   - **120 no és perfecte** ✓

**Concepte avaluat:** Relació entre nombres perfectes i primers de Mersenne, proves de validesa.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Suma de Quadrats de Fibonacci

**Enunciat:**

Existeix una identitat: `F_1^2 + F_2^2 + ... + F_n^2 = F_n × F_{n+1}`.

a) Verifica aquesta identitat per a `n = 1, 2, 3, 4, 5`.

b) Usa la identitat per calcular `F_1^2 + F_2^2 + ... + F_{10}^2` ràpidament.

**Solució:**

a) **Verificació:**
   - `n = 1`: `F_1^2 = 1^2 = 1`, `F_1 × F_2 = 1 × 1 = 1` ✓
   - `n = 2`: `F_1^2 + F_2^2 = 1 + 1 = 2`, `F_2 × F_3 = 1 × 2 = 2` ✓
   - `n = 3`: `F_1^2 + F_2^2 + F_3^2 = 1 + 1 + 4 = 6`, `F_3 × F_4 = 2 × 3 = 6` ✓
   - `n = 4`: `1 + 1 + 4 + 9 = 15`, `F_4 × F_5 = 3 × 5 = 15` ✓
   - `n = 5`: `1 + 1 + 4 + 9 + 25 = 40`, `F_5 × F_6 = 5 × 8 = 40` ✓

b) **Ús de la identitat:**
   - `F_1^2 + F_2^2 + ... + F_{10}^2 = F_{10} × F_{11}`
   - `F_{10} = 55`, `F_{11} = 89`
   - `Suma = 55 × 89 = 4.895`

**Concepte avaluat:** Identitats de Fibonacci, aplicació de patrons per simplificar càlculs.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Nombres perfectes | Moderat |
| 2 | Nombres triangulars | Intermedi |
| 3 | Seqüència de Fibonacci | Moderat |
| 4 | Nombre d'or | Intermedi |
| 5 | Classificació de nombres | Moderat |
| 6 | Propietats de triangulars | Intermedi |
| 7 | Patrons en Fibonacci | Intermedi |
| 8 | Fórmula de Binet | Intermedi |
| 9 | Primers de Mersenne | Desafiador |
| 10 | Identitats de Fibonacci | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre nombres perfectes amb triangulars**: Són categories completament diferents.
2. **Pensar que Fibonacci és una seqüència aritmètica**: Es basa en suma recurrent, no en diferència fixa.
3. **Oblidar que `F_0 = 0, F_1 = 1`**: Els índexs comencen a 0, no a 1.
4. **Negligir la convergència del nombre d'or**: Els quocients oscil·len però convergeixen.


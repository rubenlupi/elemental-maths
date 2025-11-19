# Exercicis - Mòdul 1: Bloc 14 – Consolidació i Repàs Mixt

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 2, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 3, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Repàs: Conjunts i Operacions

**Enunciat:**

Donats els conjunts:
- `A = {2, 3, 5, 7, 11}` (primers menors que 12)
- `B = {3, 6, 9, 12}` (múltiples de 3 menors que 15)
- `C = ℕ ∩ [1, 10]` (naturals entre 1 i 10)

Calcula:
a) `A ∪ B`
b) `A ∩ B`
c) `(A ∪ B) ∩ C`

**Solució:**

a) **`A ∪ B = {2, 3, 5, 6, 7, 9, 11, 12}`**
   - Unió de tots els elements de A i B

b) **`A ∩ B = {3}`**
   - Només 3 pertany a ambdós conjunts

c) **`(A ∪ B) ∩ C = {2, 3, 5, 6, 7, 9}`**
   - Elements de la unió que estan dins [1, 10]
   - `{2, 3, 5, 6, 7, 9, 11, 12} ∩ {1, 2, 3, 4, 5, 6, 7, 8, 9, 10} = {2, 3, 5, 6, 7, 9}`

**Concepte avaluat:** Operacions entre conjunts, conjunts de nombres específics.

---

### **Exercici 2** ⭐ (0.9 punts) – Repàs: Jerarquia Numèrica

**Enunciat:**

Classifica els següents nombres segons la jerarquia ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ:

- `√2`
- `-5`
- `3/4`
- `0`
- `-2/3`
- `π`
- `5`

Indica el conjunt "mínim" al qual pertany cada nombre.

**Solució:**

| Nombre | Classificació | Justificació |
|--------|---------------|-------------|
| `√2` | ℝ \ ℚ (irracional) | No és quocient d'enters |
| `-5` | ℤ | Nombre enter negatiu |
| `3/4` | ℚ | Quocient de naturals |
| `0` | ℕ (o ℤ, ℚ, ℝ) | Pertany a tots, però "mínim" és ℕ |
| `-2/3` | ℚ | Quocient de sencers |
| `π` | ℝ \ ℚ (irracional) | Nombre transcendent |
| `5` | ℕ | Natural positiu |

**Concepte avaluat:** Jerarquia de conjunts numèrics, propietats dels nombres.

---

### **Exercici 3** 🟦 (1.0 punt) – Repàs: Valor Posicional i Notació Desenvolupada

**Enunciat:**

a) Escriu `3.456` en **notació desenvolupada** (escrivint el valor de cada dígit).

b) En el nombre `5.347.291`, quin és el valor del dígit `4`?

c) Que representa la posició de la dècima en `123.456`?

**Solució:**

a) **Notació desenvolupada:**
   - `3.456 = 3 × 10^0 + 4 × 10^{-1} + 5 × 10^{-2} + 6 × 10^{-3}`
   - `= 3 + 0.4 + 0.05 + 0.006`

b) **Valor del dígit `4` en `5.347.291`:**
   - El dígit `4` està en la posició de les **desenes de miler**
   - Valor: `4 × 10^4 = 40.000`

c) **Posició de la dècima en `123.456`:**
   - La primera posició després del punt decimal
   - Valor: `4 × 10^{-1} = 0.4`

**Concepte avaluat:** Valor posicional, descomposició numèrica, interpretació de digits.

---

### **Exercici 4** 🟦 (1.1 punts) – Repàs: Divisibilitat i Criteris

**Enunciat:**

a) Usa les **regles de divisibilitat** per determinar si `3.456` és divisible per:
   - 2
   - 3
   - 4
   - 6

b) Per a cada cas, explica el criteri utilitzat.

**Solució:**

a) **Comprovacions:**

   - **Divisible per 2?** SÍ (últim dígit 6 és parell)
   - **Divisible per 3?** SÍ (suma de dígits: 3+4+5+6=18, que és divisible per 3)
   - **Divisible per 4?** SÍ (últims dos dígits: 56 és divisible per 4)
   - **Divisible per 6?** SÍ (divisible per 2 i 3, per tant per 6)

b) **Criteris aplicats:**
   - **Criteri de 2**: Un nombre és divisible per 2 si el seu últim dígit és 0, 2, 4, 6 o 8
   - **Criteri de 3**: Un nombre és divisible per 3 si la suma dels seus dígits és divisible per 3
   - **Criteri de 4**: Un nombre és divisible per 4 si els seus dos últims dígits formen un nombre divisible per 4
   - **Criteri de 6**: Un nombre és divisible per 6 si és divisible per 2 i per 3

**Concepte avaluat:** Regles de divisibilitat, criteris de divisió, aplicació a números específics.

---

### **Exercici 5** ⭐ (0.8 punts) – Repàs: Notació Científica

**Enunciat:**

Converteix els següents nombres a **notació científica**:

a) `0.00456`
b) `123.000.000`
c) `0.0000789`

**Solució:**

a) `0.00456 = 4.56 × 10^{-3}`

b) `123.000.000 = 1.23 × 10^8`

c) `0.0000789 = 7.89 × 10^{-5}`

**Concepte avaluat:** Conversió a notació científica, exponents negatius i positius.

---

### **Exercici 6** 🟦 (1.2 punts) – Síntesi: MCD, MCM i Factorització

**Enunciat:**

Donats `a = 180` i `b = 240`:

a) Calcula la **descomposició en factors primers** de cada nombre.
b) Usa la factorització per trobar `mcd(180, 240)`.
c) Usa la factorització per trobar `mcm(180, 240)`.
d) Verifica que `mcd(a, b) × mcm(a, b) = a × b`.

**Solució:**

a) **Factoritzacions:**
   - `180 = 2^2 × 3^2 × 5`
   - `240 = 2^4 × 3 × 5`

b) **MCD usant factorització:**
   - `mcd(180, 240) = 2^{min(2,4)} × 3^{min(2,1)} × 5^{min(1,1)}`
   - `= 2^2 × 3 × 5 = 4 × 3 × 5 = 60`

c) **MCM usant factorització:**
   - `mcm(180, 240) = 2^{max(2,4)} × 3^{max(2,1)} × 5^{max(1,1)}`
   - `= 2^4 × 3^2 × 5 = 16 × 9 × 5 = 720`

d) **Verificació:**
   - `mcd(180, 240) × mcm(180, 240) = 60 × 720 = 43.200`
   - `180 × 240 = 43.200` ✓
   - **Verifica** la identitat `mcd(a,b) × mcm(a,b) = a × b`

**Concepte avaluat:** Factorització, MCD, MCM, identitat multiplicativa.

---

### **Exercici 7** 🟦 (1.1 punts) – Síntesi: Nombres Especials i Patrons

**Enunciat:**

a) Determina si `28` és un **nombre perfecte** (suma dels seus divisors propis = el nombre).

b) Calcula els primers 5 **nombres triangulars**: `T_n = n(n+1)/2`.

c) Identifica el **5è terme** de la **successió de Fibonacci** (comença amb F₀=0, F₁=1).

**Solució:**

a) **`28` és perfecte?**
   - Divisors propis de 28: 1, 2, 4, 7, 14
   - Suma: 1 + 2 + 4 + 7 + 14 = 28 ✓
   - **SÍ, 28 és perfecte**

b) **Primeres 5 nombres triangulars:**
   - `T_1 = 1 × 2 / 2 = 1`
   - `T_2 = 2 × 3 / 2 = 3`
   - `T_3 = 3 × 4 / 2 = 6`
   - `T_4 = 4 × 5 / 2 = 10`
   - `T_5 = 5 × 6 / 2 = 15`
   - **Seqüència: 1, 3, 6, 10, 15**

c) **5è terme de Fibonacci:**
   - `F_0 = 0, F_1 = 1, F_2 = 1, F_3 = 2, F_4 = 3, F_5 = 5`
   - **`F_5 = 5`**

**Concepte avaluat:** Nombres perfectes, nombres triangulars, successió de Fibonacci.

---

### **Exercici 8** 🟦 (1.3 punts) – Síntesi: Aritmètica Modular i Cicles

**Enunciat:**

a) Resol el sistema de congruències:
   - `x ≡ 2 (mod 5)`
   - `x ≡ 3 (mod 7)`

b) Usa el **Teorema Xinès de Residus** (CRT) per trobar la solució general.

c) Determina la longitud del cicle de `2^n mod 11`.

**Solució:**

a) **Resolució del sistema:**
   - De la primera congruència: `x = 5k + 2` per a algun `k`
   - Substituïm a la segona: `5k + 2 ≡ 3 (mod 7)`
   - `5k ≡ 1 (mod 7)`
   - `k ≡ 3 (mod 7)` (ja que `5 × 3 = 15 ≡ 1 (mod 7)`)
   - `x = 5(7m + 3) + 2 = 35m + 17`
   - **Solució: `x ≡ 17 (mod 35)`**

b) **Verificació amb CRT:**
   - `17 mod 5 = 2` ✓
   - `17 mod 7 = 3` ✓

c) **Cicle de `2^n mod 11`:**
   - Pel Teorema d'Euler: `φ(11) = 10`, per tant `2^{10} ≡ 1 (mod 11)`
   - Comprovem: `2^1 = 2, 2^2 = 4, 2^3 = 8, 2^4 = 5, 2^5 = 10, 2^6 = 9, 2^7 = 7, 2^8 = 3, 2^9 = 6, 2^{10} = 1`
   - **Longitud del cicle: 10**

**Concepte avaluat:** Sistemes de congruències, CRT, Teorema d'Euler, cicles modular.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Problema Mixt de Síntesi

**Enunciat:**

Un comerciant desitja empaquetar 120 mançanes i 90 taronges en caixes idèntiques. Cada caixa ha de contenir només un tipus de fruita, i desitja usar el mínim nombre de caixes.

a) Quina és la **mida de cada caixa** (nombre de fruites per caixa)?

b) Quantes caixes necessita per a mançanes?

c) Quantes caixes necessita per a taronges?

d) Quin és el **nombre total de caixes**?

e) Explica per quina raó aquesta resposta està relacionada amb el **MCD**.

**Solució:**

a) **Mida de cada caixa:**
   - Cerquem el MCD(120, 90)
   - `120 = 2^3 × 3 × 5`
   - `90 = 2 × 3^2 × 5`
   - `mcd(120, 90) = 2 × 3 × 5 = 30`
   - **Mida de cada caixa: 30 fruites**

b) **Caixes per a mançanes:**
   - `120 ÷ 30 = 4 caixes`

c) **Caixes per a taronges:**
   - `90 ÷ 30 = 3 caixes`

d) **Nombre total de caixes:**
   - `4 + 3 = 7 caixes`

e) **Relació amb el MCD:**
   - El MCD és el **divisor comú més gran** de 120 i 90
   - Usar el MCD com a mida garnateix que:
     - Cada caixa pot contenir un nombre enter de fruites sense sobrants
     - Es minimitza el nombre de caixes (no es pot usar una mida més gran)
   - El concepte de MCD és fonamental en problemes de "partició en grups iguals"

**Concepte avaluat:** Aplicació de MCD, problemes de partició, connexió entre teoria i pràctica.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Investigació Integrada

**Enunciat:**

**Investigació:** Com es relacionen els conceptes del Mòdul 1?

Donada la successió definida per:
- `a_1 = 12`
- `a_{n+1}` = "nombre obtingut multiplicant `a_n` per 2, llavors dividint pels seus divisors comuns amb 10"

a) Calcula els primers 6 termes: `a_1, a_2, a_3, a_4, a_5, a_6`.

b) Expressa cada terme en **notació científica**.

c) Descompon cada terme en **factors primers**.

d) Detecta **patrons** en les factoritzacions.

e) Explica quins conceptes del Mòdul 1 es manifestem en aquesta successió.

**Solució:**

a) **Càlcul dels termes:**

   - `a_1 = 12`
   
   - `a_2`: `12 × 2 = 24`. MCD(24, 10) = 2. `a_2 = 24 ÷ 2 = 12`
   
   - `a_3`: `12 × 2 = 24`. MCD(24, 10) = 2. `a_3 = 12`
   
   - Observació: La successió es **stabilitza en 12**
   - `a_1 = 12, a_2 = 12, a_3 = 12, a_4 = 12, a_5 = 12, a_6 = 12`

b) **Notació científica:**
   - `a_1 = 1.2 × 10^1`
   - `a_2 = 1.2 × 10^1`
   - ... (tots són `1.2 × 10^1`)

c) **Factoritzacions:**
   - `12 = 2^2 × 3`
   - (per a tots els termes)

d) **Patrons:**
   - La successió es **stabilitza immediatament** en `12`
   - Això ocorre perquè `mcd(12, 10) = 2`, i `12 × 2 ÷ 2 = 12`
   - La regla de transformació és **idempotent** per a `a_1 = 12`

e) **Conceptes integrats:**
   - **Conjunts numèrics**: Operacions sobre enters
   - **Divisibilitat**: Divisors de 10 (1, 2, 5, 10)
   - **MCD**: Funció central en la transformació
   - **Factorització**: Explicació de per què la successió es stabilitza
   - **Patrons i cicles**: Detecció de comportament estacionari
   - **Aritmètica modular**: Modela relacions de divisibilitat

**Concepte avaluat:** Integració de tots els conceptes, investigació matemàtica, connexions entre tòpics.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Conceptes Principals | Nivell |
|----------|----------------------|--------|
| 1 | Conjunts, operacions | Moderat |
| 2 | Jerarquia numèrica | Moderat |
| 3 | Valor posicional, descomposició | Intermedi |
| 4 | Divisibilitat, criteris | Intermedi |
| 5 | Notació científica | Moderat |
| 6 | MCD, MCM, factorització, identitat | Intermedi |
| 7 | Nombres especials, successións | Intermedi |
| 8 | CRT, cicles modular, Teorema d'Euler | Intermedi |
| 9 | MCD aplicat, problemes de partició | Desafiador |
| 10 | Integració de tots els conceptes | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre la jerarquia**: No tots els nombres reals són racionals.
2. **Negligir el zero**: El zero pertany a ℕ, ℤ, ℚ, ℝ alhora.
3. **Erros en factorització**: Assegureu-vos de descompondre completament els nombres.
4. **MCD vs. MCM**: El MCD és el divisor comú més gran; MCM és el múltiple comú més petit.
5. **Aritmètica modular confusa**: Recordeu que `a ≡ b (mod n)` significa que el residu és igual.
6. **Cicles incomplets**: Els cicles sempre comencen a 0 o 1, depenent de la context.

---

## 🌉 Connexions amb Mòdul 2

Els conceptes de Mòdul 1 serveixen com a **fonament** per a:
- **Mòdul 2: Operacions i Estructures**: Propietats de grups i cossos
- **Mòdul 3: Geometria Numèrica**: Simetries i patrons
- **Mòdul 4: Criptografia**: Aplicacions de MCD, MCM, aritmètica modular
- **Mòdul 5: Combinatòria**: Distribucions i comptatge usant múltiples i divisors


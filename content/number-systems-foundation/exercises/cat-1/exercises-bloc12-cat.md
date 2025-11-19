# Exercicis - Mòdul 1: Bloc 12 – Concepte d'Aritmètica Modular (a ≡ b mod n)

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Definició de Congruència

**Enunciat:**

Determina si les següents congruències són vertaderes o falses:

a) `17 ≡ 5 (mod 12)`
b) `9 ≡ 1 (mod 4)`
c) `14 ≡ 3 (mod 4)`
d) `23 ≡ 8 (mod 5)`

(Recorda: `a ≡ b (mod n)` és vertader si `n` divideix `a - b`.)

**Solució:**

a) `17 ≡ 5 (mod 12)`:
   - `17 - 5 = 12`
   - `12 | 12` ✓
   - **Vertader**

b) `9 ≡ 1 (mod 4)`:
   - `9 - 1 = 8`
   - `4 | 8` (perquè `8 = 4 × 2`) ✓
   - **Vertader**

c) `14 ≡ 3 (mod 4)`:
   - `14 - 3 = 11`
   - `4 ∤ 11` (perquè `11 = 4 × 2 + 3`) ✗
   - **Fals**

d) `23 ≡ 8 (mod 5)`:
   - `23 - 8 = 15`
   - `5 | 15` (perquè `15 = 5 × 3`) ✓
   - **Vertader**

**Concepte avaluat:** Definició de congruència modular, verificació de divisibilitat.

---

### **Exercici 2** 🟦 (1.1 punts) – Equivalència de Residus

**Enunciat:**

Dos nombres són congruents mòdul `n` si deixan el **mateix residu** quan es divideixen per `n`.

a) Calcula els residus de `17` i `5` mòdul `12`.
b) Calcula els residus de `9` i `1` mòdul `4`.
c) Usa els residus per verificar les congruències de l'exercici anterior.

**Solució:**

a) **Residus mòdul 12:**
   - `17 = 12 × 1 + 5` → residu de 17 mod 12 = 5
   - `5 = 12 × 0 + 5` → residu de 5 mod 12 = 5
   - Mateixos residus (5 = 5) → `17 ≡ 5 (mod 12)` ✓

b) **Residus mòdul 4:**
   - `9 = 4 × 2 + 1` → residu de 9 mod 4 = 1
   - `1 = 4 × 0 + 1` → residu de 1 mod 4 = 1
   - Mateixos residus (1 = 1) → `9 ≡ 1 (mod 4)` ✓

c) **Verificació dels altres casos:**
   - `14 = 4 × 3 + 2` → residu = 2; `3 = 4 × 0 + 3` → residu = 3
   - Residus diferents (2 ≠ 3) → `14 ≡ 3 (mod 4)` ✗
   - `23 = 5 × 4 + 3` → residu = 3; `8 = 5 × 1 + 3` → residu = 3
   - Mateixos residus (3 = 3) → `23 ≡ 8 (mod 5)` ✓

**Concepte avaluat:** Equivalència entre definicions de congruència (divisibilitat vs. mateixos residus).

---

### **Exercici 3** ⭐ (0.9 punts) – Classes de Residus

**Enunciat:**

Una **classe de residu** `[a]_n` representa tots els nombres congruents amb `a` mòdul `n`.

a) Llista els primers 5 elements de `[3]_5` (tots els nombres ≡ 3 (mod 5)).

b) Llista els primers 5 elements de `[2]_7`.

**Solució:**

a) **`[3]_5`** (nombres amb residu 3 mòdul 5):
   - `3, 8, 13, 18, 23, ...`
   - Patró: `3 + 5k` per a `k = 0, 1, 2, 3, ...`

b) **`[2]_7`** (nombres amb residu 2 mòdul 7):
   - `2, 9, 16, 23, 30, ...`
   - Patró: `2 + 7k` per a `k = 0, 1, 2, 3, ...`

**Concepte avaluat:** Classes de residus, patrons periòdics.

---

### **Exercici 4** 🟦 (1.2 punts) – Operacions en Aritmètica Modular

**Enunciat:**

Si `a ≡ b (mod n)` i `c ≡ d (mod n)`, aleshores:
- `a + c ≡ b + d (mod n)`
- `a - c ≡ b - d (mod n)`
- `a × c ≡ b × d (mod n)`

Verifica aquestes propietats:

a) `7 ≡ 2 (mod 5)` i `4 ≡ 9 (mod 5)`. Comprova suma, resta i multiplicació.

**Solució:**

a) **Verificació:**
   - Base: `7 ≡ 2 (mod 5)` perquè `7 - 2 = 5` ✓
   - Base: `4 ≡ 9 (mod 5)` perquè `9 - 4 = 5` ✓

   **Suma:**
   - `7 + 4 = 11`, `2 + 9 = 11` → `11 ≡ 11 (mod 5)` ✓
   - Residus: `11 mod 5 = 1`, `11 mod 5 = 1` ✓

   **Resta:**
   - `7 - 4 = 3`, `2 - 9 = -7` → `3 ≡ -7 (mod 5)`?
   - `-7 = -10 + 3 = 5 × (-2) + 3` → `-7 mod 5 = 3` ✓

   **Multiplicació:**
   - `7 × 4 = 28`, `2 × 9 = 18` → `28 ≡ 18 (mod 5)`?
   - `28 mod 5 = 3`, `18 mod 5 = 3` ✓

**Concepte avaluat:** Propietats d'operacions en aritmètica modular, conservació de congruència.

---

### **Exercici 5** ⭐ (0.8 punts) – Rellotge de 12 Hores

**Enunciat:**

Un rellotge funciona amb aritmètica modular base 12 (mòdul 12).

a) Si ara és les `9`, quina hora serà en `7` hores?
b) Si ara és les `11`, quina hora serà en `4` hores?
c) Usa congruència mòdul 12 per verificar.

**Solució:**

a) **`9 + 7 hores`:**
   - `9 + 7 = 16`
   - `16 ≡ ? (mod 12)`
   - `16 mod 12 = 4` (perquè `16 = 12 × 1 + 4`)
   - **Serà les `4`.**

b) **`11 + 4 hores`:**
   - `11 + 4 = 15`
   - `15 mod 12 = 3` (perquè `15 = 12 × 1 + 3`)
   - **Serà les `3`.**

c) **Verificació:**
   - `9 + 7 ≡ 4 (mod 12)` ✓
   - `11 + 4 ≡ 3 (mod 12)` ✓

**Concepte avaluat:** Aplicació pràctica de aritmètica modular en contextos reals (rellotge).

---

### **Exercici 6** 🟦 (1.0 punt) – Residus Negatius

**Enunciat:**

Els residus negatius es transformen a positius usant: `-a ≡ n - a (mod n)`.

a) Transforma `-1 (mod 5)` a un residu positiu.
b) Transforma `-3 (mod 7)` a un residu positiu.
c) Transforma `-12 (mod 5)` a un residu positiu.

**Solució:**

a) **`-1 (mod 5)`:**
   - `-1 ≡ 5 - 1 = 4 (mod 5)`
   - Verificació: `-1 - 4 = -5`, i `5 | -5` ✓

b) **`-3 (mod 7)`:**
   - `-3 ≡ 7 - 3 = 4 (mod 7)`
   - Verificació: `-3 - 4 = -7`, i `7 | -7` ✓

c) **`-12 (mod 5)`:**
   - `-12 ≡ 5 - 12 = -7 (mod 5)` (no està en l'interval [0, 4])
   - Millor: `-12 ≡ -2 ≡ 5 - 2 = 3 (mod 5)`
   - Verificació: `-12 - 3 = -15`, i `5 | -15` ✓

**Concepte avaluat:** Conversió de residus negatius a positius, normalització de residus.

---

### **Exercici 7** 🟦 (1.1 punts) – Aplicació: Dígits de Control

**Enunciat:**

Els codis ISBN i altres sistemes usen aritmètica modular per a detecció d'errors.

a) Per a un codi de 3 dígits `d_1 d_2 d_3`, el dígit de control és `d_4 ≡ -(d_1 + d_2 + d_3) (mod 10)`.

   Si `d_1 = 2`, `d_2 = 5`, `d_3 = 7`, quin és el dígit de control?

b) Verifica que `d_1 + d_2 + d_3 + d_4 ≡ 0 (mod 10)`.

**Solució:**

a) **Dígit de control:**
   - `d_1 + d_2 + d_3 = 2 + 5 + 7 = 14`
   - `d_4 ≡ -14 (mod 10)`
   - `-14 ≡ 10 - 4 = 6 (mod 10)` (transformant a positiu: `-14 mod 10 = -4 ≡ 6 (mod 10)`)
   - **`d_4 = 6`**

b) **Verificació:**
   - `2 + 5 + 7 + 6 = 20`
   - `20 ≡ 0 (mod 10)` ✓

**Concepte avaluat:** Aplicació práctica de aritmètica modular en detecció d'errors.

---

### **Exercici 8** 🟦 (1.3 punts) – Congruència i Potències

**Enunciat:**

Calcula les potències de nombres usant aritmètica modular:

a) `2^3 (mod 5)`
b) `3^4 (mod 7)`
c) `5^2 (mod 11)`

Usa la propietat que `(a × b) mod n = ((a mod n) × (b mod n)) mod n`.

**Solució:**

a) **`2^3 (mod 5)`:**
   - `2^3 = 8`
   - `8 mod 5 = 3`
   - **Resposta: 3**

b) **`3^4 (mod 7)`:**
   - `3^4 = 81`
   - `81 mod 7 = 4` (perquè `81 = 7 × 11 + 4`)
   - **Resposta: 4**

c) **`5^2 (mod 11)`:**
   - `5^2 = 25`
   - `25 mod 11 = 3` (perquè `25 = 11 × 2 + 3`)
   - **Resposta: 3**

**Concepte avaluat:** Operacions de potència en aritmètica modular, simplificació mitjançant propietats.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Teorema Xinès del Residu

**Enunciat:**

El **Teorema Xinès del Residu** permet resoldre sistemes de congruències. Per a sistemes simples:

Si `x ≡ a (mod m)` i `x ≡ b (mod n)` (amb m i n coprims), existeix una solució única mòdul `m×n`.

Resol el sistema:
- `x ≡ 2 (mod 3)`
- `x ≡ 3 (mod 5)`

a) Llista els nombres que satisfan la primera congruència.
b) Entre ells, identifica quins satisfan la segona.
c) Expressa la solució general.

**Solució:**

a) **Nombres `x ≡ 2 (mod 3)`:**
   - `2, 5, 8, 11, 14, 17, 20, 23, ...`

b) **Entre ells, quins satisfan `x ≡ 3 (mod 5)`?**
   - `2 mod 5 = 2` ✗
   - `5 mod 5 = 0` ✗
   - `8 mod 5 = 3` ✓
   - `11 mod 5 = 1` ✗
   - `14 mod 5 = 4` ✗
   - `17 mod 5 = 2` ✗
   - `20 mod 5 = 0` ✗
   - `23 mod 5 = 3` ✓
   - Primera solució: `x = 8`

c) **Solució general:**
   - `x ≡ 8 (mod 15)` (perquè `mcd(3, 5) = 1`, per tant el cicle és `3 × 5 = 15`)
   - Verificació: `8 ≡ 2 (mod 3)` ✓ i `8 ≡ 3 (mod 5)` ✓

**Concepte avaluat:** Teorema Xinès del Residu, resolució de sistemes de congruències.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Criptografia RSA Simplificada

**Enunciat:**

En RSA, l'encriptació usa aritmètica modular. Donat un missatge `m`, s'encripta com `c ≡ m^e (mod n)`.

a) Sigui `n = 15` (product de primers 3 i 5), `e = 3`, `m = 2`. Calcula `c`.

b) Per desencriptar, usem `m ≡ c^d (mod n)` on `d` es calcula. Per simplicitat, assumeix `d = 3`.
   Verifica que el missatge original es recupera.

**Solució:**

a) **Encriptació:**
   - `c ≡ 2^3 (mod 15)`
   - `2^3 = 8`
   - `8 mod 15 = 8`
   - **`c = 8`**

b) **Desencriptació:**
   - `m ≡ 8^3 (mod 15)`
   - `8^3 = 512`
   - `512 mod 15 = ?`
   - `512 = 15 × 34 + 2`
   - `512 mod 15 = 2`
   - **`m = 2`** (recuperat!) ✓

**Concepte avaluat:** Aplicació criptogràfica de aritmètica modular, encriptació i desencriptació.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Definició de congruència | Moderat |
| 2 | Equivalència de residus | Intermedi |
| 3 | Classes de residus | Moderat |
| 4 | Operacions modulars | Intermedi |
| 5 | Aplicació: rellotge | Moderat |
| 6 | Residus negatius | Intermedi |
| 7 | Dígits de control | Intermedi |
| 8 | Potències modulars | Intermedi |
| 9 | Teorema Xinès del Residu | Desafiador |
| 10 | Criptografia RSA | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre `mod` amb divisió**: `mod` dóna residu, no quocient.
2. **Oblidar normalitzar residus negatius**: Els residus han d'estar a [0, n-1].
3. **Negligir la clausura**: Les operacions modulars sempre dónen residus válids dins del rang.


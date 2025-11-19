# Exercicis - Mòdul 1: Bloc 8 – Aplicacions del MCD (Algoritme d'Euclides)

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Definició de MCD

**Enunciat:**

Llista tots els divisors comuns de cada parell de nombres i identifica el màxim:

a) `12` i `18`
b) `24` i `36`
c) `16` i `40`

**Solució:**

a) **`12` i `18`:**
   - Divisors de 12: 1, 2, 3, 4, 6, 12
   - Divisors de 18: 1, 2, 3, 6, 9, 18
   - Divisors comuns: 1, 2, 3, 6
   - **MCD(12, 18) = 6**

b) **`24` i `36`:**
   - Divisors de 24: 1, 2, 3, 4, 6, 8, 12, 24
   - Divisors de 36: 1, 2, 3, 4, 6, 9, 12, 18, 36
   - Divisors comuns: 1, 2, 3, 4, 6, 12
   - **MCD(24, 36) = 12**

c) **`16` i `40`:**
   - Divisors de 16: 1, 2, 4, 8, 16
   - Divisors de 40: 1, 2, 4, 5, 8, 10, 20, 40
   - Divisors comuns: 1, 2, 4, 8
   - **MCD(16, 40) = 8**

**Concepte avaluat:** Identificació directa de divisors comuns, concepte de MCD.

---

### **Exercici 2** 🟦 (1.1 punts) – Algoritme d'Euclides

**Enunciat:**

Usa l'Algoritme d'Euclides per calcular el MCD dels següents parells:

a) `MCD(48, 18)`
b) `MCD(56, 42)`
c) `MCD(100, 35)`

Realitza cada pas de la divisió amb residu.

**Solució:**

a) **MCD(48, 18):**
   ```
   48 = 18 × 2 + 12
   18 = 12 × 1 + 6
   12 = 6 × 2 + 0
   ```
   - Residu final: 0
   - **MCD(48, 18) = 6**

b) **MCD(56, 42):**
   ```
   56 = 42 × 1 + 14
   42 = 14 × 3 + 0
   ```
   - Residu final: 0
   - **MCD(56, 42) = 14**

c) **MCD(100, 35):**
   ```
   100 = 35 × 2 + 30
   35 = 30 × 1 + 5
   30 = 5 × 6 + 0
   ```
   - Residu final: 0
   - **MCD(100, 35) = 5**

**Concepte avaluat:** Implementació de l'Algoritme d'Euclides, pas a pas.

---

### **Exercici 3** ⭐ (0.9 punts) – Comparació de Mètodes

**Enunciat:**

Compara la factorització prima amb l'Algoritme d'Euclides per calcular MCD(60, 90):

a) **Mètode 1 - Factorització Prima:**
   - Factoritza 60 i 90.
   - Prendre la potència més baixa de cada factor comú.
   - Calcula el MCD.

b) **Mètode 2 - Algoritme d'Euclides:**
   - Realitza les divisions successives.
   - Calcula el MCD.

c) Verifica que ambdós mètodes donen el mateix resultat.

**Solució:**

a) **Mètode 1 - Factorització Prima:**
   - `60 = 2^2 × 3 × 5`
   - `90 = 2 × 3^2 × 5`
   - Factors comuns amb potencies mínimes: `2^1 × 3^1 × 5^1 = 30`
   - **MCD(60, 90) = 30**

b) **Mètode 2 - Algoritme d'Euclides:**
   ```
   90 = 60 × 1 + 30
   60 = 30 × 2 + 0
   ```
   - **MCD(60, 90) = 30**

c) **Verificació:**
   - Ambdós mètodes donen **MCD = 30** ✓

**Concepte avaluat:** Comprensió de dos mètodes, verificació de consistència.

---

### **Exercici 4** 🟦 (1.2 punts) – Propietat de Coprimalitat

**Enunciat:**

Si MCD(a, b) = d, aleshores `a = d·a'` i `b = d·b'` on `a'` i `b'` són **coprims** (MCD(a', b') = 1).

Verifica aquesta propietat:

a) MCD(24, 36) = 12. Expresa `24 = 12·a'` i `36 = 12·b'`. Verifica que MCD(a', b') = 1.

b) MCD(50, 75) = 25. Verifica la mateixa propietat.

**Solució:**

a) **MCD(24, 36) = 12:**
   - `24 = 12 × 2` → `a' = 2`
   - `36 = 12 × 3` → `b' = 3`
   - MCD(2, 3) = 1 ✓ (coprims)

b) **MCD(50, 75) = 25:**
   - `50 = 25 × 2` → `a' = 2`
   - `75 = 25 × 3` → `b' = 3`
   - MCD(2, 3) = 1 ✓ (coprims)

**Concepte avaluat:** Propietat de coprimalitat, relació entre MCD i nombres coprims.

---

### **Exercici 5** ⭐ (0.8 punts) – Relació entre MCD i MCM

**Enunciat:**

L'identitat fonamental és: `a × b = MCD(a, b) × MCM(a, b)`.

Verifica aquesta relació per:

a) `a = 12`, `b = 18`
b) `a = 20`, `b = 30`

**Solució:**

a) **`a = 12`, `b = 18`:**
   - MCD(12, 18) = 6
   - MCM(12, 18) = 36 (mínim comú múltiple)
   - Verificació: `12 × 18 = 216` i `6 × 36 = 216` ✓

b) **`a = 20`, `b = 30`:**
   - MCD(20, 30) = 10
   - MCM(20, 30) = 60
   - Verificació: `20 × 30 = 600` i `10 × 60 = 600` ✓

**Concepte avaluat:** Relació fonamental entre MCD i MCM.

---

### **Exercici 6** 🟦 (1.0 punt) – Aplicació: Simplificació de Fraccions

**Enunciat:**

Simplifica les següents fraccions usant MCD:

a) $\frac{24}{36}$

b) $\frac{50}{75}$

c) $\frac{48}{60}$

**Solució:**

a) $\frac{24}{36}$:
   - MCD(24, 36) = 12
   - $\frac{24}{36} = \frac{24÷12}{36÷12} = \frac{2}{3}$

b) $\frac{50}{75}$:
   - MCD(50, 75) = 25
   - $\frac{50}{75} = \frac{50÷25}{75÷25} = \frac{2}{3}$

c) $\frac{48}{60}$:
   - MCD(48, 60) = 12
   - $\frac{48}{60} = \frac{48÷12}{60÷12} = \frac{4}{5}$

**Concepte avaluat:** Aplicació pràctica de MCD en simplificació de fraccions.

---

### **Exercici 7** 🟦 (1.1 punts) – MCD de Tres o Més Nombres

**Enunciat:**

Calcula el MCD dels següents conjunts de nombres:

a) MCD(12, 18, 24)
b) MCD(20, 30, 40)
c) MCD(15, 25, 35, 45)

(Pista: MCD(a, b, c) = MCD(MCD(a, b), c))

**Solució:**

a) **MCD(12, 18, 24):**
   - MCD(12, 18) = 6
   - MCD(6, 24) = 6
   - **MCD(12, 18, 24) = 6**

b) **MCD(20, 30, 40):**
   - MCD(20, 30) = 10
   - MCD(10, 40) = 10
   - **MCD(20, 30, 40) = 10**

c) **MCD(15, 25, 35, 45):**
   - MCD(15, 25) = 5
   - MCD(5, 35) = 5
   - MCD(5, 45) = 5
   - **MCD(15, 25, 35, 45) = 5**

**Concepte avaluat:** Extensió de MCD a múltiples nombres, aplicació iterativa.

---

### **Exercici 8** 🟦 (1.3 punts) – Aplicació Real: Agrupament Equitat

**Enunciat:**

Una botiga té 60 manzanes i 90 taronges. Vol preparar cistelles iguals amb manzanes i taronges (sense barrejar tipus) tal que cada cistella tingui el nombre màxim de fruites.

a) Quants cistelles pot fer?

b) Quantes manzanes i taronges aniran en cada cistella?

c) Verifica que la distribució és correcta.

**Solució:**

a) **Nombre de cistelles:**
   - MCD(60, 90) = 30
   - **Pot fer 30 cistelles.**

b) **Fruites per cistella:**
   - Manzanes per cistella: `60 ÷ 30 = 2`
   - Taronges per cistella: `90 ÷ 30 = 3`
   - **Cada cistella té 2 manzanes i 3 taronges.**

c) **Verificació:**
   - Total manzanes: `30 × 2 = 60` ✓
   - Total taronges: `30 × 3 = 90` ✓
   - Totes les cistelles són idèntiques ✓

**Concepte avaluat:** Aplicació pràctica de MCD en distribució equitativa.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Identitat de Bézout

**Enunciat:**

L'**Identitat de Bézout** afirma que per a qualsevol parell d'enters `a` i `b`, existeixen enters `x` i `y` tals que:

$$ax + by = \text{MCD}(a, b)$$

Usa l'Algoritme d'Euclides estès per trobar `x` i `y`:

a) Per a `a = 48`, `b = 18`:
   - Calcula MCD(48, 18) usant Euclides.
   - Revés els passos per trobar `x` i `y` tals que `48x + 18y = MCD`.

b) Verifica la solució.

**Solució:**

a) **Algoritme d'Euclides per a 48 i 18:**
   ```
   48 = 18 × 2 + 12   ... (1)
   18 = 12 × 1 + 6    ... (2)
   12 = 6 × 2 + 0     ... (3)
   ```
   - MCD(48, 18) = 6

   **Revés (Euclides estès):**
   
   De (2): `6 = 18 - 12 × 1`
   
   Substituint `12` de (1): `12 = 48 - 18 × 2`
   ```
   6 = 18 - (48 - 18 × 2) × 1
   6 = 18 - 48 + 18 × 2
   6 = 18 × 3 - 48 × 1
   6 = 48 × (-1) + 18 × 3
   ```
   
   **`x = -1`, `y = 3`**

b) **Verificació:**
   ```
   48 × (-1) + 18 × 3 = -48 + 54 = 6 ✓
   ```
   - **Identitat de Bézout verificada.**

**Concepte avaluat:** Algoritme d'Euclides estès, Identitat de Bézout, sistema d'equacions diofàntiques.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Aplicació a Sincronització

**Enunciat:**

Dos eventos es sincronitzen en cicles:
- Evento A es repeteix cada 12 horas.
- Evento B es repeteix cada 18 horas.

a) Usa MCM per trobar quan es sincronitzen novament (mateix moment).

b) Si comencen junts a les 0:00, a quina hora es sincronitzaran per primera vegada?

c) Quantes vegades es sincronitzaran en 5 dies?

d) Per què és important MCD en aquest context? (Pista: Pensa en relació amb MCM.)

**Solució:**

a) **MCM per a sincronització:**
   - MCD(12, 18) = 6
   - MCM(12, 18) = (12 × 18) ÷ MCD(12, 18) = 216 ÷ 6 = 36
   - **Es sincronitzen cada 36 horas.**

b) **Hora de primera sincronització:**
   - Comencen junts a les 0:00.
   - Següent sincronització: 0:00 + 36 horas = **1.5 dies = 36 horas després.**
   - Si usem format 24h: **0:00 del tercer dia** (36h més tard)
   - **A les 00:00 del dia següent (1 dia 12 horas).**

c) **Sincronitzacions en 5 dies:**
   - 5 dies = 120 horas
   - Sincronitzacions: `120 ÷ 36 = 3,33...`
   - Sincronitzacions completes: **3 vegades** (a les 0:00, 36h, 72h)
   - (La 4a seria a les 108h, la 5a a les 144h que surt dels 5 dies)

d) **Importància de MCD:**
   - MCD(12, 18) = 6 significa que comparteixen un múltiple comú de 6.
   - MCM es calcula usant MCD: `MCM = (a × b) / MCD`.
   - Sense MCD, seria difícil calcular MCM eficientment.

**Concepte avaluat:** Aplicació de MCM amb MCD en contextos de sincronització, resolució de problemes de cicles.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Definició de MCD | Moderat |
| 2 | Algoritme d'Euclides | Intermedi |
| 3 | Comparació de mètodes | Moderat |
| 4 | Coprimalitat | Intermedi |
| 5 | Relació MCD-MCM | Moderat |
| 6 | Simplificació de fraccions | Intermedi |
| 7 | MCD de múltiples nombres | Intermedi |
| 8 | Aplicació real: agrupament | Intermedi |
| 9 | Identitat de Bézout | Desafiador |
| 10 | Sincronització i cicles | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre MCD amb MCM**: MCD és el **més gran** divisor; MCM és el **més petit** múltiple.
2. **Oblidar que MCD sempre existeix**: Fins i tot per a nombres coprims, MCD = 1.
3. **Negligir 1 com a MCD possible**: Si `a` i `b` són coprims, MCD(a, b) = 1.
4. **Implementació errònia de l'Algoritme d'Euclides**: Els residus decreixen; l'últim no-nul és el MCD.


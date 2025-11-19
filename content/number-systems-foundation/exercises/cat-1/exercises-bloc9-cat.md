# Exercicis - Mòdul 1: Bloc 9 – MCM a través de Factors Primers

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Definició de MCM

**Enunciat:**

Llista els múltiples de cada nombre fins a trobar el primer múltiple comú:

a) `4` i `6`
b) `3` i `5`
c) `8` i `12`

**Solució:**

a) **`4` i `6`:**
   - Múltiples de 4: 4, 8, 12, 16, 20, ...
   - Múltiples de 6: 6, 12, 18, 24, ...
   - Primer múltiple comú: **12**
   - **MCM(4, 6) = 12**

b) **`3` i `5`:**
   - Múltiples de 3: 3, 6, 9, 12, 15, ...
   - Múltiples de 5: 5, 10, 15, 20, ...
   - Primer múltiple comú: **15**
   - **MCM(3, 5) = 15**

c) **`8` i `12`:**
   - Múltiples de 8: 8, 16, 24, 32, ...
   - Múltiples de 12: 12, 24, 36, ...
   - Primer múltiple comú: **24**
   - **MCM(8, 12) = 24**

**Concepte avaluat:** Definició directa de MCM identificant el primer múltiple comú.

---

### **Exercici 2** 🟦 (1.1 punts) – MCM usant Factorització Prima

**Enunciat:**

Calcula el MCM usant factorització prima (pren la potència més alta de cada factor primer):

a) MCM(12, 18)
b) MCM(24, 36)
c) MCM(15, 20)

**Solució:**

a) **MCM(12, 18):**
   - `12 = 2^2 × 3`
   - `18 = 2 × 3^2`
   - Potències més altes: `2^2` i `3^2`
   - MCM = `2^2 × 3^2 = 4 × 9 = 36`
   - **MCM(12, 18) = 36**

b) **MCM(24, 36):**
   - `24 = 2^3 × 3`
   - `36 = 2^2 × 3^2`
   - Potències més altes: `2^3` i `3^2`
   - MCM = `2^3 × 3^2 = 8 × 9 = 72`
   - **MCM(24, 36) = 72**

c) **MCM(15, 20):**
   - `15 = 3 × 5`
   - `20 = 2^2 × 5`
   - Potències més altes: `2^2`, `3`, `5`
   - MCM = `2^2 × 3 × 5 = 4 × 3 × 5 = 60`
   - **MCM(15, 20) = 60**

**Concepte avaluat:** Mètode de factorització prima per a MCM, selecció de potències màximes.

---

### **Exercici 3** ⭐ (0.9 punts) – MCM versus MCD

**Enunciat:**

Per a cada parell de nombres, calcula tant MCD com MCM:

a) `8` i `12`
b) `10` i `15`

Verifica la identitat: `a × b = MCD(a, b) × MCM(a, b)`.

**Solució:**

a) **`8` i `12`:**
   - `8 = 2^3`, `12 = 2^2 × 3`
   - MCD = `2^2 = 4`
   - MCM = `2^3 × 3 = 24`
   - Verificació: `8 × 12 = 96` i `4 × 24 = 96` ✓

b) **`10` i `15`:**
   - `10 = 2 × 5`, `15 = 3 × 5`
   - MCD = `5`
   - MCM = `2 × 3 × 5 = 30`
   - Verificació: `10 × 15 = 150` i `5 × 30 = 150` ✓

**Concepte avaluat:** Relació simètrica entre MCD i MCM, verificació d'identitat.

---

### **Exercici 4** 🟦 (1.2 punts) – MCM de Tres Nombres

**Enunciat:**

Calcula el MCM dels següents conjunts usant factorització prima:

a) MCM(4, 6, 9)
b) MCM(12, 18, 24)
c) MCM(5, 10, 15)

**Solució:**

a) **MCM(4, 6, 9):**
   - `4 = 2^2`
   - `6 = 2 × 3`
   - `9 = 3^2`
   - Potències més altes: `2^2`, `3^2`
   - MCM = `2^2 × 3^2 = 4 × 9 = 36`
   - **MCM(4, 6, 9) = 36**

b) **MCM(12, 18, 24):**
   - `12 = 2^2 × 3`
   - `18 = 2 × 3^2`
   - `24 = 2^3 × 3`
   - Potències més altes: `2^3`, `3^2`
   - MCM = `2^3 × 3^2 = 8 × 9 = 72`
   - **MCM(12, 18, 24) = 72**

c) **MCM(5, 10, 15):**
   - `5 = 5`
   - `10 = 2 × 5`
   - `15 = 3 × 5`
   - Potències més altes: `2`, `3`, `5`
   - MCM = `2 × 3 × 5 = 30`
   - **MCM(5, 10, 15) = 30**

**Concepte avaluat:** Extensió de MCM a múltiples nombres, generalització de mètode.

---

### **Exercici 5** ⭐ (0.8 punts) – Identificació de MCM en Contextos

**Enunciat:**

Per a cadascun dels contextos, estima si necessites MCD o MCM:

a) Dividir un pastís en porcions iguals entre 12 persones.
b) Trobar quan dos autobusos (que passen cada 15 min i cada 20 min) es troben.
c) Agrupar 24 llibres i 36 llapis en kits idènttics.
d) Trobar el següent moment en què dues alarmes (cada 8h i cada 12h) sonen simultàniament.

**Solució:**

| Context | MCD o MCM? | Justificació |
|---------|-----------|---|
| a) Porcions iguals | MCD | Dividir equitativament (divisor comú) |
| b) Autobusos | MCM | Sincronització periòdica (múltiple comú) |
| c) Kits idènttics | MCD | Agrupament equitatiu (divisor comú) |
| d) Alarmes | MCM | Sincronització periòdica (múltiple comú) |

**Concepte avaluat:** Discriminació entre contextos de MCD i MCM, aplicació conceptual.

---

### **Exercici 6** 🟦 (1.0 punt) – MCM en Denominadors Comuns

**Enunciat:**

Per a cada parell de fraccions, calcula el MCM dels denominadors i escriu una fracció amb denominador comú:

a) $\frac{1}{4}$ i $\frac{1}{6}$

b) $\frac{2}{3}$ i $\frac{5}{8}$

c) $\frac{3}{5}$ i $\frac{2}{15}$

**Solució:**

a) $\frac{1}{4}$ i $\frac{1}{6}$:
   - MCM(4, 6) = 12
   - $\frac{1}{4} = \frac{3}{12}$ i $\frac{1}{6} = \frac{2}{12}$
   - **Suma: $\frac{3}{12} + \frac{2}{12} = \frac{5}{12}$**

b) $\frac{2}{3}$ i $\frac{5}{8}$:
   - MCM(3, 8) = 24
   - $\frac{2}{3} = \frac{16}{24}$ i $\frac{5}{8} = \frac{15}{24}$
   - **Suma: $\frac{16}{24} + \frac{15}{24} = \frac{31}{24}$**

c) $\frac{3}{5}$ i $\frac{2}{15}$:
   - MCM(5, 15) = 15
   - $\frac{3}{5} = \frac{9}{15}$ i $\frac{2}{15} = \frac{2}{15}$
   - **Suma: $\frac{9}{15} + \frac{2}{15} = \frac{11}{15}$**

**Concepte avaluat:** Aplicació de MCM per trobar denominador comú en operacions fraccionàries.

---

### **Exercici 7** 🟦 (1.1 punts) – MCM en Problemes de Planejació

**Enunciat:**

En una escola:
- Un mestre de matemàtiques imparteix classe cada 3 dies.
- Un mestre de ciències imparteix classe cada 5 dies.

a) Si ambdós ensenya avui, quants dies passaran fins que tornin a ensenyar junts el mateix dia?

b) En 60 dies, quantes vegades coincidiran?

**Solució:**

a) **Dies fins a la coincidència:**
   - MCM(3, 5) = 15
   - **Coincidiran cada 15 dies.**

b) **Coincidències en 60 dies:**
   - `60 ÷ 15 = 4`
   - **Coincidiran 4 vegades** (a dia 0, 15, 30, 45)

**Concepte avaluat:** Aplicació pràctica de MCM en planejament de cicles.

---

### **Exercici 8** 🟦 (1.3 punts) – Propietat de MCM amb Coprims

**Enunciat:**

Si dos nombres `a` i `b` són **coprims** (MCD(a, b) = 1), aleshores MCM(a, b) = `a × b`.

Verifica aquesta propietat:

a) `7` i `11` (coprims)
b) `9` i `16` (coprims)
c) `Contraexemple: `6` i `9` (no coprims)

**Solució:**

a) **`7` i `11` (coprims):**
   - MCD(7, 11) = 1
   - MCM(7, 11) = 7 × 11 = 77
   - Verificació: Múltiples de 7: 7, 14, 21, ..., 77...
   - Múltiples de 11: 11, 22, 33, ..., 77...
   - Primer múltiple comú: 77 ✓

b) **`9` i `16` (coprims):**
   - MCD(9, 16) = 1
   - MCM(9, 16) = 9 × 16 = 144
   - Verificació: 144 ÷ 9 = 16 ✓; 144 ÷ 16 = 9 ✓

c) **Contraexemple: `6` i `9` (no coprims):**
   - MCD(6, 9) = 3 (no coprims)
   - 6 × 9 = 54
   - MCM(6, 9) = 18 (la propietat no es compleix: 18 ≠ 54)
   - Raó: Tendo un factor comú (3), el producte és "més gran" que cal.

**Concepte avaluat:** Propietat especial de MCM per a coprims, límits d'aplicabilitat.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: MCM i Cicles Periòdics

**Enunciat:**

Tres trens passen per una estació:
- Tren A: cada 6 hores
- Tren B: cada 8 hores
- Tren C: cada 10 hores

a) Calcula MCM(6, 8, 10) per trobar quan els tres trens coincideixen.

b) Si el tren A passa a les 6:00, a quina hora els tres passaran simultàniament?

c) En una setmana, quantes vegades coincidiran els tres trens?

**Solució:**

a) **MCM(6, 8, 10):**
   - `6 = 2 × 3`
   - `8 = 2^3`
   - `10 = 2 × 5`
   - Potències més altes: `2^3`, `3`, `5`
   - MCM = `2^3 × 3 × 5 = 8 × 3 × 5 = 120`
   - **Els tres trens coincideixen cada 120 hores.**

b) **Hora de coincidència:**
   - Primer pas: 6:00 (només A)
   - 120 hores després: 120 hores = 5 dies exactes
   - `6:00 + 120 hores = 6:00, 5 dies més tard`
   - **A les 6:00 del cinquè dia** (si avui és dia 1, demà és dia 2, etc.)

c) **Coincidències en una setmana (168 hores):**
   - `168 ÷ 120 = 1,4`
   - Coincidències completes: **1 vegada** (a les 6:00 del dia 6)
   - (La 2a seria a les 240h, que surt de la setmana)

**Concepte avaluat:** MCM amb múltiples cicles, aplicacions temporals reals.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Construcció de MCM amb Restriccions

**Enunciat:**

Trobaals números `a` i `b` que satisfacin simultàniament:

- MCD(a, b) = 6
- MCM(a, b) = 120
- `a < b`

a) Usa la relació `a × b = MCD(a, b) × MCM(a, b)` per estimar `a × b`.

b) Expressa `a = 6a'` i `b = 6b'` on MCD(a', b') = 1.

c) Usa MCM(a, b) = 120 per trobar MCM(a', b').

d) Sense enumeració, estima possibles parells `(a, b)`.

**Solució:**

a) **Producte:**
   - `a × b = 6 × 120 = 720`

b) **Expressió amb factor comú 6:**
   - `a = 6a'`, `b = 6b'` amb MCD(a', b') = 1
   - `a × b = 6a' × 6b' = 36a'b' = 720`
   - `a'b' = 720 ÷ 36 = 20`

c) **MCM(a', b'):**
   - MCM(a', b') = (a'b') / MCD(a', b') = 20 ÷ 1 = 20
   - MCM(a, b) = 6 × MCM(a', b') = 6 × 20 = 120 ✓

d) **Possibles parells (a', b'):**
   - Coprims amb producte 20: (1, 20), (4, 5), (5, 4), (20, 1)
   - Amb `a < b`: (1, 20) o (4, 5)
   
   - **Opció 1:** `a' = 1, b' = 20` → `a = 6, b = 120`
     - Verificació: MCD(6, 120) = 6 ✓; MCM(6, 120) = 120 ✓
   
   - **Opció 2:** `a' = 4, b' = 5` → `a = 24, b = 30`
     - Verificació: MCD(24, 30) = 6 ✓; MCM(24, 30) = 120 ✓
   
   - **Parells vàlids: (6, 120) i (24, 30)**

**Concepte avaluat:** Relació entre MCD i MCM, construcció inversa de nombres amb propietats prespecificades, raonament algebraic.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Definició de MCM | Moderat |
| 2 | MCM usant factorització prima | Intermedi |
| 3 | Relació MCM-MCD | Moderat |
| 4 | MCM de múltiples nombres | Intermedi |
| 5 | Discriminació MCD vs. MCM | Moderat |
| 6 | MCM en denominadors comuns | Intermedi |
| 7 | MCM en planejament | Intermedi |
| 8 | Propietat de MCM per a coprims | Intermedi |
| 9 | Cicles periòdics | Desafiador |
| 10 | Construcció inversa amb restriccions | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Confondre MCM amb MCD**: MCM és el **més petit** múltiple; MCD és el **més gran** divisor.
2. **Oblidar incloure totes les potències primeres**: Prendre només potències parcials dóna resultat incorrecte.
3. **Negligir que MCM(a, a) = a**: Un nombre és el seu propi MCM amb ell mateix.
4. **Pensar que MCM sempre és `a × b`**: Només si a i b són coprims.
5. **Aturar-se en qualsevol múltiple comú**: Cal trobar el **mínim**.

---

## 🔗 Connexions amb altres Blocs

- **Bloc 8 (MCD)**: Relació fonamental `a × b = MCD(a, b) × MCM(a, b)`.
- **Bloc 10 (Factorització)**: MCM es calcula més fàcilment usant factorització prima.
- **Mòdul 5 (Fraccions)**: MCM essencial per trobar denominador comú.
- **Mòdul 19 (Planejació)**: MCM per a sincronització de cicles.


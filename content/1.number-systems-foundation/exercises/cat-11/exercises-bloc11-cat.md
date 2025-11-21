# Exercicis Bloc 11 – Nombres Especials: Perfectes, Triangulars, Fibonacci

---

## 📌 Part 1: Comprensió de Nombres Especials

### 1.1 Completa les Definicions

**Nombre Perfect:** Un nombre que és igual a la suma dels seus ___________________.

**Nombre Triangular:** Un nombre que es pot representar com una ___________________ de punts.

**Successió de Fibonacci:** Una sèrie on cada terme és la suma dels ___________________.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 6 és un nombre perfect | | |
| 10 és un nombre triangular | | |
| Fibonacci només serveix per a matemàtiques | | |
| Els números especials no apareixen a la natura | | |

---

## 📌 Part 2: Nombres Perfectes

### 2.1 Verifica si Són Perfectes

**Mètode:** Suma tots els divisors propis (sense el número mateix).

**Exemple:** 6
- Divisors propis: 1, 2, 3
- Suma: 1 + 2 + 3 = 6 ✓ **Perfect!**

---

| Nombre | Divisors Propis | Suma | Perfect? |
|--------|----------------|------|----------|
| 6 | 1, 2, 3 | 6 | Sí |
| 10 | | | |
| 15 | | | |
| 28 | | | |

---

### 2.2 Busca Números Perfectes

**Pregunta:** Quins números menors de 100 són perfectes?

**Resposta:** _____________________________

---

**Pregunta:** Quants dígits té el següent número perfect després de 28?

**Resposta:** _____________________________

---

## 📌 Part 3: Nombres Triangulars

### 3.1 Identifica Nombres Triangulars

**Mètode:** Suma dels primers n nombres naturals.

Tn = 1 + 2 + 3 + ... + n = **n(n+1)/2**

```
n=1:  •           = 1
n=2:  • •         = 1 + 2 = 3
      •
n=3:  • • •       = 1 + 2 + 3 = 6
      •   •
      •
n=4:  • • • •     = 1 + 2 + 3 + 4 = 10
      •     •
      •     •
      •
```

---

### 3.2 Calcula Nombres Triangulars

| n | Fórmula n(n+1)/2 | Valor |
|---|-----------------|-------|
| 1 | 1(2)/2 | 1 |
| 2 | 2(3)/2 | 3 |
| 3 | 3(4)/2 | 6 |
| 4 | | |
| 5 | | |
| 10 | | |

---

### 3.3 Verifica Visualment

**Per a n=5:**

Dibuixa els punts en forma triangular:

```
• • • • •
• • • •
• • •
• •
•
```

Compte els punts: _____

Usa la fórmula: 5(6)/2 = _____

Match? **Sí / No**

---

## 📌 Part 4: La Successió de Fibonacci

### 4.1 Genera la Successió

**Mètode:** F₀ = 0, F₁ = 1, Fn = Fn₋₁ + Fn₋₂

| Posició | Cálcul | Valor |
|---------|--------|-------|
| F₀ | — | 0 |
| F₁ | — | 1 |
| F₂ | 0 + 1 | 1 |
| F₃ | 1 + 1 | 2 |
| F₄ | 1 + 2 | 3 |
| F₅ | | |
| F₆ | | |
| F₇ | | |
| F₈ | | |
| F₉ | | |
| F₁₀ | | |

---

### 4.2 Completa la Successió

**0, 1, 1, 2, 3, 5, 8, ___, ___, ___, ___, ___**

---

## 📌 Part 5: La Proporció Àuria (Phi)

### 5.1 Descobreix el Nombre d'Or

**Proporció Àuria (φ):** El ratio entre termes consecutius de Fibonacci tendeix a φ ≈ **1.618...**

| Ratio | F(n+1)/F(n) |
|-------|------------|
| F₂/F₁ | 1/1 = 1.000 |
| F₃/F₂ | 2/1 = 2.000 |
| F₄/F₃ | 3/2 = 1.500 |
| F₅/F₄ | 5/3 ≈ 1.667 |
| F₆/F₅ | 8/5 = 1.600 |
| F₇/F₆ | 13/8 = 1.625 |

---

### 5.2 Observa la Convergència

**Pregunta:** Els ratios convergeixen a quin número?

**Resposta:** _____________________________

---

## 📌 Part 6: Fibonacci a la Natura

### 6.1 Identifica Patrons

**Girasols:** Les llavors formen **espirals de Fibonacci**.

- Espiral interna: 21 llavors
- Espiral externa: 34 llavors
- Proporció: 34/21 ≈ _____

---

**Pinya (Picea abies):** Les escames formen espirals.

- Espiral dreta: 8 escames
- Espiral esquerra: 13 escames
- Números: **8 i 13 són números de Fibonacci!**

---

**Cambra Nautilus:** La closca creix en espiral logarítmica.

```
     ___
   /     \
  /       \
 | ◯       |  ← Cambra actual
  \       /
   \_____/
```

Cada cambra nova és φ vegades més gran.

---

### 6.2 Busca Més Patrons

**Pregunta:** Quins nombres de Fibonacci apareixen en:
- Petals de flor: ___________
- Branques d'arbre: ___________
- Espigues de blat: ___________

---

## 📌 Part 7: Relació entre Fibonacci i Números Triangulars

### 7.1 Descobreix la Connexió

**Identitat:** Suma de números de Fibonacci relacionats amb triangulars.

| Fibonacci | Triangular | Connexió? |
|-----------|-----------|-----------|
| F₁ = 1 | T₁ = 1 | = |
| F₂ + F₄ = 1 + 3 | T₂ + T₁ = 3 + 1 | = 4 |
| F₃ + F₅ = 2 + 5 | T₃ + T₂ = 6 + 3 | ? |

---

### 7.2 Relació amb Números Perfectes

**Fórmula d'Euclides per Números Perfectes:**

Si 2^n - 1 és primer, llavors **2^(n-1) × (2^n - 1)** és perfect.

| n | 2^n - 1 | Primer? | 2^(n-1) × (2^n - 1) | Perfect? |
|---|---------|--------|------------------|----------|
| 2 | 3 | Sí | 2 × 3 = 6 | Sí |
| 3 | 7 | Sí | 4 × 7 = 28 | Sí |
| 5 | 31 | Sí | 16 × 31 = ___ | ? |

---

## 📌 Part 8: Repte — Propietats Avançades

### 8.1 Números de Fibonacci Especials

**Pregunta 1:** Quin és el primer nombre de Fibonacci que és parell (no és 0)?

**Resposta:** F___ = ___

---

**Pregunta 2:** Cada quant elements de Fibonacci n'hi ha un que és divisible per 3?

**Resposta:** Cada ___ termes

---

**Pregunta 3:** Verifica la identitat: F₁ + F₂ + ... + Fn = F(n+2) - 1

Per a n=5:
- Suma: 1 + 1 + 2 + 3 + 5 = ___
- F(n+2) - 1 = F₇ - 1 = ___ - 1 = ___

Match? **Sí / No**

---

### 8.2 Cas del Nombre d'Or

**Pregunta:** La proporció àuria φ satisfà la següent equació:

**φ² = φ + 1**

Verifica:
- φ ≈ 1.618
- φ² ≈ ___________
- φ + 1 ≈ ___________

Match? **Sí / No**

---

## 📌 Part 9: Aplicacions en el Món Real

### 9.1 Fibonacci en Tecnologia

**Busca de Binaria (Fibonacci Search):**

Un algoritme basat en Fibonacci per a cerques eficients en dades ordenades.

**Per què funciona?** Els números de Fibonacci creixen exponencialment, com l'algoritme de cerca.

---

### 9.2 Proporció Àuria en Disseny

**Arte:** Molts pintors usen la proporció àuria (1:1.618) per a composicions harmonioses.

- Leonardo da Vinci: utilitzava φ en anatomia
- Composicions de Mondrian

**Arquitectura:** L'Alhambra (Granada) continha proporcions de Fibonacci

---

### 9.3 Biologia

**Reproducció de Conills (Problema Original de Fibonacci):**

Una parella de conills es reprodueix:
- Primer mes: 1 parella
- Segon mes: 1 parella (necessita mes per madurar)
- Tercer mes: 2 parelles (surt una nova)
- Quart mes: 3 parelles
- Quint mes: 5 parelles

**Pattern:** 1, 1, 2, 3, 5, 8, 13... **Fibonacci!**

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Nombres Especials

**Exercici 1 (Perfecte):**

"Verifica si _____ és un nombre perfect"

**Solució:** ________________

---

**Exercici 2 (Triangular):**

"Calcula el n=_____ nombre triangular usant la fórmula"

**Solució:** T___ = ___

---

**Exercici 3 (Fibonacci):**

"Genera els primers _____ nombres de Fibonacci"

**Solució:** ________________

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què els números especials apareixen tant a la natura?

_________________________________________________________________

**Pregunta 2:** Quina és la connexió entre Fibonacci i la bellesa matemàtica?

_________________________________________________________________

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Nombres Perfectes): ✓
- [ ] Part 3 (Nombres Triangulars): ✓
- [ ] Part 4 (Fibonacci): ✓
- [ ] Part 5 (Proporció Àuria): ✓
- [ ] Part 6 (Fibonacci a la Natura): ✓
- [ ] Part 7 (Relacions): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Aplicacions): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, els nombres especials ja no són secrets! 🎉

---

**Recorda:** Els números especials revelen l'ordre ocultat de l'univers! 🌿


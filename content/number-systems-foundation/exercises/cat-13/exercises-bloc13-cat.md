# Exercicis Bloc 13 – Nombres de Mersenne i Primers de Mersenne

---

## 📌 Part 1: Comprensió de Nombres de Mersenne

### 1.1 Completa les Definicions

**Nombre de Mersenne:** Un nombre de la forma _________________ on p és un nombre primer.

**Primer de Mersenne:** Un nombre de Mersenne que és _________________.

**Exponent de Mersenne:** El nombre _________________ en 2^p - 1.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 2³ - 1 = 7 és un nombre de Mersenne | | |
| Tots els 2^p - 1 són primers | | |
| Els primers de Mersenne són rars | | |
| Els primers de Mersenne són sempre parells | | |

---

## 📌 Part 2: Calcula Nombres de Mersenne

### 2.1 Taula de Números de Mersenne

| p | 2^p | 2^p - 1 | Primer? |
|---|-----|---------|---------|
| 2 | 4 | 3 | Sí |
| 3 | 8 | 7 | Sí |
| 5 | 32 | 31 | Sí |
| 7 | 128 | 127 | Sí |
| 11 | | | |
| 13 | | | |

---

### 2.2 Completa la Taula

Per a **p = 11:**
- 2^11 = _____
- 2^11 - 1 = _____
- És primer? _____

---

Per a **p = 13:**
- 2^13 = _____
- 2^13 - 1 = _____
- És primer? _____

---

## 📌 Part 3: Condició Necessària per a Primers de Mersenne

### 3.1 Comprensió: p ha de ser primer

**Teorema:** Si 2^n - 1 és primer, llavors n ha de ser primer.

**Contraexemple:** Si n és compost, 2^n - 1 NO és primer.

---

| n | Tipus | 2^n - 1 | Factorització |
|---|-------|---------|---------------|
| 4 (compost) | 2² | 15 | 3 × 5 |
| 6 (compost) | 2 × 3 | 63 | 7 × 9 |
| 8 (compost) | 2³ | 255 | 3 × 5 × 17 |
| 9 (compost) | 3² | 511 | | |

---

### 3.2 Per Què no Funciona n Compost?

**Identitat Algebraica:**

Si n = a × b, llavors **2^n - 1 = 2^(a×b) - 1 sempre és divisible per 2^a - 1**

**Exemple:** n = 6 = 2 × 3
- 2^6 - 1 = 63
- 2² - 1 = 3 (divisor!)
- 2³ - 1 = 7 (divisor!)
- 63 = 3 × 21 = 3 × 7 × 3 ✓

---

## 📌 Part 4: Primers de Mersenne Coneguts

### 4.1 Els Primers 12 Primers de Mersenne

| # | p | 2^p - 1 | Dígits | Any |
|---|---|---------|--------|-----|
| 1 | 2 | 3 | 1 | Ancient |
| 2 | 3 | 7 | 1 | Ancient |
| 3 | 5 | 31 | 2 | Ancient |
| 4 | 7 | 127 | 3 | Ancient |
| 5 | 13 | 8191 | 4 | 1461 |
| 6 | 17 | 131071 | 5 | 1588 |
| 7 | 19 | 524287 | 6 | 1588 |
| 8 | 31 | 2147483647 | 10 | 1772 |
| 9 | 61 | 2^61 - 1 | 19 | 1883 |
| 10 | 89 | 2^89 - 1 | 27 | 1911 |
| 11 | 107 | 2^107 - 1 | 33 | 1914 |
| 12 | 127 | 2^127 - 1 | 39 | 1876 |

---

### 4.2 Observa els Patrons

**Pregunta:** Els exponents p (2, 3, 5, 7, 13...) sembla que siguin?

**Resposta:** _____________________________

---

**Pregunta:** Quants dígits té 2^127 - 1?

**Resposta:** _____________________________

---

## 📌 Part 5: Proves de Primalitat

### 5.1 Prova de Lucas-Lehmer

**Algoritme eficient per verificar si 2^p - 1 és premier:**

S₀ = 4

Per i = 1 a p-2:
  Sᵢ = (Sᵢ₋₁)² - 2 mod (2^p - 1)

Si S_{p-2} = 0, llavors **2^p - 1 és premier!**

---

### 5.2 Aplica para p = 5

M₅ = 2^5 - 1 = **31**

S₀ = 4

**S₁ = (S₀)² - 2 mod 31 = (4)² - 2 mod 31 = 16 - 2 mod 31 = 14 mod 31 = ___**

**S₂ = (S₁)² - 2 mod 31 = (___)² - 2 mod 31 = ... = ___ mod 31**

**S₃ = (S₂)² - 2 mod 31 = (___)² - 2 mod 31 = ... = ___ mod 31 = 0?**

Si S₃ = 0, llavors **31 és premier!** ✓

---

## 📌 Part 6: Relació amb Números Perfectes

### 6.1 Fórmula d'Euclides

**Si 2^p - 1 és primer, llavors:**

**N = 2^(p-1) × (2^p - 1) és un número PERFECT!**

---

| p | 2^p - 1 | Primer? | N = 2^(p-1) × (2^p - 1) | Comprovar |
|---|---------|--------|----------------------|-----------|
| 2 | 3 | Sí | 2¹ × 3 = 6 | Perfect ✓ |
| 3 | 7 | Sí | 2² × 7 = 28 | Perfect ✓ |
| 5 | 31 | Sí | 2⁴ × 31 = 496 | Perfect ✓ |
| 7 | 127 | Sí | 2⁶ × 127 = 8128 | Perfect ✓ |

---

### 6.2 Descubre Números Perfectes Nous

**Per a p = 13:**
- 2^13 - 1 = _____ (és premier?)
- Si sí: N = 2^12 × (2^13 - 1) = 4096 × _____ = _____
- **Seria un número perfect MÚY GRAN!**

---

## 📌 Part 7: La Recerca Moderna

### 7.1 Llista de Descobriments

| # | p | Descoberta | Investigador |
|---|---|-----------|---------------|
| 13 | 521 | 1952 | Computador Robinson |
| 14 | 607 | 1952 | Computador Robinson |
| 15 | 1279 | 1952 | Computador Robinson |
| 20 | 4423 | 1961 | Computador Hurwitz |
| 25 | 21701 | 1978 | Noll, Nickel |
| 30 | 110503 | 1988 | Colquitt, Welsh |
| 52 | **136279279** | 2024 | Computador distribuït |

---

### 7.2 Creixement dels Exponents

**Pregunta:** Com creixen els exponents p?

- p₁ = 2, p₂ = 3, p₃ = 5, p₄ = 7, p₅ = 13, ...

**Patern:** _____________________________

---

**Pregunta:** Quants dígits té 2^136279279 - 1?

**Resposta:** Aproximadament **41 MILIONS de dígits!**

---

## 📌 Part 8: Repte — Propietats Especials

### 8.1 Números de Mersenne Imparells

**Pregunta:** Per a p > 2, 2^p - 1 sempre és senar o parell?

**Resposta:** _____________________________

---

**Pregunta:** Per què? (Pista: 2^p sempre és parell)

**Resposta:** 2^p - 1 és parell - 1 = _____

---

### 8.2 Suma de Divisors

**Per al primer de Mersenne p = 3:**
- M₃ = 7 (primer)
- Divisors: 1, 7
- σ(7) = 1 + 7 = 8

**Pregunta:** Per a tots els primers de Mersenne, σ(M) = ?

**Resposta:** σ(M) = M + 1 (perquè M és primer!)

---

## 📌 Part 9: Aplicacions i Preguntes Obertes

### 9.1 Usages del Primers de Mersenne

**Matemàtiques:**
- Teoria de números
- Números perfectes
- Criptografia

**Computació:**
- Testing de computadors (validar hardware!)
- Algoritmes de computació distribuïda
- Distribució de càrrega computacional

---

### 9.2 La Gran Pregunta Oberta

**Conjectura:** "Hi ha infinits primers de Mersenne?"

**Evidència:** 
- 52 descoberts fins 2024
- Creixen cada vegada més rares
- Però possiblement infinits?

**Premi:** Qui provi això farà história! 🏆

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Mersenne

**Exercici 1:**

"Per a p = _____, calcula 2^p - 1 i determina si és primer"

**Solució:** ________________

---

**Exercici 2:**

"Usa la fórmula d'Euclides per generar un número perfect usant p = _____"

**Solució:** N = _____ (és perfect!)

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què els primers de Mersenne són tan importants?

_________________________________________________________________

**Pregunta 2:** Creus que hi ha infinits premiers de Mersenne?

_________________________________________________________________

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

**Recorda:** Els primers de Mersenne són les joies més buscades de la matemàtica! 💎


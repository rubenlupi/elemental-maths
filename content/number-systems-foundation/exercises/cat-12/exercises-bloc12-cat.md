# Exercicis Bloc 12 – Nombres Amics i Sociables

---

## 📌 Part 1: Comprensió de Nombres Amics

### 1.1 Completa les Definicions

**Nombres Amics:** Dos nombres on la suma dels divisors propis del primer és igual al _________________.

**Parell Amic:** La menor combinació de _________________  nombres amics.

**Nombres Sociables:** Una cadena cíclica de números on cada suma de divisors mena al _________________.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| 220 i 284 són nombres amics | | |
| Todo nombre perfecte és amic amb si mateix | | |
| Els números amics són rars | | |
| La suma de dos números amics és sempre parell | | |

---

## 📌 Part 2: Descobreix Nombres Amics Clàssics

### 2.1 Verifica 220 i 284

**Divisors propis de 220 (sense 220):**
1, 2, 4, 5, 10, 11, 20, 22, 44, 55, 110

Suma: _____ + _____ + _____ + ... = _____

---

**Divisors propis de 284 (sense 284):**
1, 2, 4, 71, 142

Suma: _____ + _____ + _____ + _____ + _____ = _____

---

**Conclusió:** Els divisors de 220 sumen _____ i els de 284 sumen _____

**220 i 284 són amics? Sí / No**

---

### 2.2 Búsqueda de Parells Amics

| Parell | σ(a) | σ(b) | Amics? |
|--------|------|------|--------|
| (220, 284) | 284 | 220 | Sí |
| (1184, 1210) | | | |
| (2620, 2924) | | | |
| (5020, 5564) | | | |

---

## 📌 Part 3: Factorització i Números Amics

### 3.1 Usa Factorització per Encontrar Divisors

**Per a 220:**

220 = 2² × 5 × 11

Divisors: 1, _____, _____, _____, 5, _____, _____, _____, 10, _____, _____, 22, _____, 44, _____, 110, _____, 220

(Quants divisors?: (2+1)(1+1)(1+1) = ___ divisors)

---

**Per a 284:**

284 = 2² × 71

Divisors: 1, 2, _____, 4, _____, 142, _____

(Quants divisors?: (2+1)(1+1) = ___ divisors)

---

### 3.2 Calcula σ(n) usant Factorització

**Fórmula per suma de divisors:**

Si n = p₁^a × p₂^b, llavors:

σ(n) = (p₁^(a+1) - 1)/(p₁ - 1) × (p₂^(b+1) - 1)/(p₂ - 1)

---

**Per a 220 = 2² × 5 × 11:**

σ(220) = (2³ - 1)/(2 - 1) × (5² - 1)/(5 - 1) × (11² - 1)/(11 - 1)

σ(220) = (_____ / _____) × (_____ / _____) × (_____ / _____)

σ(220) = _____ × _____ × _____ = _____

---

## 📌 Part 4: Nombres Perfectes com a Casos Especials

### 4.1 Perfect = "Amic de si mateix"?

**Pregunta:** Si n és perfect, σ(n) - n = ?

**Resposta:** _____ (per definició de perfect)

---

**Exemple:** 6 és perfect

σ(6) = 1 + 2 + 3 + 6 = 12
σ(6) - 6 = 12 - 6 = **6** ✓

---

**Pregunta:** Per qué un nombre perfect NO és "amic amb si mateix"?

**Resposta:** Perquè per ser amics, la suma dels divisors PROPIS (sense el número) ha de igualar l'altre número.

6 → divisors propis → 1 + 2 + 3 = 6 ✓ (és perfect, no amic)

---

## 📌 Part 5: Números Sociables (Cadenes de Nombres)

### 5.1 Comprén la Cadena

**Definició:** Números a₁, a₂, ..., ak on:
- σ(a₁) - a₁ = a₂
- σ(a₂) - a₂ = a₃
- ...
- σ(ak) - ak = a₁ (torna al primer!)

---

### 5.2 Exemple: Cadena Sociable de Longitud 4

**Cadena:** 12496 → 14288 → 15472 → 14536 → 12496

Verifica el primer pas:

Divisors propis de 12496: 1, 2, 4, 8, 16, 11, 22, 44, ...

Suma: ___________

Resultat: _____ (hauria de ser 14288)

---

## 📌 Part 6: Buscant Parells Amics

### 6.1 Fórmula de Thabit ibn Qurra

**Fórmula (900 AD):**

Si a = 3 × 2^n - 1, b = 3 × 2^(n-1) - 1, c = 9 × 2^(2n-1) - 1

i a, b, c són TOTS primers, llavors:

**a₁ = 2^n × b × c** i **a₂ = 2^n × a** són nombres amics!

---

### 6.2 Aplica Thabit per a n = 2

n = 2:
- a = 3 × 2² - 1 = 3 × 4 - 1 = _____ (és primer? ____)
- b = 3 × 2¹ - 1 = 3 × 2 - 1 = _____ (és primer? ____)
- c = 9 × 2³ - 1 = 9 × 8 - 1 = _____ (és primer? ____)

Si tota són primers:
- a₁ = 2² × b × c = 4 × _____ × _____ = _____
- a₂ = 2² × a = 4 × _____ = _____

**Parell amic:** (_____, _____) ?

---

## 📌 Part 7: Propietats dels Nombres Amics

### 7.1 La Suma és Abundant

**Definició:** Un nombre és abundant si σ(n) - n > n (suma de divisors propis > n)

**Pregunta:** 220 és abundant?

σ(220) = 504
σ(220) - 220 = 284

284 > 220? **Sí / No** → 220 és _________ (abundant/deficient)

---

### 7.2 Paritat dels Números Amics

| Propietat | Explicació | Exemple |
|-----------|-----------|---------|
| (220, 284) | Ambdós parells | Tots els parells amics coneguts |
| Imparells amics | Potser no existeixen? | DESCONEGUT |
| Mixtos (parell + imparell) | Descoberts en 2023 | Nous parells! |

---

## 📌 Part 8: Repte — Buscant Nous Parells

### 8.1 Algoritme de Cerca

**Passos:**
1. Calcula σ(n) - n per a cada n
2. Si resultat = m i σ(m) - m = n, llavors (n, m) són amics!

---

**Busca manual:**

Per n = 1 a 300:
- σ(220) - 220 = 284
- σ(284) - 284 = **220** ✓ **(220, 284) encontrats!**

---

### 8.2 Parells Amics Descoberts

| Parell | Any | Descobridor |
|--------|-----|-------------|
| (220, 284) | ~1000 BC | Grega (legend diu Pythagore) |
| (1184, 1210) | 1000 AD | Al-Farabi (matemàtic persa) |
| (2620, 2924) | 1638 | Fermat |
| (5020, 5564) | 1638 | Fermat |
| (6232, 6368) | 1747 | Euler |

---

## 📌 Part 9: Aplicacions i Connexions

### 9.1 Místiques i Culturals

**Pythagoreans (Grècia, 500 BC):**

Creien que 220 i 284 tenien poder místic de fertilitat i matrimoni.

---

**Ibn Qurra (Arabia, 900 AD):**

"Si es dona 220 a un jove i 284 a una noia en secret, quedaran enamorats per sempre."

---

### 9.2 Connexió amb Tarot

En algunas tradicions ocultals, 220 i 284 estan vinculats a cartes del Tarot.

Però... **és tot superstició matemàtica! 😊**

---

## 📌 Part 10: Crea els Teus Exercicis

### 10.1 Disseny de Números Amics

**Exercici 1:**

"Verifica si (_____, _____) són nombres amics calculant les seves sumes de divisors"

**Solució:** ________________

---

**Exercici 2:**

"Usa la fórmula de Thabit per a n = _____ i calcula el parell amic resultant"

**Solució:** (_____, _____) són amics

---

### 10.2 Reflexió Final

**Pregunta 1:** Per què els números amics són tan rars?

_________________________________________________________________

**Pregunta 2:** Creus que hi ha infinits parells amics?

_________________________________________________________________

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Descoberta): ✓
- [ ] Part 3 (Factorització): ✓
- [ ] Part 4 (Perfectes): ✓
- [ ] Part 5 (Sociables): ✓
- [ ] Part 6 (Thabit): ✓
- [ ] Part 7 (Propietats): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Aplicacions): ✓
- [ ] Part 10 (Creació): ✓

**Puntuació:** Si has marcat 8 o més, els números amics ja no són misteris! 🎉

---

**Recorda:** La divisió de la suma de divisors és una dansa entre dos números! 💕


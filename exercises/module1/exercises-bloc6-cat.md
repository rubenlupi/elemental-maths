# Exercicis - Mòdul 1: Bloc 6 – Pràctica de Regles de Divisibilitat

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Aplicació Directa: Divisibilitat per 2, 5 i 10

**Enunciat:**

Determina si els següents nombres són divisibles per `2`, `5`, i `10`:

a) `240`
b) `135`
c) `407`
d) `2.560`

**Solució:**

| Nombre | Divisible per 2? | Divisible per 5? | Divisible per 10? | Justificació |
|--------|------------------|------------------|-------------------|---|
| a) 240 | ✓ (últim: 0) | ✓ (últim: 0) | ✓ (últim: 0) | Termina en 0 (parell) |
| b) 135 | ✗ (últim: 5) | ✓ (últim: 5) | ✗ (últim: 5) | Termina en 5 (imparell) |
| c) 407 | ✗ (últim: 7) | ✗ (últim: 7) | ✗ (últim: 7) | Termina en 7 (imparell, ni 0 ni 5) |
| d) 2.560 | ✓ (últim: 0) | ✓ (últim: 0) | ✓ (últim: 0) | Termina en 0 (parell) |

**Concepte avaluat:** Aplicació de regles de divisibilitat bàsiques per a 2, 5, 10 usant últim dígit.

---

### **Exercici 2** 🟦 (1.1 punts) – Divisibilitat per 3 i 9

**Enunciat:**

Determina si els següents nombres són divisibles per `3` i `9` usant la suma de dígits:

a) `372`
b) `819`
c) `1.234`
d) `2.556`

(Recorda: Divisible per `3` si suma de dígits és múltiple de `3`; divisible per `9` si suma de dígits és múltiple de `9`.)

**Solució:**

| Nombre | Suma de dígits | Divisible per 3? | Divisible per 9? |
|--------|---|---|---|
| a) 372 | 3+7+2 = 12 | ✓ (12 ÷ 3 = 4) | ✗ (12 ÷ 9 ≠ enter) |
| b) 819 | 8+1+9 = 18 | ✓ (18 ÷ 3 = 6) | ✓ (18 ÷ 9 = 2) |
| c) 1.234 | 1+2+3+4 = 10 | ✗ (10 ÷ 3 ≠ enter) | ✗ (10 ÷ 9 ≠ enter) |
| d) 2.556 | 2+5+5+6 = 18 | ✓ (18 ÷ 3 = 6) | ✓ (18 ÷ 9 = 2) |

**Verificació:**
- `372 ÷ 3 = 124` ✓; `372 ÷ 9 = 41,33...` ✗
- `819 ÷ 3 = 273` ✓; `819 ÷ 9 = 91` ✓
- `1.234 ÷ 3 = 411,33...` ✗; `1.234 ÷ 9 = 137,11...` ✗
- `2.556 ÷ 3 = 852` ✓; `2.556 ÷ 9 = 284` ✓

**Concepte avaluat:** Ús de suma de dígits per a divisibilitat per 3 i 9.

---

### **Exercici 3** ⭐ (0.9 punts) – Divisibilitat per 4 i 8

**Enunciat:**

Determina si els següents nombres són divisibles per `4` i `8`:

a) `216`
b) `524`
c) `1.032`
d) `3.200`

(Recorda: Divisible per `4` si els últims dos dígits formen un nombre divisible per `4`; divisible per `8` si els últims tres dígits formen un nombre divisible per `8`.)

**Solució:**

| Nombre | Últims 2 dígits | Divisible per 4? | Últims 3 dígits | Divisible per 8? |
|--------|---|---|---|---|
| a) 216 | 16 | ✓ (16 ÷ 4 = 4) | 216 | ✓ (216 ÷ 8 = 27) |
| b) 524 | 24 | ✓ (24 ÷ 4 = 6) | 524 | ✗ (524 ÷ 8 = 65,5) |
| c) 1.032 | 32 | ✓ (32 ÷ 4 = 8) | 032 | ✓ (32 ÷ 8 = 4) |
| d) 3.200 | 00 | ✓ (0 ÷ 4 = 0) | 200 | ✗ (200 ÷ 8 = 25) |

**Concepte avaluat:** Ús dels últims 2 i 3 dígits per a divisibilitat per 4 i 8.

---

### **Exercici 4** 🟦 (1.2 punts) – Taula de Divisibilitat Ràpida

**Enunciat:**

Completa la taula verificant si cada nombre és divisible pels divisors especificats:

| Nombre | Divisible per 2? | Divisible per 3? | Divisible per 5? | Divisible per 6? |
|--------|---|---|---|---|
| 180 | ? | ? | ? | ? |
| 267 | ? | ? | ? | ? |
| 450 | ? | ? | ? | ? |

(Recorda: Divisible per `6` si és divisible per `2` i `3` simultàniament.)

**Solució:**

| Nombre | Divisible per 2? | Divisible per 3? | Divisible per 5? | Divisible per 6? |
|--------|---|---|---|---|
| 180 | ✓ (últim 0) | ✓ (1+8+0=9) | ✓ (últim 0) | ✓ (2 i 3) |
| 267 | ✗ (últim 7) | ✓ (2+6+7=15) | ✗ (últim 7) | ✗ (no divisible per 2) |
| 450 | ✓ (últim 0) | ✓ (4+5+0=9) | ✓ (últim 0) | ✓ (2 i 3) |

**Concepte avaluat:** Aplicació de múltiples regles de divisibilitat simultàniament, combinació de regles (e.g., 6 requereix 2 i 3).

---

### **Exercici 5** ⭐ (0.8 punts) – Identificació del Divisor Comú

**Enunciat:**

Per a cada parell de nombres, identifica quin divisor comú (dels llistats) divideix tots dos:

a) `24` i `36`: divisor entre `2, 3, 4, 5, 6, 9`?

b) `45` i `60`: divisor entre `2, 3, 5, 6, 9, 10`?

c) `100` i `75`: divisor entre `2, 3, 5, 10, 25`?

**Solució:**

a) `24` i `36`:
   - `24 = 2^3 × 3`; `36 = 2^2 × 3^2`
   - Divisors comuns: `2, 3, 4, 6` (tots entre els llistats)
   - Resposta: `2, 3, 4, 6` són divisors comuns.

b) `45` i `60`:
   - `45 = 3^2 × 5`; `60 = 2^2 × 3 × 5`
   - Divisors comuns: `3, 5, 15`
   - Entre els llistats: `3, 5`
   - Resposta: `3, 5`.

c) `100` i `75`:
   - `100 = 2^2 × 5^2`; `75 = 3 × 5^2`
   - Divisors comuns: `5, 25`
   - Entre els llistats: `5, 25`
   - Resposta: `5, 25`.

**Concepte avaluat:** Identificació de divisors comuns usant divisibilitat.

---

### **Exercici 6** 🟦 (1.0 punt) – Aplicació de Transitivitat de Divisibilitat

**Enunciat:**

Si `6 | 18` (és a dir, 6 divideix 18) i `18 | 72`, aleshores `6 | 72` per transitivitat.

Per a cada conjunt, verifica la transitivitat:

a) `5 | 10`, `10 | 50` → `5 | 50`?

b) `3 | 12`, `12 | 48` → `3 | 48`?

c) `4 | 20`, `20 | 100` → `4 | 100`?

Verifica cada cas calculant les divisions.

**Solució:**

a) `5 | 10`, `10 | 50` → `5 | 50`?
   - `10 ÷ 5 = 2` ✓; `50 ÷ 10 = 5` ✓
   - `50 ÷ 5 = 10` ✓
   - **Transitivitat verificada.**

b) `3 | 12`, `12 | 48` → `3 | 48`?
   - `12 ÷ 3 = 4` ✓; `48 ÷ 12 = 4` ✓
   - `48 ÷ 3 = 16` ✓
   - **Transitivitat verificada.**

c) `4 | 20`, `20 | 100` → `4 | 100`?
   - `20 ÷ 4 = 5` ✓; `100 ÷ 20 = 5` ✓
   - `100 ÷ 4 = 25` ✓
   - **Transitivitat verificada.**

**Concepte avaluat:** Propietat de transitivitat de divisibilitat, encadenament de relacions.

---

### **Exercici 7** 🟦 (1.1 punts) – Divisibilitat de Sumes i Diferències

**Enunciat:**

Si `a | b` i `a | c`, aleshores `a | (b + c)` i `a | (b - c)`.

Verifica aquesta propietat:

a) `7 | 14` i `7 | 21`. Comprova que `7 | (14+21)` i `7 | (14-21)`.

b) `6 | 24` i `6 | 36`. Comprova que `6 | (24+36)` i `6 | (24-36)`.

**Solució:**

a) `7 | 14` i `7 | 21`:
   - `14 + 21 = 35`; `35 ÷ 7 = 5` ✓
   - `21 - 14 = 7`; `7 ÷ 7 = 1` ✓
   - **Propietat verificada.**

b) `6 | 24` i `6 | 36`:
   - `24 + 36 = 60`; `60 ÷ 6 = 10` ✓
   - `36 - 24 = 12`; `12 ÷ 6 = 2` ✓
   - **Propietat verificada.**

**Concepte avaluat:** Combinació de divisibilitat en sumes i diferències, estensió de divisibilitat.

---

### **Exercici 8** 🟦 (1.3 punts) – Aplicació Real: Distribució Equitativa

**Enunciat:**

Una escola vol distribuir `240` estudiants en grups iguals.

a) Llista tots els divisors de `240`.

b) Per a cadascun dels seguents tamanys de grup (`6, 8, 10, 12, 16, 20`), determina si es pot formar un nombre exacte de grups. Justifica usant regles de divisibilitat.

c) Quin és el nombre de grups si cada grup té `12` persones?

**Solució:**

a) Divisors de `240`:
   - `240 = 2^4 × 3 × 5`
   - Divisors: `1, 2, 3, 4, 5, 6, 8, 10, 12, 15, 16, 20, 24, 30, 40, 48, 60, 80, 120, 240`

b) Possibilitat de formar grups:

| Mida de grup | Divisible? | Justificació |
|---|---|---|
| 6 | ✓ | 240 és divisible per 2 i 3 |
| 8 | ✓ | 240 és divisible per 8 (últims 3 dígits: 240 ÷ 8 = 30) |
| 10 | ✓ | 240 termina en 0 |
| 12 | ✓ | 240 és divisible per 4 i 3 |
| 16 | ✓ | 240 ÷ 16 = 15 |
| 20 | ✓ | 240 és divisible per 20 |

c) Nombre de grups amb 12 persones per grup:
   - `240 ÷ 12 = 20` grups.

**Concepte avaluat:** Aplicació real de divisibilitat, distribució equitativa, verificació de criteris.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Construcció de Nombres amb Restriccions de Divisibilitat

**Enunciat:**

Construeix un nombre de quatre dígits que satisfaci les següents condicions simultàniament:

- Divisible per `2` (últim dígit parell)
- Divisible per `3` (suma de dígits múltiple de 3)
- Divisible per `5` (últim dígit 0 o 5)
- No divisible per `4`

a) Explica per què les condicions de `2` i `5` impliquen que l'últim dígit ha de ser `0`.

b) Construeix un nombre que compleixi totes les condicions. Verifica cada una.

c) Quin és el nombre més petit de quatre dígits que satisfà les condicions?

**Solució:**

a) Explicació:
   - Divisible per `2`: últim dígit parell (0, 2, 4, 6, 8)
   - Divisible per `5`: últim dígit 0 o 5
   - Intersecció: l'últim dígit ha de ser `0`.

b) Construcció: Escollem `_ _ _ 0` amb suma de dígits múltiple de 3, però no divisible per 4.
   - Últims 2 dígits: `_0`
   - Per no ser divisible per 4, `_0` no ha de ser múltiple de 4 (e.g., `10, 30, 50, 70, 90` són vàlids; `20, 40, 60, 80` són divisibles per 4).
   - Escollim `5130`:
     - Divisible per 2? Sí, últim dígit 0 ✓
     - Divisible per 3? 5+1+3+0 = 9 ✓
     - Divisible per 5? Sí, últim dígit 0 ✓
     - Divisible per 4? Últims 2 dígits: `30 ÷ 4 = 7,5` ✗

c) Nombre més petit de quatre dígits:
   - Comença amb `1___0` per minimitzar.
   - Suma de dígits múltiple de 3: `1 + a + b + 0 = múltiple de 3`.
   - Escollinm `1 + 2 + 0 + 0 = 3` (no vàlid, ocupen posicions 1, 4).
   - Millor: `1020` → suma = 3 ✓, últim dígit 0, divisible per 2 i 5.
   - Però `1020 ÷ 4 = 255` (divisible, no vàlid).
   - Millor: `1050` → suma = 6 ✓, últim dígit 0, últims dígits 50 (no divisible per 4).
   - Verificació: `1050 ÷ 2 = 525` ✓, `1050 ÷ 3 = 350` ✓, `1050 ÷ 5 = 210` ✓, `1050 ÷ 4 = 262,5` ✗
   - **Resposta: `1050`.**

**Concepte avaluat:** Construcció de nombres amb múltiples restriccions, síntesi de regles de divisibilitat.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Anàlisi de Patterns de Divisibilitat

**Enunciat:**

Considera la seqüència de nombres múltiples de 6: `6, 12, 18, 24, 30, 36, ...`

a) Els nombres múltiples de 6 són sempre divisibles per `2` i `3`. Per què?

b) Crea una taula per als primers 10 múltiples de 6, verificant divisibilitat per `2, 3, 4, 5, 9`.

c) Quins d'aquests múltiples de 6 són també divisibles per `4`? Quins patrons nотis?

d) Predicció: Si `n` és múltiple de 6 però **no** divisible per 4, quina és la forma general de `n`? (Pista: Pensa en múltiples de 12, 24, ...)

**Solució:**

a) Per què múltiples de 6 són divisibles per 2 i 3:
   - `6 = 2 × 3`
   - Si `n = 6k = 2 × 3 × k`, aleshores `n` conté els factors 2 i 3.
   - Per tant, `2 | n` i `3 | n`.

b) Taula per als primers 10 múltiples de 6:

| n | Divisible per 2? | Divisible per 3? | Divisible per 4? | Divisible per 5? | Divisible per 9? |
|---|---|---|---|---|---|
| 6 | ✓ | ✓ | ✗ | ✗ | ✗ |
| 12 | ✓ | ✓ | ✓ | ✗ | ✗ |
| 18 | ✓ | ✓ | ✗ | ✗ | ✓ |
| 24 | ✓ | ✓ | ✓ | ✗ | ✗ |
| 30 | ✓ | ✓ | ✗ | ✓ | ✗ |
| 36 | ✓ | ✓ | ✓ | ✗ | ✓ |
| 42 | ✓ | ✓ | ✗ | ✗ | ✗ |
| 48 | ✓ | ✓ | ✓ | ✗ | ✗ |
| 54 | ✓ | ✓ | ✗ | ✗ | ✓ |
| 60 | ✓ | ✓ | ✓ | ✓ | ✗ |

c) Múltiples de 6 divisibles per 4: `12, 24, 36, 48, 60, ...`
   - Pattern: Són múltiples de `lcm(6, 4) = 12`.
   - Cada tercer múltiple de 6 és divisible per 4.

d) Predicció sobre múltiples de 6 **no** divisibles per 4:
   - Són múltiples de 6 que no són múltiples de 12.
   - Forma general: `6(2k+1) = 6, 18, 30, 42, 54, ...`
   - Aquests són múltiples de 6 amb factor `(2k+1)` imparell.

**Concepte avaluat:** Análisi de patrons, síntesi de múltiples regles, predicció d'estructura matemàtica.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Regles de divisibilitat bàsiques (2, 5, 10) | Moderat |
| 2 | Divisibilitat per 3 i 9 usant suma de dígits | Intermedi |
| 3 | Divisibilitat per 4 i 8 usant últims dígits | Moderat |
| 4 | Aplicació múltiple de regles simultàniament | Intermedi |
| 5 | Identificació de divisors comuns | Moderat |
| 6 | Transitivitat de divisibilitat | Intermedi |
| 7 | Divisibilitat de sumes i diferències | Intermedi |
| 8 | Aplicació real: distribució equitativa | Intermedi |
| 9 | Construcció amb restriccions múltiples | Desafiador |
| 10 | Análisis de patrons de divisibilitat | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Aplicar la regla equivocada**: Suma de dígits és per a 3/9, no per a 4/8.
2. **Oblidar que 6 requereix 2 i 3**: Divisibilitat per 6 no és independent.
3. **Negligir els zeros**: Els darrers zeros són importants per a divisibilitat per 2, 5, 10.
4. **Confondre divisors amb múltiples**: `2 | 6` significa 2 divideix 6, no al revés.


# Exercicis - Mòdul 1: Bloc 5 – Introducció a la Notació Científica

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Aplicació Directa: Conversió a Notació Científica

**Enunciat:**

Converteix els següents nombres a notació científica de la forma `a × 10^n` (on `1 ≤ |a| < 10`):

a) `5.000`

b) `234.000`

c) `0,0045`

**Solució:**

a) `5.000 = 5 × 10^3`
   - Explicació: El decimal comença a `5.000,0` i es desplaça 3 llocs a l'esquerra per aconseguir `5.`

b) `234.000 = 2,34 × 10^5`
   - Explicació: El decimal comença a `234.000,0` i es desplaça 5 llocs a l'esquerra per aconseguir `2,34`.

c) `0,0045 = 4,5 × 10^-3`
   - Explicació: El decimal comença a `0,0045` i es desplaça 3 llocs a la dreta per aconseguir `4,5`. Els moviments a la dreta corresponen a exponents negatius.

**Concepte avaluat:** Conversió de nombres estàndard a notació científica, interpretació de exponents positius i negatius.

---

### **Exercici 2** 🟦 (1.1 punts) – De Notació Científica a Forma Estàndard

**Enunciat:**

Converteix les següents notacions científiques a forma estàndard:

a) `3,2 × 10^4 = ?`

b) `7 × 10^2 = ?`

c) `5,6 × 10^-2 = ?`

d) `2,1 × 10^-4 = ?`

**Solució:**

a) `3,2 × 10^4 = 32.000`
   - Explicació: Es desplaça el decimal 4 llocs a l'esquerra: `3,2` → `32` → `320` → `3.200` → `32.000`.

b) `7 × 10^2 = 700`
   - Explicació: Es desplaça el decimal 2 llocs a l'esquerra: `7,0` → `70` → `700`.

c) `5,6 × 10^-2 = 0,056`
   - Explicació: Es desplaça el decimal 2 llocs a la dreta: `5,6` → `0,56` → `0,056`.

d) `2,1 × 10^-4 = 0,00021`
   - Explicació: Es desplaça el decimal 4 llocs a la dreta: `2,1` → `0,21` → `0,021` → `0,0021` → `0,00021`.

**Concepte avaluat:** Desplaçament del decimal usant exponents, interpretació de exponents negatius en números petits.

---

### **Exercici 3** ⭐ (0.9 punts) – Validació de Notació Científica

**Enunciat:**

Determina quines de les següents expressions estan en **notació científica correcta**. Si no és correcta, explica per què i corregeix-la:

a) `52 × 10^5`

b) `7,3 × 10^-3`

c) `0,8 × 10^6`

d) `1 × 10^0`

**Solució:**

a) `52 × 10^5` **NO és correcte**.
   - **Raó**: El coeficient `52` no està entre `1` i `10` (ha de ser `1 ≤ a < 10`).
   - **Correcció**: `52 × 10^5 = 5,2 × 10^6`
   - **Verificació**: `52 × 10^5 = 5.200.000 = 5,2 × 10^6` ✓

b) `7,3 × 10^-3` **SÍ és correcte**.
   - **Raó**: El coeficient `7,3` està entre `1` i `10`, i l'exponent és un enter.

c) `0,8 × 10^6` **NO és correcte**.
   - **Raó**: El coeficient `0,8` és menor que `1` (ha de ser `≥ 1`).
   - **Correcció**: `0,8 × 10^6 = 8 × 10^5`
   - **Verificació**: `0,8 × 10^6 = 800.000 = 8 × 10^5` ✓

d) `1 × 10^0` **SÍ és correcte** (technically valid, though often simplified).
   - **Raó**: El coeficient `1` està entre `1` i `10`, i `10^0 = 1`, per tant `1 × 10^0 = 1`.

**Concepte avaluat:** Criteris de notació científica válida, correcció d'errors comuns.

---

### **Exercici 4** 🟦 (1.2 punts) – Comparació de Nombres en Notació Científica

**Enunciat:**

Compara els següents nombres (en notació científica o estàndard) i ordena'ls de menor a major:

`3,5 × 10^3, 1,2 × 10^5, 4,2 × 10^2, 9,8 × 10^4, 5,1 × 10^3`

a) Converteix tots els nombres a forma estàndard (opcional, per a verificació).

b) Compara usant els exponents primer, després els coeficients si els exponents són iguals.

c) Escriu l'ordre de menor a major.

**Solució:**

a) Formes estàndard (per verificació):
   - `3,5 × 10^3 = 3.500`
   - `1,2 × 10^5 = 120.000`
   - `4,2 × 10^2 = 420`
   - `9,8 × 10^4 = 98.000`
   - `5,1 × 10^3 = 5.100`

b) Estratègia de comparació:
   - **Primer, comparar exponents:**
     - Exponent `2`: `4,2 × 10^2` (420)
     - Exponent `3`: `3,5 × 10^3` (3.500) i `5,1 × 10^3` (5.100)
     - Exponent `4`: `9,8 × 10^4` (98.000)
     - Exponent `5`: `1,2 × 10^5` (120.000)
   
   - **Per a números amb el mateix exponent:**
     - Entre `3,5 × 10^3` i `5,1 × 10^3`: `3,5 < 5,1`, per tant `3,5 × 10^3 < 5,1 × 10^3`.

c) Ordre de menor a major:
   
   `4,2 × 10^2 < 3,5 × 10^3 < 5,1 × 10^3 < 9,8 × 10^4 < 1,2 × 10^5`
   
   o en forma estàndard:
   
   `420 < 3.500 < 5.100 < 98.000 < 120.000`

**Concepte avaluat:** Comparació sistemàtica usant exponents, ordenació de números en notació científica.

---

### **Exercici 5** ⭐ (0.8 punts) – Aplicacions Reals: Astronomia

**Enunciat:**

La distància de la Terra al Sol és aproximadament `150.000.000 km`.

a) Expressa aquesta distància en notació científica.

b) La distància a Plutó és aproximadament `5.900.000.000 km`. Expressa-la en notació científica.

c) Compara les dues distàncies usant notació científica. Quants cops més lluny està Plutó?

**Solució:**

a) Distància a la Terra-Sol:
   ```
   150.000.000 km = 1,5 × 10^8 km
   ```
   
   Explicació: Es desplaça el decimal 8 llocs a l'esquerra: `150.000.000,0` → `1,5`.

b) Distància a Plutó:
   ```
   5.900.000.000 km = 5,9 × 10^9 km
   ```
   
   Explicació: Es desplaça el decimal 9 llocs a l'esquerra: `5.900.000.000,0` → `5,9`.

c) Comparació:
   - Terra-Sol: `1,5 × 10^8 km`
   - Plutó: `5,9 × 10^9 km`
   
   Quants cops més lluny:
   ```
   (5,9 × 10^9) / (1,5 × 10^8) = (5,9 / 1,5) × 10^(9-8) = 3,93 × 10^1 ≈ 39,3 vegades
   ```
   
   Per tant, **Plutó és aproximadament 39 vegades més lluny del Sol que la Terra**.

**Concepte avaluat:** Aplicacions reals de notació científica, comparació i divisió de nombres en notació científica.

---

### **Exercici 6** 🟦 (1.0 punt) – Multiplicació en Notació Científica

**Enunciat:**

Multiplica els següents nombres en notació científica:

a) `(2 × 10^3) × (3 × 10^2) = ?`

b) `(4,5 × 10^4) × (2 × 10^-2) = ?`

c) `(1,5 × 10^-3) × (2 × 10^5) = ?`

Per a cada un, aplica la regla: `(a × 10^m) × (b × 10^n) = (a × b) × 10^(m+n)`.

**Solució:**

a) `(2 × 10^3) × (3 × 10^2)`
   ```
   = (2 × 3) × 10^(3+2)
   = 6 × 10^5
   ```
   
   Verificació estàndard: `2.000 × 300 = 600.000 = 6 × 10^5` ✓

b) `(4,5 × 10^4) × (2 × 10^-2)`
   ```
   = (4,5 × 2) × 10^(4+(-2))
   = 9 × 10^2
   = 900
   ```
   
   Verificació: `45.000 × 0,02 = 900` ✓

c) `(1,5 × 10^-3) × (2 × 10^5)`
   ```
   = (1,5 × 2) × 10^(-3+5)
   = 3 × 10^2
   = 300
   ```
   
   Verificació: `0,0015 × 200.000 = 300` ✓

**Concepte avaluat:** Multiplicació de números en notació científica, ús de la regla de suma d'exponents.

---

### **Exercici 7** 🟦 (1.1 punts) – Divisió en Notació Científica

**Enunciat:**

Divideix els següents nombres en notació científica:

a) `(6 × 10^5) ÷ (2 × 10^2) = ?`

b) `(8,4 × 10^3) ÷ (3 × 10^-1) = ?`

c) `(5 × 10^-2) ÷ (2,5 × 10^3) = ?`

Per a cada un, aplica la regla: `(a × 10^m) ÷ (b × 10^n) = (a ÷ b) × 10^(m-n)`.

**Solució:**

a) `(6 × 10^5) ÷ (2 × 10^2)`
   ```
   = (6 ÷ 2) × 10^(5-2)
   = 3 × 10^3
   = 3.000
   ```
   
   Verificació: `600.000 ÷ 200 = 3.000` ✓

b) `(8,4 × 10^3) ÷ (3 × 10^-1)`
   ```
   = (8,4 ÷ 3) × 10^(3-(-1))
   = 2,8 × 10^4
   = 28.000
   ```
   
   Verificació: `8.400 ÷ 0,3 = 28.000` ✓

c) `(5 × 10^-2) ÷ (2,5 × 10^3)`
   ```
   = (5 ÷ 2,5) × 10^(-2-3)
   = 2 × 10^-5
   = 0,00002
   ```
   
   Verificació: `0,05 ÷ 2.500 = 0,00002` ✓

**Concepte avaluat:** Divisió de números en notació científica, ús de la regla de resta d'exponents.

---

### **Exercici 8** 🟦 (1.3 punts) – Notació Científica en Contexts Científics

**Enunciat:**

La massa d'un electró és aproximadament `9,11 × 10^-31 kg`. La massa d'un protó és aproximadament `1,67 × 10^-27 kg`.

a) Compara les dues masses: quina és més gran?

b) Calcula la **diferència** entre les dues masses usant notació científica.

c) Calcula la **proporció** (quants cops més massiu és el protó que l'electró).

d) Expressa les dues masses en forma estàndard (per a referència).

**Solució:**

a) Comparació:
   - Electró: `9,11 × 10^-31 kg` (exponent: -31)
   - Protó: `1,67 × 10^-27 kg` (exponent: -27)
   
   Ja que `-27 > -31`, el protó és **més massiu** (els exponents més grans corresponen a nombres més grans).

b) Diferència:
   
   Per restar, hem de expressar ambdós amb el mateix exponent:
   ```
   1,67 × 10^-27 - 9,11 × 10^-31
   = 1,67 × 10^-27 - 0,000911 × 10^-27
   = (1,67 - 0,000911) × 10^-27
   = 1,669089 × 10^-27 kg
   ≈ 1,67 × 10^-27 kg (la diferència és negligible comparada amb la massa del protó)
   ```

c) Proporció (protó/electró):
   ```
   (1,67 × 10^-27) ÷ (9,11 × 10^-31)
   = (1,67 ÷ 9,11) × 10^(-27-(-31))
   = 0,1833 × 10^4
   = 1,833 × 10^3
   ≈ 1.833 vegades (el protó és aproximadament 1.833 vegades més massiu)
   ```

d) Forma estàndard (per a referència):
   - Electró: `0,000000000000000000000000000000911 kg` (massa molt, molt petita)
   - Protó: `0,00000000000000000000000000167 kg` (també molt petita, però més gran que l'electró)

**Concepte avaluat:** Aplicacions científiques, comparació i operacions amb notació científica en contextos reals.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Conversió i Operacions Múltiples

**Enunciat:**

Un laboratori mesura les següents quantitats:
- Mostra A: `4.500.000.000 molècules`
- Mostra B: `3,2 × 10^10 molècules`
- Mostra C: `1,8 × 10^9 molècules`

a) Expressa totes les mostres en notació científica (si no ho estan ja).

b) Ordena les mostres de menor a major nombre de molècules.

c) Calcula el total de molècules (sumant totes tres mostres). Expressa el resultat en notació científica.

d) Quin és el percentatge de molècules de la Mostra A respecte al total? (Pista: `(Mostra A / Total) × 100%`)

**Solució:**

a) Notació científica:
   - Mostra A: `4.500.000.000 = 4,5 × 10^9`
   - Mostra B: `3,2 × 10^10` (ja en notació científica)
   - Mostra C: `1,8 × 10^9` (ja en notació científica)

b) Ordre de menor a major:
   
   Comparant exponents primero:
   - Exponent `9`: Mostra A (`4,5 × 10^9`) i Mostra C (`1,8 × 10^9`)
   - Exponent `10`: Mostra B (`3,2 × 10^10`)
   
   Entre A i C (ambdós amb exponent 9): `1,8 < 4,5`, per tant C < A.
   
   **Ordre: Mostra C < Mostra A < Mostra B**
   
   o `1,8 × 10^9 < 4,5 × 10^9 < 3,2 × 10^10`

c) Total de molècules:
   ```
   Total = 4,5 × 10^9 + 3,2 × 10^10 + 1,8 × 10^9
         = 4,5 × 10^9 + 32 × 10^9 + 1,8 × 10^9
         = (4,5 + 32 + 1,8) × 10^9
         = 38,3 × 10^9
         = 3,83 × 10^10 molècules
   ```

d) Percentatge de la Mostra A:
   ```
   (Mostra A / Total) × 100%
   = (4,5 × 10^9) / (3,83 × 10^10) × 100%
   = (4,5 / 38,3) × 10^(9-10) × 100%
   = 0,1175 × 10^-1 × 100%
   = 0,01175 × 100%
   = 1,175%
   ≈ 1,18%
   ```
   
   Per tant, la Mostra A representa aproximadament **1,18%** del total.

**Concepte avaluat:** Conversió múltiple, comparació, suma i divisió de números en notació científica, càlculs de percentatge.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Relació entre Notació Científica i Valor Posicional

**Enunciat:**

La notació científica `a × 10^n` és una generalització del **valor posicional** estudiat en el Bloc 4.

a) Explica com la notació científica relaciona-se amb les potències de 10 usades en valor posicional. (Pista: Pensa en com `10^3`, `10^2`, `10^1`, `10^0` apareixien en forma desenvolupada.)

b) Donat el nombre `56.789`, expressa'l en forma desenvolupada (Bloc 4) i després en notació científica (Bloc 5).

c) Compara els dos formats:
   - Forma desenvolupada: Cada dígit × 10^(posició)
   - Notació científica: (coeficient) × 10^(exponent global)

d) Per què és útil la notació científica quan els números són molt grans o molt petits (comparats amb la forma desenvolupada)?

**Solució:**

a) Relació entre valor posicional i notació científica:
   
   **Valor posicional** escriu un nombre com a suma:
   ```
   5.234 = 5 × 10^3 + 2 × 10^2 + 3 × 10^1 + 4 × 10^0
   ```
   
   **Notació científica** expressa el mateix nombre com a producte:
   ```
   5.234 = 5,234 × 10^3
   ```
   
   La notació científica **compacta** les múltiples potències de 10 en una sola potència de 10 (l'exponent més gran), movent el coeficient.

b) Per al nombre `56.789`:
   
   **Forma desenvolupada:**
   ```
   56.789 = 5 × 10^4 + 6 × 10^3 + 7 × 10^2 + 8 × 10^1 + 9 × 10^0
   ```
   
   **Notació científica:**
   ```
   56.789 = 5,6789 × 10^4
   ```

c) Comparació:
   
   | Aspecte | Forma Desenvolupada | Notació Científica |
   |---------|---------------------|-------------------|
   | **Propòsit** | Veure el valor de cada dígit | Representar números molt grans/petits compactament |
   | **Estructura** | Suma de termes | Producte d'un coeficient i una potència de 10 |
   | **Exponents** | Múltiples (un per cada dígit) | Un exponent global |
   | **Exemple** | `5×10^4 + 6×10^3 + 7×10^2 + 8×10^1 + 9×10^0` | `5,6789 × 10^4` |
   | **Ús** | Educació sobre valor posicional | Ciència, enginyeria, números extrems |

d) Utilitat de la notació científica:
   
   - **Números molt grans**: En lloc de escriure `5.200.000.000.000.000.000.000.000.000`, escrivim `5,2 × 10^27` (molt més compacte i llegible).
   
   - **Números molt petits**: En lloc de escriure `0,000000000000000000000000000000911`, escrivim `9,11 × 10^-31` (molt més fàcil de manejar).
   
   - **Operacions amb calculadora**: Els exponents es sumen o resten, simplificant les multiplicacions i divisions.
   
   - **Comparació ràpida**: Els exponents revelen la magnitud relativa ràpidament (e.g., `10^27` és molt més gran que `10^-31`).
   
   - **Precisió científica**: La notació científica mostra clarament quants dígits significatius té una mesura (e.g., `5,2 × 10^27` suggereix 2 dígits significatius).

**Concepte avaluat:** Connexió entre valor posicional i notació científica, comprensió de l'abstracció que representa la notació científica, aplicacions comparatives.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Conversió estàndard → notació científica | Moderat |
| 2 | Conversió notació científica → estàndard | Moderat |
| 3 | Validació de notació científica correcta | Moderat |
| 4 | Comparació en notació científica | Intermedi |
| 5 | Aplicacions reals (astronomia) | Moderat |
| 6 | Multiplicació en notació científica | Intermedi |
| 7 | Divisió en notació científica | Intermedi |
| 8 | Operacions en contextos científics | Intermedi |
| 9 | Conversions múltiples i operacions complexes | Desafiador |
| 10 | Relació amb valor posicional i utilitat | Desafiador |

---

## 🎯 Consells per als Estudiants

- **Exercicis 1–3, 5**: Practica conversions bàsiques entre formes estàndard i notació científica.
- **Exercicis 4, 6–8**: Aprofundiu en operacions (multiplicació, divisió) i comparacions en notació científica.
- **Exercicis 9–10**: Consolideu amb problemes multietapa i connexions conceptuals amb valor posicional.

---

## ⚠️ Trampes Conceptuals Comunes

1. **Invertir el signe de l'exponent**: `10^-3` significa "molt petit" (0,001), no "molt gran".
2. **Oblidar ajustar l'exponent al desplaçar el decimal**: Si mous el decimal a l'esquerra, incrementa l'exponent; si ho fas a la dreta, la decrementa.
3. **Coeficient no vàlid**: El coeficient `a` ha de satisfer `1 ≤ |a| < 10`. `52 × 10^5` és invàlid; ha de ser `5,2 × 10^6`.
4. **Confondre regles d'exponents**: En multiplicació, **suma** els exponents: `10^a × 10^b = 10^(a+b)`. En divisió, **resta**: `10^a / 10^b = 10^(a-b)`.
5. **Negligir els dígits significatius**: La notació científica `3,00 × 10^2` implica 3 dígits significatius, mentre que `3 × 10^2` pot implicar només 1.

---

## 🔗 Connexions amb altres Blocs

- **Bloc 4 (Valor Posicional)**: La notació científica és una extensió compacta de valor posicional.
- **Mòdul 2 (Operacions Bàsiques)**: Les regles de suma d'exponents simplifica multiplicacions.
- **Mòdul 6 (Potències i Exponents)**: Connexió directa a través de les lleis dels exponents.
- **Mòdul 8 (Escales i Mesures)**: Ús extens de notació científica en dades científiques i astronòmiques.


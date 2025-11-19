# Exercicis - Mòdul 1: Bloc 7 – Nombres Primers/Compostos i Garbell d'Eratòstenes

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Classificació de Primers i Compostos

**Enunciat:**

Classifica els següents nombres com a primers, compostos, o ni l'un ni l'altre:

`2, 1, 17, 24, 29, 35, 40, 43`

**Solució:**

| Nombre | Classificació | Justificació |
|--------|---|---|
| 2 | Primer | Exactament 2 divisors: 1, 2 (l'únic primer parell) |
| 1 | Cap | No és primer ni compost per definició |
| 17 | Primer | Exactament 2 divisors: 1, 17 |
| 24 | Compost | Divisors: 1, 2, 3, 4, 6, 8, 12, 24 |
| 29 | Primer | Exactament 2 divisors: 1, 29 |
| 35 | Compost | 35 = 5 × 7 (divisors: 1, 5, 7, 35) |
| 40 | Compost | 40 = 2^3 × 5 (múltiples divisors) |
| 43 | Primer | Exactament 2 divisors: 1, 43 |

**Concepte avaluat:** Identificació de primers vs. compostos, comprensió de definicions.

---

### **Exercici 2** 🟦 (1.1 punts) – Garbell d'Eratòstenes (fins a 50)

**Enunciat:**

Usa el Garbell d'Eratòstenes per trobar tots els nombres primers fins a 50.

a) Llista els nombres 2 a 50.

b) Segueix l'algoritme:
   - Comença amb 2 (primer).
   - Marca tots els múltiples de 2 (excepte 2).
   - Passa al següent número no marcat (3).
   - Marca tots els múltiples de 3 (excepte 3).
   - Continua fins que només quedin primers.

c) Llista tots els primers trobats.

**Solució:**

a) Nombres 2–50 (inicials):
```
2  3  4  5  6  7  8  9  10
11 12 13 14 15 16 17 18 19 20
21 22 23 24 25 26 27 28 29 30
31 32 33 34 35 36 37 38 39 40
41 42 43 44 45 46 47 48 49 50
```

b) Aplicació del garbell:

**Pas 1 - Marcar múltiples de 2:**
```
2  3  X  5  X  7  X  9  X
11 X 13  X 15  X 17  X 19  X
21 X 23  X 25  X 27  X 29  X
31 X 33  X 35  X 37  X 39  X
41 X 43  X 45  X 47  X 49  X
```

**Pas 2 - Marcar múltiples de 3 (no marcat):**
```
2  3  X  5  X  7  X  X  X
11 X 13  X X  X 17  X 19  X
X  X 23  X 25  X X  X 29  X
31 X X  X 35  X 37  X X  X
41 X 43  X X  X 47  X 49  X
```

**Pas 3 - Marcar múltiples de 5:**
```
2  3  X  5  X  7  X  X  X
11 X 13  X X  X 17  X 19  X
X  X 23  X X  X X  X 29  X
31 X X  X X  X 37  X X  X
41 X 43  X X  X 47  X 49  X
```

**Pas 4 - Marcar múltiples de 7:**
```
2  3  X  5  X  7  X  X  X
11 X 13  X X  X 17  X 19  X
X  X 23  X X  X X  X 29  X
31 X X  X X  X 37  X X  X
41 X 43  X X  X 47  X X  X
```

c) **Primers fins a 50:**
```
2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47
```

**Concepte avaluat:** Implementació del Garbell d'Eratòstenes, identificació de primers per eliminació sistemàtica.

---

### **Exercici 3** ⭐ (0.9 punts) – Prova de Primalitat Bàsica

**Enunciat:**

Determina si els següents nombres són primers o compostos verificant divisibilitat fins a $\sqrt{n}$:

a) `49`
b) `67`
c) `91`

(Pista: Si `n` té un divisor, ha de tenir un divisor `d ≤ √n`.)

**Solució:**

a) **`49`**: $\sqrt{49} = 7$
   - Verifica divisibilitat per 2, 3, 5, 7:
     - `49 ÷ 2 = 24,5` ✗
     - `49 ÷ 3 = 16,33...` ✗
     - `49 ÷ 5 = 9,8` ✗
     - `49 ÷ 7 = 7` ✓
   - **Compost** (`49 = 7 × 7`)

b) **`67`**: $\sqrt{67} \approx 8,2$
   - Verifica divisibilitat per 2, 3, 5, 7:
     - `67 ÷ 2 = 33,5` ✗
     - `67 ÷ 3 = 22,33...` ✗
     - `67 ÷ 5 = 13,4` ✗
     - `67 ÷ 7 = 9,57...` ✗
   - **Primer** (sense divisors fins a $\sqrt{67}$)

c) **`91`**: $\sqrt{91} \approx 9,5$
   - Verifica divisibilitat per 2, 3, 5, 7:
     - `91 ÷ 2 = 45,5` ✗
     - `91 ÷ 3 = 30,33...` ✗
     - `91 ÷ 5 = 18,2` ✗
     - `91 ÷ 7 = 13` ✓
   - **Compost** (`91 = 7 × 13`)

**Concepte avaluat:** Prova de primalitat eficient usant límit de $\sqrt{n}$, verificació sistemàtica.

---

### **Exercici 4** 🟦 (1.2 punts) – Factorització i Arbre de Factors

**Enunciat:**

Crea arbres de factors per als següents nombres:

a) `30`
b) `60`
c) `84`

Per a cada un, identifica la factorització prima completa.

**Solució:**

a) **Arbre de factors per a 30:**
```
      30
     /  \
    2   15
       /  \
      3    5
      
Factorització: 30 = 2 × 3 × 5
```

b) **Arbre de factors per a 60:**
```
      60
     /  \
    2   30
       /  \
      2   15
         /  \
        3    5

Factorització: 60 = 2² × 3 × 5
```

c) **Arbre de factors per a 84:**
```
      84
     /  \
    2   42
       /  \
      2   21
         /  \
        3    7

Factorització: 84 = 2² × 3 × 7
```

**Concepte avaluat:** Construcció d'arbres de factors, factorització prima completa.

---

### **Exercici 5** ⭐ (0.8 punts) – Teorema Fonamental de l'Aritmètica

**Enunciat:**

Segons el Teorema Fonamental de l'Aritmètica, cada nombre compost té una factorització prima **única** (fins a l'ordre).

Verifica que les següents factoritzacions són correctes i completes:

a) `48 = 2^4 × 3`

b) `72 = 2^3 × 3^2`

c) `100 = 2^2 × 5^2`

**Solució:**

a) `48 = 2^4 × 3`:
   - Calcula: `2^4 × 3 = 16 × 3 = 48` ✓
   - Tots els factors són primers ✓
   - Factorització completa

b) `72 = 2^3 × 3^2`:
   - Calcula: `2^3 × 3^2 = 8 × 9 = 72` ✓
   - Tots els factors són primers ✓
   - Factorització completa

c) `100 = 2^2 × 5^2`:
   - Calcula: `2^2 × 5^2 = 4 × 25 = 100` ✓
   - Tots els factors són primers ✓
   - Factorització completa

**Concepte avaluat:** Aplicació del Teorema Fonamental, verificació de factoritzacions úniques.

---

### **Exercici 6** 🟦 (1.0 punt) – Propietats de Primers

**Enunciat:**

Respon les següents preguntes sobre propietats de primers:

a) Per què és `2` l'únic primer parell?

b) Si `p` és primer i `p | (a × b)`, aleshores `p | a` o `p | b` (Lema de d'Euclides). Verifica amb exemple: `7 | 35` i `35 = 5 × 7`.

c) Llista els 5 primers primes més grans que `50`.

**Solució:**

a) **Per què 2 és l'únic primer parell:**
   - Qualsevol altre nombre parell `2k` (amb `k > 1`) té almenys 3 divisors: `1, 2, 2k`.
   - Per tant, no són primers.
   - `2` és l'excepció perquè els seus únics divisors són `1` i `2`.

b) **Verificació del Lema de d'Euclides:**
   - `7 | 35` (perquè `35 = 7 × 5`)
   - `35 = 5 × 7`
   - Es compleix `7 | (5 × 7)` i `7 | 7` ✓
   - Per tant, `7 | a` o `7 | b` es verifica.

c) **Primers més grans que 50:**
   - `53, 59, 61, 67, 71`

**Concepte avaluat:** Propietats estructurals de primers, Lema de d'Euclides, identificació de primers.

---

### **Exercici 7** 🟦 (1.1 punts) – Tipus de Nombres Especials

**Enunciat:**

Classifica els següents nombres segons tipus especial (si aplicable):

| Nombre | Primer? | Compost? | Perfecte? | Gemells Primers? |
|--------|---------|----------|-----------|-----------------|
| 6 | ? | ? | ? (6 = 1+2+3) | ? |
| 11 | ? | ? | ? | ? |
| 13 | ? | ? | ? | ? |
| 28 | ? | ? | ? (28 = 1+2+4+7+14) | ? |

(Recorda: Un nombre **perfecte** és igual a la suma dels seus divisors propis. **Gemells primers** són parells de primers que difereixen en 2, com 11 i 13.)

**Solució:**

| Nombre | Primer? | Compost? | Perfecte? | Gemells Primers? |
|--------|---------|----------|-----------|-----------------|
| 6 | ✗ | ✓ | ✓ (6 = 1+2+3) | — |
| 11 | ✓ | ✗ | ✗ | ✓ (11, 13 són gemells) |
| 13 | ✓ | ✗ | ✗ | ✓ (11, 13 són gemells) |
| 28 | ✗ | ✓ | ✓ (28 = 1+2+4+7+14) | — |

**Concepte avaluat:** Classificacions especials (perfectes, gemells primers), tipus de nombres.

---

### **Exercici 8** 🟦 (1.3 punts) – Aplicació: Xifres de Seguretat (RSA bàsic)

**Enunciat:**

En criptografia RSA, la seguretat es basa en el fet que factoritzar nombres grans és difícil.

a) Donats dos primers `p = 11` i `q = 13`, calcula `n = p × q`.

b) Verifica que `n` és compost.

c) Estima quant de temps trigaría a un ordinador a factoritzar `n` usant força bruta. (Pista: Compara amb números reals de 300+ dígits.)

d) Per què és important que `p` i `q` siguin primers grans en criptografia?

**Solució:**

a) `n = 11 × 13 = 143`

b) Verificació que `143` és compost:
   - `143 ÷ 11 = 13` ✓
   - `143` té almenys 3 divisors: `1, 11, 13, 143`.
   - **`143` és compost.**

c) Estimació de temps de factorització:
   - Per a `n = 143`, pot facto vaja verificant divisors fins a $\sqrt{143} \approx 12$. Takes ~12 operacions.
   - Per a nombres reals de 300 dígits, factoritzar requereix algoritmes avançats i anys de computació.
   - **Conclusió:** Per a números petits és trivial; per a números grans és computacionalment infeasible amb tecnologia actual.

d) **Importància de primers grans:**
   - Si `p` i `q` són petits, `n = pq` es factoritza ràpidament.
   - Si `p` i `q` són grans (200+ dígits), `n` (400+ dígits) és pràcticament impossible de factoritzar.
   - RSA depèn de aquesta asimetria: fàcil de multiplicar primers, difícil de factoritzar resultats.

**Concepte avaluat:** Aplicacions de primers en criptografia, comprensió de complexitat computacional.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Distribució de Primers

**Enunciat:**

Els primers es distribueixen de manera irregular. Analitza el gap (distància) entre primers consecutius.

a) Llista tots els primers fins a 100 usant el Garbell d'Eratòstenes.

b) Calcula la diferència entre cada parell de primers consecutius:
   - Gap entre 2 i 3: 1
   - Gap entre 3 i 5: 2
   - ... (continua)

c) Quin és el gap més gran que observes? A quin punt ocorre?

d) Predicció: Creus que els gaps augmenten a mesura que els nombres es fan més grans? Per què o per què no?

**Solució:**

a) **Primers fins a 100:**
```
2, 3, 5, 7, 11, 13, 17, 19, 23, 29, 31, 37, 41, 43, 47, 53, 59, 61, 67, 71, 73, 79, 83, 89, 97
```

b) **Gaps entre primers consecutius:**

| Primers | Gap |
|---------|-----|
| 2 → 3 | 1 |
| 3 → 5 | 2 |
| 5 → 7 | 2 |
| 7 → 11 | 4 |
| 11 → 13 | 2 |
| 13 → 17 | 4 |
| 17 → 19 | 2 |
| 19 → 23 | 4 |
| 23 → 29 | 6 |
| 29 → 31 | 2 |
| 31 → 37 | 6 |
| 37 → 41 | 4 |
| 41 → 43 | 2 |
| 43 → 47 | 4 |
| 47 → 53 | 6 |
| 53 → 59 | 6 |
| 59 → 61 | 2 |
| 61 → 67 | 6 |
| 67 → 71 | 4 |
| 71 → 73 | 2 |
| 73 → 79 | 6 |
| 79 → 83 | 4 |
| 83 → 89 | 6 |
| 89 → 97 | 8 |

c) **Gap més gran (fins a 100):**
   - **Gap de 8** entre `89` i `97`.

d) **Predicció sobre creixement de gaps:**
   - Sí, els gaps generalment augmenten amb números més grans.
   - Raonament: A mesura que els nombres creixen, els primers es fan més escassos (per resultat del Teorema dels Nombres Primers).
   - Entre nombres més grans hi ha més "espai" i, per tant, més oportunitats que no siguin primers.
   - Però els gaps no creixen regularment; oscil·len.

**Concepte avaluat:** Análisis de distribució de primers, observació de patrons, predicció estadística.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Conjectura de Goldbach

**Enunciat:**

La **Conjectura de Goldbach** (1742) afirma que cada nombre parell més gran que 2 pot escriure's com suma de dos primers. Encara no s'ha provat, però es verifica per números grans.

a) Verifica la conjectura per als següents nombres parells:
   - `10 = ? + ?`
   - `20 = ? + ?`
   - `30 = ? + ?`

b) Per a cadascun, llista **totes** les representacions com suma de dos primers.

c) Observa: Hi ha cap nombre parell entre 2 i 100 que **no** satisfaci la conjectura?

d) Per què crees que aquesta conjectura és tan difícil de provar completament?

**Solució:**

a) **Verificació per a nombres parells:**

- **10:**
  - Primers menors de 10: 2, 3, 5, 7
  - `10 = 5 + 5` (5 és primer) ✓
  - `10 = 3 + 7` (3 i 7 són primers) ✓

- **20:**
  - Primers menors de 20: 2, 3, 5, 7, 11, 13, 17, 19
  - `20 = 3 + 17` ✓
  - `20 = 7 + 13` ✓
  - `20 = 19 + 1` (1 no és primer) ✗

- **30:**
  - Primers menors de 30: 2, 3, 5, 7, 11, 13, 17, 19, 23, 29
  - `30 = 7 + 23` ✓
  - `30 = 11 + 19` ✓
  - `30 = 13 + 17` ✓

b) **Totes les representacions:**

| Nombre Parell | Representacions com suma de dos primers |
|---|---|
| 10 | 3+7, 5+5 |
| 20 | 3+17, 7+13 |
| 30 | 7+23, 11+19, 13+17 |

c) **Observació (2–100):**
   - Verificant tots els nombres parells 2–100, **cadascun** pot representar-se com suma de dos primers.
   - **Cap excepció observada.**

d) **Per què és difícil provar completament:**
   - Hi ha **infinits** nombres parells.
   - No podem verificar-los tots manualment.
   - Requereix una prova matemàtica general que funcioni per a **qualsevol** nombre parell.
   - Els investigadors han verificat la conjectura fins a números gigantescos, però cap demostració universal.

**Concepte avaluat:** Exploració de conjectures obertes, raonament sobre infinit, limitacions de verificació empírica.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepte Principal | Nivell |
|----------|-------------------|--------|
| 1 | Classificació primers/compostos | Moderat |
| 2 | Garbell d'Eratòstenes | Intermedi |
| 3 | Prova de primalitat per $\sqrt{n}$ | Moderat |
| 4 | Arbres de factors, factorització | Intermedi |
| 5 | Teorema Fonamental de l'Aritmètica | Moderat |
| 6 | Propietats de primers | Intermedi |
| 7 | Nombres especials (perfectes, gemells) | Intermedi |
| 8 | Aplicació: Criptografia RSA | Intermedi |
| 9 | Distribució de primers, gaps | Desafiador |
| 10 | Conjectura de Goldbach | Desafiador |

---

## ⚠️ Trampes Conceptuals Comunes

1. **Pensar que 1 és primer**: 1 té només un divisor (ell mateix), per tant **no és primer ni compost**.
2. **Negligir 2 com a primer**: És l'únic primer parell.
3. **Confondre garbell amb factorització**: El garbell identifica primers; la factorització descompon en primers.
4. **Oblidar la unicitat de factorització**: Només hi ha una forma de descompondre un nombre en primers (fins a l'ordre).


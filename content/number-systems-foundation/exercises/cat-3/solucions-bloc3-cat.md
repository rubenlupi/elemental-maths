# Solucions Bloc 3 – Jerarquia de Conjunts de Nombres ℕ→ℤ→ℚ

---

## 📌 Part 1: Identificar Conjunts

### 1.1 Nombres Simples

| Nombre | Pertany a ℕ? | Pertany a ℤ? | Pertany a ℚ? | Resposta Final |
|--------|--------------|--------------|--------------|----------------|
| 7 | ✓ | ✓ | ✓ | ℕ, ℤ, ℚ (tot natural és enter és racional) |
| -3 | ✗ | ✓ | ✓ | ℤ, ℚ (enter però no natural) |
| 0 | ? | ✓ | ✓ | ℤ, ℚ (enter; 0 pot estar en ℕ depenent de convenció) |
| 15 | ✓ | ✓ | ✓ | ℕ, ℤ, ℚ |
| -8 | ✗ | ✓ | ✓ | ℤ, ℚ (enter negatiu) |
| 1 | ✓ | ✓ | ✓ | ℕ, ℤ, ℚ |

**Nota:** Per a 0, alguns matemàtics inclouen 0 en ℕ, altres no. Acceptem ambdós: `ℤ, ℚ` o `ℕ, ℤ, ℚ`.

---

### 1.2 Fraccions

| Nombre | Pertany a ℕ? | Pertany a ℤ? | Pertany a ℚ? | Resposta Final |
|--------|--------------|--------------|--------------|----------------|
| 1/2 | ✗ | ✗ | ✓ | ℚ (racional, no és enter) |
| 3/4 | ✗ | ✗ | ✓ | ℚ |
| 5/1 | ✓ | ✓ | ✓ | ℕ, ℤ, ℚ (5/1 = 5) |
| -1/2 | ✗ | ✗ | ✓ | ℚ (racional negatiu, no és enter) |
| 2/3 | ✗ | ✗ | ✓ | ℚ |
| 10/5 | ✓ | ✓ | ✓ | ℕ, ℤ, ℚ (10/5 = 2) |

**Clau:** Una fracció `a/b` pertany a ℕ o ℤ NOMÉS si resulta en un nombre sencer (sense part fraccionaria).

---

## 📌 Part 2: Escriu com a Fracció

| Nombre | Fracció |
|--------|---------|
| 5 | **5/1** |
| -2 | **-2/1** |
| 0 | **0/1** |
| 12 | **12/1** |
| -7 | **-7/1** |
| 1 | **1/1** |

**Nota:** Tot nombre enter `n` pot escribirse com `n/1`.

---

## 📌 Part 3: Jerarquia de Conjunts

### 3.1 Completa amb ⊂ o ⊄

| Afirmació | Símbol | Correcte? | Explicació |
|-----------|--------|-----------|-----------|
| ℕ ___ ℤ | **⊂** | ✓ | Tot natural és enter |
| ℤ ___ ℚ | **⊂** | ✓ | Tot enter és racional (n = n/1) |
| ℕ ___ ℚ | **⊂** | ✓ | Transitivitat: ℕ ⊂ ℤ ⊂ ℚ |
| ℚ ___ ℕ | **⊄** | ✓ | No tots els racionals són naturals (Ex: 1/2) |
| ℤ ___ ℕ | **⊄** | ✓ | No tots els enters són naturals (Ex: -3) |

---

### 3.2 Vertader o Fals?

| Afirmació | V/F? | Explicació |
|-----------|------|-----------|
| Tot nombre natural és enter | **V** | Per definició, ℕ ⊂ ℤ |
| Tot nombre enter és natural | **F** | Contraexemple: -2 és enter però no natural |
| Tot nombre enter és racional | **V** | Tot enter n es pot escribir com n/1 |
| Tot nombre natural és racional | **V** | Transitivitat: si n ∈ ℕ, aleshores n ∈ ℤ, aleshores n ∈ ℚ |
| Tot nombre racional és enter | **F** | Contraexemple: 1/2 és racional però no enter |
| Existeix un nombre que pertany a ℤ però no a ℕ | **V** | Exemple: -5, 0 (depenent de la convenció), -100 |

---

## 📌 Part 4: Aplicacions Reals

### 4.1 Classifica cada situació

| Situació | Conjunt | Per què? |
|----------|---------|---------|
| Nombre de persones en una sala | **ℕ** | Els recomptes són sempre naturals (enters positius) |
| Temperatura en graus | **ℤ** | La temperatura pot ser negativa (sota zero) |
| Altitud respecte el nivell del mar | **ℤ** | Altitud pot ser negativa (sota el nivell del mar, com en mines) |
| Preu d'un producte | **ℚ** | Els preus solen tenir decimals (€10.99, €5.50) |
| Puntuació en un joc | **ℤ** | La puntuació pot ser negativa en alguns jocs |
| Massa d'un aliment | **ℚ** | La massa pot ser fraccionada (250g = 1/4 kg, 0.5 kg) |
| Nivell d'un dipòsit (pot estar buit/ple) | **ℚ** | El nivell és una fracció (50%, 1/3 ple) |

---

### 4.2 Recomptes vs Mesures

**ℕ (Recomptes naturals):**
- Nombre de nenes en la classe
- Número de gols en un partit

**ℤ (Incloent negatius):**
- Profunditat d'un pou (sous zeros)
- Canvi de saldo en un compte

**ℚ (Mesures precises/fraccions):**
- Fracció de pa menjada
- Temps en hores i mitges
- Talla d'una samarreta (pot ser XS, M, L, o 34, 36, 38—nombres enters o racionals)
- Dosificació de medicina (0.5 mg, 1/4 comprimé)

**Alternativa:** Els últims items del ℚ podrien estar en ℕ si considerem talls estàndard (XS, M, L) o dosis discretes.

---

## 📌 Part 5: Ordre i Jerarquia

### 5.1 Ordena de menor a major

Ordena: `3, -1, 1/2, -2, 5/4, 0`

**Conversió a decimals para facilitat:**
- 3 = 3.0
- -1 = -1.0
- 1/2 = 0.5
- -2 = -2.0
- 5/4 = 1.25
- 0 = 0.0

**Ordenat de menor a major:**
**-2 < -1 < 0 < 1/2 < 5/4 < 3**

---

### 5.2 Quin nombre em falta?

**Recorda:** ℕ ⊂ ℤ ⊂ ℚ

- Posa un exemple de nombre que és ℕ però no ℚ: **NO EXISTE!** (Tot ℕ ⊆ ℚ)
  - *Nota:* Pregunta trampa; la resposta correcta és que no hi ha tal nombre, ja que ℕ ⊂ ℚ.
  - Si l'estudiant respongués, podria marcar com a incorrecte o acceptar qualsevol nombre de ℕ amb la nota que "pertany a ℚ".

- Posa un exemple de nombre que és ℤ però no ℕ: **-5, -10, -1, 0** (enters negatius)

- Posa un exemple de nombre que és ℚ però no ℤ: **1/2, 3/4, -2/3, 0.5** (fraccions no-enters)

- Posa un exemple de nombre que no és ℚ: **π, √2, e, φ** (nombres irracionals)
  - Per a aquesta edat, π és el més familiar.

---

## 📌 Part 6: Operacions dins de Conjunts

### 6.1 Sumar dins de Conjunts

| Suma | Resultat | Conjunt(s) |
|------|----------|-----------|
| 3 + 5 | **8** | ℕ, ℤ, ℚ |
| -2 + -3 | **-5** | ℤ, ℚ (enter negatiu) |
| 1/2 + 1/4 | **3/4** | ℚ (racional) |
| 5 + (-5) | **0** | ℤ, ℚ (enter zero; 0 pot estar a ℕ) |
| 2/3 + 1/3 | **1** | ℕ, ℤ, ℚ (resulta en enter) |
| -1 + 4 | **3** | ℕ, ℤ, ℚ |

**Observació:** Si sumes dos nombres del mateix conjunt, el resultat sovint pertany a aquest conjunt, excepte quan es tracta de ℕ (ja que -2 + -3 = -5 no és natural).

---

### 6.2 Restar dins de Conjunts

| Resta | Resultat | Conjunt(s) |
|-------|----------|-----------|
| 5 - 3 | **2** | ℕ, ℤ, ℚ |
| 3 - 5 | **-2** | ℤ, ℚ (enter negatiu) |
| -2 - 3 | **-5** | ℤ, ℚ |
| 1/2 - 1/4 | **1/4** | ℚ |
| 0 - 7 | **-7** | ℤ, ℚ |

**Observació:** La resta de dos naturals NO sempre és natural (3 - 5 = -2), però la resta de dos enters sempre és enter. La resta de dos racionals sempre és racional.

---

## 📌 Part 7: Repte — Problemes de Lògica

### 7.1 Pensa Lògicament

**Problema 1:** Posa un nombre entre `1/3` i `1/2`.

**Solució:**
- Converte a decimals: 1/3 ≈ 0.333..., 1/2 = 0.5
- Punt mitjà: (1/3 + 1/2) / 2 = (2/6 + 3/6) / 2 = (5/6) / 2 = 5/12
- Verificació: 5/12 ≈ 0.4166..., que està entre 0.333... i 0.5 ✓

**Respostes vàlides:** 5/12, 7/20, 0.4, 0.45, etc.

---

**Problema 2:** Si `a ∈ ℕ` i `b ∈ ℕ`, aleshores `a - b` sempre pertany a ℕ?

**Solució:** **NO**

**Contraexemple:** a = 2, b = 5. Aleshores a - b = 2 - 5 = -3, que NO pertany a ℕ.

**Conclusió:** La resta de dos naturals pot ser negativa, el qual no pertany a ℕ. Per tant, ℕ NO és tancat sob la resta.

---

**Problema 3:** Ordena de la més restrictiu a la més general:
- ℕ, ℤ, ℚ, enters negatius

**Solució:**
1. **Enters negatius** (subconjunt de ℤ, ex: {-1, -2, -3, ...})
2. **ℕ** (naturals, ex: {1, 2, 3, ...})
3. **ℤ** (enters: combines ℕ i enters negatius + 0)
4. **ℚ** (racionals: includes tots els enters més fraccions)

**Ordre:** Enters negatius ⊂ ℕ (parcial overlap) ⊂ ℤ ⊂ ℚ

*Nota:* Enters negatius i ℕ no estan en relació de subconjunt; ambdós estan dins de ℤ.

---

### 7.2 Crea una Taula Pròpia (Exemple de Resposta)

| Nombre | ℕ? | ℤ? | ℚ? |
|--------|----|----|-----|
| 10 | ✓ | ✓ | ✓ |
| -4 | ✗ | ✓ | ✓ |
| 2/5 | ✗ | ✗ | ✓ |
| 0 | ? | ✓ | ✓ |
| -3/2 | ✗ | ✗ | ✓ |

*(Les respostes variaran segons l'estudiant. L'important és que siguin lògiques.)*

---

## 📌 Part 8: Reflexió Final

### 8.1 Resposta Curta

**1. Per què necessitem els enters (ℤ) si ja tenim els naturals (ℕ)?**

**Resposta:** Els enters permeten representar situacions on els valors poden ser negatius, com temperatures sota zero, deutes o altituds sous el nivell del mar. Els naturals només cobreixen els positius i el zero (en alguns casos).

---

**2. Per què necessitem els racionals (ℚ) si ja tenim els enters (ℤ)?**

**Resposta:** Els racionals permeten representar parts de coses (fraccions), com 1/2 de pizza, 3/4 de litro, o preus amb decimals (€5.50). Els enters només cobreixen els sencers.

---

**3. Pot existir un nombre que no sigui ℚ?**

**Resposta:** **SÍ!** Els nombres irracionals NO es poden escribir com a fracció. Exemples famosos:
- **π** (perímetre del cercle): 3.14159265...
- **√2** (diagonal d'un quadrat): 1.41421356...
- **e** (base del logaritme natural): 2.71828182...

Aquests decimals MAI es repeteixen i NUNCA terminen, per tant no es poden escribir com a `a/b`.

---

## 📍 Extensió Avançada

### Extensió 1: Densitat de Racionals

Posa un nombre racional entre:

**1. Entre `1/4` i `1/3`:**
- Decimals: 1/4 = 0.25, 1/3 ≈ 0.333...
- Punt mitjà: (1/4 + 1/3) / 2 = (3/12 + 4/12) / 2 = (7/12) / 2 = 7/24
- **Resposta:** 7/24 ≈ 0.2916..., o també 5/18, 9/32, etc.

**2. Entre `0.5` i `0.6`:**
- Punt mitjà: (0.5 + 0.6) / 2 = 1.1 / 2 = 0.55
- **Resposta:** 0.55 = 11/20, o també 0.51, 0.55, 0.59, etc.

**3. Entre `-1/2` i `0`:**
- Decimals: -1/2 = -0.5, 0 = 0
- Punt mitjà: (-0.5 + 0) / 2 = -0.25
- **Resposta:** -0.25 = -1/4, o també -0.1, -0.3, -1/3, etc.

---

### Extensió 2: Infinit

**Pregunta:** Si totes dues són infinites, és un infinit "més gran" que l'altre?

**Resposta Conceptual:**
- Els **racionals** són "numerables" (pots enumerar-los: 1/1, 1/2, 2/1, 1/3, 3/1, ...).
- Els **irracionals** són "non-numerables" (no pots enumerar-los, fins i tot en teoria infinita).
- Per tant, **els irracionals són més nombrosos que els racionals**, malgrat ambdós senyar infinits!

Aquesta és una idea avançada (cardinalitat de Georg Cantor), però la intuïció és: existeixen "tipus" d'infinit, i alguns infinits són "més grans" que altres.

---

### Extensió 3: Connexió Històrica

**Per què els pitagòrics van negar que √2 existís?**
- Els pitagòrics creien que tot en l'univers podia expressar-se com a fracció (nombre racional).
- Aleshores van descobrir que √2 NO es pot escribir com a fracció (és irracional).
- Això va contraddir la seva filosofia sencera, per tant alguns van negar que √2 "existís" o van mantenir-ho secret.

**Quin és el número irracional més famós que coneixes?**
- **π (pi):** Usat per calcular cercles i esferes. 3.14159265...
- O **√2:** La diagonal d'un quadrat de costat 1.

---

## 🎯 Autoavaluació

Marca quines preguntes vas respondre correctament:

- [ ] Part 1 (Identificar Conjunts): Esperem 9/12 correctes (75%)
- [ ] Part 2 (Escriure com a Fracció): Esperem 6/6 correctes (100%)
- [ ] Part 3 (Jerarquia): Esperem 8/8 correctes (100%)
- [ ] Part 4 (Aplicacions): Esperem 11/11 correctes (100%)
- [ ] Part 5 (Ordre): Esperem 2/2 correctes (100%)
- [ ] Part 6 (Operacions): Esperem 12/12 correctes (100%)
- [ ] Part 7 (Repte): Esperem 2/3 (reflexió és més oberta)
- [ ] Part 8 (Reflexió): Esperem 2/3 correctes

**Puntuació Esperada:**
- 8/8 parts amb major punt: **Mestre de Bloc 3!** 🎉
- 6/8 parts: **Molt bé! Repassa les parts que fallaren.** 👍
- 4/8 parts: **Bé, però necessites practicar més.** 📚

---

## 📝 Notes Addicionals

**Punts Clau a Recordar:**
1. La jerarquia ℕ ⊂ ℤ ⊂ ℚ és com caixes imbricades.
2. Tot nombre enter és racional (podem escribir-lo com n/1).
3. No tots els racionals són enters (1/2 és racional, però no enter).
4. Existeixen nombres que NO són racionals (π, √2).
5. Operacions: suma i multiplicació són "tanques" en ℚ; resta i divisió requereixen cura.

---

**Molt bé pels exercicis! Que dominis la jerarquia de nombres!** 🎓


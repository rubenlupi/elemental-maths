# Solucions Bloc 9 – MCM via Factors Primers

---

## 📌 Part 1: Comprensió del MCM

### 1.1 Completa les Definicions

**MCM (Mínim Comú Múltiple):** El nombre **MÉS PETIT** que és divisible per dos nombres.

**Múltiple:** Un nombre que es pot obtenir multiplicant per **un nombre enter**.

**Múltiples Comuns:** Nombres que són **divisibles** per ambdós nombres.

---

### 1.2 Vertader o Fals?

| Afirmació | V/F | Per què? |
|-----------|-----|---------|
| MCM(4, 6) = 12 | **V** | Els múltiples comuns més petits de 4 i 6 és 12 |
| MCM(5, 10) = 5 | **F** | El MCM és 10 (perquè 10 és el múltiple més petit comú) |
| MCM(3, 7) = 21 | **V** | 3 i 7 són coprims, per tant MCM = 3 × 7 = 21 |
| El MCM és sempre més gran que els números | **F** | Si un nombre divideix l'altre, MCM = el nombre més gran |

---

## 📌 Part 2: Trobar Múltiples

### 2.1 Llista Múltiples Comuns

| Parella | Múltiples 1r | Múltiples 2n | Comuns | MCM |
|---------|-------------|-------------|--------|-----|
| MCM(3, 5) | 3, 6, 9, 12, 15, ... | 5, 10, 15, 20, ... | 15, 30, 45, ... | **15** |
| MCM(4, 6) | 4, 8, 12, 16, 20, 24, ... | 6, 12, 18, 24, ... | 12, 24, 36, ... | **12** |
| MCM(6, 8) | 6, 12, 18, 24, 30, ... | 8, 16, 24, 32, ... | 24, 48, ... | **24** |
| MCM(10, 15) | 10, 20, 30, 40, ... | 15, 30, 45, ... | 30, 60, ... | **30** |

---

## 📌 Part 3: MCM usant Factors Primers

### 3.1 Completa la Factorització

| Números | Factorització 1 | Factorització 2 | MCM |
|---------|----------------|----------------|-----|
| 12, 18 | 2² × 3 | 2 × 3² | 2² × 3² = 4 × 9 = **36** |
| 20, 30 | 2² × 5 | 2 × 3 × 5 | 2² × 3 × 5 = 4 × 3 × 5 = **60** |
| 8, 12 | 2³ | 2² × 3 | 2³ × 3 = 8 × 3 = **24** |
| 15, 25 | 3 × 5 | 5² | 3 × 5² = 3 × 25 = **75** |

**Clau:** Per cada factor primer, tria la potència MÉS GRAN que apareix.

---

### 3.2 Practica amb Factors Primers

**MCM(15, 20):**
- 15 = **3 × 5**
- 20 = **2² × 5**
- Potència més gran de cada factor: 2², 3, 5
- **MCM = 2² × 3 × 5 = 4 × 3 × 5 = 60**

---

**MCM(12, 16):**
- 12 = **2² × 3**
- 16 = **2⁴**
- **MCM = 2⁴ × 3 = 16 × 3 = 48**

---

## 📌 Part 4: Relació MCD i MCM

### 4.1 Usa la Fórmula

**Recorda:** a × b = MCD(a, b) × MCM(a, b)

Per tant: **MCM(a, b) = (a × b) / MCD(a, b)**

| a | b | MCD | a × b | MCM |
|---|---|-----|-------|-----|
| 12 | 18 | 6 | 216 | 36 |
| 20 | 30 | **10** | 600 | **60** |
| 8 | 12 | **4** | 96 | **24** |
| 10 | 15 | **5** | 150 | **30** |

**Explicació:** MCM = (20 × 30) / 10 = 600 / 10 = 60

---

### 4.2 Verifica la Relació

**Comprovació: MCM(12, 18) × MCD(12, 18) = 12 × 18?**

- MCM(12, 18) = 36
- MCD(12, 18) = 6
- 36 × 6 = 216
- 12 × 18 = 216 ✓

**Altres exemples:**

MCM(20, 30) × MCD(20, 30) = 60 × 10 = 600 = 20 × 30 ✓

MCM(8, 12) × MCD(8, 12) = 24 × 4 = 96 = 8 × 12 ✓

---

## 📌 Part 5: Problemes de Sincronització

### 5.1 Cicles Repetitius

**Problema 1:** Dues campanes sonen: una cada 4 segons, l'altra cada 6 segons. Quan sonen juntes novament?

- Múltiples de 4: 4, 8, 12, 16, 20, ...
- Múltiples de 6: 6, 12, 18, 24, ...
- MCM(4, 6) = **12**
- **Resposta:** Cada **12 segons** sonen juntes

---

**Problema 2:** Dues llums parpellegen: una cada 8 minuts, l'altra cada 12 minuts. Quan parpellegen juntes?

- 8 = 2³
- 12 = 2² × 3
- MCM(8, 12) = 2³ × 3 = **24**
- **Resposta:** Cada **24 minuts** parpellegen juntes

---

### 5.2 Horaris Que Coincideixen

**Problema:** Una activitat es fa cada 6 dies, l'altra cada 9 dies. Quan coincideixen?

- 6 = 2 × 3
- 9 = 3²
- MCM(6, 9) = 2 × 3² = **18**
- **Resposta:** Coincideixen cada **18 dies**

---

## 📌 Part 6: Denominador Comú en Fraccions

### 6.1 Suma de Fraccions

| Suma | MCM | Primer Converteix | Suma |
|------|-----|------------------|------|
| 1/3 + 1/5 | **15** | 5/15 + 3/15 | **8/15** |
| 2/6 + 1/8 | **24** | 8/24 + 3/24 | **11/24** |
| 3/4 + 1/6 | **12** | 9/12 + 2/12 | **11/12** |

**Explicació (primer exemple):**
- MCM(3, 5) = 15 (perquè 3 i 5 són coprims: 3 × 5 = 15)
- 1/3 = 5/15 (multiplica per 5)
- 1/5 = 3/15 (multiplica per 3)
- 5/15 + 3/15 = 8/15

---

### 6.2 Verifica si els Denominadors Coincideixen

| Fraccions | Mateix Denominador? | MCM |
|-----------|------------------|-----|
| 1/4 i 1/6 | NO | MCM(4, 6) = **12** |
| 3/8 i 5/12 | NO | MCM(8, 12) = **24** |
| 2/9 i 4/15 | NO | MCM(9, 15) = **45** |

---

## 📌 Part 7: MCM de Tres o Més Números

### 7.1 Calcula MCM de Tres

| Números | MCM 1r i 2n | MCM Resultat i 3r | Final |
|---------|------------|------------------|-------|
| 4, 6, 8 | MCM(4,6)=12 | MCM(12,8)=24 | **24** |
| 6, 8, 12 | MCM(6,8)=24 | MCM(24,12)=24 | **24** |
| 3, 5, 7 | MCM(3,5)=15 | MCM(15,7)=105 | **105** |

**Explicació (3, 5, 7):**
- 3, 5, 7 són tots coprims
- MCM = 3 × 5 × 7 = 105

---

### 7.2 Usa Factors Primers per a Tres

**MCM(12, 18, 24):**
- 12 = 2² × 3
- 18 = 2 × 3²
- 24 = 2³ × 3
- **MCM = 2³ × 3² = 8 × 9 = 72**

(Potència més gran de 2 és 2³, potència més gran de 3 és 3²)

---

## 📌 Part 8: Repte — Problemes Avançats

### 8.1 Casos Especials

**Pregunta 1:** Si a divideix b, què és MCM(a, b)?

**Resposta:** **MCM = b** (el nombre més gran)

Exemple: MCM(4, 12) = 12 (perquè 4 divideix 12)

---

**Pregunta 2:** Si MCD(a, b) = 1 (coprims), què és MCM(a, b)?

**Resposta:** **MCM = a × b** (el producte)

Exemple: MCM(5, 7) = 35 (perquè MCD(5,7) = 1)

---

**Pregunta 3:** Relació entre MCD i MCM: Si MCD(a, b) és gran, MCM és gran o petit?

**Resposta:** **MCM és PETIT** (ja que MCM × MCD = a × b, si MCD és gran, MCM és petit)

---

### 8.2 Problemes Reals Complexos

**Pregunta 1:** Tres autobús passen: A cada 12 minuts, B cada 15 minuts, C cada 20 minuts. Quan passen junts?

- 12 = 2² × 3
- 15 = 3 × 5
- 20 = 2² × 5
- **MCM(12, 15, 20) = 2² × 3 × 5 = 4 × 3 × 5 = 60**
- **Resposta:** Cada **60 minuts** (1 hora) passen junts

---

**Pregunta 2:** Tres colors de balles: vermelles cada 6, blaves cada 8, grogues cada 10. Quan es col·loquen juntes?

- 6 = 2 × 3
- 8 = 2³
- 10 = 2 × 5
- **MCM(6, 8, 10) = 2³ × 3 × 5 = 8 × 3 × 5 = 120**
- **Resposta:** Cada **120 posicions** es col·loquen juntes

---

## 📌 Part 9: Crea els Teus Exercicis

### 9.1 Disseny de Problemes

**Exemple de resposta (Sincronització):**

"Dos events succeeixen: un cada **8 dies** i l'altre cada **12 dies**. Quan coincideixen?"

**Solució:** MCM(8, 12) = 24 dies

---

**Exemple de resposta (Fraccions):**

"Suma 1/**8** + 1/**12** usant MCM"

**Solució:** MCM(8, 12) = 24
- 1/8 = 3/24
- 1/12 = 2/24
- Suma = 5/24

---

## 🎯 Autoavaluació

Marca les parts que vas respondre correctament:

- [ ] Part 1 (Comprensió): ✓
- [ ] Part 2 (Múltiples): ✓
- [ ] Part 3 (Factors primers): ✓
- [ ] Part 4 (Relació MCD-MCM): ✓
- [ ] Part 5 (Sincronització): ✓
- [ ] Part 6 (Denominador comú): ✓
- [ ] Part 7 (Tres números): ✓
- [ ] Part 8 (Repte): ✓
- [ ] Part 9 (Creació): ✓

---

## 🌍 Context Històric: MCM a Través dels Segles

### Sincronització Celeste (3000 BC - Babilonians)

Els astrònoms babilònics necessitaven predir quan coincidien els cicles dels planets. El **MCM** els permetia:
- Venus: cicle de 584 dies
- Mart: cicle de 780 dies
- Quan coincidien? MCM(584, 780) = 227,640 dies (623 anys)

Els babilònics aplicaven aquest concepte sense fórmules formals, usant **taules de múltiples**.

---

### Armonies Musicals (1000-1400 AD - Edat Mitjana)

Els músics medievals découvrien que **els MCM dels períodes de vibració creen armonies**.

Exemple:
- Nota A: vibra 440 vegades/segon
- Nota E: vibra 330 vegades/segon
- **MCM(440, 330) determina la consonància**

Aquesta observació va portar a la teoria d'armonies de les esferes!

---

### Enginyeria de Rellotges (1300-1600 AD - Renaixentista)

Els enginyedors de rellotges usaven **MCM per sincronitzar engranatges**:
- Engranatge A: 12 dents
- Engranatge B: 18 dents
- **MCM(12, 18) = 36**: cada 36 dents, els engranatges es sincronitzen

Aquesta tècnica va revolucionar la precisió dels rellotges!

---

### Sincronització Ferroviària (1800s)

Quan es va inventar el tren, els ferrocarrils usaven **MCM per coordinar horaris**:
- Tren A surt cada 30 minuts
- Tren B surt cada 45 minuts
- **MCM(30, 45) = 90 minuts**: cada 1,5 hores coincideixen en l'estació

Això va permetre crear **xarxes eficients de transport**.

---

### Xarxes Digitals (1900s-Present)

En xarxes informàtiques modernes, el **MCM determina la sincronització de paquets**:

- Dispositiu A envia cada 8 milisegons
- Dispositiu B envia cada 12 milisegons
- **MCM(8, 12) = 24 ms**: cicle de sincronització complet

**Cada vegada que compres online o envies un email**, els teus paquets de dades es sincronitzen usant **MCM**!

---

## 🧮 Relació MCD-MCM: Una Bellesa Matemàtica

### La Identitat Goldstone

**a × b = MCD(a, b) × MCM(a, b)**

Aquesta relació és profunda:

**Exemple:** 12 i 18
- 12 × 18 = 216
- MCD(12, 18) = 6
- MCM(12, 18) = 36
- 6 × 36 = 216 ✓

### Per què és veritat?

Quan factoritzem:
- 12 = 2² × 3
- 18 = 2 × 3²

**MCD pren la potència MÉS PETITA:** 2¹ × 3¹ = 6

**MCM pren la potència MÉS GRAN:** 2² × 3² = 36

**El producte MCD × MCM recupera TOTS els factors:** (2¹ × 3¹) × (2² × 3²) = 2³ × 3³ = 216 ✓

---

## 💡 Aplicacions Modernes del MCM

### 1. **Internet: Sincronització de Routers**
Els routers sincronitzen buffers cada MCM de microsegons per evitar col·lisions.

### 2. **Medicina: Medicacions Peròdiques**
Si prens tres medicaments:
- Cada 6 hores
- Cada 8 hores
- Cada 12 hores
- **MCM(6, 8, 12) = 24 hores**: cada dia complet es sincronitzen

### 3. **Fabricació: Manteniment de Màquines**
- Màquina A: manteniment cada 500 hores
- Màquina B: manteniment cada 750 hores
- **MCM(500, 750) = 1500 hores**: quan es coincideix el manteniment (estalvi d'energia!)

### 4. **Astronomia: Conjuncions Planetàries**
Dos planetes:
- Conjunció cada 2 anys
- L'altre cada 3 anys
- **MCM(2, 3) = 6 anys**: cada 6 anys es veuen junts en el cel

---

## 🎓 Resum de Conceptes Clau

| Concepte | Definició | Exemple |
|----------|-----------|---------|
| MCM | Múltiple més PETIT comú | MCM(4,6) = 12 |
| Múltiple | Resultat de multiplicar per enter | 12 és múltiple de 4 |
| Múltiple comú | Divisible per ambdós | 12 és múltiple comú de 4 i 6 |
| Via factors | Potència més GRAN de cada factor | MCM(12, 18) = 2² × 3² |
| Relació MCD-MCM | a × b = MCD × MCM | 12 × 18 = 6 × 36 |
| Coprims | MCD = 1 | MCM(5, 7) = 35 |

---

## ✅ Verificació Final

**MCM és la base de:**

✅ Sincronització de cicles (campanes, llums, transports)
✅ Suma de fraccions (denominador comú)
✅ Enginyeria (engranatges, horaris)
✅ Informàtica (routers, xarxes)
✅ Biologia (cicles, medicacions)

**Has dominat el MCM quan pots explicar PER QUÈ és necessari en cada context!**


# Exercicis - Mòdul 1: Bloc 1 – Conjunts i Notació Bàsica

## 📊 Distribució de Dificultats

- **Moderats (0.8–1.0 punts)**: Exercicis 1, 3, 5
- **Intermedis (1.0–1.3 punts)**: Exercicis 2, 4, 6, 7, 8
- **Desafiadors (1.5 punts)**: Exercicis 9, 10

---

## 🟦 EXERCICIS

### **Exercici 1** ⭐ (0.8 punts) – Aplicació Directa: Notació de Pertinença

**Enunciat:**

Considera el conjunt `A = {2, 5, 8, 11, 14}` que representa els múltiples de 3 més 2, fins a 14.

a) Escriu tres afirmacions vertaderes utilitzant els símbols `∈` o `∉` per a elements del conjunt `A`.

b) Quin dels següents elements **NO** pertany a `A`? Justifica.
   - `8`
   - `6`
   - `11`

**Solució:**

a) Tres afirmacions vertaderes:
   - `5 ∈ A` ✓ (5 està en la llista)
   - `10 ∉ A` ✓ (10 no està en la llista)
   - `14 ∈ A` ✓ (14 està en la llista)

b) L'element `6` **NO** pertany a `A` perquè no apareix a la llista d'elements. Els múltiples de 3 més 2 són: `2, 5, 8, 11, 14, ...`, i `6` no segueix aquest patró.

**Concepte avaluat:** Símbol de pertinença `∈` i no pertinença `∉`.

---

### **Exercici 2** 🟦 (1.1 punts) – Notació de Comprensió: Traducció Bidireccional

**Enunciat:**

Tradueix el següent conjunt descrit en comprensió a forma enumerada, i després justifica per què és finit:

`D = {n | n és un nombre enter, 0 < n < 10, i n és divisible per 2}`

a) Enumera tots els elements de `D`.

b) Explica per què `D` és finit i quants elements té.

c) Reescriu `D` en forma de comprensió usant un patró (pista: `n = 2k` per a `k ∈ ℕ₀`).

**Solució:**

a) Els nombres enters entre 0 i 10 divisibles per 2 són:
   - `2, 4, 6, 8`
   - Per tant, `D = {2, 4, 6, 8}`

b) `D` és finit perquè tenim una cota superior clara (`n < 10`) i inferior clara (`n > 0`). El conjunt conté exactament **4 elements**.

c) Forma alternativa de comprensió:
   - `D = {2k | k ∈ ℕ, 1 ≤ k ≤ 4}`
   - O bé: `D = {n | n = 2k, k ∈ {1, 2, 3, 4}}`

**Concepte avaluat:** Comprensió matemàtica de conjunts, traducció entre formes enumerada i de comprensió, finitud.

---

### **Exercici 3** ⭐ (0.9 punts) – Ordre i Repetició en Conjunts

**Enunciat:**

Per a cada grup de símbols, determina si representan el **mateix conjunt** o **conjunts diferents**. Justifica en una frase per a cada cas.

a) `{1, 2, 3}` i `{3, 2, 1}`

b) `{a, b, c}` i `{a, b, c, a}`

c) `{vermell, blau}` i `{blau, vermell, blau}`

**Solució:**

a) **Mateix conjunt.** L'ordre dels elements no importa en conjunts; ambdós contenen els mateixos tres elements.

b) **Mateix conjunt.** Els conjunts no repeteixen elements, així que `{a, b, c, a}` es redueix a `{a, b, c}`.

c) **Mateix conjunt.** Els elements `{blau, vermell, blau}` es redueixen a `{blau, vermell}`, que és igual a `{vermell, blau}`.

**Concepte avaluat:** Propietats fonamentals: ordre irrelevant, sense repeticions.

---

### **Exercici 4** 🟦 (1.2 punts) – Problema Real: Club d'Escola

**Enunciat:**

En una escola, el Club de Matemàtiques té membres representats pel conjunt `M = {Anna, Begonya, Carles, Diana}`.

El Mestre de Matemàtiques anota:
- Anna ∈ M
- Enrique ∉ M
- Carles ∈ M

a) Explica per què Enrique no pertany a M.

b) Si demà s'uneix l'estudiante Francesca al club, com s'escriuria el nou conjunt de membres `M'`? (Nota: No escrius cada membre; escrius la transformació.)

c) Si el professor escriu `M = {x | x és estudiant del club de matemàtiques}`, quina és l'avantatge d'aquesta notació respecte de l'enumerada?

**Solució:**

a) Enrique no pertany a M perquè no és estudiant que hagi acceptat unir-se al Club de Matemàtiques. El conjunt `M` només inclou els membres confirmats del club.

b) El nou conjunt seria:
   - `M' = {Anna, Begonya, Carles, Diana, Francesca}`
   - O usant comprensió: `M' = {x | x és estudiant del club de matemàtiques}`

c) Avantatges de la notació de comprensió:
   - Permet descriure el conjunt sense necesitat de llistar tots els noms (especialment si el club creix).
   - és més flexible si canvien els membres.
   - Clarifica la **regla d'inclusió** clarament (ser member del club).

**Concepte avaluat:** Aplicació real de conjunts, interpretació de pertinença i notació flexible.

---

### **Exercici 5** ⭐ (0.8 punts) – Identificació d'Errores en Notació

**Enunciat:**

Revisa les següents afirmacions. Identifica quina és **correcta** i quina és **incorrecta**; per a la incorrecta, explica l'error.

a) `{1, 1, 2, 3} = {1, 2, 3}`

b) `{5} = 5`

c) `{ } és un conjunt buit`

**Solució:**

a) **Correcta.** Els conjunts no permeten repeticions, així que `{1, 1, 2, 3}` és equivalent a `{1, 2, 3}`.

b) **Incorrecta.** L'error és confondre un element amb un conjunt. `{5}` és un conjunt que conté l'element `5`, mentre que `5` és sols el número. La notació correcta seria `5 ∈ {5}`, no `{5} = 5`.

c) **Correcta.** El conjunt buit `{ }` és una col·lecció sense elements, i s'escriu correctament amb aquesta notació.

**Concepte avaluat:** Distincions crítica entre elements, conjunts, i notació.

---

### **Exercici 6** 🟦 (1.1 punts) – Anàlisi de Patrons i Notació de Comprensió

**Enunciat:**

Dona dos conjunts différents que descriguin els nombres que veiem en el patró:
- `2, 5, 8, 11, 14, ...`

a) Escriu el patró en forma de comprensió matemàtica usant `n` o `k` com a variable.

b) Enumera els primers 5 elements si el conjunt es limita a `n < 20`.

c) Quin és l'avantatge de descriure un conjunt infinit com aquest usant comprensió en lloc d'enumeració?

**Solució:**

a) Forma de comprensió:
   - `A = {n | n = 3k + 2, k ∈ ℕ₀}` (on `k = 0, 1, 2, 3, ...`)
   - O: `A = {n | n = 2 + 3k, k ∈ ℕ₀}`
   - O: `A = {3n + 2 | n ∈ ℕ₀}`

b) Primers 5 elements amb `n < 20`:
   - Per a `k = 0`: `3(0) + 2 = 2` ✓
   - Per a `k = 1`: `3(1) + 2 = 5` ✓
   - Per a `k = 2`: `3(2) + 2 = 8` ✓
   - Per a `k = 3`: `3(3) + 2 = 11` ✓
   - Per a `k = 4`: `3(4) + 2 = 14` ✓
   - Resposta: `{2, 5, 8, 11, 14}`

c) Avantatge de comprensió per a conjunts infinits:
   - **Compactesa:** Es pot descriure un conjunt infinit en una única línia.
   - **Claredat de patró:** La fórmula `3k + 2` deixa evident la regla generadora.
   - **Escalabilitat:** Permet extendre el conjunt a tants elements com es desitgi sense escriure'ls tots.

**Concepte avaluat:** Notació de comprensió, identificació de patrons, diferència entre conjunts finits i infinits.

---

### **Exercici 7** 🟦 (1.3 punts) – Conceptual: Distinció Element vs Subconjunt (Preparació per a Bloc 2)

**Enunciat:**

Considera el conjunt `S = {1, {2, 3}, 5}`. (Nota: Un dels elements de `S` és un altre conjunt!)

a) Quan es veritable cadascuna de les següents?
   - `2 ∈ S`
   - `{2, 3} ∈ S`
   - `{1, 5} ⊂ S` (aquest símbol es tractarà al Bloc 2)

b) Explica per què `2 ∈ S` és **falsa** fins i tot que `2` apareix a l'interior de `{2, 3}`.

**Solució:**

a) 
   - `2 ∈ S` → **FALSA.** L'element `2` no està directament dins de `S`; l'element que hi és es `{2, 3}` com a bloc.
   - `{2, 3} ∈ S` → **VERTADERA.** `{2, 3}` és un element complet de `S`.
   - `{1, 5} ⊂ S` → **VERTADERA.** Ambdós `1` i `5` són elements de `S` (és a dir, `{1, 5}` és un subconjunt de `S`).

b) L'error és comum: veure `2` dins `{2, 3}` i pensar que pertany a `S`. Però en realitat, els elements directes de `S` són: `1`, `{2, 3}` (tractada com una unitat), i `5`. El `2` és un element **del** subconjunt `{2, 3}`, no de `S` mateixa. Per a que `2 ∈ S`, hauria de ser llistat directament a nivel superior: per exemple, `S = {1, 2, 3, 5}`.

**Concepte avaluat:** Distinció crítca entre "element de" i "dins de" (preparació per a subconjunts); evitar la confusió de nivells.

---

### **Exercici 8** 🟦 (1.0 punt) – Aplicació: Notació de Conjunts en Context Real

**Enunciat:**

Una botiga de fruites anota els productes disponibles:

`F = {poma, plàtan, taronja, préssec, raïm}`

Un client pregunta si la botiga té `melons`. A més, al final del dia, la botiga reb un enviament de `figues` i `maduixes`.

a) Escriu l'afirmació correcta usant `∈` o `∉` per a la pregunta del client.

b) Escriu el conjunt actualitzat `F'` després de rebre els nous productes.

c) Si la botiga vol descriure "tots els productes que venen" en lugar de llistar-los, com escriuries aquesta idea usant notació de comprensió?

**Solució:**

a) `melons ∉ F` (els melons no están en el conjunt de productes disponibles).

b) `F' = {poma, plàtan, taronja, préssec, raïm, figues, maduixes}`

c) Usant comprensió:
   - `F = {x | x és un producte de fruita que venen a la botiga}`
   - O més específic: `F = {x | x és una fruita disponible a la botiga}`

**Concepte avaluat:** Aplicació pràctica a contextos reals; flexibilitat entre notació enumerada i de comprensió.

---

### **Exercici 9** 🔴 (1.5 punts) – Desafiador: Contrucció Lògica i Raonament Invers

**Enunciat:**

A una biblioteca, el bibliotecari documenta els llibres del gènere "Sci-Fi" amb símbols especialment. Ell afirma:

- `{Blade Runner 2049, Dune, Foundation, Matrix}` és el conjunt de "Sci-Fi clàssics recomanats".
- `{Blade Runner 2049, Dune, Foundation, Matrix, Inception, Interstellar, Twisters}` és el conjunt de "Sci-Fi que té a la biblioteca".

a) Utilitza `∈` i `∉` per a expressar que Inception és un llibre de la biblioteca però NO un clàssic recomanat.

b) Si el bibliotecari vol afegir tres llibres nous a "Clàssics Recomanats" de manera que inclogui "almenys" tots els clàssics originals, quin seria el conjunt mínim de noms que hauria d'afegir? Planteja un exemple.

c) Explica per què la frase "Twisters és a la biblioteca però no és clàssic" no contradict la definició de conjunt clàssic.

**Solució:**

a) 
   - `Inception ∈ {Blade Runner 2049, Dune, Foundation, Matrix, Inception, Interstellar, Twisters}` ✓ (Inception és a la biblioteca)
   - `Inception ∉ {Blade Runner 2049, Dune, Foundation, Matrix}` ✓ (Inception NO és un clàssic recomanat)

b) El conjunt mínim seria:
   - Mantenir els 4 clàssics originals.
   - Afegir 3 nous, per exemple: `{Blade Runner 2049, Dune, Foundation, Matrix, Inception, Interstellar, Twisters}`
   - O qualsevol altra selecció, com: `{Blade Runner 2049, Dune, Foundation, Matrix, Arrival, Oblivion, Gravity}`
   - El conjunt actualitzat seria més gran, però sempre inclou almenys els 4 originals.

c) Aquesta frase **NO contradict** la definició perquè els conjunts categoritzen objectes segons criteris. "Clàssic recomanat" és una categoría específica, mentre que "a la biblioteca" és una categoría més àmplua. Un llibre pot estar a la biblioteca sense ser un clàssic recomanat. Són dos conjunts amb regles diferents de pertinença.

**Concepte avaluat:** Raonament lògic sobre pertinença, distinció entre criteris de categorització, construcció de conjunts amb restrictions.

---

### **Exercici 10** 🔴 (1.5 punts) – Desafiador: Resolució de Misteris amb Notació de Conjunts

**Enunciat:**

En una sala de classe, el professor fa una prova de classificació. Els estudiants han de classificar alguns números en dos grups:
- `A = {números que son divisibles per 3}`
- `B = {números que son divisibles per 2}`

Es fa la següent afirmació sobre quatre números misteris `x, y, z, w`:
1. `x ∈ A` i `x ∉ B`
2. `y ∉ A` i `y ∉ B`
3. `z ∈ A` i `z ∈ B`
4. `w ∈ B` i `w ∉ A`

a) Per a cada cas `x, y, z, w`, dóna un exemple de número que satisfaci les condicions.

b) Justifica per què `6` és un bon exemple per a `z`, però `3` NO seria un bon exemple.

c) Si el professor demana "Quants números positius menors de 10 pertanyen tant a `A` com a `B`?", quina és la resposta? Llista'ls.

**Solució:**

a) Exemples:
   - `x ∈ A` i `x ∉ B`: `x = 3` (divisible per 3, però odd, no divisible per 2) ✓
   - `y ∉ A` i `y ∉ B`: `y = 5` (no divisible per 3, no divisible per 2) ✓
   - `z ∈ A` i `z ∈ B`: `z = 6` (divisible per 3 i per 2) ✓
   - `w ∈ B` i `w ∉ A`: `w = 4` (divisible per 2, però no divisible per 3) ✓

b) 
   - `6` **és** un bon exemple per a `z` perquè: `6 ÷ 3 = 2` (és divisible per 3) ✓, i `6 ÷ 2 = 3` (és divisible per 2) ✓. Per tant, `6 ∈ A` i `6 ∈ B`.
   - `3` **NO seria** un bon exemple perquè: `3 ÷ 3 = 1` (és divisible per 3) ✓, però `3 ÷ 2 = 1.5` (NO és divisible per 2) ✗. Per tant, `3 ∈ A` però `3 ∉ B`, el que significa que `3` NO satisfaria la condició `z ∈ A` i `z ∈ B`.

c) Números positius menors de 10 que pertanyen a TANT `A` com `B`:
   - Han de ser divisibles per 3 **i** per 2, és a dir, divisibles per 6.
   - Números menors de 10 divisibles per 6: **`6`**
   - Resposta: Hi ha **1 número**, que és `6`.

**Concepte avaluat:** Raonament combinat entre múltiples conjunts, interpretació lògica de condicions simultànies, aplicació de criteris de pertinença.

---

## 📈 Resum de Conceptes Avaluats

| Exercici | Concepto Principal | Nivell |
|----------|-------------------|--------|
| 1 | Símbols `∈`, `∉` | Moderat |
| 2 | Comprensió ↔ Enumeració | Intermedi |
| 3 | Ordre i repetició | Moderat |
| 4 | Aplicació real (club) | Intermedi |
| 5 | Errors comuns | Moderat |
| 6 | Patrons i infinitat | Intermedi |
| 7 | Element vs subconjunt | Intermedi |
| 8 | Comprensió en context | Intermedi |
| 9 | Lògica i múltiples criteris | Desafiador |
| 10 | Intersecció de criteris | Desafiador |

---

## 🎯 Consells per als Estudiants

- **Exercicis 1–3, 5:** Practica identificant i usant correctament `∈` i `∉`.
- **Exercicis 2, 4, 6, 8:** Combina enumeració amb comprensió per veure els avantatges de cada forma.
- **Exercicis 7, 9, 10:** Mira les trapes conceptuals (element vs conjunt, nivells de pertinença, interseccions).


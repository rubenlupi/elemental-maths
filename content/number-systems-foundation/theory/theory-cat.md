## Fonaments dels sistemes numèrics

#### Blocs:
1. Conjunts i notació bàsica
2. Subconjunts, subconjunts propis, visuals de Venn
3. Jerarquia de conjunts de nombres ℕ→ℤ→ℚ
4. Valor posicional i formes desenvolupades
5. Introducció a la notació científica
6. Pràctica de regles de divisibilitat
7. Primer/compost + mètode del garbell
8. Aplicacions MCD (Euclides)
9. MCM via factors primers
10. Factorització i teorema fonamental
11. Nombres especials (perfectes, triangulars, Fibonacci)
12. Concepte d'aritmètica modular (a ≡ b mod n)
13. Exploració de patrons de resta
14. Consolidació mixta i repàs

#### Teoria

##### Bloc 1 – Conjunts i Notació Bàsica

En matemàtiques, necessitem maneres de parlar sobre col·leccions d'objectes. Un **conjunt** és simplement una col·lecció ben definida d'objectes diferents anomenats **elements**. L'idea és que sàpigui clarament si alguna cosa pertany al conjunt o no.

🔹 **Definició:** Un **conjunt** és una col·lecció ben definida d'objectes diferents anomenats **elements**; escrivim conjunts amb claus com `A = {1, 2, 3}` i mostrem la pertinença amb `∈`.

Per exemple, si penses en un conjunt de fruites que t'agraden, pots escriure `{poma, plàtan, taronja}`. Cada fruita és un element del conjunt. Si et pregunto "¿la poma pertany al conjunt?", la resposta és "sí", perquè sí que apareix a la llista.

🔹 **Exemples:**
- `B = {vermell, blau, verd}` llista tres colors. Pots dir que `blau ∈ B` (el blau pertany a B), però `groc ∉ B` (el groc NO pertany a B, no està a la llista).
- El conjunt `C = {n | n és un nombre sencer parell}` utilitza una notació més avançada (set-builder notation) que significa "tots els nombres n que són parells", és a dir `0, 2, 4, 6, ...` i així successivament fins a l'infinit.
- Contraexemple important: Si escrius `{1, 1, 2}`, això no és correcte perquè els conjunts no permeten repetir elements. Simplement escriu `{1, 2}`. Els conjunts només es preocupen per quins elements hi ha, no per quantes vegades els llistes.

🔹 **Notació Matemàtica:**
La manera com escrivim els conjunts segueix unes normes estàndard:
- Les claus `{ }` envolten tots els elements del conjunt. La barra `|` (o de vegades dos punts `:`) significa "tal que" en les expressions més complexes. Per exemple, `{n | n > 0}` es llegeix com "el conjunt de tots els n tal que n és major que 0".
- El símbol `x ∈ S` es llegeix "`x` pertany a `S`" o "`x` és element de `S`". El símbol `x ∉ S` significa "`x` NO pertany a `S`".
- Per conveni, utilitzen les lletres majúscules (`S`, `T`, `A`, `B`) per nomenar conjunts, i les lletres minúscules (`a`, `x`, `n`) per nomenar elements individuals.

🔹 **Representacions Visuals:**
```
Exemplos de conjunts:
S = {rojo, blau, verd}  (3 colors)
T = {1, 2, 3, 4, 5}     (5 nombres)
```
```
Recta numèrica de nombres parells:
<---•---•---•---•--->
	0   2   4   6
```

🔹 **Conjunt Buit i Casos Especials:**

Un cas especial molt important és el **conjunt buit**, que és el conjunt que no conté cap element. L'escrivim com `∅` o simplement `{ }`.

- El **conjunt buit** `∅` és vàlid i és un subconjunt de tots els conjunts (veurem més tard què significa subconjunt). Pensa-hi: no hi ha cap element al conjunt buit que contradiga la condició de ser membre de qualsevol altre conjunt.
- Per exemple, `{x | x és un nombre sencer i x < 0}` descriu un conjunt que seria buit perquè no existeixen nombres sencers negatius (els enters negatius és un concepte diferent que estudiarem més tard).
- Una distinció important: el conjunt `{∅}` NO és buit! Conté exactament un element: el conjunt buit en si mateix. Té mida `|{∅}| = 1`. Es diria que "conté el conjunt buit com element".
- Contraexemple comú: els estudiants sovint confonen `∅` amb `{0}`. El primer és el conjunt buit (sense res). El segon és un conjunt que conté el nombre zero. Són completament diferents!

🔹 **Propietats o Regles Clau:**

Aquí hi ha algunes veritats fonamentals sobre els conjunts:

- **L'ordre no importa:** `{1, 2, 3}` és exactament el mateix conjunt que `{3, 2, 1}`. En matemàtiques, als conjunts no els importa l'ordre dels elements. Només els importa quins elements hi ha dins. Aquesta es crida la **propietat commutativa per a conjunts**.
- **No hi ha duplicats:** Els elements apareixen una vegada; si accidentalment escrius el mateix element dues vegades, els duplicats simplement "es col·lapsen" en una sola entrada. `{1, 2, 2, 3}` és exactament `{1, 2, 3}`.
- **Mida variable:** Els conjunts poden ser finits (amb un nombre exacte d'elements) o infinits (continuant sense fi). Per exemple, `{1, 2, 3}` és finit, mentre que `{1, 2, 3, ...}` (tots els nombres positius) és infinit.
- **Propietat Commutativa per a la Unió:** Si tens dos conjunts A i B, la unió `A ∪ B` (que significa "tots els elements que estan en A o en B o ambdós") és exactament la mateixa que `B ∪ A`. L'ordre en què combines els conjunts no importa.
- **Propietat Commutativa per a la Intersecció:** La intersecció `A ∩ B` (que significa "els elements que estan tant en A com en B") és exactament la mateixa que `B ∩ A`.
- **El conjunt buit és subconjunt de tot:** `∅ ⊆ S` per a qualsevol conjunt `S`. Per estrany que sembli, el conjunt buit és considerada part de tots els altres conjunts.

🔹 **Exemples Detallats amb Unió i Intersecció:**

Aquestes dues operacions són molt importants quan treballes amb conjunts. La **unió** combina tots els elements, mentre que la **intersecció** només guarda els que són comuns.

- Sigui `A = {1, 2, 3}` i `B = {2, 3, 4}`.
  - **Unió:** `A ∪ B = {1, 2, 3, 4}` (tots els elements dels dos conjunts, però cada un només una vegada). Pensa que combineixes tot, però elimineixes duplicats.
  - **Verificació de commutativitat:** `B ∪ A = {2, 3, 4, 1} = {1, 2, 3, 4}` (mateix resultat! L'ordre de la unió no importa).
  - **Intersecció:** `A ∩ B = {2, 3}` (només els elements que apareixen en ambdós conjunts). Els nombres 2 i 3 estan a A i també estan a B, però l'1 és només a A i el 4 és només a B.
  - **Verificació de commutativitat:** `B ∩ A = {2, 3}` (mateix resultat!).
  
- Sigui `C = {5, 6}` i `D = {7, 8}` (dos conjunts que no comparteixen elements).
  - **Unió:** `C ∪ D = {5, 6, 7, 8}` (tots els elements junts).
  - **Intersecció:** `C ∩ D = ∅` (no hi ha cap element comú, així que la intersecció és el conjunt buit).

- Un cas especial: `{a, b} ∪ ∅ = {a, b}` (si fas la unió amb el conjunt buit, retornes el conjunt original incanviat, perquè el conjunt buit no afegeix res nou).

🔹 **Malentesos Comuns:**

Aquí hi ha alguns errors que els estudiants solen cometre:

- **"Els conjunts {2, 4, 6, ...} han d'acabar-se en algún lloc."** No! Les punts suspensius `...` significa que continua per sempre. Aquest conjunt representa tots els nombres parells positius fins a l'infinit.
- **Confondre elements amb subconjunts:** És molt diferent! `{1, 2}` és un subconjunt del conjunt `{1, 2, 3}`, però el nombre `1` és un element del mateix conjunt. Els elements són "coses dins", mentre que els subconjunts són "col·leccions dins". Tindrem més detalls en el Bloc 2.
- **"Si reorganitzo els elements canvia el conjunt."** No! `{1, 2, 3}` i `{3, 2, 1}` són exactament el mateix conjunt. L'ordre no importa, com ja hem dit. Els estudiants de vegades pensen que la posició dels elements importa, però en conjunts no ho fa.

🔹 **Connexions:**
- Organitza conjunts de nombres com `ℕ`, `ℤ` i `ℚ` més tard al mòdul.
- Suporta diagrames de Venn revisitats al Mòdul 18.

🔹 **Aplicacions i Trucs de Memòria:**

Els conjunts no són només una idea abstracta de matemàtiques pures. S'utilitzen tot el temps en la vida real:

- **A l'escola:** Si vols categoritzar els estudiants per la seves pertinences a clubs, pots usar conjunts. Per exemple, el conjunt de "Membres del club de xaix" o el conjunt de "Membre del club de science fiction". Un alumne pot estar en múltiples conjunts (tant xaix com ciència-ficció), o en cap, o en només un.
- **Consell per recordar:** Imagina cada conjunt com una "carpeta de matemàtiques" etiquetada que conté els objectes relacionats dins. Quan vols saber si alguna cosa pertany al conjunt, simplement mireu dins de la carpeta.

##### Bloc 2 – Subconjunts i Visuals de Venn

Una vegada entenems els conjunts, és hora de parlar sobre les relacions **entre** conjunts. Quan tots els elements d'un conjunt estan dins d'un altre conjunt, tenim una relació especial llamada **subconjunt**.

🔹 **Definició:** Un **subconjunt** `A ⊆ B` significa que tots els elements d'`A` pertanyen a `B`. En altres paraules, A \"està dins\" de B. Un **subconjunt propi** `A ⊂ B` és més estricte: no només tots els elements d'A estan en B, sinó que A és diferent de B (és a dir, B té almenys un element més que A no té).

🔹 **Exemples que il·lustren la idea:**
- Si `B = {1, 2, 3, 4}`, aleshores `A = {2, 4}` és un subconjunt de B (escrivim `A ⊆ B`), ja que tots els seus elements (2 i 4) apareixen en B. A més, com que A té menys elements que B, és un **subconjunt propi** (`A ⊂ B`).
- Un fet interessant: `∅ ⊆ B` per a qualsevol conjunt B. Per què? Perquè el conjunt buit no té cap element que contradiga la definició de subconjunt. No hi ha cap element del conjunt buit que \"falli\" a estar en B.
- Contraexemple: Si intentes dir que `{5}` és un subconjunt de `B = {1, 2, 3, 4}`, estàs equivocat. Això és perquè `5 ∉ B` (el nombre 5 no està a B), de manera que no tots els elements de `{5}` estan en B.

🔹 **Notació Matemàtica:**
Usem símbols específics per expressar les relacions entre conjunts:
- `A ⊆ B` significa \"A és subconjunt de B\" (pot incloure el cas on A = B).
- `A ⊂ B` significa \"A és un subconjunt propi de B\" (A és diferent de B, és més petit).
- `A ⊄ B` significa \"A NO és un subconjunt de B\" (hi ha almenys un element en A que no està en B).
- El conjunt buit `∅` (també escrit `{ }`) no conté cap element, però és subconjunt de tot.

🔹 **Representacions Visuals:**
```
  _________
 /         \
/    A      \
|  _____     |
| |  B  |    |
| |_____|    |
 \           /
  \_________/
```

🔹 **Propietats o Regles Clau:**
- **Reflexivitat:** Tot conjunt és subconjunt de si mateix (`B ⊆ B`). Això pot semblar estrany, però té sentit: tots els elements de B estan clarament en B, oi?
- **Comptatge de subconjunts:** Un conjunt amb `n` elements té exactament `2^n` subconjunts. Per exemple, si tens un conjunt de 3 elements, tindrà 2³ = 8 subconjunts (incloent el conjunt buit i el conjunt sencer).
- **Transitivitat:** Si A és subconjunt de B, i B és subconjunt de C, aleshores A ha de ser subconjunt de C (`A ⊆ B` i `B ⊆ C` ⇒ `A ⊆ C`). Això és lògic: si tot el que està en A està en B, i tot el que està en B està en C, aleshores tot el que està en A està en C.

🔹 **Malentesos Comuns:**
- **\"Un subconjunt ha de ser més petit\":** Fals! Si bé és veritat que `A ⊂ B` (subconjunt propi) significa que A és més petit, la relació `A ⊆ B` permet que A sigui igual a B. Per exemple, `{1, 2, 3} ⊆ {1, 2, 3}` és totalment correcte.
- **\"El conjunt buit no és un subconjunt de res\":** Totalment fals! El conjunt buit és subconjunt de TOTS els conjunts. Alguns estudiants pensen que \"buit\" significa \"no pertany a res\", però en realitat significa \"no té elements que contradiguin la pertinença\".
- **Confondre elements amb subconjunts:** Si tens l'element `5 ∈ B`, NO es segueix automàticament que `{5}` sia un subconjunt de B. Per exemple, si B = {1, 2, 3}, aleshores `3 ∈ B` però `{4} ⊄ B`. Sempre has de comprovar cada element del subconjunt potencial.

🔹 **Connexions:**
- Construeix la jerarquia de nombres `ℕ ⊂ ℤ ⊂ ℚ` al Bloc 3.
- Suporta comparacions d'esdeveniments de probabilitat (Mòdul 17).

🔹 **Aplicacions i Trucs de Memòria:**

La idea de subconjunts és omnipresent en la vida real:

- **Jerarquies organitzatives:** Els gerents ⊂ Empleats (tots els gerents són empleats, però no tots els empleats són gerents). Els metges ⊂ Personal hospitalari. Els membres premium ⊂ Tots els membres d'un servei.
- **Formes geomètriques:** Els quadrats ⊂ Rectangles ⊂ Paral·lelograms. Cada categoria és menys general que l'anterior. Tot quadrat és rectangle, però no tot rectangle és quadrat.
- **Categories d'aliments:** Les verdures ⊂ Productes frescos (tota verdura és fresca, però hi ha altres coses fresques com fruites). Els plats italians ⊂ Menú de restaurant.
- **Gestió de dispositius:** Els telèfons intel·ligents ⊂ Dispositius mòbils. Els cotxes elèctrics ⊂ Tots els vehicles.
- **Nivells de permisos en programari:** Els administradors ⊂ Usuaris avançats ⊂ Usuaris normals. La cadena de subconjunts propis determina qui té accés a què.
- **Aplicacions mèdiques:** Els pacients diabètics ⊂ Pacients amb malaltia crònica. L'anàlisi de subconjunts ajuda els hospitals a assignar recursos mèdics adequadament.

**Consell per recordar:** El símbol de subconjunt propi `⊂` té una aresta aguda que apunta cap al conjunt més gran, recordant-nos que els dos conjunts difereixen (el primer és més petit).

##### Bloc 3 – Jerarquia de Conjunts de Nombres ℕ→ℤ→ℚ

Ara aplicarem la idea de subconjunts als nombres. En matemàtiques, tenim diferents tipus de nombres, i cadascun està \"dins\" del següent. Aquesta és la **jerarquia de nombres**.

🔹 **Definició:** La **jerarquia de nombres** és l'imbricació de conjunts de nombres on cada conjunt més gran inclou l'anterior: naturals `ℕ`, enters `ℤ`, i racionals `ℚ`.

Comencem amb els nombres més simples (els que comptem) i vam afegint més i més tipus:

🔹 **Exemples:**
- `ℕ = {1, 2, 3, 4, 5, ...}` són els **nombres naturals** o \"nombres de compte\". Aquests són els nombres que uses per comptar objectes. (Nota: Alguns matemàtics inclouen el 0, altres no—depèn de la convenció).
- `ℤ = {..., -3, -2, -1, 0, 1, 2, 3, ...}` són els **enters**. Aquests étenen el conjunt ℕ afegint el zero i tots els nombres negatius. Els enters permeten parlar de "deutes" o \"temperatures sota zero\".
- `ℚ` conté cada **fracció** `a/b` on a i b són enters i b ≠ 0. Per exemple, 3 = 3/1 (tot nombre enter és racional), però també 1/2, 3/4, -5/3, etc. Els racionals permetem fraccionar les coses.

🔹 **Notació Matemàtica:**
- La cadena d'inclusió és: `ℕ ⊂ ℤ ⊂ ℚ`. Això significa que tot nombre natural és enter, i tot enter és racional.
- Els racionals es defineixen formalment como: `ℚ = {a/b | a, b ∈ ℤ, b ≠ 0}` que es llegeix \"el conjunt de totes les fraccions a/b on a i b són enters i b no és zero\".

🔹 **Representacions Visuals:**
```
[ℚ]
 └─[ℤ]
	 └─[ℕ]
```
```
Recta numèrica:
... -2 -1 0 1 2 ... | afegir fraccions entre enters per a ℚ
```

🔹 **Propietats o Regles Clau:**
- **Subconjunts:** Tot nombre natural és automàticament un enter (`ℕ ⊂ ℤ`), i tot enter és automàticament un racional (`ℤ ⊂ ℚ`). Si el nombre 5 és natural, aleshores és enter, i és racional (pots escribir 5 com 5/1).
- **Els racionals són \"densos\":** Entre qualsevol dos nombres racionals, sempre pots trobar un altre nombre racional. Per exemple, entre 1/2 i 2/3, hi ha 7/12. Entre 7/12 i 2/3, hi ha 13/24. I pots continuar per sempre! No hi ha \"forats\" en els racionals.

🔹 **Malentesos Comuns:**
- **\"Les fraccions no són racionals\":** Totalment fals! Les fraccions SÓN la definició de racionals. Si pots escribir quelcom como a/b (dos enters, b ≠ 0), aleshores és racional.
- **\"El 0 ha de estar en ℕ\":** Aquí depèn del context i la convenció. Alguns matemàtics inclouen el 0, altres no. L'important és saber que els enters definitely inclouen 0, i els racionals també.
- **\"Els decimals repetits com 0.333... no són racionals\":** Fals! 0.333... = 1/3, que és una fracció. Qualsevol nombre decimal que es repeteix és sempre racional (pot escribirse como fracció). Els nombres NO racionals son aquells com π o √2, que no es repeteixen mai i no es poden escribirse como fracció.

🔹 **Connexions:**
- Prepara per a decimals (Mòdul 3) i sistemes estesos (Mòdul 4).
- Suporta operacions de fraccions en Mòdul 5.

🔹 **Aplicacions i Trucs de Memòria:**
- **Banca i temperatura:** Els comptes poden ser negatius (ℤ), però els recomptes de caramels no—tria ℕ per a inventari, ℤ per a saldo de compte.
- **Mesuraments de cuina:** Les receptes utilitzen fraccions ℚ (1/2 tassa de farina, 3/4 colzada de sal); els pesos de menjar utilitzen ℕ (2 ous, 6 pastanagues).
- **Dosis de medicina:** Les dosis fraccionades (ℚ) com 0.5 mg o 1/4 de comprimé; els recomptes de pacients (ℕ) o canvis de temperatura (ℤ si per sota del normal).
- **Dades d'elevació:** Les altures de muntanyes ∈ ℕ (positives); les profunditats de mar poden ser enters negatius (ℤ); les mesures precisas utilitzen ℚ.
- **Escenaris financers:** Preus d'accions (ℚ—€45.75 per acció), recomptes de transaccions (ℕ), saldos de comptes inclosa deute (ℤ).
- **Mesuraments de física:** Els ràtios de distància utilitzen ℚ; els intervals de temps ℕ; la posició relativa a l'origen ℤ.
- Consell: Visualitza caixes imbricades etiquetades `ℕ`, `ℤ`, `ℚ` per recordar inclusió.


##### Bloc 3.5 – Símbol de Comparació i Desigualtats

🔹 **Definició:** Els símbols `<` (menor que), `>` (major que), `=` (igual a), `≤` (menor o igual a), `≥` (major o igual a) comparen magnituds de nombres a la recta numèrica.

🔹 **Exemples:**
- `3 < 5` (3 és menor que 5).
- `7 > 2` (7 és major que 2).
- `4 = 4` (4 és igual a 4).
- `-2 < 0 < 3` (cadena de desigualtats).
- `5 ≥ 5` i `5 ≥ 3` (major o igual a).

🔹 **Notació Matemàtica:**
- `a < b`, `a > b`, `a = b`, `a ≤ b`, `a ≥ b`.
- Propietat de transitivitat: si `a < b` i `b < c`, aleshores `a < c`.

🔹 **Representacions Visuals:**
```
Recta numèrica:
<----|----|----|----|----|---->
    -2   0    2    4    6

3 està a l'ESQUERRA de 5 → 3 < 5
7 està a la DRETA de 2 → 7 > 2
```

```
Desigualtat en un segment de recta numèrica:
[a)----------o---------(b]
   tancat     punt      obert
   a a       valor      a b
```

🔹 **Propietats o Regles Clau:**
- El símbol **apunta el nombre menor**: `3 < 5` (apunt a 3).
- Invertir direcció inverteix significat: `3 < 5` és equivalent a `5 > 3`.
- **Ordre preservat en suma/resta:** si `a < b`, aleshores `a + c < b + c` i `a - c < b - c`.
- **Multiplicació per positiu preserva ordre:** si `a < b` i `c > 0`, aleshores `ac < bc`.
- **Multiplicació per negatiu inverteix desigualtat:** si `a < b` i `c < 0`, aleshores `ac > bc`.
- **Igualtat és reflexiva:** `a = a`; **simètrica:** si `a = b` aleshores `b = a`; **transitiva:** si `a = b` i `b = c`, aleshores `a = c`.

🔹 **Malentesos Comuns:**
- Assumir que `<` i `>` són intercanviables; la **forma importa** (apunt cap al valor menor).
- Oblidar la **inversió de desigualtat quan es multiplica/divideix per negatius**.
- Confondre comparacions en cadena: `2 < 5 > 3` és ambigua; en lloc d'això escriu `2 < 5` i `5 > 3` per separat o usa `2 < 5 > 3` amb intenció cuidadosa.
- Tractar `=` com a direccional; és simètric—ambdós costats són idèntics.
- Creure que `≤` i `≥` funcionen com desigualtats estrictes; inclouen el valor límit.

🔹 **Connexions:**
- Fonament per resoldre desigualtats (extensions de Mòdul 11).
- Suporta l'ordenació de nombres a la recta numèrica (Mòdul 1).
- Essencial per notació d'interval i rangs en funcions (Mòdul 13).
- Apareix en interpretació de dades i comparacions estadístiques (Mòdul 16).

🔹 **Aplicacions i Trucs de Memòria:**
- **Comparació de preus:** iPhone A ($700) > iPhone B ($650); descompte ≤ 20% del preu original.
- **Estadístiques d'esports:** La mitjana de punts del jugador A ≥ 15 punts; victòries de l'equip < derrotes; temperatura durant partit -2°C ≤ T ≤ 25°C.
- **Gestió de pes:** "Pes objectiu ≤ 75 kg"; "augment de pes < 5 kg per mes."
- **Planificació de pressupost:** "Despeses mensuals ≤ €2000"; "Estalvis > Despesa."
- **Trànsit i viatge:** "Límit de velocitat < 50 km/h en zones urbanes"; "Distància a destinació ≥ 10 km."
- **Rangs mèdics:** "Colesterol normal < 200 mg/dL"; "Rang segur de sucre en sang: 70 ≤ lectura ≤ 100."
- **Sistemes de qualificacions:** "Nota de aprovació ≥ 60%"; "Excel·lent ≥ 90%."
- **Consell:** "El punt **menja** el nombre més gran" (interpretació de sauró famell—l'obertura fa cara al valor més gran).
- **Alternativa:** "Esquerra és menor, dreta és major" (posició a la recta numèrica).
- **Verificació ràpida:** Substitueïx nombres petits (`a = 1, b = 3`) per verificar direcció.



##### Bloc 4 – Valor Posicional i Formes Desenvolupades

Un dels conceptes més fonamentals de les matemàtiques és entendre que els dígits en un nombre no significan la mateixa cosa depenent d'on estan. El \"5\" a la dreta significa 5, però el \"5\" una posició a l'esquerra significa 50. Això és el **valor posicional**.

🔹 **Definició:** El **valor posicional** assigna a cada dígit un valor basat en la seva posició en potències de `10`. La **forma desenvolupada** descompon un nombre en la suma de cada dígit multiplicat per la seva potència de 10 corresponent. Per exemple, 4,582 no és només \"quatre, cinc, vuit, dos\", sinó una suma especial on cada dígit contribueix diferentment.

🔹 **Exemples:**
- `4,582 = 4×1000 + 5×100 + 8×10 + 2×1 = 4×10^3 + 5×10^2 + 8×10^1 + 2×10^0`. El 4 contribueix 4,000 (quatre mil), el 5 contribueix 500 (cinc cents), el 8 contribueix 80 (vuitanta), i el 2 contribueix 2 (dos).
- `307` és més interessant: té `3` centenes, `0` desenes, i `7` unitats. Nota que el zero és crucial! Sense el zero, seria 37, no 307.
- Contraexemple: Si escrius `307 = 3×100 + 7×10`, omitis el zero i gets 370 en lloc de 307. Els zeros \"ocupen posició\" però no contribueixen magnitud—són molt importants!

🔹 **Notació Matemàtica:**
- La notació posicional usa potències de deu: dígit `d_k × 10^k`.
- Forma desenvolupada: `2,045 = 2×10^3 + 4×10^1 + 5×10^0`.

🔹 **Representacions Visuals:**
```
Milers | Centenes | Desenes | Unitats
   4       5          8        2
```
```
Blocs de base-10: [■■■■] milers, [□□□□□] centenes, etc.
```

🔹 **Propietats o Regles Clau:**
- **Cada lloc és deu vegades el valor del lloc a la seva dreta:** Les unitats valen 1, les desenes valen 10, les centenes valen 100, els milers valen 1,000, etc. Cada pas a l'esquerra multiplica per 10.
- **El zero és un ocupant de posició:** El zero no afegeix magnitud, però sí que marca posicions. Sense el zero, els nombres colapserien (no podries distinguir entre 102 i 12).
- **Els nombres es poden reescriure:** Qualsevol nombre pot expressar-se de forma desenvolupada. `205 = 2×100 + 0×10 + 5×1`. Tant si el dígit és zero com no-zero, tots els dígits contribueixen a la forma desenvolupada.

🔹 **Malentesos Comuns:**
- **\"Puc tirar els zeros\":** Fals! Tirar els zeros canvia completament el nombre. 102 i 12 són completament diferents.
- **\"Llegeixo els dígits per separat\":** Alguns estudiants diuen \"dos zero cinc\" per `205`, però aquest és un error conceptual. Hauries de pensar \"dos-cents-cinc\", no dígits individuals.
- **\"La forma desenvolupada només necessita dígits no-zero\":** Fals! Tots els dígits, incloent els zeros, són part de la forma desenvolupada correcta. `205 = 2×100 + 0×10 + 5×1`, no `2×100 + 5×1`.

🔹 **Connexions:**
- Suporta comprensió de decimals (Mòdul 3) i notació científica.
- Essencial per estratègies de càlcul mental en Mòdul 2.

🔹 **Aplicacions i Trucs de Memòria:**
- Ajuda a interpretar xifres de població o moneda.
- Recorda: "Saltar esquerra multiplica per deu" quan desplaçar dígits.

##### Bloc 5 – Introducció a la Notació Científica

Quan treballes amb nombres molt grans (com la distància a les estrelles) o molt petits (com la mida d'un àtom), escribir tots els zeros és tedios i propenso a errors. La **notació científica** és una manera estàndard de escribir aquests nombres compacte i clarament.

🔹 **Definició:** La **notació científica** expressa qualsevol nombre en forma `a × 10^n` on:
- `a` (el **coeficient**) és un nombre entre 1 i 10 (més exactament, 1 ≤ |a| < 10)
- `n` (el **exponent**) és un enter que pot ser positiu, negatiu, o zero
- Això permet representar nombres molt grans o molt petits de manera compacte.

Per exemple, en lloc de escribir 5,200,000, escribim 5.2 × 10^6. En lloc de 0.00034, escribim 3.4 × 10^-4.

🔹 **Exemples:**
- `5,200,000 = 5.2 × 10^6` (el decimal es desplaça 6 posicions a l'esquerra).
- `0.00034 = 3.4 × 10^-4` (el decimal es desplaça 4 posicions a la dreta, per tant -4).
- Contraexemple: `52 × 10^5` NO és correcte! Perquè el coeficient 52 no està entre 1 i 10. Hauries escribir `5.2 × 10^6` en lloc d'això.

🔹 **Notació Matemàtica:**
- `a` és el **coeficient** (o de vegades cridat \"mantissa\"). Ha d'estar entre 1 (inclòs) i 10 (no inclòs).
- `10^n` és la **potència de 10** que determina on va el decimal. Si `n` és positiu, desplaçem el decimal a la dreta (nombres grans). Si `n` és negatiu, desplaçem a l'esquerra (nombres petits).
- Per convertir: `5.2 × 10^6` significa \"agafar 5.2 i desplaçar el decimal 6 posicions a la dreta\", donant 5,200,000.

🔹 **Representacions Visuals:**
```
5.2 × 10^6 → 5.2 → 52 → 520 → ... → 5,200,000
```

🔹 **Propietats o Regles Clau:**
- `10^a × 10^b = 10^(a+b)`; `10^a / 10^b = 10^(a-b)`.
- Multiplicar nombres en notació científica combina coeficients i suma exponents.

🔹 **Malentesos Comuns:**
- **\"Oblidar d'ajustar l'exponent quan desplaçar el decimal\":** Si tens 52.0 i vols convertir a notació científica, primer moves el decimal: 5.2. Has movit 1 posició a l'esquerra, per tant l'exponent és +1: `5.2 × 10^1`. Els estudiants sovint cometen errors aquí contant les posicions incorrectament.
- **\"Invertir el signe del exponent\":** Alguns pensen que els nombres petits com 0.00034 necessiten exponents positius. FALS! Els nombres petits (< 1) necessiten exponents negatius. Pensa-ho: `10^-4 = 0.0001`, que és petit.
- **\"El coeficient pot ser < 1 o ≥ 10\":** Esto viola la definició! Sempre necessita estar entre 1 i 10. Si el coeficient no està en aquest rang, has fet quelcom malament.

🔹 **Connexions:**
- Enllaça amb lleis d'exponent (Mòdul 6) i escales de mesurament (Mòdul 8).
- Essencial per representació de dades científiques (Mòdul 16).

🔹 **Aplicacions i Trucs de Memòria:**
- **Astronomia:** Distàncies (1.5 × 10^8 km al Sol, 4.4 × 10^16 m a l'estrella més propera) s'ajusten ben a notació científica per comparació.
- **Química:** Nombre d'Avogadro ≈ 6.02 × 10^23 (molècules en un mol); mides atòmiques ≈ 10^-10 metres.
- **Microbiologia:** Mida de virus ≈ 10^-7 a 10^-8 metres; bacteris ≈ 10^-6 metres—comparació d'escala requereix notació científica.
- **Finances:** PIB mundial ≈ 10^13 euros; transacció individual ≈ 10^2 euros—la notació mostra diferències d'escala.
- **Emmagatzematge de dades:** Capacitat de disc dur 2 × 10^12 bytes (2 TB); mida de fitxer 5 × 10^6 bytes (5 MB).
- **Càlculs de física:** Velocitat de la llum ≈ 3 × 10^8 m/s; massa de partícula nuclear ≈ 10^-27 kg.
- **Ciència del clima:** Emissions anuals de CO₂ ≈ 3.7 × 10^10 tones; contaminació de partícules ≈ 10^-6 grams.
- **Sabies que...?** Distància al Sol és sobre `1.5 × 10^8 km`; escriure això com 150,000,000 km és feixuc i propenso a errors.

##### Bloc 6 – Pràctica de Regles de Divisibilitat

Aquí és on comencem a veure patrons interessants en els nombres. Les **regles de divisibilitat** són trucs que et permeten determinar ràpidament si un nombre es divideix per un altre sense tenir de fer la divisió completa.

🔹 **Definició:** Una **regla de divisibilitat** és un drecera o patró que et permet saber si un nombre és divisible per un altre (és a dir, si la divisió dóna com a resultat un enter sense resta) només observant els dígits, sense fer divisió llarga.

Per exemple, tots sabem que els nombres parells acaben en 0, 2, 4, 6, o 8. Això és una regla de divisibilitat per 2. No necessites dividir—només mires l'últim dígit!

🔹 **Exemples:**
- Un nombre és divisible per `2` si el seu **últim dígit** és `0, 2, 4, 6, 8`. Per exemple, 1,346 és divisible per 2 perquè acaba en 6.
- Un nombre és divisible per `3` si la **suma dels seus dígits** és múltiple de 3. Per exemple, `7,524` té suma de dígits `7+5+2+4 = 18`, i 18 és divisible per 3, per tant 7,524 és divisible per 3.
- Contraexemple: `123` NO és divisible per 4, tot i que 123 ÷ 4 = 30.75. La regla per 4 és que els **últims dos dígits** han de formar un nombre divisible per 4. Els últims dos dígits de 123 són 23, i 23 ÷ 4 = 5.75 (no enter), per tant 123 no és divisible per 4.

🔹 **Notació Matemàtica:**
- `a | b` es llegeix \"`a` **divideix** `b`\" i significa que la divisió `b ÷ a` dóna un enter (sense resta).
- `a ∤ b` significa \"`a` **NO divideix** `b`\" (hi ha una resta no-zero).
- Les regles es solen llistar en una taula perquè és fàcil de consultar ràpidament.

🔹 **Representacions Visuals:**
```
Taula de divisibilitat
Divisor | Prova ràpida
   2    | últim dígit parell
   3    | suma de dígits múltiple de 3
   5    | últim dígit 0 o 5
   9    | suma de dígits múltiple de 9
```

🔹 **Propietats o Regles Clau:**
- **Transitivitat:** Si `a | b` (a divideix b) i `b | c` (b divideix c), aleshores `a | c` (a divideix c). Per exemple, si 2 divideix 10 i 10 divideix 100, aleshores 2 divideix 100.
- **Suma i resta:** Si `a | b` i `a | c`, aleshores `a` divideix tant `b + c` com `b - c`. Per exemple, si 3 divideix 12 i 3 divideix 9, aleshores 3 divideix 12 + 9 = 21.

🔹 **Malentesos Comuns:**
- **\"Aplicar la regla equivocada al divisor equivocat\":** Una regla que funciona per 3 (suma de dígits) NO funciona per 4 (últims dos dígits). Els estudiants confonen aquestes regles fàcilment.
- **\"Oblidar que la divisibilitat per 6 requereix TANT 2 com 3\":** 6 = 2 × 3, per tant un nombre és divisible per 6 si és divisible pels dos. No pots dir que 15 és divisible per 6 només perquè és divisible per 3.
- **\"Creure que les regles prediuen primarietat\":** Una regla de divisibilitat NO diu si un nombre és primer. Només diu si és divisible per un factor específic. Per exemple, 9 passa la prova de divisibilitat per 3, però 9 NO és primer (= 3 × 3).

🔹 **Connexions:**
- Porta a primers, MCD i MCM (Blocs 7–9).
- Suporta simplificació de fraccions en Mòdul 5.

🔹 **Aplicacions i Trucs de Memòria:**
- Verificacions ràpides per compartir entre grups.
- Consell: "Six necessita parell i triple" per recordar `6` necessita divisibilitat tant per `2` com `3`.

##### Bloc 7 – Primer/Compost i Mètode del Garbell

Un dels descobriments més profunds en matemàtiques és que tots els nombres (excepte alguns casos especials) es poden construir multiplicant nombres més petits anomenats **primers**. Entendre els nombres primers és comprendre els \"blocs de construcció\" de totes les matemàtiques.

🔹 **Definició:** Un **nombre primer** és un nombre natural major que 1 que té exactament dos divisors positius distints: 1 i ell mateix. Un **nombre compost** té més de dos divisors (pot dividir-se per altres nombres a més d'1 i ell mateix). El nombre 1 és especial—no és primer ni compost.

El **Garbell d'Eratòstenes** és un algoritme antic però potent per trobar tots els primers fins a un nombre donat eliminant sistemàticament els múltiples.

🔹 **Exemples:**
- `2, 3, 5, 7` són primers. Cadascun només es pot dividir per 1 i per si mateix.
  - 2 és divisible per: 1, 2. Dos divisors ✓ primer
  - 5 és divisible per: 1, 5. Dos divisors ✓ primer
- `4, 6, 9, 12` són compostos. Cada un té més de dos divisors.
  - 4 és divisible per: 1, 2, 4. Tres divisors ✓ compost (2 × 2)
  - 9 és divisible per: 1, 3, 9. Tres divisors ✓ compost (3 × 3)
- `1` NO és primer ni compost. Per definició, els primers han de tenir exactament dos divisors, però 1 només té un (ell mateix).
- Contraexemple: Cridar `9` primer és un error comú. Tot i que 9 és un nombre sencer, és compost perquè `9 = 3 × 3`.

🔹 **Notació Matemàtica:**
- `p ∈ ℕ`, `p > 1`, `d | p ⇒ d ∈ {1, p}`.
- El garbell usa marcat seqüencial de múltiples de cada primer descobert.

🔹 **Representacions Visuals:**
```
1  2  3  4  5  6  7  8  9 10
   P  P  X  P  X  P  X  X  X
P = primer, X = múltiple creuat
```
```
Arbre de factors per a 12:
   12
  /  \
 3    4
	 / \
	2   2
```

🔹 **Propietats o Regles Clau:**
- **El 2 és l'únic primer parell:** Tots els altres nombres parells (4, 6, 8, 10, ...) són compostos perquè es divideixen per 2. Per tant, 2 és especial.
- **Tot nombre > 1 és primer o compost:** No hi ha un \"terce categoria\". Cada nombre natural major que 1 ha de ser un dels dos.
- **El garbell comença a p²:** En el garbell d'Eratòstenes, quan elimines múltiples de p, pots começar a p² perquè tots els múltiples més petits ja hauran estat marcats per nombres primers més petits.

🔹 **Malentesos Comuns:**
- **\"Els nombres negatius poden ser primers de la mateixa manera\":** La definició estàndard de primers només aplica a nombres naturals positius. Per tant, -5 NO és primer (tot i que 5 sí).
- **\"Els nombres molt grans no poden ser primers\":** Fals! Existeixen primers colosals! De fet, els matemàtics segueixen descobrint nombres primers més grans. Només perquè un nombre és gran no significa que no sia primer.
- **\"El garbell encontra primers per divisió\":** No! El garbell NO utilitza divisió. Marques sistemàticament els múltiples de cada primer que trobes. Això és muito més eficient que provar cada nombre amb divisió.

🔹 **Connexions:**
- Factorització primer (Bloc 10) i criptografia (Mòdul 21).
- Apareix en nombres especials de Mòdul 9.

🔹 **Aplicacions i Trucs de Memòria:**
- Utilitzat en teoria de codificació i dades segures.
- Recorda: "Primer significa precisament dos divisors."

##### Bloc 8 – Aplicacions MCD (Euclides)

En molts problemes pràctics, necessitem trobar el \"nombre més gran que divideix dos nombres diferentes\". Per exemple, si vols dividir 24 estudiants i 36 llibres en grups iguals, quin és el màxim nombre de grups que pots fer? La resposta és el **màxim comú divisor** (MCD).

🔹 **Definició:** El **màxim comú divisor** (MCD) de dos nombres `a` i `b` és el nombre enter més gran que divideix tant `a` com `b`. L'**algoritme d'Euclides** és un mètode elegant i ràpid per calcular-lo usant divisió repetida amb restes.

Per exemple, els divisors de 24 són: 1, 2, 3, 4, 6, 8, 12, 24. Els divisors de 36 són: 1, 2, 3, 4, 6, 9, 12, 18, 36. Els divisors comuns són: 1, 2, 3, 4, 6, 12. El **màxim** comú divisor és 12.

🔹 **Exemples:**
- `gcd(24, 36) = 12` (12 és el nombre més gran que divideix tant 24 com 36).
- `gcd(48, 18)` via l'algoritme d'Euclides (molt més ràpid):
  - `48 = 18×2 + 12` (48 dividit per 18 dóna 2 amb resta 12)
  - `18 = 12×1 + 6` (18 dividit per 12 dóna 1 amb resta 6)
  - `12 = 6×2 + 0` (12 dividit per 6 dóna 2 amb resta 0)
  - Quan la resta és 0, el MCD és 6. ✓
- Contraexemple: Endevinar que `9` divideix tant `12` com `18` falla. 9 NO divideix 12 (12 ÷ 9 = 1.33...), per tant 9 NO és un divisor comú.

🔹 **Notació Matemàtica:**
- `gcd(a, b) = gcd(b, a mod b)` iterativament fins que resta `0`.
- `gcd(a, b, c)` símbol abreviat per `gcd(a, gcd(b, c))`.

🔹 **Representacions Visuals:**
```
Escala d'Euclides per a gcd(48,18)
48 = 18×2 + 12
18 = 12×1 + 6
12 = 6×2 + 0
```
```
Enrajolat de rectangle: mida de quadrat comú que enrajola ambdós rectangles.
```

🔹 **Propietats o Regles Clau:**
- **Descomposició coprima:** Si `d = gcd(a, b)`, aleshores pots escribir `a = d·a'` i `b = d·b'` on `a'` i `b'` són **coprims** (el seu MCD és 1). Això significa que els únics divisors comuns de `a'` i `b'` són 1.
- **Relació amb MCM:** Els números `gcd(a, b)` i `lcm(a, b)` (mínim comú múltiple) estan relacionats: `a × b = gcd(a, b) × lcm(a, b)`. Aquesta és una fórmula útil!

🔹 **Malentesos Comuns:**
- **\"Confondre MCD amb MCM\":** Són conceptes completament oposts! MCD és el nombre **més GRAN** que divideix ambdós. MCM és el nombre **més PETIT** que és divisible per ambdós. Són gairebé oposats!
- **\"Oblidar que 1 és un divisor comú\":** Tot parell de nombres té almenys 1 com a divisor comú, per tant el MCD és sempre almenys 1.
- **\"Esperar que els passos d'Euclides s'aturin quan els nombres coincideixen\":** No! L'algoritme s'atura quan la resta és 0, no quan els nombres són iguals. Això és una confusió comú.

🔹 **Connexions:**
- Simplifica fraccions (Mòdul 5) i congruències modulars.
- Demostra pensament algorítmic rellevant a estratègies de Mòdul 19.

🔹 **Aplicacions i Trucs de Memòria:**
- Utilitzat en agrupació d'elements equitativament o sincronització de cicles.
- Consell: "Màxim Comú Divideix" resumeix el seu significat.

##### Bloc 9 – MCM via Factors Primers

Mentre que el MCD és el nombre **més gran** que divideix dos nombres, el **mínim comú múltiple** (MCM) és l'oposat: el nombre **més petit** que és divisible pels dos. Si el MCD és sobre \"quants grups\", el MCM és sobre \"quan coincideixen de nou\".

🔹 **Definició:** El **mínim comú múltiple** (MCM) de `a` i `b` és el nombre enter positiu **més petit** que és divisible tant per `a` com per `b`. Sovint el calcules usant factorització primera, prenent la potència més alta de cada factor primer.

Per exemple, si vols trobar quan dues campanes que sonen cada 4 i 6 segons sonen simultàniament, necessites el MCM de 4 i 6.

🔹 **Exemples:**
- `lcm(4, 6) = 12` (12 és el nombre més petit divisible tant per 4 com per 6).
  - Múltiples de 4: 4, 8, 12, 16, 20, ...
  - Múltiples de 6: 6, 12, 18, 24, ...
  - El primer múltiple comú és 12. ✓
- `lcm(8, 12, 15) = 120` (usa factorització primera: 8 = 2³, 12 = 2²×3, 15 = 3×5; prens les potències més altes: 2³×3×5 = 120).
- Contraexemple: Triar `24` com `lcm(4, 6)` és incorrecte perquè 24 és un múltiple comú, però NO és el més petit. 12 és més petit i funciona.

🔹 **Notació Matemàtica:**
- Mètode de factor primer: prén la potència més alta de cada primer entre nombres.
- Identitat: `a × b = gcd(a, b) × lcm(a, b)`.

🔹 **Representacions Visuals:**
```
Llista de múltiples:
4 → 4,8,12,16,...
6 → 6,12,18,...
Primera comú → 12
```

🔹 **Propietats o Regles Clau:**
- **Simetria:** `lcm(a, b) = lcm(b, a)` (l'ordre no importa).
- **Relació amb divisibilitat:** Si `a | b` (si a divideix b), aleshores `lcm(a, b) = b`. Per exemple, `lcm(3, 12) = 12` perquè 3 ja divideix 12.
- **Regla del MCD-MCM:** `a × b = gcd(a, b) × lcm(a, b)`. Aquesta relació sempre es manté!

🔹 **Malentesos Comuns:**
- **\"Aturar-se en qualsevol múltiple comú\":** Necessites el **MENOR** múltiple comú, no només qualsevol múltiple comú. 24, 36, 48 són tots múltiples comuns de 4 i 6, però 12 és el mínim.
- **\"Oblidar d'incloure totes les potències primers\":** Si calcules `lcm(8, 12)`, els factors primers són 8 = 2³ i 12 = 2²×3. El MCM és 2³×3 = 24, no 2×3 = 6 (seria massa petit!).
- **\"El MCM ha de ser el producte dels nombres\":** Alguns estudiants pensen que `lcm(a, b) = a × b` sempre. Fals! Això només és veritat si `a` i `b` són coprims (gcd = 1). Si comparteixen factors, el MCM és més petit que el producte.

🔹 **Connexions:**
- Essencial per denominadors comuns (Mòdul 5).
- Suporta problemes de programació (Mòdul 19).

🔹 **Aplicacions i Trucs de Memòria:**
- Sincronitzar esdeveniments, com horaris de classes o cicles de semàfor.
- Recorda: "Menor significa primer partit, després atura't."

##### Bloc 10 – Factorització i Teorema Fonamental

**Introducció Narrativa:**
Fins ara hem après a identificar nombres primers i a trobar factors comuns. Però aquí descobreixes una de les veritats més profundes de la matemàtica: cada nombre natural (més gran que 1) es pot descompondre en un únic conjunt de nombres primers. Això significa que els nombres primers són literalment els **"àtoms"** de les matemàtiques. Així com tots els elements químics es formen a partir de combinacions de partícules subatòmiques, tot nombre es forma a partir de primers. Aquesta revelació és el **Teorema Fonamental de l'Aritmètica**, i és la base per a quasi tota la teoria de nombres.

**Definició:**
La **factorització en primers** (o descomposició en factors primers) és el procés d'escriure un nombre com a producte de nombres primers, cadascun elevat a una potència positiva. Per exemple:
- 12 = 2² × 3 (no és 2 × 6, perquè 6 no és primer)
- 30 = 2 × 3 × 5 (és l'únic producte de primers que dóna 30)
- 100 = 2² × 5²

El **Teorema Fonamental de l'Aritmètica** estableix que aquesta representació és **única** per a cada nombre. Això significa que no hi ha dos nombres que tinguin la mateixa factorització en primers — cadascun té la seva pròpia "signatura" matemàtica.

**Exemples Detallats:**
- **Factorització de 60:**
  - Comencem: 60 = 2 × 30
  - Continua: 60 = 2 × 2 × 15
  - Continua: 60 = 2 × 2 × 3 × 5
  - **Forma final:** 60 = 2² × 3 × 5
  - Per què és única? No hi ha cap altra combinació de primers que multiplicats donin exactament 60.

- **Per contrast: 30 vs. 60**
  - 30 = 2 × 3 × 5
  - 60 = 2² × 3 × 5
  - La diferència? Una potència extra de 2. Per això 60 és el doble de 30.

- **Nombres primers en la factorització:**
  - 7 = 7¹ (els nombres primers són la seva pròpia factorització)
  - 1 no es factoritza (és la identitat multiplicativa)

- **Factorització de 84:**
  - 84 = 2² × 3 × 7
  - Compara amb 60 = 2² × 3 × 5: és diferent perquè els factors primers són distints.

🔹 **Notació Matemàtica:**
- Arbres de factors per visualitzar la descomposició
- Exponents per indicar potències: `2³` significa 2 × 2 × 2
- Notació formal: `n = p_1^{a_1} × p_2^{a_2} × ... × p_k^{a_k}` on `p_i` són primers diferents
- Unicitat formal: si `n = p_1^{a_1} × ... = q_1^{b_1} × ...`, aleshores els primers i exponents han de ser idèntics

🔹 **Representacions Visuals:**
```
Arbre de factors de 60:
   60
  /  \
 6   10
 /\  / \
2 3 2  5

Resultado: 60 = 2 × 2 × 3 × 5 = 2² × 3 × 5
```

🔹 **Propietats Importants:**
- **Unicitat:** Per a cada nombre n > 1, existeix una única factorització en primers. Pots trobar-la de formes diferents (començant pels factors més petits o més grans), però arribaràs sempre al mateix resultat. Això no és obvi! De fet, hi ha sistemes de nombres on aquesta propietat NO es cumpleix, mostrant per què el Teorema Fonamental és tan especial pels nombres naturals.

- **Relació amb MCD i MCM:** 
  - Si 12 = 2² × 3 i 18 = 2 × 3²
  - MCD(12, 18) = 2¹ × 3¹ = 6 (prens la potència MÉS PETITA de cada primer comú)
  - MCM(12, 18) = 2² × 3² = 36 (prens la potència MÉS GRAN de cada primer comú)
  - La factorització en primers t'ajuda a veure exactament per què això és veritat!

- **Conexió amb divisibilitat:**
  - Un nombre a divideix un nombre b si i només si **tots els factors primers de a (amb les seves potències) apareixen en b**.
  - Per exemple: 6 divideix 30? Comprova: 6 = 2 × 3, 30 = 2 × 3 × 5. Sí, els factors de 6 estan en 30. ✓
  - Per exemple: 8 divideix 30? Comprova: 8 = 2³, 30 = 2 × 3 × 5. No! 30 només té un 2, però 8 en necessita tres. ✗

- **Els nombres primers en la factorització apareixen exactament una vegada cadascun:** Per exemple, 8 = 2³ (no 2 × 2 × 2 com a tres factors distints, sinó una sola potència de 2).

🔹 **Malentesos Comuns:**
- **\"La factorització pot ser múltiple\":** NO! El Teorema Fonamental declara que és única. Si trobas dues factoritzacions diferentes d'un nombre, has comès un error. Per exemple: 12 = 2² × 3 = 4 × 3? No, 4 no és primer, així que no és una factorització vàlida.

- **\"Pots aturar-te quan conegues alguns factors\":** Alguns estudiants pensen que 12 = 2 × 6 és la factorització final. Però necessites continuar fins que TOTS els factors siguin primers: 12 = 2 × 2 × 3.

- **\"Els nombres primers no es factoritzen\":** Veritat! Un nombre primer p sempre es factoritza com p¹. No es pot descompondre més. Per eso els primers són els \"blocs de construcció\" fonamentals de tots els nombres.

- **\"La factorització depèn de l'ordre\":** La multiplicació és commutativa, així que 12 = 2 × 2 × 3 = 3 × 2 × 2 = 2 × 3 × 2. Els factors són els mateixos! Escrivim en ordre crescrent per estandarditzar: 2² × 3.

- **\"Incompletesa de factorització parcial\":** 45 = 3 × 15 NO és una factorització completa perquè 15 = 3 × 5 no és primer. La factorització completa és 45 = 3² × 5. Sempre continua fins que TOTS els factors siguin primers.

🔹 **Aplicacions Reals:**
- **Criptografia (RSA):** Els sistemes de seguretat usan nombres enormes que són el producte de dos primers gegants. Només es pot trencar si pots factoritzar aquest producte en els seus primers components, que és computacionalment casi impossible amb nombres prou grans. La factorització en primers és la clau de la seguretat digital moderna! Els algoritmes de criptografia depenen del fet que és fàcil multiplicar dos primers però molt difícil trobar quins primers van produir un producte donat.

- **Compressió de dades:** Algorithms de compressió analitzen la estructura factorial dels nombres per optimitzar emmagatzematge i transmissió de dades.

- **Predicció de paterns:** En teoria de nombres, la factorització ajuda a entendre paterns en propietats de nombres (com quants divisors té un nombre, o altres funcions numèriques).

- **Química computacional:** Algorismes de química usen factorització per calcular energies moleculars i estructures atòmiques.

##### Bloc 11 – Nombres Especials (Perfectes, Triangulars, Fibonacci)

**Introducció Narrativa:**
Fins ara hem estudiat propietats estructurals de nombres — com es factoritzen, com es comparen, com es relacionen. Però hi ha certes categories de nombres que semblen "especials" perquè apareixen amb sorprenent freqüència en la natura i en fenòmens reals. Els nombres triangulars apareixen en contextos geomètrics (apilar objectes), els nombres de Fibonacci es troben en flors i caragols, i els nombres perfectes han fascinat matemàtics durant segles. Aquests blocs ens mostren que les matemàtiques no són només abstractes—les veem arreu en la natura.

**Definició:**
Hi ha tres famílies importants de nombres especials:

1. **Nombres Perfectes:** Un nombre és perfecte si és igual a la suma de tots els seus divisors propis (divisors menys el nombre mateix). Per exemple, 6 = 1 + 2 + 3. Els divisors propis de 6 són {1, 2, 3}, i sumen exactament 6. Els nombres perfectes parells segueixen un patró especial: `2^{p-1}(2^p - 1)` quan `2^p - 1` és primer (anomenats "primers de Mersenne").

2. **Nombres Triangulars:** Imagina apilant boles en files: primera fila 1 bola, segona fila 2 boles, tercera fila 3 boles, etc. El total després de n files és el nombre triangular `T_n = 1 + 2 + 3 + ... + n = n(n+1)/2`. Per exemple, `T_4 = 1 + 2 + 3 + 4 = 10`.

3. **Seqüència de Fibonacci:** Cada terme (excepte els primers dos) és la suma dels dos termes anteriors. Definida com `F_0 = 0`, `F_1 = 1`, i `F_n = F_{n-1} + F_{n-2}` per a `n ≥ 2`. Això genera: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, ...

**Exemples Detallats:**

- **Nombres Perfectes:**
  - `6 = 1 + 2 + 3` (divisors propis: {1, 2, 3})
  - `28 = 1 + 2 + 4 + 7 + 14` (divisors propis: {1, 2, 4, 7, 14})
  - `496 = 1 + 2 + 4 + 8 + 16 + 31 + 62 + 124 + 248` (el següent número perfecte parell)
  - Nota: Els nombres perfectes són extremadament rars! Entre 1 i 1000 només tenim dos: 6 i 28.

- **Nombres Triangulars:**
  - `T_1 = 1` (1 fila, 1 bola)
  - `T_2 = 3` (2 files, 1 + 2 = 3 boles)
  - `T_3 = 6` (3 files, 1 + 2 + 3 = 6 boles)
  - `T_4 = 10` (4 files, 1 + 2 + 3 + 4 = 10 boles)
  - `T_5 = 15` (5 files, 1 + 2 + 3 + 4 + 5 = 15 boles)
  - Per contrast: 9 NO és triangular perquè no existeix `n` tal que `n(n+1)/2 = 9`.

- **Fibonacci en Contextos Reals:**
  - `F_7 = 13` i `F_8 = 21`, la seva ratio `21/13 ≈ 1.615` s'aproxima a la secció àuria (φ ≈ 1.618)
  - Com els nombres creixen: el 10è terme és 55, el 20è és 6765, mostra creixement exponencial
  - **Comparació amb aritmètica:** Una seqüència aritmètica com 1, 2, 3, 4, 5 creix linealment. Fibonacci (1, 1, 2, 3, 5, 8, 13) creix exponencialment!

🔹 **Notació Matemàtica:**
- Nombres triangulars: `T_n = n(n + 1)/2` o equivalentment `T_n = C(n+1, 2)` (combinacions)
- Recursió de Fibonacci: `F_n = F_{n-1} + F_{n-2}` amb casos base `F_0 = 0`, `F_1 = 1`
- Verificació de nombre perfecte: Suma de divisors propis `σ(n) - n = n`, o `σ(n) = 2n`
- Ràtio d'or: `lim_{n→∞} F_{n+1}/F_n = φ = (1 + √5)/2 ≈ 1.618`

🔹 **Representacions Visuals:**
```
Nombres Triangulars (apilament de boles):
T_1 = 1:    •

T_2 = 3:    •
           • •

T_3 = 6:    •
           • •
          • • •

T_4 = 10:   •
           • •
          • • •
         • • • •
```

```
Fibonacci en arquitectura natural—Espiral d'or amb quadrats Fibonacci:
Els quadrats de mides 1, 1, 2, 3, 5, 8 s'ajusten junts formant una espiral aproximant l'espiral d'or.
```

🔹 **Propietats Importants:**
- **Els nombres perfectes parells segueixen un patró:** Si `2^p - 1` és primer (primer de Mersenne), aleshores `2^{p-1}(2^p - 1)` és un nombre perfecte parell. Per exemple, `p = 2` dóna `2^1 × 3 = 6`; `p = 3` dóna `2^2 × 7 = 28`.

- **Els nombres triangulars es relacionen amb combinacions:** `T_n = C(n+1, 2)` significa que `T_n` compta les maneres de triar 2 elements d'un conjunt de `n+1` elements. Això és una connexió profunda entre seqüències i combinatòria.

- **Els ràtios de Fibonacci convergeixen a la secció àuria:** Com més termes calcules, `F_{n+1}/F_n` s'aproxima a `φ ≈ 1.618...`. Aquesta secció àuria apareix en proporcions estètiques naturals (flors, caragols, arquitectura).

- **Fibonacci creix exponencialment:** Es pot demostrar que `F_n ≈ φ^n / √5`. Això explica per què les seqüències de Fibonacci apareixen en creixements de població i altres processos naturals.

- **Els nombres triangulars suma de sèries:** `T_n = 1 + 2 + 3 + ... + n` és la fórmula per a la suma d'una progressió aritmètica de primer terme 1 i diferència comuna 1.

🔹 **Malentesos Comuns:**
- **\"Els nombres triangulars són nombres perfectes\":** NO! Aquestes són dues categories completament distintes. 6 és tant triangular com perfecte (`T_3 = 6` i `6 = 1 + 2 + 3`), però aquesta és una coincidència rara. 10 és triangular (`T_4 = 10`) però no és perfecte (1 + 2 + 5 = 8 ≠ 10).

- **\"Fibonacci sempre comença amb 1, 1\":** La convencional moderna és `F_0 = 0, F_1 = 1`, que dona 0, 1, 1, 2, 3, 5, 8, ... Alguns textos antics comencen amb 1, 1, però aquesta és una opció de notació, no una regla matemàtica.

- **\"Tractant Fibonacci com una progressió aritmètica\":** Alguns estudiants pensen que si 3 - 2 = 1 i 5 - 3 = 2, aleshores Fibonacci té diferències constants. Fals! Fibonacci és **recursiva** (cada terme depèn dels dos anteriors), no **aritmètica** (diferència constant).

- **\"Els nombres perfectes són comuns\":** Els estudiants sovint assumeixen que és fàcil trobar nombres perfectes. De fet, només es coneixen 51 nombres perfectes, i els dos més petits són 6 i 28. El tercer (496) és molt més gran!

- **\"El ràtio de Fibonacci és exactament φ\":** El ràtio `F_{n+1}/F_n` s'**aproxima** a φ però mai és exactament φ per a cap `n` finit. Per exemple, `F_8/F_7 = 21/13 ≈ 1.615`, molt a prop però no exacto.

🔹 **Aplicacions Reals:**
- **Arquitectura i Disseny:** Els arquitectes usan nombres de Fibonacci i la secció àuria (φ) per crear proporcions estètiques agradables. Els rectangles de proporció φ:1 es consideren especialment harmoniosos. Els nombres triangulars ajuden en disseny modular (stackings, tessellacions).

- **Biologia i Botànica:** Els pètals de flors, les espires de caragols marins, la disposició de llavors en girasols — tots segueixen patterns de Fibonacci. Els científics pensen que les plantes evolucionen cap a distribucions de Fibonacci perquè maximitzen l'exposició a la llum solar.

- **Informatica (Algoritmes):** Els algoritmes de Fibonacci apareixen en estructures de dades (heaps de Fibonacci), i la seqüència es usa per a estudiar complexitat computacional. La recursió de Fibonacci és un exemple clàssic d'programació dinàmica.

- **Finances i Economia:** Els analistes utilitzen els «retraços de Fibonacci» (els nombres de Fibonacci escala per a predicció de mercats). Els gràfics de preus sovint reverb en nivells associats a ràtios de Fibonacci (38.2%, 50%, 61.8% de correccions).

- **Criptografia i Teoria de Nombres:** Els nombres de Fibonacci es usan en algoritmes criptogràfics, generators de nombres pseudo-aleatoires, i en teoria de nombres per provar conjectures profundes.

- **Música:** Els ràtios d'intervals musicals (quarta, quinta, octava) es relacionan amb ràtios simples. La secció àuria apareix en estructures de composicions musicals.

- **Sabies que...?** La seqüència de Fibonacci va ser descrita per Leonardo Fibonacci el 1202 en el context d'un problema de conills. Es demana: si comences amb una parella de conills que es reprodueixen cada mes (cada parella nova triga 1 mes per madurar), quants conills tindràs al cap de n mesos? La resposta és exactament `F_{n+2}`!

##### Bloc 12 – Concepte d'Aritmètica Modular (a ≡ b mod n)

**Introducció Narrativa:**
Fins ara hem estudiat números com entitats individuals—els seus factors, les seves propietats. Però hi ha situacions on no ens importa el nombre exacte, sinó només el **residu** quan es divideix per alguna quantitat. Això és aritmètica modular, i és una de les eines més poderoses de les matemàtiques modernes. Cada vegada que mires un rellotge, calcules un dia de la setmana, o usas un codi de seguretat digital, estigues usant aritmètica modular. És el mode en què les matemàtiques "embolcallen"—quan arribes al final, comences de nou.

**Definició:**
L'**aritmètica modular** (o "modular arithmetic") estudia números basada en les seves **restes** quan es divideixen per un nombre fix, anomenat el **modulus**. Dos nombres `a` i `b` són **congruents mòdul n** (escrit `a ≡ b (mod n)`) si `n` divideix exactament la seva diferència `a - b`. 

Per exemple:
- `17 ≡ 5 (mod 12)` perquè `17 - 5 = 12`, que és divisible per 12.
- `9 ≡ 1 (mod 4)` perquè `9 - 1 = 8 = 2 × 4`, que és divisible per 4.

Una manera equivalent de pensar-ho: `a ≡ b (mod n)` significa que `a` i `b` deixan la **mateixa resta** quan es divideixen per `n`.

**Exemples Detallats:**

- **Aritmètica de rellotge (mod 12):**
  - Els números 1, 13, 25, 37, ... són tots congruents mòdul 12 (diuen "1" en un rellotge).
  - `14 ≡ 2 (mod 12)` (les 14:00 són les 2:00 PM)
  - `25 ≡ 1 (mod 12)` (la 25a hora és la 1a hora del dia següent)
  - `0 ≡ 12 (mod 12)` (mitjanit és el "12" en el rellotge)

- **Comparació de restes (mod 5):**
  - 7 i 12 són ambdós congruents a 2 mòdul 5 (7 = 5 + 2, 12 = 2×5 + 2)
  - Per tant, `7 ≡ 12 (mod 5)`
  - Mentre que `8 ≢ 3 (mod 5)` perquè 8 deixa resta 3, però... espera, deixa resta 3? Sí! `8 ≡ 3 (mod 5)` (8 = 5 + 3).

- **Contextos negatius:**
  - `-1 ≡ 11 (mod 12)` (un dia menys que 0 és com la 11a posició)
  - `-3 ≡ 2 (mod 5)` (perquè -3 + 5 = 2)
  - Les restes negatives "embolcallen"—sempre pots sumar el modulus per obtenir un equivalent positiu.

- **Contraexemple clarificador:**
  - `14 ≢ 3 (mod 4)` és **fals**. Per què? 14 - 3 = 11, i 4 no divideix 11. Però 14 div 4 deixa resta 2, i 3 div 4 deixa resta 3. Restes distintes!
  - Mentre que `14 ≡ 2 (mod 4)` és veritat.

🔹 **Notació Matemàtica:**
- Símbol de congruència: `a ≡ b (mod n)` (no és igualtat, és congruència)
- **Classe de resta** o classe de congruència: `[a]_n = {b ∈ ℤ : a ≡ b (mod n)}` representa tots els enters congruents a `a` mòdul `n`
- Per exemple, `[1]_5 = {..., -9, -4, 1, 6, 11, 16, ...}`
- **Restes reduces**: 0 ≤ r < n representa el conjunt complet de restes possibles per mòdul `n`

🔹 **Representacions Visuals:**
```
Rellotge (mod 12) - Els números s'embolcallen:
        12
    11      1
  10          2
 9              3
  8           4
    7       5
        6
```

```
Taula de congruències mòdul 5:
n       | n mod 5  | Classe
--------|----------|---------------------------
0, 5, 10 |    0    | [0]_5 = {..., -10, -5, 0, 5, 10, ...}
1, 6, 11 |    1    | [1]_5 = {..., -9, -4, 1, 6, 11, ...}
2, 7, 12 |    2    | [2]_5 = {..., -8, -3, 2, 7, 12, ...}
3, 8, 13 |    3    | [3]_5 = {..., -7, -2, 3, 8, 13, ...}
4, 9, 14 |    4    | [4]_5 = {..., -6, -1, 4, 9, 14, ...}
```

🔹 **Propietats Importants:**
- **Propietats de preservació operativa:** Si `a ≡ b (mod n)` i `c ≡ d (mod n)`, aleshores:
  - `a + c ≡ b + d (mod n)` (sumar congruències preserva congruencia)
  - `a - c ≡ b - d (mod n)` (restar congruències preserva congruencia)
  - `a × c ≡ b × d (mod n)` (multiplicar congruències preserva congruencia)
  - **Exemple:** `17 ≡ 5 (mod 12)` i `25 ≡ 1 (mod 12)`, així que `17 + 25 ≡ 5 + 1 (mod 12)`, donant `42 ≡ 6 (mod 12)`. Verifiquem: 42 - 6 = 36 = 3×12. ✓

- **Restes negatives embolcallen:** `-1 ≡ n - 1 (mod n)`. Per exemple, mòdul 12: `-1 ≡ 11 (mod 12)`. Això és perquè `-1 - 11 = -12`, que és divisible per 12.

- **Divisió modular és trickier:** No sempre pots dividir. Per exemple, `6 ≡ 2 (mod 4)`, però `6/2 ≡ 2/2 (mod 4)` donaría `3 ≡ 1 (mod 4)`, que és FALS. La divisió modular només funciona sota certes condicions (quan els divisors són coprims al modulus).

- **Propietat reflexiva, simètrica, transitiva:** L'aritmètica modular forma una **relació d'equivalència**:
  - Reflexiva: `a ≡ a (mod n)`
  - Simètrica: Si `a ≡ b (mod n)`, aleshores `b ≡ a (mod n)`
  - Transitiva: Si `a ≡ b (mod n)` i `b ≡ c (mod n)`, aleshores `a ≡ c (mod n)`

🔹 **Malentesos Comuns:**
- **\"Tractar `mod` com divisió\":** `17 mod 5` NO significa "17 ÷ 5". Significa **la resta** quan 17 es divideix per 5, que és 2. El símbol `≡` és per a congruencia, no igualtat.

- **\"Oblidar de reduir restes\":** Les restes sempre han de ser en el rang `0 ≤ r < n`. Si cometzes un error i obté `-3 mod 5`, has de convertir a `2` (perquè `-3 + 5 = 2`).

- **\"Assumir que nombres congruents han de ser propers\":** `17 ≡ 5 (mod 12)` però 17 i 5 no són "propers" en valor. Són congruents perquè difereixen per 12, que és múltiple del modulus.

- **\"Creure que tota operació és permissible\":** Suma, resta i multiplicació preserven congruencia. Però divisió i exponenciació requereixen cura especial. Per exemple, `6 ≡ 3 (mod 3)` però `2^6 = 64 ≢ 2^3 = 8 (mod 3)`. De fet, `64 ≡ 1 (mod 3)` i `8 ≡ 2 (mod 3)`.

- **\"El modulus pot ser negatiu o zero\":** El modulus `n` ha de ser un nombre natural positiu (n > 0). Si pregunten sobre `a mod 0`, això és indefinit.

🔹 **Aplicacions Reals:**
- **Aritmètica de rellotge:** Quan són les 14:00 + 11 hores? `(14 + 11) mod 12 = 25 mod 12 = 1`, així que l'1:00 AM. Les operacions de rellotge són essencialment aritmètica modular.

- **Calendaris i Dies de la Setmana:** Si avui és dimecres (dia 3) i afegim 10 dies: `(3 + 10) mod 7 = 13 mod 7 = 6`, que és dissabte. Els calendaris es basan completament en aritmètica modular.

- **Códigos de Verificació (Checksums):** Els números de targeta de crèdit, codis ISBN, i barras de codi utilizen aritmètica modular per detectar errors. L'algoritme de Luhn per targetes de crèdit es basa en mod 10.

- **Gràfics per Ordinador:** Els canals de color RGB es limiten a valors 0-255. Quan calcules "color + ajustament", usas `mod 256` per mantenir el resultat en rang. Per exemple, `255 + 5 mod 256 = 4`.

- **Criptografia:** Els sistemes de criptografia pública (RSA) es basen completament en aritmètica modular. Els missatges es codifiquen com `message^key mod n`.

- **Balanceig de càrrega en programació:** Si tens 100 clients i 5 servidors, pots assignar client `i` al servidor `i mod 5` per distribució equilibrada.

- **Seqüències periòdiques:** Qualsevol seqüència que es repeteix (patrons de traffic, cicles biològics, estacions del any) pot modelar-se amb aritmètica modular.

- **Sabies que...?** Les notes musicals embolcallen octaves com aritmètica mòdul 12. Hi ha 12 semitons en una octava, i quan superes B, comences de nou en C. Els músics no saben que estan usant matemàtiques, però ho fan!

##### Bloc 13 – Exploració de Patrons de Resta

**Introducció Narrativa:**
L'aritmètica modular no és només un concepte estàtic—és el sement per a la dinàmica. Quan mires com es comporten els números en una seqüència (potències, múltiples, o transformacions), sovint descobreixes que les restes es repeteixen en un cicle previsible. Aquesta exploració de patrons és fascinant perquè revela l'ordre ocult dins del que pot semblar caòtic. Els científics usan aquest principi per predir el comportament a llarg termini, els criptògrafs el usan per crear sistemes segurs, i la natura el usa per crear ritmes i cicles. Els patrons de resta són la respiració de les matemàtiques—ordre emergent de la repetició.

**Definició:**
Un **patró de resta** (o **cicle de restes**) és la seqüència de restes que s'obté quan es calcula una funció o operació repetidament mòdul un nombre fix, fins que el patró es comença a repetir. Es pot aplicar a:
1. **Potències:** `2^1 mod 5, 2^2 mod 5, 2^3 mod 5, ...`
2. **Múltiples:** `1×7 mod 3, 2×7 mod 3, 3×7 mod 3, ...`
3. **Sumes:** `n + 3 mod 8` per a `n = 0, 1, 2, 3, ...`
4. **Dígits:** Els dígits finals (mod 10) de quadrats: `1^2, 2^2, 3^2, ...`

Degut al **Principi de Pigeonhole**, un patró sempre es repeteix eventualment (en el cas de potències, dins d'almenys `n-1` passos per a mòdul `n`).

**Exemples Detallats:**

- **Potències de 2 mòdul 5:**
  - `2^1 mod 5 = 2`
  - `2^2 mod 5 = 4`
  - `2^3 mod 5 = 8 mod 5 = 3`
  - `2^4 mod 5 = 16 mod 5 = 1`
  - `2^5 mod 5 = 32 mod 5 = 2` ← **COMENÇA A REPETIR!**
  - El cicle és `[2, 4, 3, 1]` amb **període 4**. Es repeteix cada 4 passos.

- **Múltiples de 7 mòdul 3:**
  - `7 × 1 mod 3 = 7 mod 3 = 1`
  - `7 × 2 mod 3 = 14 mod 3 = 2`
  - `7 × 3 mod 3 = 21 mod 3 = 0`
  - `7 × 4 mod 3 = 28 mod 3 = 1` ← **REPETEIX!**
  - El cicle és `[1, 2, 0]` amb **període 3**. (Nota: és el mateix que `1, 2, 0` sempre perquè `gcd(7, 3) = 1`.)

- **Dígits últims (mod 10) de potències de 3:**
  - `3^1 mod 10 = 3`
  - `3^2 mod 10 = 9`
  - `3^3 mod 10 = 27 mod 10 = 7`
  - `3^4 mod 10 = 81 mod 10 = 1`
  - `3^5 mod 10 = 3 mod 10 = 3` ← **COMENÇA A REPETIR!**
  - Els últims dígits de 3, 9, 27, 81, 243, 729, ... són sempre 3, 9, 7, 1, 3, 9, ... en cicle.

- **Contraexemple clarificador:**
  - "No tots els cicles comencen a `n=0` o `n=1`." Per exemple, els residus de `2^n mod 7` són:
    - `2^1 mod 7 = 2`
    - `2^2 mod 7 = 4`
    - `2^3 mod 7 = 1`
    - `2^4 mod 7 = 2` ← **Aquí comença el cicle [2, 4, 1]**
  - El cicle NO comença a la posició 1; comença al tercer element.

🔹 **Notació Matemàtica:**
- Una seqüència `(a_n)` definida com `a_n ≡ f(n) (mod m)` per a alguna funció `f`
- **Període** `T`: el nombre més petit de passos fins que el patró es repeteix. Es denota `T = T_f` per a la funció `f`.
- **Cicle**: `[a_1, a_2, ..., a_T]` on `a_{n+T} = a_n` per a tot `n`
- **Totient d'Euler** `φ(n)`: el nombre de nombres entre 1 i `n-1` que són coprims a `n`. Per exemple, `φ(5) = 4` (els números 1, 2, 3, 4 són coprims a 5).

🔹 **Representacions Visuals:**
```
Cicle de restes de 2^n mod 5:
    2
   ↙ ↖
  1   4
   ↖ ↙
    3

(Els números es "rotan" en aquesta roda)
```

```
Taula de potències de 2 mòdul 5 (mostrant el cicle):
n  | 2^n mod 5 | Pattern
----|-----------|--------
1  | 2         | Cicle comença
2  | 4         | 
3  | 3         | 
4  | 1         | 
5  | 2         | ← Repetició! Cicle = [2, 4, 3, 1]
6  | 4         | 
7  | 3         | 
8  | 1         | (continua repetint)
```

🔹 **Propietats Importants:**
- **Principi de Pigeonhole garanteix cicles:** Quan calcules `a^n mod m`, només hi ha `m` possibles restes (0 a m-1). Després de com a màxim `m` càlculs, has de trobar una repetició. Per tant, CADA seqüència de potències mòdul `m` es repeteix!

- **La longitud del cicle es relaciona amb la totient d'Euler:** Per a `gcd(a, m) = 1`, la longitud del cicle de `a^n mod m` divideix `φ(m)`. Per exemple:
  - Per a mòdul 5: `φ(5) = 4`, i la longitud del cicle de `2^n mod 5` és 4 (perfectament divisible).
  - Per a mòdul 7: `φ(7) = 6`, i la longitud del cicle de `3^n mod 7` és 6 (perfectament divisible).

- **No tots els cicles comencen a posició 1:** Els cicles "purs" (seqüències que comencen immediatament a repetir-se) es diuen "cicles simples". Altre cop, potències amb bases coprimes al modulus sempre donan cicles simples (comencen la repetició de seguida).

- **Additivitat en cicles:** Si `a_n` i `b_n` són periòdics amb períodes `T_a` i `T_b`, aleshores `(a_n + b_n)` té període que divideix `lcm(T_a, T_b)`.

🔹 **Malentesos Comuns:**
- **\"Els cicles sempre comencen a `n=0` o `n=1`\":** Fals! Els cicles "purs" comencen immediatament, però si la base i modulus no són coprims, pots tenir un "preamble" abans del cicle. Per exemple, `2^n mod 6`:
  - `2^1 mod 6 = 2`
  - `2^2 mod 6 = 4`
  - `2^3 mod 6 = 2` ← Aquí comença el cicle [2, 4]
  - El preamble és només `2^0 = 1`, però `1 mod 6 = 1` és fora del cicle.

- **\"Cada modulus dóna longitud de cicle igual al modulus\":** NO! Per exemple, mòdul 5, el cicle de `2^n` té longitud 4, no 5. Longitudes varient en 1, 2, 3, 4... depenen de la base i modulus.

- **\"Assumir que una vegada un valor es repeteix, la seqüència acaba\":** Fals! Quan veus `2^5 mod 5 = 2` (igual que `2^1 mod 5 = 2`), NO has acabat. El cicle continua: `2^6 mod 5 = 4` (igual que `2^2`), i així successivament. El cicle es **repeteix infinitament**.

- **\"La primera repetició determina l'inici del cicle\":** Si `a^i ≡ a^j (mod m)` amb `i < j`, aleshores la longitud del cicle és `j - i`, però el cicle pot no começar a `i`. Per exemple, si `a^2 = a^5` (mòdul), el cicle té longitud 3, però pot comenzar abans de la posició 2.

🔹 **Aplicacions Reals:**
- **Predicció a llarg termini:** Si saps que una seqüència té cicle, pots predir el valor en el milió-èssim pas sense calcular-lo. Per exemple, si `2^n mod 5` té cicle 4 i vols `2^1000000 mod 5`:
  - `1000000 mod 4 = 0`, que mapeja al 4t element del cicle [2, 4, 3, 1], que és 1.
  - Resposta: `2^1000000 ≡ 1 (mod 5)`.

- **Criptografia de clau pública:** Els sistemes RSA es basen en la dificultat de trobar la longitud del cicle de `a^n mod p` per a `p` primer. Si poguessis trobar aquest cicle ràpidament, podrías trencar l'encriptació.

- **Detecció de patrons en dades:** Els científics de dades usan aritmètica modular per detectar cicles en dades temporals (weather patterns, stock markets, comportament de portals).

- **Generadors de nombres pseudo-aleatories:** Els algoritmes com el "Linear Congruential Generator" es basen en cicles modulars per generar seqüències que "semblan" aleatòries pero són previsibles.

- **Programes de "repeat every N days":** Si una tasca es repeteix cada 29 dies (cicle lunar), i vols saber quan es completa per a la tasca 10000:
  - Dia = `10000 mod 29 = 14`. Resposta: es completa en la 14a tasca de cada cicle.

- **Música i ritme:** La música occidental té cicles de 12 tonos (mod 12). Els compositors usan cicles de 4, 8, 16 compases para crear estructura. Totes aquestes són aritmètica modular!

- **Sabies que...?** Els primers de Mersenne (primers de la forma `2^p - 1`) es troben buscant patrons de cicles! Els científics usan la teoria de cicles modulars per a identificar quins exponents `p` podrien produir primers. El nombre primer més gran conhecut és un primer de Mersenne amb més de 24 milions de dígits!



# Paraules clau
Conjunt, element, notació, claus, pertinença, subconjunt, subconjunt propi, Venn, conjunt buit, ℕ, ℤ, ℚ, jerarquia, valor posicional, forma desenvolupada, notació científica, divisibilitat, primer, compost, garbell, MCD, algoritme d'Euclides, MCM, factorització, nombres perfectes, nombres triangulars, Fibonacci, aritmètica modular, congruència, patrons de resta
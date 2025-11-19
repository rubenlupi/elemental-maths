Conjunts, notació, pertinença, subconjunts, conjunts de nombres bàsics (ℕ, ℤ, ℚ), valor posicional, notació científica, divisibilitat, nombres primers, MCD/MCM, nombres especials, aritmètica modular introductòria.

Paraules clau: conjunt, element, notació, claus, pertinença, subconjunt, subconjunt propi, Venn, conjunt buit, ℕ, ℤ, ℚ, jerarquia, valor posicional, forma desenvolupada, notació científica, divisibilitat, primer, compost, garbell, MCD, algoritme d'Euclides, MCM, factorització, nombres perfectes, nombres triangulars, Fibonacci, aritmètica modular, congruència, patrons de resta

Blocs:
1 Conjunts i notació bàsica
2 Subconjunts, subconjunts propis, visuals de Venn
3 Jerarquia de conjunts de nombres ℕ→ℤ→ℚ
4 Valor posicional i formes desenvolupades
5 Introducció a la notació científica
6 Pràctica de regles de divisibilitat
7 Primer/compost + mètode del garbell
8 Aplicacions MCD (Euclides)
9 MCM via factors primers
10 Factorització i teorema fonamental
11 Nombres especials (perfectes, triangulars, Fibonacci)
12 Concepte d'aritmètica modular (a ≡ b mod n)
13 Exploració de patrons de resta
14 Consolidació mixta i repàs

#### Teoria

##### Bloc 1 – Conjunts i Notació Bàsica
🔹 **Definició:** Un **conjunt** és una col·lecció ben definida d'objectes diferents anomenats **elements**; escrivim conjunts amb claus com `A = {1, 2, 3}` i mostrem la pertinença amb `∈`.

🔹 **Exemples:**
- `B = {vermell, blau, verd}` llista tres colors; `blau ∈ B` però `groc ∉ B`.
- El conjunt `C = {n | n és un nombre sencer parell}` utilitza notació de conjunt comprensiu per a tots els nombres parells `0, 2, 4, ...`.
- Contraexemple: `{1, 1, 2}` és escrit malament perquè els conjunts no repeteixen elements; escriu `{1, 2}` en lloc d'això.

🔹 **Notació Matemàtica:**
- `{ }` tanca els elements; la barra `|` o dos punts `:` significa "tal que" en forma de conjunt comprensiu.
- `x ∈ S` es llegeix "`x` pertany a `S`"; `x ∉ S` es llegeix "`x` no pertany a `S`".
- Les lletres majúscules (`S`, `T`) anomenen conjunts; les lletres minúscules (`a`, `x`) anomenen elements.

🔹 **Representacions Visuals:**
```
S = {⚽, 🏀, 🎾}
Índex:   1   2   3
```
```
Idea de recta numèrica per a nombres parells:
<---•---•---•---•--->
	0   2   4   6
```

🔹 **Conjunt Buit i Casos Especials:**
- El **conjunt buit** `∅` (també escrit `{ }`) no conté elements; és un conjunt vàlid i és subconjunt de tots els conjunts.
- Exemple: `{x | x és un nombre sencer i x < 0} = ∅` (no hi ha nombres sencers negatius).
- Distinció important: El conjunt `{∅}` conté un element (el conjunt buit en si) i **no** és buit; `|{∅}| = 1`.
- Contraexemple: Confondre `∅` amb `{0}` (que conté l'element `0`) és un error comú.

🔹 **Propietats o Regles Clau:**
- L'ordre no importa: `{1, 2, 3}` és igual a `{3, 2, 1}`. Aquesta és la **propietat commutativa per a conjunts**.
- Els elements apareixen una vegada; els duplicats es col·lapsen en entrades úniques.
- Els conjunts poden ser finits o infinits segons quants elements contenen.
- **Propietat Commutativa per a la Unió:** `A ∪ B = B ∪ A` (l'ordre dels conjunts no afecta la unió).
- **Propietat Commutativa per a la Intersecció:** `A ∩ B = B ∩ A` (l'ordre dels conjunts no afecta la intersecció).
- **Propietat del conjunt buit:** `∅ ⊆ S` per a qualsevol conjunt `S`.

🔹 **Exemples Detallats amb Unió i Intersecció:**
- Sigui `A = {1, 2, 3}` i `B = {2, 3, 4}`.
  - Unió: `A ∪ B = {1, 2, 3, 4}` (tots els elements dels dos conjunts, llistats una vegada).
  - També: `B ∪ A = {2, 3, 4, 1} = {1, 2, 3, 4}` (mateix resultat, mostrant commutativitat).
  - Intersecció: `A ∩ B = {2, 3}` (elements que apareixen a ambdós).
  - També: `B ∩ A = {2, 3}` (mateix resultat).
- Sigui `C = {5, 6}` i `D = {7, 8}`.
  - Unió: `C ∪ D = {5, 6, 7, 8}`.
  - Intersecció: `C ∩ D = ∅` (cap element comú; el resultat és el conjunt buit).
- Contraexemple: `{a, b} ∪ ∅ = {a, b}` (unió amb conjunt buit retorna el conjunt original incanviat).

🔹 **Malentesos Comuns:**
- Pensar que `{2, 4, 6, ...}` ha d'acabar-se; les punts suspensius significa que continua per sempre.
- Confondre elements amb subconjunts; `{1, 2}` és un subconjunt de `{1, 2, 3}`, mentre que `1` és un element.
- Assumir que reorganitzar elements canvia el conjunt, de manera que `{1, 2, 3}` i `{3, 2, 1}` es veu com a diferents.

🔹 **Connexions:**
- Organitza conjunts de nombres com `ℕ`, `ℤ` i `ℚ` més tard al mòdul.
- Suporta diagrames de Venn revisitats al Mòdul 18.

🔹 **Aplicacions i Trucs de Memòria:**
- Categoritzar estudiants per pertinença a club utilitza conjunts.
- Consell: Imagina cada conjunt com a una "carpeta de matemàtiques" etiqu etada que conté objectes relacionats.

##### Bloc 2 – Subconjunts i Visuals de Venn
🔹 **Definició:** Un **subconjunt** `A ⊆ B` significa que tots els elements d'`A` pertanyen a `B`. Un **subconjunt propi** `A ⊂ B` requereix addicionalment que `A ≠ B`.

🔹 **Exemples:**
- Si `B = {1, 2, 3, 4}`, aleshores `A = {2, 4}` és un subconjunt ja que tots els seus elements apareixen en `B`.
- `∅ ⊆ B` perquè el conjunt buit no té elements que trenqui la pertinença.
- Contraexemple: `{5}` no és un subconjunt de `B` perquè `5 ∉ B`.

🔹 **Notació Matemàtica:**
- `A ⊆ B` (subconjunt), `A ⊂ B` (subconjunt propi), `A ⊄ B` (no és un subconjunt).
- El conjunt buit `∅` (també `{ }`) no conté elements.

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
- Tot conjunt és subconjunt de si mateix (`B ⊆ B`).
- Un conjunt amb `n` elements té `2^n` subconjunts.
- La relació de subconjunt és transitiva: si `A ⊆ B` i `B ⊆ C`, aleshores `A ⊆ C`.

🔹 **Malentesos Comuns:**
- Creure que un subconjunt ha de ser més petit; la igualtat encara comptes.
- Oblidar que `∅` és un subconjunt de tots els conjunts.
- Tractar un element llistat `5 ∈ B` com si `{5}` fos automàticament un subconjunt sense confirmar pertinença.

🔹 **Connexions:**
- Construeix la jerarquia de nombres `ℕ ⊂ ℤ ⊂ ℚ` al Bloc 3.
- Suporta comparacions d'esdeveniments de probabilitat (Mòdul 17).

🔹 **Aplicacions i Trucs de Memòria:**
- **Jerarquies organitzatives:** Gerents ⊂ Empleats; Metges ⊂ Personal hospitalari; Membres Premium ⊂ Tots els Membres.
- **Formes geomètriques:** Quadrats ⊂ Rectangles ⊂ Paral·lelograms (cadascun és un subconjunt propi del següent).
- **Categories d'aliments:** Verdures ⊂ Productes Frescos; Plats Italians ⊂ Menú de Restaurant.
- **Gestió de dispositius:** Telèfons Intel·ligents ⊂ Dispositius Mòbils; Cotxes Elèctrics ⊂ Tots els Vehicles.
- **Nivells de permisos en programari:** Administradors ⊂ Usuaris Avançats ⊂ Usuaris Normals (la cadena de subconjunts propis determina l'accés).
- **Aplicacions mèdiques:** Pacients diabètics ⊂ Pacients amb malaltia crònica—l'anàlisi de subconjunts ajuda els hospitals a assignar recursos.
- Recorda: El símbol de subconjunt propi `<` té una aresta aguda recordant-nos que els conjunts difereixen.

##### Bloc 3 – Jerarquia de Conjunts de Nombres ℕ→ℤ→ℚ
🔹 **Definició:** La **jerarquia de nombres** és l'imbricació de conjunts de nombres on cada conjunt més gran inclou l'anterior: naturals `ℕ`, enters `ℤ`, i racionals `ℚ`.

🔹 **Exemples:**
- `ℕ = {1, 2, 3, ...}` compta nombres sencers positius.
- `ℤ = {..., -2, -1, 0, 1, 2, ...}` estén `ℕ` amb negatius i zero.
- `ℚ` conté cada fracció `a/b` amb enters `a` i `b ≠ 0`, de manera que `3 = 3/1` és també racional.

🔹 **Notació Matemàtica:**
- Cadena d'inclusió: `ℕ ⊂ ℤ ⊂ ℚ`.
- Forma racional: `ℚ = {a/b | a, b ∈ ℤ, b ≠ 0}`.

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
- Tot nombre natural és automàticament un enter i un racional.
- Els racionals són densos: entre dos racionals qualsevol, existeix un altre racional.

🔹 **Malentesos Comuns:**
- Assumir que les fraccions no són racionals; defineixen el conjunt.
- Pensar que `0` ha de estar en `ℕ`; les convencions varien, així que aclareix el context.
- Creure que els decimals repetits com `0.333...` no poden ser racionals tot i que sí que són iguals a fraccions.

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
🔹 **Definició:** El **valor posicional** assigna a cada dígit un valor basat en la seva posició en potències de `10`; la **forma desenvolupada** escriu el nombre com la suma de cada dígit per el seu valor posicional.

🔹 **Exemples:**
- `4,582 = 4×10^3 + 5×10^2 + 8×10^1 + 2×10^0`.
- `307` té `3` centenes, `0` desenes, `7` unitats.
- Contraexemple: Escriure `307 = 3×100 + 7×10` ignora les zero desenes.

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
- Cada lloc és deu vegades el valor del lloc a la seva dreta.
- El zero ocupa un lloc fins i tot sense contribuir valor.

🔹 **Malentesos Comuns:**
- Tirar zeros i canviar magnitud.
- Llegir dígits per separat en lloc de per lloc ("dos zero cinc" per `205`).
- Assumir que la forma desenvolupada ha de llistar només dígits no zero, causant que els estudiants omitgin termes de posició.

🔹 **Connexions:**
- Suporta comprensió de decimals (Mòdul 3) i notació científica.
- Essencial per estratègies de càlcul mental en Mòdul 2.

🔹 **Aplicacions i Trucs de Memòria:**
- Ajuda a interpretar xifres de població o moneda.
- Recorda: "Saltar esquerra multiplica per deu" quan desplaçar dígits.

##### Bloc 5 – Introducció a la Notació Científica
🔹 **Definició:** La **notació científica** expressa nombres com `a × 10^n` amb `1 ≤ |a| < 10` i enter `n`, habilitant representació compacta de quantitats molt grans o petites.

🔹 **Exemples:**
- `5,200,000 = 5.2 × 10^6`.
- `0.00034 = 3.4 × 10^-4`.
- Contraexemple: `52 × 10^5` és inválid perquè el coeficient `52` no està entre `1` i `10`.

🔹 **Notació Matemàtica:**
- `a` és el **coeficient** (o mantissa); `10^n` desplaça el decimal `n` places.
- `n` positiu desplaça decimal esquerra (nombres grans); `n` negatiu desplaça dreta (nombres petits).

🔹 **Representacions Visuals:**
```
5.2 × 10^6 → 5.2 → 52 → 520 → ... → 5,200,000
```

🔹 **Propietats o Regles Clau:**
- `10^a × 10^b = 10^(a+b)`; `10^a / 10^b = 10^(a-b)`.
- Multiplicar nombres en notació científica combina coeficients i suma exponents.

🔹 **Malentesos Comuns:**
- Oblidar d'ajustar exponent quan desplaçar decimal.
- Invertir direcció del signe exponent.
- Pensar que coeficient pot ser zero o excedir `10`, que trenca regles de notació científica.

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
🔹 **Definició:** Una **regla de divisibilitat** és un drecera per determinar si un enter divideix un altre sense divisió completa.

🔹 **Exemples:**
- Un nombre és divisible per `2` si el seu últim dígit és `0, 2, 4, 6, 8`.
- Divisible per `3` si la suma de dígits és múltiple de `3` (`7,524 → 7+5+2+4 = 18`).
- Contraexemple: `123` no és divisible per `4` perquè els últims dos dígits `23` no són divisibles per `4`.

🔹 **Notació Matemàtica:**
- `a | b` significa "`a` divideix `b`"; `a ∤ b` significa que no ho fa.
- Les llistes de regles sovint utilitzen taules per referència ràpida.

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
- Si `a | b` i `b | c`, aleshores `a | c` (transitiva).
- Si `a | b` i `a | c`, aleshores `a | (b ± c)`.

🔹 **Malentesos Comuns:**
- Aplicar la prova equivocada (ex. suma de dígits per `4`).
- Oblidar que divisibilitat per `6` requereix tant `2` com `3`.
- Assumir que les regles de divisibilitat garanteixen primarietat en lloc de només provar factors.

🔹 **Connexions:**
- Porta a primers, MCD i MCM (Blocs 7–9).
- Suporta simplificació de fraccions en Mòdul 5.

🔹 **Aplicacions i Trucs de Memòria:**
- Verificacions ràpides per compartir entre grups.
- Consell: "Six necessita parell i triple" per recordar `6` necessita divisibilitat tant per `2` com `3`.

##### Bloc 7 – Primer/Compost i Mètode del Garbell
🔹 **Definició:** Un **nombre primer** té exactament dos divisors positius distints (`1` i es mateix); un **nombre compost** té més de dos divisors. El **Garbell d'Eratòstenes** filtra primers eliminant múltiples.

🔹 **Exemples:**
- `2, 3, 5, 7` són primers; `4, 6, 9, 12` són compostos.
- `1` no és primer ni compost.
- Contraexemple: Cridar `9` primer ignora `3 × 3`.

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
- L'únic primer parell és `2`.
- Tot enter major que `1` és primer o compost.
- El garbell requereix marcar múltiples començant des de `p^2`.

🔹 **Malentesos Comuns:**
- Pensar que els nombres negatius poden ser primers en el mateix sentit; la definició estàndard usa enters positius.
- Assumir que els nombres grans no poden ser primers.
- Creure que el garbell trova primers per divisió en lloc de sistemàticament colpejar múltiples.

🔹 **Connexions:**
- Factorització primer (Bloc 10) i criptografia (Mòdul 21).
- Apareix en nombres especials de Mòdul 9.

🔹 **Aplicacions i Trucs de Memòria:**
- Utilitzat en teoria de codificació i dades segures.
- Recorda: "Primer significa precisament dos divisors."

##### Bloc 8 – Aplicacions MCD (Euclides)
🔹 **Definició:** El **màxim comú divisor** `gcd(a, b)` és el major enter positiu dividint tant `a` com `b`. L'**algoritme d'Euclides** el encuentra via divisió repetida amb restes.

🔹 **Exemples:**
- `gcd(24, 36) = 12`.
- `gcd(48, 18)` via passos d'Euclides: `48 = 18×2 + 12`, `18 = 12×1 + 6`, `12 = 6×2 + 0`, de manera que `gcd = 6`.
- Contraexemple: Endevinar `9` divideix tant `12` com `18` falla perquè `9 ∤ 12`.

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
- Si `d = gcd(a, b)`, aleshores `a = d·a'` i `b = d·b'` amb `a'`, `b'` coprims.
- Relació amb MCM: `a × b = gcd(a, b) × lcm(a, b)`.

🔹 **Malentesos Comuns:**
- Barrejar MCD amb MCM.
- Neglecting `1` com a possible MCD.
- Esperant que els passos d'Euclides s'aturin quan els nombres coincideixen en lloc que quan la resta colpeja zero.

🔹 **Connexions:**
- Simplifica fraccions (Mòdul 5) i congruències modulars.
- Demostra pensament algorítmic rellevant a estratègies de Mòdul 19.

🔹 **Aplicacions i Trucs de Memòria:**
- Utilitzat en agrupació d'elements equitativament o sincronització de cicles.
- Consell: "Màxim Comú Divideix" resumeix el seu significat.

##### Bloc 9 – MCM via Factors Primers
🔹 **Definició:** El **mínim comú múltiple** `lcm(a, b)` és el menor enter positiu divisible tant per `a` com per `b`, sovint descobert usant factorització primera.

🔹 **Exemples:**
- `lcm(4, 6) = 12`.
- `lcm(8, 12, 15) = 120` (factors primers `2^3`, `3`, `5`).
- Contraexemple: Triar `24` com `lcm(4, 6)` és incorrecte perquè `12` és menor.

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
- Simètric: `lcm(a, b) = lcm(b, a)`.
- Si `a | b`, aleshores `lcm(a, b) = b`.

🔹 **Malentesos Comuns:**
- Aturar-se en qualsevol múltiple comú en lloc del menor.
- Oblidar d'incloure totes les potències primers.
- Assumir que el mínim comú múltiple ha de ser el producte dels nombres fins i tot quan comparteixen factors.

🔹 **Connexions:**
- Essencial per denominadors comuns (Mòdul 5).
- Suporta problemes de programació (Mòdul 19).

🔹 **Aplicacions i Trucs de Memòria:**
- Sincronitzar esdeveniments, com horaris de classes o cicles de semàfor.
- Recorda: "Menor significa primer partit, després atura't."

##### Bloc 10 – Factorització i Teorema Fonamental
🔹 **Definició:** La **factorització primera** descompon un enter en factors primers. El **Teorema Fonamental de l'Aritmètica** estableix que tot enter major que `1` té una única factorització primera (fins l'ordre).

🔹 **Exemples:**
- `60 = 2^2 × 3 × 5`.
- `84 = 2^2 × 3 × 7`.
- Contraexemple: `45 = 3 × 15` és incomplet perquè `15` no és primer; factorització completa `3^2 × 5`.

🔹 **Notació Matemàtica:**
- Arbres de factors, exponents (`p^k`).
- Unicitat: si `n = p_1^{a_1} ... p_k^{a_k} = q_1^{b_1} ... q_m^{b_m}`, aleshores `k = m` i els primers coincideixen amb exponents idèntics.

🔹 **Representacions Visuals:**
```
   60
  /  \
 6   10
 /\  / \
2 3 2  5
```

🔹 **Propietats o Regles Clau:**
- Multiplicar primers idèntics suma exponents.
- La factorització primera suporta MCD/MCM via exponents mín/màx.

🔹 **Malentesos Comuns:**
- Aturar-se en factors compostos.
- Creure que `1` té factors primers; no ho té.
- Pensar que diferents disposicions d'arbre de factors produeixen factoritzacions primers diferents en lloc del mateix multiconjunt de primers.

🔹 **Connexions:**
- Construeix habilitats d'exponent (Mòdul 6) i teoria de nombres (Mòdul 9).
- Assistent en simplificació de radicals (Mòdul 6).

🔹 **Aplicacions i Trucs de Memòria:**
- **Criptografia:** La seguretat de l'encriptació RSA depèn de factoritzar nombres com 143 = 11 × 13; l'encriptació moderna usa compostos de 2048-bits (>600 dígits).
- **Simplificació de fraccions:** 60/84 = (2² × 3 × 5)/(2² × 3 × 7) = 5/7 usant factorització primera.
- **Disseny i manufactura:** Crear productes modulars—si unitat bàsica = 2² × 3 = 12 cm, variants (12, 24, 36, 48 cm) escalen predictablement.
- **Informàtica:** L'optimització de compilador usa factorització per rescriure estructures de bucle eficientment.
- **Harmonia musical:** Els ràtios de freqüència com 5/4 (tercera major justa) emergeixen de factoritzacions primeres de freqüències de nota.
- **Compressió de dades:** La codificació de Huffman assigna patrons de bits basats en factoritzacions de freqüència per compressió òptima.
- **Finances:** Els càlculs d'interès compost depenen de factoritzar per trobar taxes de creixement igualant inversions objectiu.
- **Sabies que...?** L'encriptació moderna depèn de la dificultat de factoritzar nombres enormes. Trencar RSA-2048 requereria factoritzar un nombre de 617-dígits—estimat portar segles!

##### Bloc 11 – Nombres Especials (Perfectes, Triangulars, Fibonacci)
🔹 **Definició:** Els **nombres perfectes** sumen els seus divisors propis; els **nombres triangulars** compten punts formant triangles equilàters; la **seqüència de Fibonacci** té cada terme igual a la suma dels dos termes anteriors (`F_n = F_{n-1} + F_{n-2}`).

🔹 **Exemples:**
- Perfectes: `6 = 1 + 2 + 3`, `28 = 1 + 2 + 4 + 7 + 14`.
- Triangulars: `T_4 = 10` formant un triangle de `4` files.
- Fibonacci: `0, 1, 1, 2, 3, 5, 8, ...`; contraexemple: `9` no és triangular ja que `n(n+1)/2 ≠ 9` per enter `n`.

🔹 **Notació Matemàtica:**
- Nombres triangulars `T_n = n(n + 1)/2`.
- Recursió de Fibonacci amb `F_0 = 0`, `F_1 = 1`.
- Verificació de nombre perfecte via suma de divisor `σ(n) - n = n`.

🔹 **Representacions Visuals:**
```
Punts triangulars (T4):
•
••
•••
••••
```
```
Quadrats de Fibonacci formant espiral: 1×1, 1×1, 2×2, 3×3, 5×5.
```

🔹 **Propietats o Regles Clau:**
- Els nombres perfectes parells segueixen `2^{p-1}(2^p - 1)` quan `2^p - 1` és primer (primer de Mersenne).
- `T_n = C(n + 1, 2)` connecta a combinacions.
- Els ràtios de Fibonacci aproximen la secció àuria `≈ 1.618`.

🔹 **Malentesos Comuns:**
- Assumir que els nombres triangulars són nombres perfectes; són seqüències distintes.
- Tractar Fibonacci com aritmètica (diferència fixa) en lloc de suma recursiva.
- Creure que Fibonacci ha de començar amb `1, 1` i ignorant la convencional `0, 1` utilitzada en moltes fórmules.

🔹 **Connexions:**
- Enllaça a combinatòria (Mòdul 20) i patrons (Mòdul 10).
- Fibonacci apareix en discussions de creixement exponencial (Mòdul 6).

🔹 **Aplicacions i Trucs de Memòria:**
- Apareix en arquitectura, natura (pinyes, girasols).
- Recorda: "Triangular `T` apila `n` i `n+1`, després divideix a la meitat."

##### Bloc 12 – Concepte d'Aritmètica Modular (a ≡ b mod n)
🔹 **Definició:** L'**aritmètica modular** compara nombres per restes: `a ≡ b (mod n)` quan `n` divideix `a - b`.

🔹 **Exemples:**
- `17 ≡ 5 (mod 12)` perquè `17 - 5 = 12`.
- `9 ≡ 1 (mod 4)` ja que ambdós deixen resta `1` en divisió per `4`.
- Contraexemple: `14 ≡ 3 (mod 4)` és fals perquè `14 - 3 = 11`, que `4` no divideix.

🔹 **Notació Matemàtica:**
- Símbol de congruència `≡`; modulus anotat `(mod n)`.
- Classe de resta `[a]_n` representa tots els enters congruents a `a` mòdul `n`.

🔹 **Representacions Visuals:**
```
Rellotge (mod 12):
1 ↔ 13 ↔ 25 ↔ ... tots ≡ 1 (mod 12)
```
```
Taula de resta mod 5
n | n mod 5
0 | 0
1 | 1
2 | 2
3 | 3
4 | 4
5 | 0
```

🔹 **Propietats o Regles Clau:**
- Si `a ≡ b (mod n)` i `c ≡ d (mod n)`, aleshores `a ± c ≡ b ± d (mod n)` i `ac ≡ bd (mod n)`.
- Les restes negatives embolcallen: `-1 ≡ n - 1 (mod n)`.

🔹 **Malentesos Comuns:**
- Tractar `mod` com divisió en lloc de comparació de resta.
- Oblidar de reduir restes al rang `0` a `n - 1`.
- Assumir que els nombres congruents han de ser propers en tamany en lloc de diferir per múltiples del modulus.

🔹 **Connexions:**
- Suporta lògica de divisibilitat i patrons cíclics (Bloc 13).
- Retorna en enriquiment Mòdul 21 i contextos de criptografia.

🔹 **Aplicacions i Trucs de Memòria:**
- **Aritmètica de rellotge:** 14:00 (2:00 PM) + 11 hores = 1:00 AM (25 ≡ 1 mod 12).
- **Predicció de dia de setmana:** Si avui és dimecres (dia 3) + 10 dies ≡ 13 ≡ 6 (mod 7) = dissabte.
- **Gràfics per ordinador:** Els canals de color utilitzen mod 256 per mantenir valors RGB en rang [0, 255].
- **Codis de seguretat:** Els dígits de verificació de targeta de crèdit utilitzen aritmètica mod 10 (algoritme de Luhn) per detectar errors.
- **Inventari de magatzem:** Els contenidors numerats 0–49; el codi de barres d'article 1537 va al contenidor 1537 mod 50 = 37.
- **Programació:** Repetir cada 29 dies (cicle lunar), la tasca del dia 100 és igual a la tasca del dia 100 mod 29 = 13.
- **Jocs en línia:** Els IDs de jugador assignats usant mod per equilibri de càrrega entre múltiples instàncies de joc.
- Recorda: "L'aritmètica modular embolcalla—com una cara de rellotge."

🔹 **Aplicacions i Trucs de Memòria:**
- Ajuda a calcular dies de la setmana, temps de rellotge, dígits de verificació de suma.
- **Sabies que...?** Les notes musicals embolcallen octaves com aritmètica mod `12`.

##### Bloc 13 – Exploració de Patrons de Resta
🔹 **Definició:** Un **patró de resta** rastreja les restes repetides quan els nombres es divideixen per un modulus fix, revelant cicles.

🔹 **Exemples:**
- Potències de `2 mod 5`: `2, 4, 3, 1` repetint cada `4` passos.
- Múltiples de `7 mod 3`: les restes `1, 2, 0, 1, 2, 0, ...`.
- Contraexemple: Reclamar `2^n mod 5` sempre iguals `2` ignora el cicle.

🔹 **Notació Matemàtica:**
- Seqüències `(a_n)` amb `a_n ≡ k (mod m)`.
- El període denota la longitud del cicle.

🔹 **Representacions Visuals:**
```
Roda de resta mod 5 per a potències de 2
2 → 4 → 3 → 1 → (retorn a 2)
```
```
Taula:
n | 2^n mod 5
1 | 2
2 | 4
3 | 3
4 | 1
5 | 2
```

🔹 **Propietats o Regles Clau:**
- Els moduli finits garanteixen eventual repetició (Principi de Pigeonhole).
- La longitud del cicle per a potències es relaciona amb la totient d'Euler `φ(n)` quan la base i el modulus són coprims.

🔹 **Malentesos Comuns:**
- Esperant que els cicles comencin a `n = 0`; els termes inicials poden diferir.
- Creure que cada modulus rend una longitud de cicle igual al modulus sense verificar ordre real.
- Assumir que una vegada un valor es repeteix, la seqüència acaba immediatament en lloc de continuar amb el cicle establert.

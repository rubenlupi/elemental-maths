### Mòdul 1: Fonaments dels Sistemes Numèrics (≈4.5h)
Conjunts, notació, pertinença, subconjunts, conjunts numèrics bàsics (ℕ, ℤ, ℚ), valor posicional, notació científica, divisibilitat, primers, MCD/MCM, nombres especials, aritmètica modular introductòria.

Paraules clau: conjunt, element, notació, claus, pertinença, subconjunt, subconjunt propi, Venn, conjunt buit, ℕ, ℤ, ℚ, jerarquia, valor posicional, forma desenvolupada, notació científica, divisibilitat, primer, compost, garbell, MCD, algoritme d’Euclides, MCM, factorització, nombres perfectes, nombres triangulars, Fibonacci, aritmètica modular, congruència, patrons de residus

Blocs:
1 Conjunts i notació bàsica
2 Subconjunts, subconjunts propis, visuals de Venn
3 Jerarquia de conjunts numèrics ℕ→ℤ→ℚ
4 Valor posicional i formes desenvolupades
5 Introducció a la notació científica
6 Pràctica de regles de divisibilitat
7 Nombres primers/compostos i mètode del garbell
8 Aplicacions del MCD (algoritme d’Euclides)
9 MCM a través de factors primers
10 Factorització i teorema fonamental
11 Nombres especials (perfectes, triangulars, Fibonacci)
12 Concepte d’aritmètica modular (a ≡ b mod n)
13 Exploració de patrons de residus
14 Consolidació i repàs mixt

#### Teoria

##### Bloc 1 – Conjunts i Notació Bàsica
🔹 **Definició:** Un **conjunt** és una col·lecció ben definida d’objectes diferents anomenats **elements**; escrivim conjunts amb claus com `A = {1, 2, 3}` i mostrem pertinença amb `∈`.

🔹 **Exemples:**
- `B = {vermell, blau, verd}` llista tres colors; `blau ∈ B` però `groc ∉ B`.
- El conjunt `C = {n | n és un nombre parell enter}` utilitza notació de comprensió per a tots els nombres parells `0, 2, 4, ...`.
- Contraexemple: `{1, 1, 2}` està mal escrit perquè als conjunts no es repeteixen els elements; escriu `{1, 2}`.

🔹 **Notació Matemàtica:**
- `{ }` envolta els elements; la barra `|` o dos punts `:` significa “tal que” en forma de comprensió.
- `x ∈ S` es llegeix “`x` pertany a `S`”; `x ∉ S` es llegeix “`x` no pertany a `S`”.
- Les lletres majúscules (`S`, `T`) designen conjunts; les minúscules (`a`, `x`) designen elements.

🔹 **Representacions Visuals:**
```
S = {⚽, 🏀, 🎾}
Índex: 1 2 3
```
```
Idea de recta numèrica per als nombres parells:
<---•---•---•---•--->
 0  2  4  6
```

🔹 **Propietats o Regles Clau:**
- L’ordre no importa: `{1, 2, 3}` és igual a `{3, 2, 1}`.
- Els elements apareixen una sola vegada; les repeticions es redueixen a una única entrada.
- Els conjunts poden ser finits o infinits segons el nombre d’elements que contenen.

🔹 **Concepcions Errònies Habituals:**
- Pensar que `{2, 4, 6, ...}` ha d’acabar; els punts suspensius indiquen que continua indefinidament.
- Confondre elements amb subconjunts; `{1, 2}` és un subconjunt de `{1, 2, 3}`, mentre que `1` és un element.

🔹 **Connexions:**
- Organitza conjunts numèrics com `ℕ`, `ℤ` i `ℚ` més endavant al mòdul.
- Dona suport als diagrames de Venn que es reprenen al Mòdul 18.

🔹 **Aplicacions i Records Mnemotècnics:**
- Clasificar estudiants per pertinença a clubs utilitza conjunts.
- Consell: Visualitza cada conjunt com una “carpeta matemàtica” etiquetada que conté objectes relacionats.

##### Bloc 2 – Subconjunts i Visualitzacions de Venn
🔹 **Definició:** Un **subconjunt** `A ⊆ B` significa que cada element de `A` pertany a `B`. Un **subconjunt propi** `A ⊂ B` requereix a més que `A ≠ B`.

🔹 **Exemples:**
- Si `B = {1, 2, 3, 4}`, llavors `A = {2, 4}` és un subconjunt perquè tots els seus elements apareixen a `B`.
- `∅ ⊆ B` perquè el conjunt buit no conté elements que trenquin la pertinença.
- Contraexemple: `{5}` no és subconjunt de `B` perquè `5 ∉ B`.

🔹 **Notació Matemàtica:**
- `A ⊆ B` (subconjunt), `A ⊂ B` (subconjunt propi), `A ⊄ B` (no subconjunt).
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
- Cada conjunt és subconjunt de si mateix (`B ⊆ B`).
- Un conjunt amb `n` elements té `2^n` subconjunts.
- La relació de subconjunt és transitiva: si `A ⊆ B` i `B ⊆ C`, aleshores `A ⊆ C`.

🔹 **Concepcions Errònies Habituals:**
- Creure que un subconjunt ha de ser més petit; la igualtat també compta.
- Oblidar que `∅` és subconjunt de qualsevol conjunt.

🔹 **Connexions:**
- Construeix la jerarquia de nombres `ℕ ⊂ ℤ ⊂ ℚ` del Bloc 3.
- Dona suport a la comparació d’esdeveniments en probabilitat (Mòdul 17).

🔹 **Aplicacions i Records Mnemotècnics:**
- S’utilitza quan s’organitzen famílies de formes geomètriques (rectangles dins de paral·lelograms).
- Recorda: El símbol de subconjunt propi `<` té una vora afilada que recorda que els conjunts són diferents.

##### Bloc 3 – Jerarquia de Conjunts Numèrics ℕ→ℤ→ℚ
🔹 **Definició:** La **jerarquia numèrica** és l’anidament de conjunts numèrics on cada conjunt més gran inclou l’anterior: naturals `ℕ`, enters `ℤ` i racionals `ℚ`.

🔹 **Exemples:**
- `ℕ = {1, 2, 3, ...}` compta nombres naturals positius.
- `ℤ = {..., -2, -1, 0, 1, 2, ...}` amplia `ℕ` amb negatius i zero.
- `ℚ` conté qualsevol fracció `a/b` amb enters `a` i `b ≠ 0`, així `3 = 3/1` també és racional.

🔹 **Notació Matemàtica:**
- Cadena d’inclusió: `ℕ ⊂ ℤ ⊂ ℚ`.
- Forma racional: `ℚ = {a/b | a, b ∈ ℤ, b ≠ 0}`.

🔹 **Representacions Visuals:**
```
[ℚ]
 └─[ℤ]
    └─[ℕ]
```
```
Recta numèrica:
... -2 -1 0 1 2 ... | afegeix fraccions entre enters per ℚ
```

🔹 **Propietats o Regles Clau:**
- Cada nombre natural és automàticament enter i racional.
- Els racionals són densos: entre qualsevol parell de racionals n’hi ha un altre.

🔹 **Concepcions Errònies Habituals:**
- Assumir que les fraccions no són racionals; en són la definició.
- Pensar que `0` ha d’estar a `ℕ`; les convencions varien, cal aclarir-ho.

🔹 **Connexions:**
- Prepara per als decimals (Mòdul 3) i sistemes ampliats (Mòdul 4).
- Dona suport a operacions amb fraccions al Mòdul 5.

🔹 **Aplicacions i Records Mnemotècnics:**
- Útil quan es trien nombres adequats per a mesures o comptatges.
- Consell: Visualitza caixes anidades etiquetades `ℕ`, `ℤ`, `ℚ` per recordar la inclusió.

##### Bloc 4 – Valor Posicional i Formes Desenvolupades
🔹 **Definició:** El **valor posicional** assigna a cada dígit un valor segons la seva posició en potències de `10`; la **forma desenvolupada** escriu el nombre com la suma de cada dígit multiplicat pel seu valor posicional.

🔹 **Exemples:**
- `4.582 = 4×10^3 + 5×10^2 + 8×10^1 + 2×10^0`.
- `307` té `3` centenes, `0` desenes, `7` unitats.
- Contraexemple: Escriure `307 = 3×100 + 7×10` ignora les desenes nul·les.

🔹 **Notació Matemàtica:**
- La notació posicional usa potències de deu: dígit `d_k × 10^k`.
- Forma desenvolupada: `2.045 = 2×10^3 + 4×10^1 + 5×10^0`.

🔹 **Representacions Visuals:**
```
Mil·lars | Centenes | Desenes | Unitats
   4          5          8         2
```
```
Blocs base-10: [■■■■] miler, [□□□□□] centenes, etc.
```

🔹 **Propietats o Regles Clau:**
- Cada posició val deu vegades la posició de la dreta.
- El zero manté el lloc encara que no aporti valor.

🔹 **Concepcions Errònies Habituals:**
- Ometre zeros i canviar l’ordre de magnitud.
- Llegir dígits per separat en lloc de per posició (“dos zero cinc” per `205`).

🔹 **Connexions:**
- Dona suport a la comprensió dels decimals (Mòdul 3) i a la notació científica.
- Essencial per a estratègies de càlcul mental al Mòdul 2.

🔹 **Aplicacions i Records Mnemotècnics:**
- Ajuda a interpretar xifres de població o moneda.
- Recorda: “Un salt a l’esquerra multiplica per deu” quan desplacem dígits.

##### Bloc 5 – Introducció a la Notació Científica
🔹 **Definició:** La **notació científica** expressa nombres com `a × 10^n` amb `1 ≤ |a| < 10` i `n` enter, facilitant representar valors molt grans o petits.

🔹 **Exemples:**
- `5.200.000 = 5,2 × 10^6`.
- `0,00034 = 3,4 × 10^-4`.
- Contraexemple: `52 × 10^5` és invàlid perquè el coeficient `52` no és entre `1` i `10`.

🔹 **Notació Matemàtica:**
- `a` és el **coeficient** (o mantissa); `10^n` desplaça el decimal `n` llocs.
- `n` positiu mou el decimal cap a l’esquerra (nombres grans); `n` negatiu el mou cap a la dreta (nombres petits).

🔹 **Representacions Visuals:**
```
5,2 × 10^6 → 5,2 → 52 → 520 → ... → 5.200.000
```

🔹 **Propietats o Regles Clau:**
- `10^a × 10^b = 10^(a+b)`; `10^a / 10^b = 10^(a-b)`.
- Multiplicar nombres en notació científica combina coeficients i suma exponents.

🔹 **Concepcions Errònies Habituals:**
- Oblidar ajustar l’exponent quan es mou el decimal.
- Invertir el signe de l’exponent.

🔹 **Connexions:**
- Enllaça amb les lleis dels exponents (Mòdul 6) i escales de mesura (Mòdul 8).
- Essencial per representar dades científiques (Mòdul 16).

🔹 **Aplicacions i Records Mnemotècnics:**
- S’utilitza en astronomia, química, finances per comparar valors extrems.
- Sabies que...? La distància al Sol és aproximadament `1,5 × 10^8 km`.

##### Bloc 6 – Pràctica de Regles de Divisibilitat
🔹 **Definició:** Una **regla de divisibilitat** és un truc per determinar si un enter divideix un altre sense fer la divisió completa.

🔹 **Exemples:**
- Un nombre és divisible per `2` si l’últim dígit és `0, 2, 4, 6, 8`.
- Divisible per `3` si la suma de dígits és múltiple de `3` (`7.524 → 7+5+2+4 = 18`).
- Contraexemple: `123` no és divisible per `4` perquè els dos últims dígits `23` no són múltiples de `4`.

🔹 **Notació Matemàtica:**
- `a | b` significa “`a` divideix `b`”; `a ∤ b` significa que no ho fa.
- Les llistes de regles sovint empren taules de consulta ràpida.

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
- Si `a | b` i `b | c`, aleshores `a | c` (transitivitat).
- Si `a | b` i `a | c`, aleshores `a | (b ± c)`.

🔹 **Concepcions Errònies Habituals:**
- Aplicar la prova equivocada (p. ex., suma de dígits per a `4`).
- Oblidar que la divisibilitat per `6` requereix complir les de `2` i `3`.

🔹 **Connexions:**
- Porta als nombres primers, MCD i MCM (Blocs 7–9).
- Dona suport a la simplificació de fraccions al Mòdul 5.

🔹 **Aplicacions i Records Mnemotècnics:**
- Comprovacions ràpides per compartir en parts iguals.
- Consell: “Sis requereix parell i triple” per recordar que `6` demana divisibilitat per `2` i `3`.

##### Bloc 7 – Nombres Primers/Compostos i Garbell d’Eratòstenes
🔹 **Definició:** Un **nombre primer** té exactament dos divisors positius distintius (`1` i ell mateix); un **nombre compost** en té més de dos. El **Garbell d’Eratòstenes** filtra primers eliminant múltiples.

🔹 **Exemples:**
- `2, 3, 5, 7` són primers; `4, 6, 9, 12` són compostos.
- `1` no és primer ni compost.
- Contraexemple: Dir que `9` és primer ignora `3 × 3`.

🔹 **Notació Matemàtica:**
- `p ∈ ℕ`, `p > 1`, `d | p ⇒ d ∈ {1, p}`.
- El garbell marca seqüencialment múltiples de cada primer descobert.

🔹 **Representacions Visuals:**
```
1  2  3  4  5  6  7  8  9 10
   P  P  X  P  X  P  X  X  X
P = primer, X = múltiple eliminat
```
```
Arbre de factors de 12:
   12
  /  \
 3    4
     / \
    2   2
```

🔹 **Propietats o Regles Clau:**
- L’únic primer parell és `2`.
- Cada enter més gran que `1` és primer o compost.
- El garbell requereix marcar múltiples a partir de `p^2`.

🔹 **Concepcions Errònies Habituals:**
- Pensar que els nombres negatius poden ser primers en el mateix sentit; la definició estàndard usa enters positius.
- Assumir que els nombres grans no poden ser primers.

🔹 **Connexions:**
- Factorització prima (Bloc 10) i criptografia (Mòdul 21).
- Apareix en nombres especials del Mòdul 9.

🔹 **Aplicacions i Records Mnemotècnics:**
- Usats en teoria de codis i seguretat de dades.
- Recorda: “Primer significa precisament dos divisors”.

##### Bloc 8 – Aplicacions del MCD (Algoritme d’Euclides)
🔹 **Definició:** El **màxim comú divisor** `mcd(a, b)` és el nombre positiu més gran que divideix `a` i `b`. L’**algoritme d’Euclides** el troba amb divisions successives amb residu.

🔹 **Exemples:**
- `mcd(24, 36) = 12`.
- `mcd(48, 18)` amb passos euclidians: `48 = 18×2 + 12`, `18 = 12×1 + 6`, `12 = 6×2 + 0`, així que `mcd = 6`.
- Contraexemple: Endevinar que `9` divideix `12` i `18` falla perquè `9 ∤ 12`.

🔹 **Notació Matemàtica:**
- `mcd(a, b) = mcd(b, a mod b)` iterant fins que el residu és `0`.
- `mcd(a, b, c)` és abreviatura de `mcd(a, mcd(b, c))`.

🔹 **Representacions Visuals:**
```
Escala euclidiana per a mcd(48,18)
48 = 18×2 + 12
18 = 12×1 + 6
12 = 6×2 + 0
```
```
Til·les rectangulars: mida comuna de quadrat que recobreix els dos rectangles.
```

🔹 **Propietats o Regles Clau:**
- Si `d = mcd(a, b)`, aleshores `a = d·a'` i `b = d·b'` amb `a'`, `b'` coprimers.
- Relació amb l’MCM: `a × b = mcd(a, b) × mcm(a, b)`.

🔹 **Concepcions Errònies Habituals:**
- Confondre MCD amb MCM.
- Negligir `1` com a possible MCD.

🔹 **Connexions:**
- Simplifica fraccions (Mòdul 5) i congruències modulars.
- Demostra pensament algorítmic rellevant per a estratègies del Mòdul 19.

🔹 **Aplicacions i Records Mnemotècnics:**
- S’utilitza per agrupar elements igualment o sincronitzar cicles.
- Consell: “Màxim Comú Divideix” resumeix el seu significat.

##### Bloc 9 – MCM a través de Factors Primers
🔹 **Definició:** El **mínim comú múltiple** `mcm(a, b)` és el nombre positiu més petit divisible per `a` i `b`, sovint trobat amb factorització prima.

🔹 **Exemples:**
- `mcm(4, 6) = 12`.
- `mcm(8, 12, 15) = 120` (factors primers `2^3`, `3`, `5`).
- Contraexemple: Escollir `24` com a `mcm(4, 6)` és incorrecte perquè `12` és més petit.

🔹 **Notació Matemàtica:**
- Mètode de factors primers: prendre la potència més alta de cada primer entre els nombres.
- Identitat: `a × b = mcd(a, b) × mcm(a, b)`.

🔹 **Representacions Visuals:**
```
Llistes de múltiples:
4 → 4,8,12,16,...
6 → 6,12,18,...
Primer múltiple comú → 12
```

🔹 **Propietats o Regles Clau:**
- Simètric: `mcm(a, b) = mcm(b, a)`.
- Si `a | b`, aleshores `mcm(a, b) = b`.

🔹 **Concepcions Errònies Habituals:**
- Aturar-se en qualsevol múltiple comú en lloc del mínim.
- Oblidar incloure totes les potències primeres.

🔹 **Connexions:**
- Essencial per als denominadors comuns (Mòdul 5).
- Dona suport a problemes de planificació (Mòdul 19).

🔹 **Aplicacions i Records Mnemotècnics:**
- Sincronitzar esdeveniments, com horaris de classes o cicles de semàfor.
- Recorda: “Mínim vol dir primer encaix, després atura’t”.

##### Bloc 10 – Factorització i Teorema Fonamental
🔹 **Definició:** La **factorització prima** descompon un enter en factors primers. El **Teorema Fonamental de l’Aritmètica** afirma que cada enter més gran que `1` té una factorització prima única (fins a l’ordre).

🔹 **Exemples:**
- `60 = 2^2 × 3 × 5`.
- `84 = 2^2 × 3 × 7`.
- Contraexemple: `45 = 3 × 15` és incomplet perquè `15` no és primer; factorització completa `3^2 × 5`.

🔹 **Notació Matemàtica:**
- Arbres de factors, exponents (`p^k`).
- Unicitat: si `n = p_1^{a_1} ... p_k^{a_k} = q_1^{b_1} ... q_m^{b_m}`, aleshores `k = m` i els primers coincideixen amb els mateixos exponents.

🔹 **Representacions Visuals:**
```
   60
  /  \
 6   10
 /\  / \
2 3 2  5
```

🔹 **Propietats o Regles Clau:**
- Multiplicar primes iguals suma exponents.
- La factorització prima dona suport al MCD/MCM via exponents mínims/màxims.

🔹 **Concepcions Errònies Habituals:**
- Aturar-se en factors compostos.
- Creure que `1` té factors primers; no en té.

🔹 **Connexions:**
- Construeix habilitats amb exponents (Mòdul 6) i teoria de nombres (Mòdul 9).
- Ajuda a simplificar radicals (Mòdul 6).

🔹 **Aplicacions i Records Mnemotècnics:**
- Ús en criptografia i simplificació de fraccions.
- Sabies que...? L’encriptació moderna depèn de la dificultat de factoritzar nombres gegants.

##### Bloc 11 – Nombres Especials (Perfectes, Triangulars, Fibonacci)
🔹 **Definició:** Els **nombres perfectes** igualen la suma dels divisors propis; els **nombres triangulars** conten punts que formen triangles equilàters; la **seqüència de Fibonacci** té cada terme igual a la suma dels dos anteriors (`F_n = F_{n-1} + F_{n-2}`).

🔹 **Exemples:**
- Perfectes: `6 = 1 + 2 + 3`, `28 = 1 + 2 + 4 + 7 + 14`.
- Triangulars: `T_4 = 10` formant un triangle de 4 files.
- Fibonacci: `0, 1, 1, 2, 3, 5, 8, ...`; contraexemple: `9` no és triangular perquè `n(n+1)/2 ≠ 9` per a cap `n` enter.

🔹 **Notació Matemàtica:**
- Nombres triangulars `T_n = n(n + 1)/2`.
- Recurrència de Fibonacci amb `F_0 = 0`, `F_1 = 1`.
- Comprovació de nombre perfecte via suma de divisors `σ(n) - n = n`.

🔹 **Representacions Visuals:**
```
Punts triangulars (T4):
•
••
•••
••••
```
```
Quadrats de Fibonacci que formen una espiral: 1×1, 1×1, 2×2, 3×3, 5×5.
```

🔹 **Propietats o Regles Clau:**
- Els nombres perfectes parells segueixen `2^{p-1}(2^p - 1)` quan `2^p - 1` és primer (primer de Mersenne).
- `T_n = C(n + 1, 2)` connecta amb combinacions.
- Els quocients de Fibonacci s’aproximen al nombre d’or `≈ 1,618`.

🔹 **Concepcions Errònies Habituals:**
- Assumir que els nombres triangulars són perfectes; són seqüències diferents.
- Tractar Fibonacci com a aritmètica (diferència fixa) en lloc d’afegeixió recurrent.

🔹 **Connexions:**
- Enllaça amb combinatòria (Mòdul 20) i patrons (Mòdul 10).
- Fibonacci apareix en discussions de creixement exponencial (Mòdul 6).

🔹 **Aplicacions i Records Mnemotècnics:**
- Present en arquitectura, natura (pinyes, gira-sols).
- Recorda: “Triangular `T` apila `n` i `n+1`, després divideix per dos”.

##### Bloc 12 – Concepte d’Aritmètica Modular (a ≡ b mod n)
🔹 **Definició:** L’**aritmètica modular** compara nombres per residus: `a ≡ b (mod n)` quan `n` divideix `a - b`.

🔹 **Exemples:**
- `17 ≡ 5 (mod 12)` perquè `17 - 5 = 12`.
- `9 ≡ 1 (mod 4)` perquè tots dos deixen residu `1` en dividir per `4`.
- Contraexemple: `14 ≡ 3 (mod 4)` és fals perquè `14 - 3 = 11`, i `4` no divideix `11`.

🔹 **Notació Matemàtica:**
- Símbol de congruència `≡`; mòdul indicat `(mod n)`.
- Classe de residu `[a]_n` representa tots els enters congruents amb `a` mòdul `n`.

🔹 **Representacions Visuals:**
```
Rellotge (mod 12):
1 ↔ 13 ↔ 25 ↔ ... tots ≡ 1 (mod 12)
```
```
Taula de residus mod 5
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
- Els residus negatius es transformen: `-1 ≡ n - 1 (mod n)`.

🔹 **Concepcions Errònies Habituals:**
- Tractar `mod` com divisió en lloc de comparació de residus.
- Oblidar reduir residus a l’interval `0` a `n - 1`.

🔹 **Connexions:**
- Dona suport a la lògica de divisibilitat i patrons cíclics (Bloc 13).
- Torna al Mòdul 21 d’enriquiment i en contextos de criptografia.

🔹 **Aplicacions i Records Mnemotècnics:**
- Ajuda a calcular dies de la setmana, hores del rellotge, dígits de control.
- Sabies que...? Les notes musicals es repeteixen cada octava com l’aritmètica mod `12`.

##### Bloc 13 – Exploració de Patrons de Residus
🔹 **Definició:** Un **patró de residus** rastreja residus repetits quan els nombres es divideixen per un mòdul fix, revelant cicles.

🔹 **Exemples:**
- Potències de `2 mod 5`: `2, 4, 3, 1` repetint cada `4` passos.
- Múltiples de `7 mod 3`: residus `1, 2, 0, 1, 2, 0, ...`.
- Contraexemple: Afirmar que `2^n mod 5` sempre val `2` ignora el cicle.

🔹 **Notació Matemàtica:**
- Seqüències `(a_n)` amb `a_n ≡ k (mod m)`.
- El període denota la longitud del cicle.

🔹 **Representacions Visuals:**
```
Roda de residus mod 5 per a potències de 2
2 → 4 → 3 → 1 → (torna a 2)
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
- Els mòduls finits garanteixen repetició eventual (principi del colom).
- La longitud del cicle per a potències es relaciona amb la funció φ d’Euler quan la base i el mòdul són coprimers.

🔹 **Concepcions Errònies Habituals:**
- Esperar que els cicles comencin a `n = 0`; els termes inicials poden diferir.
- Creure que cada residu apareix una sola vegada; els cicles poden saltar alguns valors depenent de la base.

🔹 **Connexions:**
- Prepara temes de teoria de nombres, dóna suport a exponents encriptats.

🔹 **Aplicacions i Records Mnemotècnics:**
- Detectar periodicitat en seqüències, simplificar residus en concursos.
- Consell: “Segueix els residus fins que tornin a aparèixer”.

##### Bloc 14 – Consolidació i Repàs Mixt
🔹 **Definició:** Un repàs mixt combina criteris, patrons i factorizacions per enfortir la flexibilitat numèrica.

🔹 **Exemples:**
- Problemes que barregen divisibilitat, MCD/MCM i notació científica.
- Taules de residus combinades amb jerarquia de conjunts.
- Contraexemple: Enfocar només un tema impedeix veure connexions.

🔹 **Notació Matemàtica:**
- Paquets de problemes que requereixen múltiples eines.
- Etiquetes per identificar quines tècniques s’han utilitzat.

🔹 **Representacions Visuals:**
```
Mapa mental connectant conjunts, divisibilitat, notació científica.
```

🔹 **Propietats o Regles Clau:**
- Practicar canvis ràpids entre estratègies.
- Revisar errors comuns col·loca barreres de prevenció.

🔹 **Concepcions Errònies Habituals:**
- Pensar que hi ha una única seqüència d’estratègies.
- Saltar la comprovació final quan es combinen mètodes.

🔹 **Connexions:**
- Enllaça tot el Mòdul 1 amb futurs mòduls avançats.

🔹 **Aplicacions i Records Mnemotècnics:**
- Serveix de preparació per a exàmens i projectes interdisciplinaris.
- Recorda: “Combina, contrasta i confirma”.

### Mòdul 2: Operacions Bàsiques i Estratègies Mentals (≈4h)
Modelatge d’addició/subtracció, problemes de múltiples passos, propietats (commutativa, associativa, distributiva), domini de multiplicació/divisió, ordre de les operacions, estimació i estratègies de càlcul mental.

Paraules clau: modelatge de l’addició, modelatge de la subtracció, recta numèrica, problemes multi-pas, anàlisi de text de problemes, commutativa, associativa, distributiva, estratègies de multiplicació, algoritme de divisió, divisió llarga, PEMDAS, estimació, càlcul mental, arrodoniment, estimació frontal, nombres compatibles, comprovació de raonabilitat

Blocs:
1 Modelatge d’operacions en la recta numèrica
2 Estructura de problemes textuals multi-pas
3 Propietats (commutativa, associativa)
4 Aplicacions de la propietat distributiva
5 Estratègies de multiplicació (reixa, descomposició)
6 Algoritme de divisió i residus
7 Domini de la divisió llarga
8 Complexitat de l’ordre de les operacions
9 Tècniques d’estimació i arrodoniment
10 Drills d’estratègies de càlcul mental
11 Mètodes de comprovació d’errors
12 Conjunt de reptes mixtos

#### Teoria

##### Bloc 1 – Modelatge d’Operacions a la Recta Numèrica
🔹 **Definició:** Un model de **recta numèrica** mostra l’addició com moviments cap a la dreta i la subtracció com moviments cap a l’esquerra des d’un punt inicial.

🔹 **Exemples:**
- `3 + 5`: comença a `3`, salta `5` unitats a la dreta i acaba a `8`.
- `7 - 9`: comença a `7`, es mou `9` unitats a l’esquerra fins a `-2`.
- Contraexemple: Moure’s a la dreta per `7 - 4` donaria `11`, que contradiu la subtracció.

🔹 **Notació Matemàtica:**
- Punts etiquetats amb enters `... -2, -1, 0, 1 ...`.
- Fletxes `→` (positiu) i `←` (negatiu).

🔹 **Representacions Visuals:**
```
Recta numèrica per a 4 - 6
-2 -1 0 1 2 3 4
             ^ comença a 4
<--6 salts cap a l’esquerra--> resultat -2
```

🔹 **Propietats o Regles Clau:**
- L’addició combina distàncies, la subtracció compara posicions.
- L’addició i la subtracció són moviments inversos a la recta.

🔹 **Concepcions Errònies Habituals:**
- Saltar el zero quan es passa de nombres positius a negatius.
- Creure que restar un nombre negatiu també implica moure’s cap a l’esquerra; en realitat, suma un salt a la dreta.

🔹 **Connexions:**
- Prepara per la geometria coordenada (Mòdul 12) i operacions amb enters.

🔹 **Aplicacions i Records Mnemotècnics:**
- Modela canvis de temperatura o guanys/pèrdues financeres.
- Recorda: “Dreta per sumar, esquerra per restar.”

##### Bloc 2 – Estructura de Problemes Textuals Multi-pas
🔹 **Definició:** Els problemes textuals de múltiples passos requereixen seqüenciar diverses operacions per modelar escenaris reals amb precisió.

🔹 **Exemples:**
- Botiga escolar: `3` llibretes a `€2` més una carpeta a `€4` → `3×2 + 4 = 10`.
- Ciclisme setmanal: `15 km` per dia durant `4` dies → `15×4 = 60 km`.
- Contraexemple: Aturar-se després de `3×2 = 6` perd el cost total.

🔹 **Notació Matemàtica:**
- Usa parèntesis per mostrar l’ordre: `total = (3×2) + 4`.
- Taula organitzadora amb **Saps**, **Necessites**, **Pla**.

🔹 **Representacions Visuals:**
```
| Pas | Operació | Resultat |
|-----|----------|----------|
|  1  | 3×2      | 6 €      |
|  2  | 6+4      | 10 €     |
```

🔹 **Propietats o Regles Clau:**
- Traduir el llenguatge a matemàtiques abans de calcular.
- Verificar la raonabilitat després de cada pas per evitar errors acumulats.

🔹 **Concepcions Errònies Habituals:**
- Barrejar unitats (p. ex., euros amb objectes) o fer passos fora de seqüència.
- Assumir que cada detall del text s’ha d’utilitzar, fet que porta a forçar nombres irrellevants.

🔹 **Connexions:**
- Dona suport a la modelització algebraica (Mòdul 11) i estratègies de resolució de problemes (Mòdul 19).

🔹 **Aplicacions i Records Mnemotècnics:**
- Essencial per a pressupost familiar o planificació de viatges.
- Consell: “Saps, Necessites, Següent” resumeix els passos de planificació.

##### Bloc 3 – Propietats (Commutativa, Associativa)
🔹 **Definició:** La propietat **commutativa** permet intercanviar l’ordre (`a + b = b + a`, `ab = ba`); la propietat **associativa** permet reagrupar (`(a + b) + c = a + (b + c)`).

🔹 **Exemples:**
- `3 + 5 = 5 + 3`.
- `(2 + 4) + 7 = 2 + (4 + 7)`.
- Contraexemple: `7 - 5 ≠ 5 - 7`; la subtracció no és commutativa.

🔹 **Notació Matemàtica:**
- Per a tot `a, b, c ∈ ℝ`, l’addició i la multiplicació satisfan la commutativitat i associativitat.
- Parèntesis clarifiquen l’agrupament.

🔹 **Representacions Visuals:**
```
Fitxes numèriques:
[3][+][5] ↔ [5][+][3]
```
```
Arbre d’agrupació mostrant `(a+b)+c` vs `a+(b+c)` amb les mateixes fulles.
```

🔹 **Propietats o Regles Clau:**
- Només vàlides per a addició i multiplicació en aritmètica bàsica.
- Faciliten reorganitzar números mentalment.

🔹 **Concepcions Errònies Habituals:**
- Assumir que la subtracció o divisió comparteixen aquestes propietats.
- Oblidar que reagrupar associativament encara exigeix la mateixa operació; no es pot substituir per resta.

🔹 **Connexions:**
- Sosté el càlcul mental (Bloc 10) i l’àlgebra (Mòdul 11).

🔹 **Aplicacions i Records Mnemotècnics:**
- Útil quan es reordenen despeses o es grupen totals.
- Recorda: “Commuta = canvia lloc; associa = canvia company.”

##### Bloc 4 – Aplicacions de la Propietat Distributiva
🔹 **Definició:** La **propietat distributiva** reparteix la multiplicació sobre l’addició o la subtracció: `a(b ± c) = ab ± ac`.

🔹 **Exemples:**
- `7×18 = 7×(10 + 8) = 70 + 56 = 126`.
- Àrea d’un rectangle `7 × 13` via `7(10 + 3)`.
- Contraexemple: `5(3 + 2) = 5×3 + 2` és incorrecte; ambdós termes necessiten multiplicació.

🔹 **Notació Matemàtica:**
- Funciona en ambdós sentits: `ab + ac = a(b + c)` (factorització).
- Usa claudàtors per remarcar la distribució: `5{(3 + 2)}`.

🔹 **Representacions Visuals:**
```
Rectangle dividit:
[#####-----] amplada 18 = 10 + 8
```

🔹 **Propietats o Regles Clau:**
- Manté la igualtat quan cada terme rep el factor.
- És la base per expandir expressions algebraiques més endavant.

🔹 **Concepcions Errònies Habituals:**
- Ometre els signes negatius quan es distribueix sobre una resta.
- Creure que només s’aplica quan el factor està a l’esquerra; també es pot distribuir des de la dreta o recollir factors comuns.

🔹 **Connexions:**
- Pont cap a la manipulació algebraica (Mòdul 11) i les lleis d’exponents (Mòdul 6).

🔹 **Aplicacions i Records Mnemotècnics:**
- Multiplicacions mentals ràpides i ajustos de preus.
- Consell: Imagina obrir un paraigua (factor) sobre cada terme.

##### Bloc 5 – Estratègies de Multiplicació
🔹 **Definició:** La **multiplicació estratègica** utilitza descomposició (models d’àrea, productes parcials, reixa) per simplificar productes complexos.

🔹 **Exemples:**
- Productes parcials: `34 × 27 = (30 + 4)(20 + 7) = 600 + 210 + 80 + 28`.
- La reixa organitza la multiplicació de dígits amb sumes diagonals donant `918`.
- Contraexemple: Multiplicar només les desenes `3×2` i ignorar la resta de dígits.

🔹 **Notació Matemàtica:**
- Expressa `(a + b)(c + d)` per aplicar distribució.
- La reixa utilitza sumes diagonals per als valors posicional.

🔹 **Representacions Visuals:**
```
Reixa per a 34×27
      3 | 4
     --------
2 | 06|08
7 | 21|28
Sumes diagonals → 918
```

🔹 **Propietats o Regles Clau:**
- Dividir nombres respecta el valor posicional i evita errors.
- Recombinar implica sumar els productes parcials.

🔹 **Concepcions Errònies Habituals:**
- Oblidar sumar tots els productes parcials.
- Desalinear dígits a la reixa provocant errors de posició.

🔹 **Connexions:**
- Prepara la multiplicació de polinomis (Mòdul 11) i l’exponentiació (Mòdul 6).

🔹 **Aplicacions i Records Mnemotècnics:**
- Útil en càlculs mentals, pressupostos o escales de mesures.
- Recorda: “Divideix, multiplica, suma.”

##### Bloc 6 – Algoritme de Divisió i Residus
🔹 **Definició:** L’**algoritme de divisió** estableix que per a enters `a` i divisor positiu `d`, existeixen enters únics `q` i `r` amb `0 ≤ r < d` tal que `a = dq + r`.

🔹 **Exemples:**
- `23 ÷ 5` dóna `q = 4`, `r = 3` perquè `23 = 5×4 + 3`.
- `59 ÷ 7` produeix `q = 8`, `r = 3`.
- Contraexemple: Escriure `23 = 5×5 - 2` trenca la regla del residu.

🔹 **Notació Matemàtica:**
- Forma abreujada `a ÷ d = q R r`.
- Congruència relacionada: `a ≡ r (mod d)`.

🔹 **Representacions Visuals:**
```
 4 R3
5 )23
  20
  --
   3
```

🔹 **Propietats o Regles Clau:**
- El residu ha de ser menor que el divisor.
- Garanteix una parella quocient-residu única.

🔹 **Concepcions Errònies Habituals:**
- Permetre residu ≥ divisor.
- Confondre quocient i residu.
- Assumir que tota divisió ha de donar un quocient enter i, per tant, ignorar o informar erròniament els residus.

🔹 **Connexions:**
- Porta a la divisió llarga (Bloc 7) i a l’aritmètica modular (Mòdul 1).

🔹 **Aplicacions i Records Mnemotècnics:**
- Necessari per repartir en parts iguals o empaquetar.
- Consell: “Dividir = divisor × quocient + residu.”

##### Bloc 7 – Domini de la Divisió Llarga
🔹 **Definició:** La **divisió llarga** resta repetidament múltiples del divisor de seccions del dividend per construir el quocient dígit a dígit.

🔹 **Exemples:**
- `784 ÷ 16` resulta en `49`.
- `104,5 ÷ 5 = 20,9` estenent decimals.
- Contraexemple: Ometre el pas de baixar el següent dígit trenca l’algoritme.

🔹 **Notació Matemàtica:**
- Col·loca els dígits del quocient sobre el dividend alineats amb el tros restat.
- Afegeix zeros per continuar dividint decimals.

🔹 **Representacions Visuals:**
```
   49
16 )784
   64
   --
   144
   144
   ---
     0
```

🔹 **Propietats o Regles Clau:**
- Cada residu parcial és menor que el divisor.
- Equivalent a resta repetida i estimació de quocients parcials.

🔹 **Concepcions Errònies Habituals:**
- Oblidar baixar el dígit següent.
- Escriure el residu a la part superior en lloc de restar.
- Aturar-se quan es repeteix un residu, en lloc d’afegir zeros per continuar amb decimals.

🔹 **Connexions:**
- Dona suport a operacions amb decimals (Mòdul 3) i conversions de fraccions (Mòdul 5).

🔹 **Aplicacions i Records Mnemotècnics:**
- Necessària per calcular preus unitats o taxes exactes.
- Recorda: Cicle “Divideix → Multiplica → Resta → Baixa”.

##### Bloc 8 – Complexitat de l’Ordre de les Operacions
🔹 **Definició:** L’**ordre de les operacions** (PEMDAS) dicta la seqüència de càlcul: Parèntesis, Exponents, Multiplicació/Divisió (d’esquerra a dreta), Addició/Subtracció (d’esquerra a dreta).

🔹 **Exemples:**
- `6 + 3 × 4 = 6 + 12 = 18`.
- `20 ÷ 5 × 2 = 4 × 2 = 8` (processa d’esquerra a dreta dins del nivell MD).
- Contraexemple: `(6 + 3) × 4 = 36` només quan els parèntesis ho exigeixen.

🔹 **Notació Matemàtica:**
- Símbols addicionals `[ ]`, `{ }` anul·len l’ordre per defecte.
- Els exponents negatius requereixen parèntesis: `(-3)^2` vs `-3^2`.

🔹 **Representacions Visuals:**
```
Escala PEMDAS:
P
E
MD ⇢ esquerra a dreta
AS ⇢ esquerra a dreta
```

🔹 **Propietats o Regles Clau:**
- Multiplicació i divisió comparteixen prioritat; es resolen d’esquerra a dreta.
- Addició i subtracció també comparteixen prioritat; també d’esquerra a dreta.

🔹 **Concepcions Errònies Habituals:**
- Creure que la multiplicació sempre precedeix la divisió sense considerar l’ordre.
- Gestionar malament nombres negatius amb exponents.
- Ignorar que les barres de fracció o radicals impliquen parèntesis implícits que prevalen sobre la regla general.

🔹 **Connexions:**
- Crucial per avaluar expressions algebraiques (Mòdul 11).
- Dona suport a situacions de resolució de problemes complexos (Mòdul 19).

🔹 **Aplicacions i Records Mnemotècnics:**
- Assegura que les fórmules introduïdes a la calculadora donen resultats correctes.
- Consell: “Please Excuse My Dear Aunt Sally” per recordar PEMDAS.

##### Bloc 9 – Tècniques d’Estimació i Arrodoniment
🔹 **Definició:** L’**estimació** proporciona respostes aproximades ràpides; l’**arrodoniment** ajusta nombres a un lloc determinat per simplificar càlculs.

🔹 **Exemples:**
- Arrodoneix `73` a la desena més propera → `70`.
- Estima `198 + 523 ≈ 200 + 500 = 700`.
- Contraexemple: Arrodonir `1,49` a `0` ignora la norma; correcte és `1`.

🔹 **Notació Matemàtica:**
- `≈` denota aproximació.
- Funció d’arrodoniment `round(x, k)` per `k` decimals.

🔹 **Representacions Visuals:**
```
Recta numèrica arrodonint 23 a la desena més propera
20 ---|--- 25 ---|--- 30
               ^ 23 més a prop de 20
```

🔹 **Propietats o Regles Clau:**
- Dígit `5` o superior arrodoneix cap amunt; inferiors a `5` cap avall.
- Mètodes d’estimació inclouen front-end, nombres compatibles, agrupament.

🔹 **Concepcions Errònies Habituals:**
- Arrodonir sempre cap avall sense mirar el dígit de referència.
- Tractar les estimacions com a respostes exactes.

🔹 **Connexions:**
- Dona suport a la precisió de mesures (Mòdul 8) i a la presentació de dades (Mòdul 16).

🔹 **Aplicacions i Records Mnemotècnics:**
- Útil per fer pressupostos, planificar viatges, ajustar receptes.
- Recorda: “5 o més, puja el marcador; 4 o menys, deixa’l com és.”

##### Bloc 10 – Drills d’Estratègies de Càlcul Mental
🔹 **Definició:** El **càlcul mental** aprofita propietats numèriques (compensació, descomposició, nombres amigables) per calcular sense llapis ni paper.

🔹 **Exemples:**
- `48 + 17 = 50 + 15 = 65` utilitzant compensació.
- `25 × 4 = 100` considerant quarts.
- Contraexemple: Endevinar sense estructura augmenta els errors.

🔹 **Notació Matemàtica:**
- Mostra ajustos: `48 + 17 = (48 + 2) + (17 - 2)`.
- Fletxes indiquen passos d’ajust i correcció.

🔹 **Representacions Visuals:**
```
Taula T
Original | Ajust | Resultat
48+17    | +2,-2 | 65
```

🔹 **Propietats o Regles Clau:**
- Utilitza propietats commutativa i associativa per reorganitzar nombres.
- Divideix números per valor posicional per reduir la càrrega cognitiva.

🔹 **Concepcions Errònies Habituals:**
- Pensar que el càlcul mental és aproximat o a l’atzar; segueix una lògica.

🔹 **Connexions:**
- Enllaça amb la manipulació de decimals (Mòdul 3) i l’estimació (Bloc 9).

🔹 **Aplicacions i Records Mnemotècnics:**
- Suporta comprovacions ràpides de preus, marcadors esportius, pràctiques d’aula.
- Consell: “Fes-ho amigable, després corregeix.”

##### Bloc 11 – Mètodes de Comprovació d’Errors
🔹 **Definició:** La **verificació d’errors** utilitza operacions inverses, estimacions o estratègies alternatives per confirmar la precisió dels resultats.

🔹 **Exemples:**
- Comprova `27 × 4 = 108` verificant que `108 ÷ 4 = 27`.
- Estima `524 + 197 ≈ 700`; el resultat exacte `721` és raonable.
- Contraexemple: Repetir el mateix mètode erroni no detecta errors.

🔹 **Notació Matemàtica:**
- Fletxes inverses `⇄` indiquen comprovació: `×` ↔ `÷`, `+` ↔ `-`.
- Usa `≈` per a estimacions de raonabilitat.

🔹 **Representacions Visuals:**
```
Flux:
Resol → Comprova invertint → Compara amb estimació → Confirma
```

🔹 **Propietats o Regles Clau:**
- Les operacions inverses es desfan mútuament.
- Comparar amb estimacions detecta errors de valor posicional.

🔹 **Concepcions Errònies Habituals:**
- Creure que la verificació és opcional; els errors petits es propaguen.

🔹 **Connexions:**
- Reforça la resolució algebraica (Mòdul 11) i la precisió de mesures (Mòdul 8).

🔹 **Aplicacions i Records Mnemotècnics:**
- Vital en enginyeria, finances, programació per evitar costos.
- Recorda: “Fes-ho, desfés-ho, comprova-ho.”

##### Bloc 12 – Conjunt de Reptes Mixtos
🔹 **Definició:** Els reptes mixtos integren múltiples operacions i estratègies, exigint flexibilitat en la resolució de problemes.

🔹 **Exemples:**
- Problema de recaptació que combina multiplicació, subtracció i estimació.
- Enigma que necessita PEMDAS i trucs mentals junts.
- Contraexemple: Aplicar només un algoritme d’un pas a un escenari multipas.

🔹 **Notació Matemàtica:**
- Expressions com `[(a + b) × c] ÷ d` amb anotacions de l’estratègia triada.

🔹 **Representacions Visuals:**
```
Web d’estratègies que connecta operacions, estimació, càlcul mental, propietats.
```

🔹 **Propietats o Regles Clau:**
- Encoratja escollir l’eina més adequada en lloc de seguir plantilles rígides.
- Construeix resiliència amb pràctica variada.

🔹 **Concepcions Errònies Habituals:**
- Creure que només existeix un mètode vàlid; múltiples camins poden ser correctes.

🔹 **Connexions:**
- Prepara tasques reals integrades en mòduls posteriors.

🔹 **Aplicacions i Records Mnemotècnics:**
- Reflecteix la presa de decisions autèntica on diverses operacions interactuen.
- Sabies que...? Els concursos de càlcul mental premien la rapidesa en canviar d’estratègia.

### Mòdul 3: Decimals i Nombres Racionals (≈2.25h)
Valor posicional decimal, comparació/arrodoniment, operacions amb decimals, conversions fracció↔decimal, racionals vs irracionals (introducció), densitat a la recta numèrica.

Paraules clau: decimals, valor posicional, dècimes, centèsimes, mil·lèsimes, comparar decimals, arrodoniment, xifres significatives, operacions decimals, conversió fraccions, decimals periòdics, decimals finits, racionals vs irracionals, densitat

Blocs:
1 Valor posicional decimal i representació
2 Comparar i ordenar decimals
3 Arrodoniment i xifres significatives
4 Operacions decimals (+ − × ÷)
5 Conversiones fracció↔decimal
6 Decimals periòdics vs finits; idea de densitat
7 Pràctica mixta i resum

#### Teoria

##### Bloc 1 – Valor Posicional Decimal i Representació
🔹 **Definició:** Un **nombre decimal** expressa parts d’un sencer amb potències de `10`; les posicions a la dreta del punt representen dècimes (`10^-1`), centèsimes (`10^-2`), mil·lèsimes (`10^-3`), etc.

🔹 **Exemples:**
- `3,47 = 3 + 4/10 + 7/100`.
- `0,205` té `0` dècimes, `2` centèsimes, `0` mil·lèsimes, `5` deu-mil·lèsimes.
- Contraexemple: Llegir `0,5` com `0,05` ignora el valor posicional; `0,5 = 1/2`.

🔹 **Notació Matemàtica:**
- El punt decimal separa la part entera (esquerra) de la fraccional (dreta).
- Cada posició és el dígit multiplicat per `10^-k`.

🔹 **Representacions Visuals:**
```
Graella 10×10: 34 quadrats ombrejats → 0,34
[■■■■■■■■■■........................]
```
```
Recta numèrica de 0 a 1 dividida en dècimes amb 0,47 marcat.
```

🔹 **Propietats o Regles Clau:**
- Moures una posició a la dreta divideix per deu; cap a l’esquerra multiplica per deu.
- Els zeros finals després del decimal no canvien el valor (`3,40 = 3,4`).

🔹 **Concepcions Errònies Habituals:**
- Creure que més dígits sempre impliquen valor major; cal comparar la posició de la primera diferència.

🔹 **Connexions:**
- Amplia el valor posicional dels enters (Mòdul 1) i dona suport a operacions decimals (Bloc 4).

🔹 **Aplicacions i Records Mnemotècnics:**
- Essencial en moneda (`€3,47`) i mesures (metres, litres).
- Recorda: “Cada pas a la dreta divideix per deu.”

##### Bloc 2 – Comparar i Ordenar Decimals
🔹 **Definició:** Comparar decimals implica alinear punts decimals i revisar dígits d’esquerra a dreta per decidir quin valor és més gran.

🔹 **Exemples:**
- `0,75 > 0,7` perquè la comparació de centèsimes mostra `5 > 0`.
- Ordena `2,35, 2,305, 2,4`: `2,305 < 2,35 < 2,4`.
- Contraexemple: Usar dígits crus `75` vs `8` per afirmar `0,75 > 0,8` ignora l’alineació posicional.

🔹 **Notació Matemàtica:**
- Símbols de comparació `<`, `>`, `=`.
- Omplir amb zeros: `0,7 = 0,70` per alinear posicions.

🔹 **Representacions Visuals:**
```
Recta numèrica de 0,7 a 0,8 mostrant marques a 0,70, 0,75, 0,80.
```
```
Taula de valor posicional:
Unitats | Dècimes | Centèsimes | Mil·lèsimes
 0        7           5             0  → 0,750
 0        8           0             0  → 0,800
```

🔹 **Propietats o Regles Clau:**
- Afegeix zeros finals per assegurar la mateixa longitud de dígits.
- El primer dígit diferent des de l’esquerra determina l’ordre.

🔹 **Concepcions Errònies Habituals:**
- Tractar la part decimal com un nombre sencer sense considerar la posició.

🔹 **Connexions:**
- Enllaça amb decisions d’arrodoniment (Bloc 3) i comparacions amb fraccions (Bloc 5).

🔹 **Aplicacions i Records Mnemotècnics:**
- Pràctic per comparar preus o precisió de mesures.
- Consell: “Alinea els punts, compara les posicions.”

##### Bloc 3 – Arrodoniment i Xifres Significatives
🔹 **Definició:** L’**arrodoniment** simplifica nombres a la posició deseada; les **xifres significatives** compten dígits rellevants que transmeten precisió.

🔹 **Exemples:**
- Arrodona `4,768` a dues decimals → `4,77`.
- `0,00340` té tres xifres significatives (`3`, `4` i el `0` final perquè el punt decimal fixa la precisió).
- Contraexemple: Arrodonir `5,15` a una decimal com `5,1` ignora la regla del `5`; correcte és `5,2`.

🔹 **Notació Matemàtica:**
- Funció `round(x, n)`.
- Xifres significatives s’anoten com `3 x.s.` etc.

🔹 **Representacions Visuals:**
```
Recta numèrica 4,76 a 4,77 amb punt mig a 4,765 mostrant decisió d’arrodoniment.
```
```
Ressalt de dígits: 0 . 0 0 3 4 0
                              ↑ primera xifra significativa
```

🔹 **Propietats o Regles Clau:**
- Dígit `≥ 5` arrodoneix cap amunt; en cas contrari es manté.
- Zeros inicials mai compten com significatius; zeros finals compten només si hi ha punt decimal.

🔹 **Concepcions Errònies Habituals:**
- Confondre decimals amb xifres significatives (mesuren aspectes diferents de la precisió).

🔹 **Connexions:**
- Dona suport a la notació científica (Mòdul 6) i als informes de mesures (Mòdul 8).

🔹 **Aplicacions i Records Mnemotècnics:**
- Usat en laboratoris científics i especificacions d’enginyeria.
- Recorda: “Les xifres significatives indiquen seguretat.”

##### Bloc 4 – Operacions Decimals (+ − × ÷)
🔹 **Definició:** Operar amb decimals requereix alinear valors posicional per a l’addició/subtracció, seguir el recompte total de decimals per a la multiplicació i ajustar divisor i dividend per a la divisió.

🔹 **Exemples:**
- Addició: `2,45 + 0,7 = 3,15` (omple amb zero).
- Multiplicació: `1,2 × 0,03 = 0,036` (dues xifres decimals en total).
- Contraexemple: Dir `0,5 × 0,5 = 2,5` ignora la ubicació del decimal; el producte real és `0,25`.

🔹 **Notació Matemàtica:**
- Alinea columnes per sumar/restar.
- Multiplica comptant decimals: decimals totals igual a la suma dels decimals dels factors.
- Divisió: multiplica numerador i denominador per una potència de `10` per eliminar decimals al divisor.

🔹 **Representacions Visuals:**
```
    2,45
+   0,70
--------
    3,15
```
```
Model d’àrea: rectangle 1,2 per 0,3 representant 0,36 (escalat a 36 petits quadrats de 100).
```

🔹 **Propietats o Regles Clau:**
- El punt decimal s’ha d’alinear per a suma i resta.
- El nombre de decimals en el producte és la suma dels decimals dels factors.
- En divisió, moure el punt en ambdós operands manté la proporció.

🔹 **Concepcions Errònies Habituals:**
- Deixar punts decimals sense alinear.
- Posar el punt decimal en posició incorrecta després de multiplicar.
- Oblidar convertir el divisor en enter abans de dividir decimals.

🔹 **Connexions:**
- Crucial per a finances i ciència de dades (Mòdul 16).
- Relaciona fraccions i decimals (Bloc 5).

🔹 **Aplicacions i Records Mnemotècnics:**
- Càlcul de factures, conversió de mesures, projectes científics.
- Consell: “Alinea, compta decimals, ajusta divisor.”

##### Bloc 5 – Conversiones Fracció↔Decimal
🔹 **Definició:** Convertir entre fraccions i decimals utilitza divisió: fracció `a/b` equival a decimal obtingut de `a ÷ b`.

🔹 **Exemples:**
- `3/4 = 0,75`.
- `5/8 = 0,625`.
- Contraexemple: Escriure `1/3 = 0,3` sense indicar que és periòdic (`0,3̅`).

🔹 **Notació Matemàtica:**
- Fraccions com `a/b` amb `b ≠ 0`.
- Decimals periòdics notats amb barra (`0,3̅`).

🔹 **Representacions Visuals:**
```
Divisió llarga 1 ÷ 3 mostrant decimals repetits.
```
```
Graella per a 3/4 amb 75 quadrats ombrejats de 100.
```

🔹 **Propietats o Regles Clau:**
- Fraccions amb denominadors factors de 2 i 5 donen decimals finits.
- Altres generen decimals periòdics.

🔹 **Concepcions Errònies Habituals:**
- Pensar que cada fracció té un decimal finit.
- Ometre el símbol periòdic per decimals repetits.

🔹 **Connexions:**
- Enllaça amb racionals vs irracionals (Bloc 6) i operacions decimals.

🔹 **Aplicacions i Records Mnemotècnics:**
- Conversió de preus, mesures, probabilitats.
- Recorda: “Divideix el numerador pel denominador per revelar el decimal.”

##### Bloc 6 – Decimals Periòdics vs Finit s; Idea de Densitat
🔹 **Definició:** Els decimals **periòdics** tenen un patró que es repeteix infinitament; els decimals **finits** s’aturen. La **densitat** indica que entre qualsevol dos racionals hi ha un altre racional.

🔹 **Exemples:**
- `1/3 = 0,333...` periòdic.
- `1/4 = 0,25` finit.
- Entre `0,2` i `0,3`, `0,25` és un altre racional.
- Contraexemple: Creure que `0,999...` és menor que `1`; en realitat són iguals.

🔹 **Notació Matemàtica:**
- Periòdic `0,¯{ab}` indica repetició.
- Densitat: per `a < b`, existeix `c = (a + b)/2` amb `a < c < b`.

🔹 **Representacions Visuals:**
```
Recta numèrica amb punts densament col·locats mostrant decimals entre 0,2 i 0,3.
```
```
Taula comparant decimals finits i periòdics.
```

🔹 **Propietats o Regles Clau:**
- Els decimals periòdics representen racionals.
- No hi ha “forats” entre racionals en la recta numèrica.

🔹 **Concepcions Errònies Habituals:**
- Considerar decimals infinits automàticament irracionals.
- Analitzar la densitat com un conjunt limitat de decimals.

🔹 **Connexions:**
- Prepara el contrast amb irracionals (Mòdul 4).
- Dona suport a la comprensió de límits bàsics.

🔹 **Aplicacions i Records Mnemotècnics:**
- Comparacions d’interessos, regressió de dades.
- Consell: “Sempre hi ha un decimal entre dos racionals.”

##### Bloc 7 – Pràctica Mixta i Resum
🔹 **Definició:** La pràctica mixta reforça habilitats decimals combinant lectura, ordenació, operacions i conversions.

🔹 **Exemples:**
- Problemes de factures que necessiten sumes, multiplicacions i arrodoniments.
- Conversió de receptes amb decimals i fraccions.
- Contraexemple: Centrar-se només en sumes decimals sense practicar altres habilitats.

🔹 **Notació Matemàtica:**
- Fulls de càlcul amb columnes per operació i verificació.

🔹 **Representacions Visuals:**
```
Diagrama de flux que enllaça comparació → arrodoniment → operacions → conversions.
```

🔹 **Propietats o Regles Clau:**
- Permet detectar debilitats específiques.
- Enforteix la fluïdesa decimal.

🔹 **Concepcions Errònies Habituals:**
- Saltar la comprovació final per pressa.

🔹 **Connexions:**
- Integra les habilitats del mòdul abans de passar a racionals avançats.

🔹 **Aplicacions i Records Mnemotècnics:**
- Reflecteix la gestió de pressupostos, dades experimentals.
- Recorda: “Combina habilitats per dominar decimals.”


### Mòdul 4: Sistemes de Nombres Estesos (≈2.25h)
Jerarquia ℕ ⊂ ℕ₀ ⊂ ℤ ⊂ ℚ ⊂ ℝ, distincions entre racionals i irracionals, proves (idea de √2 irracional), tancament i propietats d'operacions entre conjunts.

Paraules clau: jerarquia de nombres, ℕ₀, enters, racionals, reals, exemples d'irracionals, idea de prova de √2, tancament, propietats d'operacions, algebraic vs transcendental (introducció), inclusió de conjunts

Blocs:
1 Jerarquia ℕ → ℕ₀ → ℤ
2 Extensió al concepte ℚ (fraccions)
3 Característiques dels nombres irracionals
4 Esquema de prova de √2 irracional
5 Recta real i densitat
6 Taula de tancament i propietats d'operacions
7 Classificació mixta i raonament

#### Teoria

##### Bloc 1 – Jerarquia ℕ → ℕ₀ → ℤ
🔹 **Definició:** La jerarquia estesa introdueix **ℕ₀** (nombres sencers incloent `0`) entre els naturals `ℕ` i els enters `ℤ`, mostrant que cada conjunt es find dins del següent més gran.

🔹 **Exemples:**
- `ℕ = {1, 2, 3, ...}` compta els enters positius.
- `ℕ₀ = {0, 1, 2, 3, ...}` afegeix el zero.
- `ℤ = {..., -2, -1, 0, 1, 2, ...}` inclou els negatius.
- Contraexemple: La fracció `1/2` no està a `ℤ`; pertany a `ℚ`.

🔹 **Notació Matemàtica:**
- `ℕ ⊂ ℕ₀ ⊂ ℤ` i cada inclusió és pròpia (estricta).
- Utilitza símbols de subconjunt `⊂`, `⊆` per comunicar inclusió.

🔹 **Representacions Visuals:**
```
[ ℤ ]
	[ ℕ₀ ]
		[ ℕ ]
```
```
Marques de la recta numèrica: negatius (només ℤ), zero (ℕ₀ i ℤ), positius (compartits per tots tres).
```

🔹 **Propietats o Regles Clau:**
- Afegir `0` crea un conjunt tancat sota resta sempre que el resultat sigui no-negatiu.
- Els enters permeten solucions a equacions com `x + 5 = 2` (requereix negatius).

🔹 **Malentesos Comuns:**
- Assumir que tots els sistemes de nombres comencen amb zero; aclareix convencions.
- Creure que els negatius pertanyen a `ℕ`. Només apareixen a `ℤ`.

🔹 **Connexions:**
- Es construeix sobre la jerarquia del Mòdul 1 i prepara pels racionals i reals.
- Suporta solucions algebraiques que requereixen valors negatius (Mòdul 11).

🔹 **Aplicacions i Ganxos de Memòria:**
- Útil quan es descriuen guanys (ℕ), saldos que poden arribar a zero (ℕ₀), o deutes (ℤ).
- Recorda: Pensa en tres calaixos nidificats etiquetats `ℕ`, `ℕ₀`, `ℤ`.

##### Bloc 2 – Extensió al Concepte ℚ
🔹 **Definició:** L'extensió als **racionals `ℚ`** significa permetre raons d'enters (`a/b` amb `b ≠ 0`), capturant fraccions i enters alhora.

🔹 **Exemples:**
- `2/3`, `-5/4`, `0 = 0/1` tots es troben a `ℚ`.
- Qualsevol enter `k` és igual a `k/1`, per tant `ℤ ⊂ ℚ`.
- Contraexemple: `√2` no pot escriure's com `a/b` amb enters, així que no és racional.

🔹 **Notació Matemàtica:**
- `ℚ = {a/b | a, b ∈ ℤ, b ≠ 0}`.
- Simplificació: `a/b = (ka)/(kb)` per a enter no-nul `k`.

🔹 **Representacions Visuals:**
```
Recta numèrica amb fraccions omplint buits entre enters: 0, 1/2, 1, 3/2, 2, ...
```
```
Taula de fraccions equivalents:
1/2 = 2/4 = 3/6
```

🔹 **Propietats o Regles Clau:**
- Els racionals són tancats sota suma, resta, multiplicació i divisió (excepte divisió per zero).
- Entre dos racionals qualssevol es troben infinits racionals més (densitat).

🔹 **Malentesos Comuns:**
- Pensar que només les fraccions pròpies són racionals; els enters també ho són.
- Assumir que les representacions decimals han de ser terminals; els decimals que es repeteixen també són racionals.

🔹 **Connexions:**
- Essencial per a decimals (Mòdul 3) i fraccions (Mòdul 5).
- Condueix a nombres reals quan es discuteix la completat.

🔹 **Aplicacions i Ganxos de Memòria:**
- Útil per a mesuraments, raons i problemes d'escalat.
- Consell: "ℚ significa quocient," recordant-nos que els racionals són raons.

##### Bloc 3 – Característiques dels Nombres Irracionals
🔹 **Definició:** Els **nombres irracionals** no es poden escriure com `a/b` amb enters; les seves expansions decimals són infinites i no repeients.

🔹 **Exemples:**
- `√2`, `π`, i `e` són irracionals.
- El decimal `0.1010010001...` (patró de zeros creixents) mai es repeteix, així que irracional.
- Contraexemple: `0.333...` es repeteix, així que és racional (`1/3`).

🔹 **Notació Matemàtica:**
- `ℝ \ ℚ` denota el conjunt dels nombres irracionals (reals excloent racionals).
- Utilitza expressions radicals infinites o d'exponent per denotar certs irracionals.

🔹 **Representacions Visuals:**
```
Recta numèrica: marca √2 entre 1 i 2 amb posició aproximada 1.414...
```
```
Gràfica decimal mostrant patró no repeient en cada columna.
```

🔹 **Propietats o Regles Clau:**
- Els decimals irracionals ni terminen ni es repeteixen.
- Sumar o multiplicar racionals i irracionals pot produir resultats racionals o irracionals depenent de la combinació (p.ex., `(√2 - √2) = 0` racional).

🔹 **Malentesos Comuns:**
- Creure que tots els decimals no terminals són irracionals; els decimals que es repeteixen són racionals.
- Assumir que les arrels quadrades de no-quadrats perfectes són indefinides; són reals irracionals.

🔹 **Connexions:**
- Completa el sistema de nombres reals amb els racionals.
- Obrir el camí per a discussió sobre densitat i completat.

🔹 **Aplicacions i Ganxos de Memòria:**
- Apareixen en geometria (diagonals, cercles) i fórmules de física.
- Ho sabies...? La diagonal d'un quadrat unitari és `√2`, una longitud irracional clàssica.

##### Bloc 4 – Esquema de Prova de √2 Irracional
🔹 **Definició:** La prova clàssica per contradicció mostra que `√2` és irracional assumint que és igual a una fracció en forma redu·ïda i arribant a una impossibilitat lògica.

🔹 **Exemples:**
- Assume `√2 = p/q` amb `gcd(p, q) = 1`. Elevar al quadrat dóna `2 = p^2/q^2`, així `p^2 = 2q^2`.
- Això força que `p` sigui parell; escriu `p = 2k`, substitueix enrere per concloure que `q` és parell, contradient `gcd(p, q) = 1`.
- Contraexemple: Afirmar que `√4` és irracional repeteix el procés però falla perquè `√4 = 2`, un enter.

🔹 **Notació Matemàtica:**
- Passos de prova per contradicció: `assume`, `deriva`, `contradiu`, `conclou`.
- Els arguments de paritat utilitzen `p = 2k` per indicar enters parells.

🔹 **Representacions Visuals:**
```
Flux de prova:
Assume √2 = p/q (en forma redu·ïda)
→ p^2 = 2q^2
→ p parell → p = 2k
→ substitueix → q parell
→ gcd(p,q) ≠ 1 contradicció
```

🔹 **Propietats o Regles Clau:**
- Es basa en el teorema fonamental de l'aritmètica (factorització en primers única).
- Demostra irracionalitat via contradicció de paritat.

🔹 **Malentesos Comuns:**
- Assumir que la prova mostra que totes les arrels quadrades són irracionals; només les no-quadrats perfectes produeixen contradicció.

🔹 **Connexions:**
- Reforça factorització en primers (Mòdul 1) i raonament lògic (Mòdul 18).

🔹 **Aplicacions i Ganxos de Memòria:**
- Il·lustra l'estructura de prova matemàtica utilitzada en estudis superiors.
- Recorda: "La contradicció parell-parell" és el pols de l'argument.

##### Bloc 5 – Recta Real i Densitat
🔹 **Definició:** La **recta real** inclou tots els racionals i irracionals ordenats; **densitat** significa que entre dos nombres reals diferents quals quelssevol es troben infinits nombres reals més, sovint molts.

🔹 **Exemples:**
- Entre `1` i `2`, nombres com `1.5`, `√2`, `3/2` tots apareixen.
- Entre `π` i `π + 0.01`, podem trobar racionals (`22/7`) i irracionals (`π + 0.001`).
- Contraexemple: Afirmar que hi ha un nombre real "següent" després de `5`; la densitat evita salts discrets.

🔹 **Notació Matemàtica:**
- Notació d'interval `[a, b]`, `(a, b)` etc. capturen segments a la recta.
- Propietat de densitat: per `a < b`, existeix `c` amb `a < c < b` (p.ex., `c = (a + b)/2`).

🔹 **Representacions Visuals:**
```
---|----|----|----|----
	 a   c   d   b
Marques infinites entre a i b il·lustren densitat.
```

🔹 **Propietats o Regles Clau:**
- Els reals formen un continu—sense buits.
- Tant racionals com irracionals són densos dins dels reals.

🔹 **Malentesos Comuns:**
- Pensar que els racionals formen una xarxa amb buits; de fet són densos.
- Creure que la longitud decimal és igual a la distància entre nombres.

🔹 **Connexions:**
- Suporta geometria de coordenades (Mòdul 12) i preparació pel càlcul.

🔹 **Aplicacions i Ganxos de Memòria:**
- Les mesures del món real es basen en escales contínues (temperatura, longitud).
- Consell: "La màgia del punt mitjà" trova un nombre nou entre quals qualsevol dos.

##### Bloc 6 – Tancament i Taula de Propietats d'Operacions
🔹 **Definició:** El **tancament** indica que realitzar una operació en elements del conjunt es queda dins del conjunt. Diferents conjunts de nombres tenen propietats de tancament diferents sota suma, resta, multiplicació, divisió.

🔹 **Exemples:**
- `ℕ` tancat sota suma (`2 + 3 = 5`) però no sota resta (`2 - 5` surt de `ℕ`).
- `ℤ` tancat sota suma, resta, multiplicació, però no divisió (`1/2` no és enter).
- `ℚ` tancat sota tots quatre operacions excepte divisió per zero.
- Contraexemple: Afirmar que els irracionals són tancats sota suma; `√2 + (-√2) = 0` és racional.

🔹 **Notació Matemàtica:**
- Taula de tancament: marca `✔` o `✘` per a cada parella conjunt-operació.
- Utilitza declaracions com `∀ a, b ∈ S, a ∘ b ∈ S` per definir tancament.

🔹 **Representacions Visuals:**
```
Taula de tancament d'operacions
Conjunt | + | - | × | ÷
ℕ       |✔ |✘ |✔ |✘
ℕ₀      |✔ |✘ |✔ |✘
ℤ       |✔ |✔ |✔ |✘
ℚ       |✔ |✔ |✔ |✘ (si ÷0)
ℝ       |✔ |✔ |✔ |✘ (si ÷0)
```

🔹 **Propietats o Regles Clau:**
- Conèixer el tancament guia quin sistema de nombres és suficient per a un problema.
- Les excepcions de divisió depenen del denominador zero.

🔹 **Malentesos Comuns:**
- Assumir que el tancament s'estén automàticament a totes les operacions noves (p.ex., arrels a ℕ).

🔹 **Connexions:**
- Suporta estructures algebraiques (Mòdul 11) i elecció d'estratègia de resolució de problemes (Mòdul 19).

🔹 **Aplicacions i Ganxos de Memòria:**
- Ajuda decidir quan canviar de nombres sencers a enters o racionals.
- Recorda: "Porta tancada manté resultats dins del conjunt."

##### Bloc 7 – Classificació Mixta i Raonament
🔹 **Definició:** Les tasques de classificació mixta requereixen identificar tipus de nombres, explicar relacions d'inclusió, i justificar quines operacions mantenen resultats dins dels conjunts desitjats.

🔹 **Exemples:**
- Classifica `-√9` com a racional i enter (`-3`).
- Determina si `0` està a cada conjunt (`ℕ?` convencional, `ℕ₀?` sí, `ℤ?` sí, `ℚ?` sí).
- Contraexemple: Etiquetar `√5` com a racional; contradicció perquè el decimal mai es repeteix.

🔹 **Notació Matemàtica:**
- Declaracions combinades: `-√9 ∈ ℤ ⊂ ℚ ⊂ ℝ`.
- Utilitza fletxes de justificació: `x = -3 ⇒ x ∈ ℤ`.

🔹 **Representacions Visuals:**
```
Arbre de decisió:
Està enter? → Està enter? → Està racional? → Si no, irracional.
```

🔹 **Propietats o Regles Clau:**
- Anima els estudiants a citar definicions quan classifiquen.
- Compara expansió decimal o forma radical per decidir categoria.

🔹 **Malentesos Comuns:**
- Assumir que els nombres pertanyen a només un conjunt; molts pertanyen a múltiples conjunts nidificats.

🔹 **Connexions:**
- Prepara per a proves en mòdul de lògica i aplicacions en àlgebra, geometria.

🔹 **Aplicacions i Ganxos de Memòria:**



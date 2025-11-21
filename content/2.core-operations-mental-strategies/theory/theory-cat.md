### Mòdul 2: Operacions Bàsiques i Estratègies Mentals (≈4h)
Modelatge d'adició/sustracció, problemes de múltiples passos, propietats (commutativa, associativa, distributiva), domini de multiplicació/divisió, ordre de les operacions, tècniques d'estimació i estratègies de matemàtiques mentals.

Paraules clau: modelatge d'adició, modelatge de sustracció, línia numèrica, problemes de múltiples passos, anàlisi de problemes de text, commutativa, associativa, distributiva, estratègies de multiplicació, algorisme de divisió, divisió llarga, PEMDAS, estimació, matemàtiques mentals, arrodoniment, estimació de front-end, nombres compatibles, verificació de raonabilitat

Blocs:
1 Modelatge d'operacions en línia numèrica
2 Estructura de problemes de text multi-pas
3 Propietats (commutativa, associativa)
4 Aplicacions de la propietat distributiva
5 Estratègies de multiplicació (celosia, partició)
6 Algorisme de divisió i residus
7 Domini de la divisió llarga
8 Complexitat de l'ordre de les operacions
9 Tècniques d'estimació i arrodoniment
10 Exercicis de estratègies de matemàtiques mentals
11 Mètodes de verificació i comprovació d'errors
12 Conjunt de reptes mixtes

#### Teoria

##### Bloc 1 – Modelatge d'Operacions en Línia Numèrica
🔹 **Definició:** Una **línia numèrica** és una forma visual de veure com els números es mouen cap a la dreta quan sumes i cap a l'esquerra quan restes.

🔹 **Exemples:**
- `3 + 5`: col·loca't al 3, després mou 5 llocs cap a la dreta. On aterres? Al 8.
- `7 - 9`: comença al 7, mou 9 llocs cap a l'esquerra. Aterres al -2.
- Compte: Si mous a la dreta per restar, algo està malament.

🔹 **Com s'escriu:**
- Els números `... -2, -1, 0, 1 ...` marcats en ordre.
- Utilitzar `→` per anar a la dreta i `←` per anar a l'esquerra.

🔹 **Dibuix útil:**
```
Línia numèrica per a 4 - 6
-2 -1 0 1 2 3 4
					^ comença a 4
<--6 salts cap a esquerra--> resultat -2
```

🔹 **Regles Importants:**
- Quan sumes, camines cap a la dreta. Quan restes, camines cap a l'esquerra.
- La suma i la resta són com caminar cap endavant o cap enrere pel mateix camí.

🔹 **Errors Comuns:**
- Oblidar de comptar el zero quan passes de números positius a negatius.

🔹 **Per Què Ho Necessites:**
- T'ajudarà a entendre el plà (Mòdul 12) i els números negatius.

🔹 **Usos en la Vida Real:**
- Termostat: puja la temperatura (dreta) o baixa (esquerra).
- Compte bancari: diners que entren (dreta) o diners que treuen (esquerra).
- **Trucada:** "Dreta = pujar, esquerra = baixar."

##### Bloc 2 – Estructura de Problemes de Text Multi-Pas
🔹 **Definició:** Els problemes de text multi-pas requereixen sequenciar múltiples operacions per modelar escenaris reals amb precisió.

🔹 **Exemples:**
- Botiga escolar: `3` quaderns a `€2` més una carpeta a `€4` → `3×2 + 4 = 10`.
- Passejada setmanal: `15 km` per dia durant `4` dies, després descans → `15×4 = 60 km`.
- Contraexemple: Parar després de `3×2 = 6` omit el cost total.

🔹 **Notació Matemàtica:**
- Usa parèntesis per mostrar ordre: `total = (3×2) + 4`.
- Taula organitzadora que llista **Conegut**, **Necessari**, **Pla**.

🔹 **Representacions Visuals:**
```
| Pas | Operació | Resultat |
|------|----------|----------|
|  1   | 3×2      | 6 €      |
|  2   | 6+4      | 10 €     |
```

🔹 **Propietats o Regles Clau:**
- Tradueix el llenguatge a matemàtiques amb cura abans de calcular.
- Comprova la raonabilitat després de cada pas per evitar errors acumulatius.

🔹 **Concepcions Incorrectes Comunes:**
- Mesclar unitats (p. ex., euros amb elements) o realitzar passos fora d'ordre.

🔹 **Connexions:**
- Suporta la modelació algebraica (Mòdul 11) i estratègies de resolució de problemes (Mòdul 19).

🔹 **Aplicacions i Ganxos de Memòria:**
- Essencial per a pressupostos o planificació de viatges.
- Pista: "Sap, Necessita, Següent" resumeix els passos de planificació.

##### Bloc 3 – Propietats (Commutativa, Associativa)
🔹 **Definició:** La propietat **commutativa** permet intercanviar l'ordre (`a + b = b + a`, `ab = ba`); la propietat **associativa** permet reagrupar (`(a + b) + c = a + (b + c)`).

🔹 **Exemples:**
- `3 + 5 = 5 + 3`.
- `(2 + 4) + 7 = 2 + (4 + 7)`.
- Contraexemple: `7 - 5 ≠ 5 - 7`; la sustracció no és commutativa.

🔹 **Notació Matemàtica:**
- Per a tots els `a, b, c ∈ ℝ`, l'adició i la multiplicació satisfan la commutativitat i l'associativitat.
- Els parèntesis aclareixen l'agrupació.

🔹 **Representacions Visuals:**
```
Fitxes numèriques:
[3][+][5] ↔ [5][+][3]
```
```
Arbre d'agrupació mostrant `(a+b)+c` vs `a+(b+c)` amb les mateixes fulles.
```

🔹 **Propietats o Regles Clau:**
- Vàlid només per a adició i multiplicació en aritmètica bàsica.
- Facilita la reordenació mental de números.

🔹 **Concepcions Incorrectes Comunes:**
- Assumir que la sustracció o divisió comparteixen aquestes propietats.

🔹 **Connexions:**
- Suporta matemàtiques mentals (Bloc 10) i àlgebra (Mòdul 11).

🔹 **Aplicacions i Ganxos de Memòria:**
- Útil quan es reordenen despeses o es grups totals.
- Recorda: "Commuta = canviar de lloc; associa = canviar de parella."

##### Bloc 4 – Aplicacions de la Propietat Distributiva
🔹 **Definició:** La **propietat distributiva** estén la multiplicació sobre l'adició o sustracció: `a(b ± c) = ab ± ac`.

🔹 **Exemples:**
- `7×18 = 7×(10 + 8) = 70 + 56 = 126`.
- Àrea de `7 × 13` rectangle via `7(10 + 3)`.
- Contraexemple: `5(3 + 2) = 5×3 + 2` és incorrecte; tots dos termes necessiten multiplicació.

🔹 **Notació Matemàtica:**
- Funciona ambdues direccions: `ab + ac = a(b + c)` (factorització).
- Usa claus per destacar la distribució: `5{(3 + 2)}`.

🔹 **Representacions Visuals:**
```
Rectangle dividit:
[#####-----] amplada 18 = 10 + 8
```

🔹 **Propietats o Regles Clau:**
- Manté la igualtat quan cada terme rep el factor.
- Forma la base per expandir expressions algebraiques posteriorment.

🔹 **Concepcions Incorrectes Comunes:**
- Deixar caure signes negatius quan es distribueix sobre sustracció.

🔹 **Connexions:**
- Pont cap a manipulació algebraica (Mòdul 11) i lleis d'exponents (Mòdul 6).

🔹 **Aplicacions i Ganxos de Memòria:**
- Multiplicacions mentals ràpides i ajustos en preus.
- Pista: Imagina obrir una umbrella (factor) sobre cada terme.

##### Bloc 5 – Estratègies de Multiplicació
🔹 **Definició:** La **multiplicació estratègica** utilitza descomposició (models d'àrea, productes parcials, celosia) per simplificar productes complexos.

🔹 **Exemples:**
- Productes parcials: `34 × 27 = (30 + 4)(20 + 7) = 600 + 210 + 80 + 28`.
- La xarxa de celosia organitza la multiplicació de dígits amb sumes diagonals donant `918`.
- Contraexemple: Multiplicar només dígits de desenes `3×2` i ignorar altres.

🔹 **Notació Matemàtica:**
- Expressa com `(a + b)(c + d)` per aplicar distribució.
- La celosia utilitza sumes diagonals per a valors de lloc.

🔹 **Representacions Visuals:**
```
Celosia per a 34×27
		3 | 4
	--------
2 |06|08
7 |21|28
Sumes diagonals → 918
```

🔹 **Propietats o Regles Clau:**
- Trencar números respecta el valor de lloc, prevenint errors.
- La recombinació utilitza suma de productes parcials.

🔹 **Concepcions Incorrectes Comunes:**
- Oblidar de sumar tots els productes parcials.
- Alinear incorrectament dígits en celosia causant errors de lloc.

🔹 **Connexions:**
- Prepara per multiplicar polinomis (Mòdul 11) i exponentització (Mòdul 6).

🔹 **Aplicacions i Ganxos de Memòria:**
- Útil en càlculs mentals, pressupostos o escalat de mesuraments.
- Recorda: "Divideix, multiplica, suma."

##### Bloc 6 – Algorisme de Divisió i Residus
🔹 **Definició:** L'**algorisme de divisió** afirma que per a enters `a` i divisor positiu `d`, existeixen enters únics `q` i `r` amb `0 ≤ r < d` tals que `a = dq + r`.

🔹 **Exemples:**
- `23 ÷ 5` dóna `q = 4`, `r = 3` ja que `23 = 5×4 + 3`.
- `59 ÷ 7` produeix `q = 8`, `r = 3`.
- Contraexemple: Escriure `23 = 5×5 - 2` trenca la regla del residu.

🔹 **Notació Matemàtica:**
- Notació curta `a ÷ d = q R r`.
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
- Garanteix un parell únic quocient-residu.

🔹 **Concepcions Incorrectes Comunes:**
- Permetre residu ≥ divisor.
- Confondre quocient amb residu.

🔹 **Connexions:**
- Porta a divisió llarga (Bloc 7) i aritmètica modular (Mòdul 1).

🔹 **Aplicacions i Ganxos de Memòria:**
- Utilitzat en problemes de compartició equitativa o empacat.
- Pista: "Divideix = divisor × quocient + residu."

##### Bloc 7 – Domini de la Divisió Llarga
🔹 **Definició:** La **divisió llarga** resta repetidament múltiples del divisor de sections del dividend per construir el quocient dígit per dígit.

🔹 **Exemples:**
- `784 ÷ 16` resulta en `49`.
- `104.5 ÷ 5 = 20.9` estenant llocs decimals.
- Contraexemple: Saltar el pas de baixada trenca l'algorisme.

🔹 **Notació Matemàtica:**
- Coloca dígits del quocient sobre el dividend alineat amb el chunk restat.
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
- El residu de cada pas és menor que el divisor.
- Equivalent a subtracció repetida i estimació de quocients parcials.

🔹 **Concepcions Incorrectes Comunes:**
- Oblidar de baixar el següent dígit.
- Escriure el residu a sobre en lloc de restar.

🔹 **Connexions:**
- Suporta operacions decimals (Mòdul 3) i conversions de fraccions (Mòdul 5).

🔹 **Aplicacions i Ganxos de Memòria:**
- Necessari per a càlculs precisos de preu unitari o taxa.
- Recorda: Cicle "Divideix → Multiplica → Resta → Baixa."

##### Bloc 8 – Complexitat de l'Ordre de les Operacions
🔹 **Definició:** L'**ordre de les operacions** (PEMDAS) dicta la seqüència de càlcul: Parèntesis, Exponents, Multiplicació/Divisió (d'esquerra a dreta), Adició/Sustracció (d'esquerra a dreta).

🔹 **Exemples:**
- `6 + 3 × 4 = 6 + 12 = 18`.
- `20 ÷ 5 × 2 = 4 × 2 = 8` (processa d'esquerra a dreta dins del nivell MD).
- Contraexemple: `(6 + 3) × 4 = 36` només quan els parèntesis ho requereixen.

🔹 **Notació Matemàtica:**
- Símbols d'agrupació adicionals `[ ]`, `{ }` sobreescriuen l'ordre per defecte.
- Els exponents negatius requereixen parèntesis: `(-3)^2` vs `-3^2`.

🔹 **Representacions Visuals:**
```
Escala PEMDAS:
P
E
MD ⇢ d'esquerra a dreta
AS ⇢ d'esquerra a dreta
```

🔹 **Propietats o Regles Clau:**
- Multiplicació i divisió comparteixen prioritat; va d'esquerra a dreta.
- Adició i sustracció comparteixen prioritat; també d'esquerra a dreta.

🔹 **Concepcions Incorrectes Comunes:**
- Creure que la multiplicació sempre ve abans que la divisió independentment de l'ordre.
- Tractar malament números negatius amb exponents.

🔹 **Connexions:**
- Crucial per avaluar expressions algebraiques (Mòdul 11).
- Suporta situacions de resolució de problemes complexes (Mòdul 19).

🔹 **Aplicacions i Ganxos de Memòria:**
- Assegura que les fórmules introduïdes a calculadores donen resultats correctes.
- Pista: "Perdona Elisa Meu Estimat Amic Sergi" per a PEMDAS.

##### Bloc 9 – Tècniques d'Estimació i Arrodoniment
🔹 **Definició:** L'**estimació** proporciona respostes aproximades ràpides; l'**arrodoniment** ajusta números a un valor de lloc escollit per simplificar càlculs.

🔹 **Exemples:**
- Arrodoneix `73` al deu més proper → `70`.
- Estima `198 + 523 ≈ 200 + 500 = 700`.
- Contraexemple: Arrodonir `1.49` a `0` ignora la regla; correcte és `1`.

🔹 **Notació Matemàtica:**
- `≈` denota aproximació.
- Funció d'arrodoniment `round(x, k)` per a `k` decimals.

🔹 **Representacions Visuals:**
```
Arrodoniment de línia numèrica 23 al 10 més proper
20 ---|--- 25 ---|--- 30
				^ 23 més proper a 20
```

🔹 **Propietats o Regles Clau:**
- El dígit `5` o major arrodoneix cap amunt; menor que `5` arrodoneix cap avall.
- Els mètodes d'estimació inclouen front-end, nombres compatibles, agrupació.

🔹 **Concepcions Incorrectes Comunes:**
- Sempre arrodonir cap avall independentment del dígit.
- Tractar estimates com respostes exactes.

🔹 **Connexions:**
- Suporta precisió de mesurament (Mòdul 8) i informe de dades (Mòdul 16).

🔹 **Aplicacions i Ganxos de Memòria:**
- Útil per pressupostos, planificació de viatges, ajustos de cuina.
- Recorda: "5 o més, puja la puntuació; 4 o menys, deixa'l reposar."

##### Bloc 10 – Exercicis d'Estratègies de Matemàtiques Mentals
🔹 **Definició:** Les **matemàtiques mentals** aprofiten propietats de números (compensació, descomposició, nombres amics) per calcular sense llapis i paper.

🔹 **Exemples:**
- `48 + 17 = 50 + 15 = 65` utilitzant compensació.
- `25 × 4 = 100` utilitzant quarters.
- Contraexemple: Endevinar aleatòriament sense estructura augmenta errors.

🔹 **Notació Matemàtica:**
- Mostra ajustos: `48 + 17 = (48 + 2) + (17 - 2)`.
- Fletxes per mostrar passos d'ajust i correcció.

🔹 **Representacions Visuals:**
```
Taula en T
Original | Ajust | Resultat
48+17    | +2,-2 | 65
```

🔹 **Propietats o Regles Clau:**
- Utilitza propietats commutativa i associativa per reorganitzar números.
- Trenca números per valor de lloc per reduir càrrega cognitiva.

🔹 **Concepcions Incorrectes Comunes:**
- Pensar que les matemàtiques mentals són aproximades o endevinació; segueix lògica.

🔹 **Connexions:**
- Enllaça a manipulació decimal (Mòdul 3) i estimació (Bloc 9).

🔹 **Aplicacions i Ganxos de Memòria:**
- Suporta verificacions ràpides de preu, puntuació d'esports, exercicis mentals en classe.
- Pista: "Fes-ho amigable, després arregla-ho."

##### Bloc 11 – Mètodes de Verificació i Comprovació d'Errors
🔹 **Definició:** La **comprovació d'errors** utilitza operacions inverses, estimació o estratègies alternatives per confirmar l'exactitud dels resultats.

🔹 **Exemples:**
- Comprova `27 × 4 = 108` verificant `108 ÷ 4 = 27`.
- Estima `524 + 197 ≈ 700`; exacte `721` és raonable.
- Contraexemple: Repetir el mateix mètode incorrecte no detecta errors.

🔹 **Notació Matemàtica:**
- Fletxes inverses `⇄` indiquen comprovació: `×` ↔ `÷`, `+` ↔ `-`.
- Usa `≈` per a estimates de raonabilitat.

🔹 **Representacions Visuals:**
```
Flux:
Resol → Comprova invers → Compara estimate → Confirma
```

🔹 **Propietats o Regles Clau:**
- Les operacions inverses es desfan mútuament.
- Comparar amb estimates detecta errors de valor de lloc.

🔹 **Concepcions Incorrectes Comunes:**
- Assumir que la verificació és opcional; els petits errors es propaguen.

🔹 **Connexions:**
- Suporta la resolució de problemes (Mòdul 19) i precisió de càlcul.

🔹 **Aplicacions i Ganxos de Memòria:**
- Vital en enginyeria, finances, codificació per prevenir errors costosos.
- Recorda: "Fes-ho, desfés-ho, té-ho en compte."

##### Bloc 12 – Conjunt de Reptes Mixtes
🔹 **Definició:** Els reptes mixtes integren múltiples operacions i estratègies, requerint resolució de problemes flexible.

🔹 **Exemples:**
- Problema de recaptat de fons combinant multiplicació, sustracció, estimació.
- Enigma necessitant PEMDAS i dreceres mentals junts.
- Contraexemple: Aplicar només un algorisme d'un pas a un escenari multi-pas.

🔹 **Notació Matemàtica:**
- Expressions com `[(a + b) × c] ÷ d` amb anotació d'estratègies escollides.

🔹 **Representacions Visuals:**
```
Xarxa d'estratègia enllaçant operacions, estimació, matemàtiques mentals, propietats.
```

🔹 **Propietats o Regles Clau:**
- Encoratja seleccionar la millor eina, no seguir plantilles rígides.
- Construeix resiliència mitjançant pràctica variada.

🔹 **Concepcions Incorrectes Comunes:**
- Creure que hi ha només un mètode vàlid; múltiples camins poden ser correctes.

🔹 **Connexions:**
- Prepara per tasques integrades del món real en mòduls posteriors.

🔹 **Aplicacions i Ganxos de Memòria:**
- Reflecteix la presa de decisions autèntica on s'interaccionen diversos càlculs.
- Curiositat: Els concursos de matemàtiques mentals recompensen el canvi ràpid d'estratègia.

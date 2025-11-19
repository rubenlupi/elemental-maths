Sets, notation, membership, subsets, basic number sets (ℕ, ℤ, ℚ), place value, scientific notation, divisibility, primes, GCD/LCM, special numbers, introductory modular arithmetic.

Keywords: set, element, notation, braces, membership, subset, proper subset, Venn, empty set, ℕ, ℤ, ℚ, hierarchy, place value, expanded form, scientific notation, divisibility, prime, composite, sieve, GCD, Euclidean algorithm, LCM, factorization, perfect numbers, triangular numbers, Fibonacci, modular arithmetic, congruence, remainder patterns

Blocks:
1 Sets & notation basics
2 Subsets, proper subsets, Venn visuals
3 Number set hierarchy ℕ→ℤ→ℚ
4 Place value & expanded forms
5 Scientific notation intro
6 Divisibility rules practice
7 Prime/composite + sieve method
8 GCD (Euclidean) applications
9 LCM via prime factors
10 Factorization & fundamental theorem
11 Special numbers (perfect, triangular, Fibonacci)
12 Modular arithmetic concept (a ≡ b mod n)
13 Remainder pattern exploration
14 Mixed consolidation & review

#### Theory

##### Block 1 – Sets & Notation Basics
🔹 **Definition:** A **set** is a well-defined collection of distinct objects called **elements**; we write sets with braces like `A = {1, 2, 3}` and show membership with `∈`.

🔹 **Examples:**
- `B = {red, blue, green}` lists three colors; `blue ∈ B` but `yellow ∉ B`.
- The set `C = {n | n is an even whole number}` uses set-builder notation for all even numbers `0, 2, 4, ...`.
- Counterexample: `{1, 1, 2}` is poorly written because sets do not repeat elements; write `{1, 2}` instead.

🔹 **Mathematical Notation:**
- `{ }` encloses elements; the bar `|` or colon `:` means “such that” in set-builder form.
- `x ∈ S` reads “`x` belongs to `S`”; `x ∉ S` reads “`x` does not belong to `S`”.
- Capital letters (`S`, `T`) name sets; lowercase letters (`a`, `x`) name elements.

🔹 **Visual Representations:**
```
S = {⚽, 🏀, 🎾}
Index:   1   2   3
```
```
Number line idea for even numbers:
<---•---•---•---•--->
	0   2   4   6
```

🔹 **Empty Set & Special Cases:**
- The **empty set** `∅` (also written `{ }`) contains no elements; it is a valid set and is a subset of every set.
- Example: `{x | x is a whole number and x < 0} = ∅` (no whole numbers are negative).
- Important distinction: The set `{∅}` contains one element (the empty set itself) and is **not** empty; `|{∅}| = 1`.
- Counterexample: Confusing `∅` with `{0}` (which contains the element `0`) is a common error.

🔹 **Key Properties or Rules:**
- Order does not matter: `{1, 2, 3}` equals `{3, 2, 1}`. This is the **commutative property for sets**.
- Elements appear once; duplicates collapse into single entries.
- Sets can be finite or infinite depending on how many elements they contain.
- **Commutative Property for Union:** `A ∪ B = B ∪ A` (order of sets does not affect the union).
- **Commutative Property for Intersection:** `A ∩ B = B ∩ A` (order of sets does not affect the intersection).
- **Empty set property:** `∅ ⊆ S` for any set `S`.

🔹 **Detailed Examples with Union & Intersection:**
- Let `A = {1, 2, 3}` and `B = {2, 3, 4}`.
  - Union: `A ∪ B = {1, 2, 3, 4}` (all elements from both sets, listed once).
  - Also: `B ∪ A = {2, 3, 4, 1} = {1, 2, 3, 4}` (same result, showing commutativity).
  - Intersection: `A ∩ B = {2, 3}` (elements appearing in both).
  - Also: `B ∩ A = {2, 3}` (same result).
- Let `C = {5, 6}` and `D = {7, 8}`.
  - Union: `C ∪ D = {5, 6, 7, 8}`.
  - Intersection: `C ∩ D = ∅` (no common elements; the result is the empty set).
- Counterexample: `{a, b} ∪ ∅ = {a, b}` (union with empty set returns original set unchanged).

🔹 **Common Misconceptions:**
- Thinking `{2, 4, 6, ...}` must stop; ellipsis means it continues forever.
- Confusing elements with subsets; `{1, 2}` is a subset of `{1, 2, 3}`, while `1` is an element.
- Assuming rearranging elements changes the set, so `{1, 2, 3}` and `{3, 2, 1}` are viewed as different.

🔹 **Connections:**
- Organizes number sets like `ℕ`, `ℤ`, and `ℚ` later in the module.
- Supports Venn diagrams revisited in Module 18.

🔹 **Applications & Memory Hooks:**
- Categorizing students by club membership uses sets.
- Tip: Picture each set as a labeled “math folder” holding related objects.

##### Block 2 – Subsets & Venn Visuals
🔹 **Definition:** A **subset** `A ⊆ B` means every element of `A` belongs to `B`. A **proper subset** `A ⊂ B` additionally requires `A ≠ B`.

🔹 **Examples:**
- If `B = {1, 2, 3, 4}`, then `A = {2, 4}` is a subset since all its elements appear in `B`.
- `∅ ⊆ B` because the empty set has no elements that break membership.
- Counterexample: `{5}` is not a subset of `B` because `5 ∉ B`.

🔹 **Mathematical Notation:**
- `A ⊆ B` (subset), `A ⊂ B` (proper subset), `A ⊄ B` (not a subset).
- The empty set `∅` (also `{ }`) contains no elements.

🔹 **Visual Representations:**
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

🔹 **Key Properties or Rules:**
- Every set is a subset of itself (`B ⊆ B`).
- A set with `n` elements has `2^n` subsets.
- Subset relation is transitive: if `A ⊆ B` and `B ⊆ C`, then `A ⊆ C`.

🔹 **Common Misconceptions:**
- Believing a subset must be smaller; equality still counts.
- Forgetting that `∅` is a subset of every set.
- Treating a listed element `5 ∈ B` as if `{5}` were automatically a subset without confirming membership.

🔹 **Connections:**
- Builds the number hierarchy `ℕ ⊂ ℤ ⊂ ℚ` in Block 3.
- Supports probability event comparisons (Module 17).

🔹 **Applications & Memory Hooks:**
- **Organizational hierarchies:** Managers ⊂ Employees; Doctors ⊂ Hospital Staff; Premium Members ⊂ All Members.
- **Geometric shapes:** Squares ⊂ Rectangles ⊂ Parallelograms (each is a proper subset of the next).
- **Food categories:** Vegetables ⊂ Fresh Produce; Italian Dishes ⊂ Restaurant Menu.
- **Device management:** Smartphones ⊂ Mobile Devices; Electric Cars ⊂ All Vehicles.
- **Permission levels in software:** Administrators ⊂ Power Users ⊂ Regular Users (proper subset chain determines access).
- **Medical applications:** Diabetic patients ⊂ Patients with chronic disease—subset analysis helps hospitals allocate resources.
- Remember: Proper subset symbol `<` has a sharp edge reminding us the sets differ.

##### Block 3 – Number Set Hierarchy ℕ→ℤ→ℚ
🔹 **Definition:** The **number hierarchy** is the nesting of number sets where each larger set includes the previous one: naturals `ℕ`, integers `ℤ`, and rationals `ℚ`.

🔹 **Examples:**
- `ℕ = {1, 2, 3, ...}` counts positive whole numbers.
- `ℤ = {..., -2, -1, 0, 1, 2, ...}` extends `ℕ` with negatives and zero.
- `ℚ` contains every fraction `a/b` with integers `a` and `b ≠ 0`, so `3 = 3/1` is also rational.

🔹 **Mathematical Notation:**
- Inclusion chain: `ℕ ⊂ ℤ ⊂ ℚ`.
- Rational form: `ℚ = {a/b | a, b ∈ ℤ, b ≠ 0}`.

🔹 **Visual Representations:**
```
[ℚ]
 └─[ℤ]
	 └─[ℕ]
```
```
Number line:
... -2 -1 0 1 2 ... | add fractions between integers for ℚ
```

🔹 **Key Properties or Rules:**
- Every natural number is automatically an integer and a rational.
- Rationals are dense: between any two rationals, another rational exists.

🔹 **Common Misconceptions:**
- Assuming fractions are not rationals; they define the set.
- Thinking `0` must be in `ℕ`; conventions vary, so clarify context.
- Believing repeating decimals like `0.333...` cannot be rational even though they equal fractions.

🔹 **Connections:**
- Prepares for decimals (Module 3) and extended systems (Module 4).
- Supports fraction operations in Module 5.

🔹 **Applications & Memory Hooks:**
- **Banking and temperature:** Accounts can go negative (ℤ), but candy counts cannot—choose ℕ for inventory, ℤ for account balance.
- **Cooking measurements:** Recipes use ℚ fractions (1/2 cup flour, 3/4 tsp salt); food weights use ℕ (2 eggs, 6 carrots).
- **Medicine dosages:** Fractional (ℚ) doses like 0.5 mg or 1/4 tablet; patient counts (ℕ) or temperature changes (ℤ if below normal).
- **Elevation data:** Mountain heights ∈ ℕ (positive); sea depths can be negative integers (ℤ); precise measurements use ℚ.
- **Financial scenarios:** Stock prices (ℚ—$45.75 per share), transaction counts (ℕ), account balances including debt (ℤ).
- **Physics measurements:** Distance ratios use ℚ; time intervals ℕ; position relative to origin ℤ.
- Tip: Visualize nested boxes labeled `ℕ`, `ℤ`, `ℚ` to recall inclusion.


##### Block 3.5 – Comparison Symbols & Inequalities

🔹 **Definition:** The symbols `<` (less than), `>` (greater than), `=` (equal to), `≤` (less than or equal to), `≥` (greater than or equal to) compare magnitudes of numbers on the number line.

🔹 **Examples:**
- `3 < 5` (3 is less than 5).
- `7 > 2` (7 is greater than 2).
- `4 = 4` (4 equals 4).
- `-2 < 0 < 3` (chain of inequalities).
- `5 ≥ 5` and `5 ≥ 3` (greater than or equal to).

🔹 **Mathematical Notation:**
- `a < b`, `a > b`, `a = b`, `a ≤ b`, `a ≥ b`.
- Transitivity property: if `a < b` and `b < c`, then `a < c`.

🔹 **Visual Representations:**
```
Number line:
<----|----|----|----|----|---->
    -2   0    2    4    6

3 is to the LEFT of 5 → 3 < 5
7 is to the RIGHT of 2 → 7 > 2
```

```
Inequality on a number line segment:
[a)----------o---------(b]
   closed     point    open
   at a       value    at b
```

🔹 **Key Properties or Rules:**
- The symbol's **point faces the smaller number**: `3 < 5` (point at 3).
- Reversing direction reverses meaning: `3 < 5` is equivalent to `5 > 3`.
- **Order preserved in addition/subtraction:** if `a < b`, then `a + c < b + c` and `a - c < b - c`.
- **Multiplication by positive preserves order:** if `a < b` and `c > 0`, then `ac < bc`.
- **Multiplication by negative reverses inequality:** if `a < b` and `c < 0`, then `ac > bc`.
- **Equality is reflexive:** `a = a`; **symmetric:** if `a = b` then `b = a`; **transitive:** if `a = b` and `b = c`, then `a = c`.

🔹 **Common Misconceptions:**
- Assuming `<` and `>` are interchangeable; the **shape matters** (point toward smaller value).
- Forgetting inequality **reversal when multiplying/dividing by negatives**.
- Mixing up chain comparisons: `2 < 5 > 3` is ambiguous; instead write `2 < 5` and `5 > 3` separately or use `2 < 5 > 3` with careful intent.
- Treating `=` as directional; it is symmetric—both sides are identical.
- Believing that `≤` and `≥` work like strict inequalities; they include the boundary value.

🔹 **Connections:**
- Foundation for solving inequalities (Module 11 extensions).
- Supports ordering numbers on the number line (Module 1).
- Essential for interval notation and ranges in functions (Module 13).
- Appears in data interpretation and statistical comparisons (Module 16).

🔹 **Applications & Memory Hooks:**
- **Comparing prices:** iPhone A ($700) > iPhone B ($650); discount ≤ 20% of original price.
- **Sports statistics:** Player A's average score ≥ 15 points; team wins < team losses; temperature during match -2°C ≤ T ≤ 25°C.
- **Weight management:** "Goal weight ≤ 75 kg"; "increase in weight < 5 kg per month."
- **Budget planning:** "Monthly expenses ≤ €2000"; "Savings > Spending."
- **Traffic & travel:** "Speed limit < 50 km/h in urban zones"; "Distance to destination ≥ 10 km."
- **Medical ranges:** "Normal cholesterol < 200 mg/dL"; "Safe blood sugar range: 70 ≤ reading ≤ 100."
- **Grading systems:** "Pass grade ≥ 60%"; "Excellent ≥ 90%."
- **Tip:** "The point **eats** the bigger number" (hungry alligator interpretation—the opening faces the larger value).
- **Alternative:** "Left is less, right is greater" (position on the number line).
- **Quick check:** Substitute small numbers (`a = 1, b = 3`) to verify direction.



##### Block 4 – Place Value & Expanded Forms
🔹 **Definition:** **Place value** assigns each digit a value based on its position in powers of `10`; **expanded form** writes the number as the sum of each digit times its place value.

🔹 **Examples:**
- `4,582 = 4×10^3 + 5×10^2 + 8×10^1 + 2×10^0`.
- `307` has `3` hundreds, `0` tens, `7` ones.
- Counterexample: Writing `307 = 3×100 + 7×10` ignores the zero tens.

🔹 **Mathematical Notation:**
- Positional notation uses powers of ten: digit `d_k × 10^k`.
- Expanded form: `2,045 = 2×10^3 + 4×10^1 + 5×10^0`.

🔹 **Visual Representations:**
```
Thousands | Hundreds | Tens | Ones
	4          5         8      2
```
```
Base-10 blocks: [■■■■] thousands, [□□□□□] hundreds, etc.
```

🔹 **Key Properties or Rules:**
- Each place is ten times the value of the place to its right.
- Zero holds a place even without contributing value.

🔹 **Common Misconceptions:**
- Dropping zeros and changing magnitude.
- Reading digits separately instead of by place (“two zero five” for `205`).
- Assuming expanded form must list only nonzero digits, causing students to omit placeholder terms.

🔹 **Connections:**
- Supports decimal understanding (Module 3) and scientific notation.
- Essential for mental math strategies in Module 2.

🔹 **Applications & Memory Hooks:**
- Helps interpret population figures or currency.
- Remember: “Hop left multiplies by ten” when shifting digits.

##### Block 5 – Scientific Notation Intro
🔹 **Definition:** **Scientific notation** expresses numbers as `a × 10^n` with `1 ≤ |a| < 10` and integer `n`, enabling compact representation of very large or small quantities.

🔹 **Examples:**
- `5,200,000 = 5.2 × 10^6`.
- `0.00034 = 3.4 × 10^-4`.
- Counterexample: `52 × 10^5` is invalid because the coefficient `52` is not between `1` and `10`.

🔹 **Mathematical Notation:**
- `a` is the **coefficient** (or mantissa); `10^n` shifts the decimal `n` places.
- Positive `n` moves decimal left (large numbers); negative `n` moves it right (small numbers).

🔹 **Visual Representations:**
```
5.2 × 10^6 → 5.2 → 52 → 520 → ... → 5,200,000
```

🔹 **Key Properties or Rules:**
- `10^a × 10^b = 10^(a+b)`; `10^a / 10^b = 10^(a-b)`.
- Multiplying numbers in scientific notation combines coefficients and adds exponents.

🔹 **Common Misconceptions:**
- Forgetting to adjust exponent when moving decimal.
- Reversing direction of exponent sign.
- Thinking coefficient may be zero or exceed `10`, which breaks scientific notation rules.

🔹 **Connections:**
- Links with exponent laws (Module 6) and measurement scales (Module 8).
- Essential for scientific data representation (Module 16).

🔹 **Applications & Memory Hooks:**
- **Astronomy:** Distances (1.5 × 10^8 km to Sun, 4.4 × 10^16 m to nearest star) fit nicely in scientific notation for comparison.
- **Chemistry:** Avogadro's number ≈ 6.02 × 10^23 (molecules in one mole); atomic sizes ≈ 10^-10 meters.
- **Microbiology:** Virus size ≈ 10^-7 to 10^-8 meters; bacteria ≈ 10^-6 meters—scale comparison requires scientific notation.
- **Finance:** Global GDP ≈ 10^13 euros; individual transaction ≈ 10^2 euros—notation shows scale differences.
- **Data storage:** Hard drive capacity 2 × 10^12 bytes (2 TB); file size 5 × 10^6 bytes (5 MB).
- **Physics calculations:** Speed of light ≈ 3 × 10^8 m/s; nuclear particle mass ≈ 10^-27 kg.
- **Climate science:** Annual CO₂ emissions ≈ 3.7 × 10^10 tons; particle pollution ≈ 10^-6 grams.
- Did you know...? Distance to the Sun is about `1.5 × 10^8 km`; writing this as 150,000,000 km is cumbersome and error-prone.

##### Block 6 – Divisibility Rules Practice
🔹 **Definition:** A **divisibility rule** is a shortcut to determine whether an integer divides another without full division.

🔹 **Examples:**
- A number is divisible by `2` if its last digit is `0, 2, 4, 6, 8`.
- Divisible by `3` if the sum of digits is a multiple of `3` (`7,524 → 7+5+2+4 = 18`).
- Counterexample: `123` is not divisible by `4` because the last two digits `23` are not divisible by `4`.

🔹 **Mathematical Notation:**
- `a | b` means “`a` divides `b`”; `a ∤ b` means it does not.
- Lists of rules often use tables for quick reference.

🔹 **Visual Representations:**
```
Divisibility table
Divisor | Quick test
   2    | last digit even
   3    | digit sum multiple of 3
   5    | last digit 0 or 5
   9    | digit sum multiple of 9
```

🔹 **Key Properties or Rules:**
- If `a | b` and `b | c`, then `a | c` (transitive).
- If `a | b` and `a | c`, then `a | (b ± c)`.

🔹 **Common Misconceptions:**
- Applying the wrong test (e.g., digit sum for `4`).
- Forgetting divisibility by `6` requires both `2` and `3`.
- Assuming divisibility rules guarantee primality rather than only testing factors.

🔹 **Connections:**
- Leads into primes, GCD, and LCM (Blocks 7–9).
- Supports fraction simplification in Module 5.

🔹 **Applications & Memory Hooks:**
- Quick checks for sharing equally among groups.
- Tip: “Six needs even and triple” to recall `6` needs divisibility by both `2` and `3`.

##### Block 7 – Prime/Composite & Sieve Method
🔹 **Definition:** A **prime number** has exactly two distinct positive divisors (`1` and itself); a **composite number** has more than two divisors. The **Sieve of Eratosthenes** filters primes by removing multiples.

🔹 **Examples:**
- `2, 3, 5, 7` are prime; `4, 6, 9, 12` are composite.
- `1` is neither prime nor composite.
- Counterexample: Calling `9` prime ignores `3 × 3`.

🔹 **Mathematical Notation:**
- `p ∈ ℕ`, `p > 1`, `d | p ⇒ d ∈ {1, p}`.
- Sieve uses sequential marking multiples of each discovered prime.

🔹 **Visual Representations:**
```
1  2  3  4  5  6  7  8  9 10
   P  P  X  P  X  P  X  X  X
P = prime, X = crossed multiple
```
```
Factor tree for 12:
   12
  /  \
 3    4
	 / \
	2   2
```

🔹 **Key Properties or Rules:**
- Only even prime is `2`.
- Every integer greater than `1` is prime or composite.
- Sieve requires marking multiples starting from `p^2`.

🔹 **Common Misconceptions:**
- Thinking negative numbers can be prime in the same sense; standard definition uses positive integers.
- Assuming large numbers cannot be prime.
- Believing the sieve finds primes by division instead of systematically striking multiples.

🔹 **Connections:**
- Prime factorization (Block 10) and cryptography (Module 21).
- Appears in number theory Module 9 special numbers.

🔹 **Applications & Memory Hooks:**
- Used in coding theory and secure data.
- Remember: “Prime means precisely two divisors.”

##### Block 8 – GCD (Euclidean) Applications
🔹 **Definition:** The **greatest common divisor** `gcd(a, b)` is the largest positive integer dividing both `a` and `b`. The **Euclidean algorithm** finds it via repeated division with remainders.

🔹 **Examples:**
- `gcd(24, 36) = 12`.
- `gcd(48, 18)` via Euclidean steps: `48 = 18×2 + 12`, `18 = 12×1 + 6`, `12 = 6×2 + 0`, so `gcd = 6`.
- Counterexample: Guessing `9` divides both `12` and `18` fails because `9 ∤ 12`.

🔹 **Mathematical Notation:**
- `gcd(a, b) = gcd(b, a mod b)` iteratively until remainder `0`.
- `gcd(a, b, c)` shorthand for `gcd(a, gcd(b, c))`.

🔹 **Visual Representations:**
```
Euclidean ladder for gcd(48,18)
48 = 18×2 + 12
18 = 12×1 + 6
12 = 6×2 + 0
```
```
Rectangle tiling: common square size that tiles both rectangles.
```

🔹 **Key Properties or Rules:**
- If `d = gcd(a, b)`, then `a = d·a'` and `b = d·b'` with `a'`, `b'` coprime.
- Relation with LCM: `a × b = gcd(a, b) × lcm(a, b)`.

🔹 **Common Misconceptions:**
- Mixing GCD with LCM.
- Neglecting `1` as possible GCD.
- Expecting Euclidean steps to stop when numbers match rather than when remainder hits zero.

🔹 **Connections:**
- Simplifies fractions (Module 5) and modular congruences.
- Demonstrates algorithmic thinking relevant to Module 19 strategies.

🔹 **Applications & Memory Hooks:**
- Used in grouping items equally or synchronizing cycles.
- Tip: “Greatest Common Divides” summarises its meaning.

##### Block 9 – LCM via Prime Factors
🔹 **Definition:** The **least common multiple** `lcm(a, b)` is the smallest positive integer divisible by both `a` and `b`, often found using prime factorization.

🔹 **Examples:**
- `lcm(4, 6) = 12`.
- `lcm(8, 12, 15) = 120` (prime factors `2^3`, `3`, `5`).
- Counterexample: Choosing `24` as `lcm(4, 6)` is incorrect because `12` is smaller.

🔹 **Mathematical Notation:**
- Prime factor method: take highest power of each prime across numbers.
- Identity: `a × b = gcd(a, b) × lcm(a, b)`.

🔹 **Visual Representations:**
```
Multiples list:
4 → 4,8,12,16,...
6 → 6,12,18,...
First common → 12
```

🔹 **Key Properties or Rules:**
- Symmetric: `lcm(a, b) = lcm(b, a)`.
- If `a | b`, then `lcm(a, b) = b`.

🔹 **Common Misconceptions:**
- Stopping at any common multiple instead of the least.
- Forgetting to include all prime powers.
- Assuming least common multiple must be the product of the numbers even when they share factors.

🔹 **Connections:**
- Essential for common denominators (Module 5).
- Supports scheduling problems (Module 19).

🔹 **Applications & Memory Hooks:**
- Synchronizing events, like class schedules or traffic light cycles.
- Remember: “Least means first match, then stop.”

##### Block 10 – Factorization & Fundamental Theorem
🔹 **Definition:** **Prime factorization** decomposes an integer into prime factors. The **Fundamental Theorem of Arithmetic** states every integer greater than `1` has a unique prime factorization (up to order).

🔹 **Examples:**
- `60 = 2^2 × 3 × 5`.
- `84 = 2^2 × 3 × 7`.
- Counterexample: `45 = 3 × 15` is incomplete because `15` is not prime; full factorization `3^2 × 5`.

🔹 **Mathematical Notation:**
- Factor trees, exponents (`p^k`).
- Uniqueness: if `n = p_1^{a_1} ... p_k^{a_k} = q_1^{b_1} ... q_m^{b_m}`, then `k = m` and primes match with same exponents.

🔹 **Visual Representations:**
```
   60
  /  \
 6   10
 /\  / \
2 3 2  5
```

🔹 **Key Properties or Rules:**
- Multiplying identical primes adds exponents.
- Prime factorization supports GCD/LCM via min/max exponents.

🔹 **Common Misconceptions:**
- Stopping at composite factors.
- Believing `1` has prime factors; it does not.
- Thinking different factor tree layouts produce different prime factorizations rather than the same multiset of primes.

🔹 **Connections:**
- Builds exponent skills (Module 6) and number theory (Module 9).
- Assists in simplifying radicals (Module 6).

🔹 **Applications & Memory Hooks:**
- **Cryptography:** RSA encryption's security depends on factoring numbers like 143 = 11 × 13; modern encryption uses 2048-bit composites (>600 digits).
- **Simplifying fractions:** 60/84 = (2² × 3 × 5)/(2² × 3 × 7) = 5/7 using prime factorization.
- **Design and manufacturing:** Creating modular products—if base unit = 2² × 3 = 12 cm, variants (12, 24, 36, 48 cm) scale predictably.
- **Computer science:** Compiler optimization uses factorization to rewrite loop structures efficiently.
- **Music harmony:** Frequency ratios like 5/4 (just major third) emerge from prime factorizations of note frequencies.
- **Data compression:** Huffman coding assigns bit patterns based on frequency factorizations for optimal compression.
- **Finance:** Compound interest calculations rely on factoring to find growth rates matching target investments.
- Did you know...? Modern encryption relies on difficulty of factoring huge numbers. Breaking RSA-2048 would require factoring a 617-digit number—estimated to take centuries!

##### Block 11 – Special Numbers (Perfect, Triangular, Fibonacci)
🔹 **Definition:** **Perfect numbers** equal the sum of proper divisors; **triangular numbers** count dots forming equilateral triangles; the **Fibonacci sequence** has each term equal to the sum of the two previous terms (`F_n = F_{n-1} + F_{n-2}`).

🔹 **Examples:**
- Perfect: `6 = 1 + 2 + 3`, `28 = 1 + 2 + 4 + 7 + 14`.
- Triangular: `T_4 = 10` forming a `4`-row triangle.
- Fibonacci: `0, 1, 1, 2, 3, 5, 8, ...`; counterexample: `9` is not triangular since `n(n+1)/2 ≠ 9` for integer `n`.

🔹 **Mathematical Notation:**
- Triangular numbers `T_n = n(n + 1)/2`.
- Fibonacci recursion with `F_0 = 0`, `F_1 = 1`.
- Perfect number check via divisor sum `σ(n) - n = n`.

🔹 **Visual Representations:**
```
Triangular dots (T4):
•
••
•••
••••
```
```
Fibonacci squares forming spiral: 1×1, 1×1, 2×2, 3×3, 5×5.
```

🔹 **Key Properties or Rules:**
- Even perfect numbers follow `2^{p-1}(2^p - 1)` when `2^p - 1` is prime (Mersenne prime).
- `T_n = C(n + 1, 2)` connects to combinations.
- Fibonacci ratios approach the golden ratio `≈ 1.618`.

🔹 **Common Misconceptions:**
- Assuming triangular numbers are perfect numbers; they are distinct sequences.
- Treating Fibonacci as arithmetic (fixed difference) instead of recursive addition.
- Believing Fibonacci must start with `1, 1` and overlooking the standard `0, 1` convention used in many formulas.

🔹 **Connections:**
- Links to combinatorics (Module 20) and patterns (Module 10).
- Fibonacci appears in exponential growth discussions (Module 6).

🔹 **Applications & Memory Hooks:**
- Shows up in architecture, nature (pinecones, sunflowers).
- Remember: “Triangular `T` stacks `n` and `n+1`, then halves.”

##### Block 12 – Modular Arithmetic Concept (a ≡ b mod n)
🔹 **Definition:** **Modular arithmetic** compares numbers by remainders: `a ≡ b (mod n)` when `n` divides `a - b`.

🔹 **Examples:**
- `17 ≡ 5 (mod 12)` because `17 - 5 = 12`.
- `9 ≡ 1 (mod 4)` since both leave remainder `1` upon division by `4`.
- Counterexample: `14 ≡ 3 (mod 4)` is false because `14 - 3 = 11`, which `4` does not divide.

🔹 **Mathematical Notation:**
- Congruence symbol `≡`; modulus noted `(mod n)`.
- Remainder class `[a]_n` represents all integers congruent to `a` modulo `n`.

🔹 **Visual Representations:**
```
Clock (mod 12):
1 ↔ 13 ↔ 25 ↔ ... all ≡ 1 (mod 12)
```
```
Remainder table mod 5
n | n mod 5
0 | 0
1 | 1
2 | 2
3 | 3
4 | 4
5 | 0
```

🔹 **Key Properties or Rules:**
- If `a ≡ b (mod n)` and `c ≡ d (mod n)`, then `a ± c ≡ b ± d (mod n)` and `ac ≡ bd (mod n)`.
- Negative remainders wrap: `-1 ≡ n - 1 (mod n)`.

🔹 **Common Misconceptions:**
- Treating `mod` as division rather than remainder comparison.
- Forgetting to reduce remainders into `0` to `n - 1` range.
- Assuming congruent numbers must be close in size instead of differing by multiples of the modulus.

🔹 **Connections:**
- Supports divisibility logic and cyclic patterns (Block 13).
- Returns in enrichment Module 21 and cryptography contexts.

🔹 **Applications & Memory Hooks:**
- **Clock arithmetic:** 14:00 (2:00 PM) + 11 hours = 1:00 AM (25 ≡ 1 mod 12).
- **Weekday prediction:** If today is Wednesday (day 3) + 10 days ≡ 13 ≡ 6 (mod 7) = Saturday.
- **Computer graphics:** Color channels use mod 256 to keep RGB values in range [0, 255].
- **Security codes:** Credit card check digits use mod 10 arithmetic (Luhn algorithm) to detect errors.
- **Warehouse inventory:** Shelf bins numbered 0–49; item barcode 1537 goes to bin 1537 mod 50 = 37.
- **Scheduling:** Repeating every 29 days (lunar cycle), task on day 100 equals task on day 100 mod 29 = 13.
- **Online gaming:** Player IDs assigned using mod for server load balancing across multiple game instances.
- Remember: "Modular arithmetic wraps around—like a clock face."

🔹 **Applications & Memory Hooks:**
- Helps compute weekdays, clock times, checksum digits.
- Did you know...? Musical notes wrap around octaves like mod `12` arithmetic.

##### Block 13 – Remainder Pattern Exploration
🔹 **Definition:** A **remainder pattern** tracks repeating remainders when numbers are divided by a fixed modulus, revealing cycles.

🔹 **Examples:**
- Powers of `2 mod 5`: `2, 4, 3, 1` repeating every `4` steps.
- Multiples of `7 mod 3`: remainders `1, 2, 0, 1, 2, 0, ...`.
- Counterexample: Claiming `2^n mod 5` always equals `2` ignores the cycle.

🔹 **Mathematical Notation:**
- Sequences `(a_n)` with `a_n ≡ k (mod m)`.
- Period denotes cycle length.

🔹 **Visual Representations:**
```
Remainder wheel mod 5 for powers of 2
2 → 4 → 3 → 1 → (back to 2)
```
```
Table:
n | 2^n mod 5
1 | 2
2 | 4
3 | 3
4 | 1
5 | 2
```

🔹 **Key Properties or Rules:**
- Finite moduli guarantee eventual repetition (Pigeonhole Principle).
- Cycle length for powers relates to Euler’s totient `φ(n)` when base and modulus are coprime.

🔹 **Common Misconceptions:**
- Expecting cycles to start at `n = 0`; initial terms may differ.
- Believing every modulus yields a cycle of length equal to the modulus without checking actual order.
- Assuming once a value repeats, the sequence immediately ends instead of continuing with the established cycle.

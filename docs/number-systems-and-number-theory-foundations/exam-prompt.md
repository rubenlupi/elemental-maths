# 🟦 EXAM PROMPT: SISTEMES DE NUMERACIÓ I VALOR POSICIONAL

**Topic:** Number Systems and Number Theory Foundations - Day 1  
**Language:** Catalan  
**Level:** Gifted students (9-10 years)

---

## 📥 HOW TO USE THIS PROMPT

To generate a new exam for this topic:

1. Read the theory document: `teoria.md`
2. Use the general exam generator prompt: `../../prompts/general-exam-prompt.md`
3. Specify the concepts to cover (see below)
4. Generate in CATALAN

---

## 📚 THEORY REFERENCE

The theory document covers:

### **1. Number Sets**
- Natural numbers (ℕ)
- Integers (ℤ)
- Rational numbers (ℚ)
- Set relationships: ℕ ⊂ ℤ ⊂ ℚ

### **2. Place Value in Base-10**
- Positional value system
- Powers of 10
- Expanded form with exponents
- Decomposing large numbers

### **3. Scientific Notation**
- Format: a × 10ⁿ (where 1 ≤ a < 10)
- Converting large numbers (positive exponents)
- Converting small numbers (negative exponents)
- Operations with scientific notation

### **4. Real-World Applications**
- Astronomy (distances, stellar measurements)
- Computing (data storage, speeds)
- Biology (cell sizes, bacteria)
- Physics (atomic scales)

---

## 🎯 CONCEPTS TO TEST IN EXAMS

### **Core Concepts (Must Include)**
1. Classifying numbers by set (ℕ, ℤ, ℚ)
2. Understanding set relationships
3. Place value identification
4. Expanded form with exponents
5. Converting to/from scientific notation
6. Ordering numbers in scientific notation
7. Solving real-world problems with large/small numbers

### **Skills to Assess**
- **Recognition:** Identify number sets correctly
- **Conversion:** Standard ↔ scientific notation
- **Decomposition:** Write numbers in expanded form
- **Application:** Use scientific notation in context
- **Comparison:** Order numbers efficiently
- **Problem-solving:** Apply concepts to real scenarios
- **Reverse reasoning:** Find missing values or exponents

---

## 📋 EXAM STRUCTURE GUIDELINES

### **Difficulty Distribution**
- **3 moderate exercises** (0.8-1.0 points): Basic classification, simple conversions
- **5 intermediate exercises** (1.0-1.3 points): Multi-step conversions, place value, applications
- **2 challenging exercises** (1.5 points): Complex real-world problems, reverse reasoning

### **Exercise Types to Include**
1. **Classification exercise:** Identify number sets (ℕ, ℤ, ℚ)
2. **Expanded form:** Write large numbers with exponents
3. **Conversion to scientific notation:** Both large and small numbers
4. **Ordering exercise:** Compare numbers in scientific notation
5. **Real-world application:** Practical problem with context
6. **Multi-step problem:** Combining concepts (e.g., unit conversion + scientific notation)
7. **Place value identification:** Find value of specific digits
8. **Complex application:** Real data (astronomy, computing, biology)
9. **Challenging problem:** Multiple operations or complex reasoning
10. **Reverse reasoning:** Find unknown exponent or value

### **Contexts for Real-World Problems**
- Astronomy: distances between planets, stars, galaxies
- Computing: data storage (bytes, GB, TB), internet speeds
- Biology: cell sizes, bacteria populations, virus dimensions
- Physics: atomic masses, particle charges, speed of light
- Geography: Earth dimensions, ocean depths, mountain heights
- Time: large time periods, historical dates

---

## ⚙️ GENERATION PARAMETERS

### **When generating a new exam:**

**Input:**
```
Topic: Sistemes de numeració i valor posicional
Theory file: docs/number-systems-and-number-theory-foundations/teoria.md
Language: Catalan
Level: Gifted students (9-10 years)

Concepts to cover:
- Number set classification (ℕ, ℤ, ℚ)
- Place value and expanded form with exponents
- Scientific notation conversions (large and small numbers)
- Ordering numbers in scientific notation
- Real-world applications (2-3 exercises minimum)
- Reverse reasoning problems

Use general-exam-prompt.md to generate exam
```

**Output folder format:**
```
docs/number-systems-and-number-theory-foundations/exam_YYYYMMDD_HHMMSS/
├── exercises.md
└── solutions.md
```

---

## ✅ QUALITY CHECKLIST

Before finalizing exam, verify:

**Content Coverage:**
- [ ] All main concepts from theory are tested
- [ ] Exercises progress from simple to complex
- [ ] At least 2-3 real-world application problems
- [ ] Minimum 5 exercises require reverse reasoning
- [ ] Different number ranges tested (millions, billions, decimals, etc.)
- [ ] Both large numbers (positive exponents) and small numbers (negative exponents)

**Technical Requirements:**
- [ ] Total points = exactly 10
- [ ] Difficulty: 3 moderate, 5 intermediate, 2 challenging
- [ ] Each exercise has unique solution approach
- [ ] No trivial problems solvable by inspection
- [ ] Solutions include complete step-by-step justifications
- [ ] Mathematical notation matches theory document

**Language & Format:**
- [ ] All content in Catalan
- [ ] Clear problem statements (unambiguous)
- [ ] Appropriate space for student answers
- [ ] Consistent formatting throughout
- [ ] Headers in exercises.md: "Nom:", "Data:"
- [ ] Point format: "(X punts)" or "(X punt)"

---

## 📌 EXAMPLE EXERCISE TYPES

### **Moderate (0.8-1.0 punts)**
```
Classifica els següents nombres: 5, -3, 0.5, 0
Escriu 45.000 en notació científica
Identifica el valor del dígit subratllat en 3.456.789
```

### **Intermediate (1.0-1.3 punts)**
```
Ordena de menor a major: 3.2 × 10⁵, 5 × 10⁴, 2.8 × 10⁵
Escriu 2.473.586 en forma expandida amb exponents
La distància Terra-Lluna és 384.000 km. Expressa en notació científica
```

### **Challenging (1.5 punts)**
```
Un any llum és 9.5 × 10¹² km. Pròxima Centauri està a 4.24 anys llum. 
Quina distància en km? (notació científica)

Un nombre en notació científica és 7.2 × 10ⁿ = 72.000. 
Troba el valor de n. (raonament invers)
```

---

## 🔄 GENERATING ADDITIONAL EXAMS

Each new exam should:
1. Cover the same core concepts
2. Use **different numbers and contexts**
3. Vary the specific skills tested
4. Maintain the same difficulty distribution
5. Be stored in a new timestamped folder
6. Test the same learning objectives differently

**Variety sources:**
- Different astronomical objects and distances
- Various computing contexts (USB, SSD, internet speeds)
- Diverse biological examples (bacteria, cells, viruses)
- Alternative real-world scenarios

---

## 📝 NOTES FOR FUTURE EXAMS

**What works well:**
- Real-world contexts make problems engaging
- Reverse reasoning exercises test deep understanding
- Multi-step problems combine multiple concepts effectively
- Clear visual tables help organize information

**Avoid:**
- Repetitive exercise structures
- Purely computational problems without context
- Ambiguous wording that confuses students
- Numbers that are too similar (leads to careless errors)

---

**Last updated:** November 18, 2025